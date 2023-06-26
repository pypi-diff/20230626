# Comparing `tmp/collective.documentgenerator-3.8.tar.gz` & `tmp/collective.documentgenerator-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.documentgenerator-3.8.tar", last modified: Tue Aug 13 07:53:09 2019, max compression
+gzip compressed data, was "dist/collective.documentgenerator-3.9.tar", last modified: Mon Oct 14 11:59:36 2019, max compression
```

## Comparing `collective.documentgenerator-3.8.tar` & `collective.documentgenerator-3.9.tar`

### file list

```diff
@@ -1,198 +1,197 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/developer.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1026 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/technical.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1966 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/user.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14018 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/images/AddPODTTemplateMenu.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2867 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/images/addPloneSite.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18167 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/images/viewlet.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9992 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/docs/images/demoInstal.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3756 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      347 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28480 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      163 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/jenkins.cfg
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28480 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8934 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      362 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/not-zip-safe
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1815 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/DX_renderer.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      722 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/controlpanel.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      519 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      184 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/browserlayer.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2095 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/PODTemplate.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2281 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/ConfigurablePODTemplate.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2095 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/SubTemplate.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2165 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/StyleTemplate.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2143 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/MailingLoopTemplate.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      228 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/testing/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      231 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/testing/propertiestool.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/testing/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3990 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/testing/types/member.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11386 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/possibly_mailed_model.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9209 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/styles_2.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8120 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/modele_general.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8990 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/mailing.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10991 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/modele_general.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    89772 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/sub_template.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9388 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/styles.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12279 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/modèle_collection.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      494 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/collectivedocumentgenerator_demo_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       41 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone4/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      185 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone4/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone4/collectivedocumentgenerator_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      252 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone4/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      371 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone4/cssregistry.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone5/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      185 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone5/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      591 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone5/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5622 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/helper/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      532 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/helper/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2338 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/helper/archetypes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5725 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/helper/dexterity.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1828 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/helper/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9626 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/helper/base.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2434 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/generationlinks.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      556 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/generationlinks.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/batchactions.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      557 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/demo/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/demo/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7182 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/demo/helper.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      872 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/demo/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      497 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/events/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/events/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      831 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/events/pod_templates_events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5714 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/events/styles_events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1222 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/events/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1995 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/file_representation.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1404 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/style_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17488 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/pod_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      277 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/merge_templates.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1739 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/condition.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2710 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/vocabulary.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2022 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/document_factory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      349 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/merge_templates.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      869 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/conditions.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      894 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/file_representation.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      791 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8421 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/content/vocabulary.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8596 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4676 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6108 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/renderer.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1063 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_3.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      939 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_7.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1059 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_8.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      646 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_6.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      865 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_5.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1703 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_9.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1927 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6752 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_base_helper_view.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8713 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/failing_template.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4243 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13802 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_DX_helper_view.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4467 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_demo_profile.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28113 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_generation_view.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1590 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_mailing_loop_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6168 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_vocabulary.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7154 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_pod_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4392 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_templates_listing_view.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2690 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1603 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_sub_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17655 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_configurable_pod_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5241 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      685 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_robot.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10193 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_AT_helper_view.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/robot/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      515 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_style_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9904 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5370 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/profiles.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3568 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1119 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4386 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      624 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/children_pod_template.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8633 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/table.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23051 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/generation_view.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4306 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/controlpanel.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      535 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/doc.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1506 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/libreoffice_icon.xcf
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      826 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/ods.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      569 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/configurable.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/docx.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/rtf.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      562 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/mailinglooptemplate.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      534 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/style.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      483 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/pdf.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      568 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/xls.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      515 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/subtemplate.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/nok.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/odt.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      823 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/ok.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      487 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/podtemplate.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6170 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      819 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/templates_listing.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/overrides.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/resources/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/resources/css/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      777 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/browser/resources/css/documentgenerator.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2952 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/AT_renderer.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      161 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/manual.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13410 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/fr/LC_MESSAGES/collective.documentgenerator.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      579 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9096 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/collective.documentgenerator.pot
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      225 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/documentgenerator/locales/update.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/src/collective/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      390 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/.coveragerc
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      198 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/travis.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2200 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6501 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/bootstrap.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17923 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1773 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/.travis.yml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      864 2019-08-13 07:53:09.000000 collective.documentgenerator-3.8/Makefile
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/developer.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1026 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/technical.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1966 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/user.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14018 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/images/AddPODTTemplateMenu.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2867 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/images/addPloneSite.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18167 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/images/viewlet.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9992 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/docs/images/demoInstal.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3756 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28499 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      163 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/jenkins.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28499 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8917 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      362 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/not-zip-safe
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1815 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/DX_renderer.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      722 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/controlpanel.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      519 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      184 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/browserlayer.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2095 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/PODTemplate.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2281 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/ConfigurablePODTemplate.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2095 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/SubTemplate.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2165 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/StyleTemplate.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2143 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/MailingLoopTemplate.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/testing/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      228 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/testing/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      231 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/testing/propertiestool.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/testing/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3990 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/testing/types/member.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11386 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/possibly_mailed_model.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9209 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/styles_2.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8120 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/modele_general.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8990 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/mailing.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10991 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/modele_general.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    89772 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/sub_template.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9388 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/styles.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12279 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/modèle_collection.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      494 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/collectivedocumentgenerator_demo_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       41 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone4/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      185 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone4/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone4/collectivedocumentgenerator_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      252 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone4/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      371 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone4/cssregistry.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone5/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      185 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone5/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      591 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone5/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5622 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/helper/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      532 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/helper/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2338 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/helper/archetypes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5725 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/helper/dexterity.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1828 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/helper/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9652 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/helper/base.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2434 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/generationlinks.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      556 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/generationlinks.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/batchactions.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      557 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/demo/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/demo/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7182 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/demo/helper.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      872 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/demo/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      497 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/events/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/events/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      831 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/events/pod_templates_events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6020 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/events/styles_events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1222 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/events/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1995 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/file_representation.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1404 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/style_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17758 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/pod_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      277 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/merge_templates.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1739 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/condition.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2710 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/vocabulary.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2022 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/document_factory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      349 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/merge_templates.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      869 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/conditions.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      894 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/file_representation.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      791 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8448 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/content/vocabulary.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8596 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4676 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6108 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/renderer.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1063 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_3.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      939 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_7.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1059 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_8.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      646 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_6.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      865 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_5.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1703 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_9.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1927 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7256 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_base_helper_view.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8713 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/failing_template.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4243 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14040 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_DX_helper_view.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4467 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_demo_profile.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28113 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_generation_view.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1590 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_mailing_loop_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6168 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_vocabulary.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7154 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_pod_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4392 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_templates_listing_view.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2690 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1603 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_sub_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18574 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_configurable_pod_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5241 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      685 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_robot.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10193 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_AT_helper_view.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/robot/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/robot/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      515 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_style_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9904 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5370 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3616 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1119 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4386 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      624 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/children_pod_template.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8633 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/table.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23051 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/generation_view.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4349 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/controlpanel.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      535 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/doc.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1506 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/libreoffice_icon.xcf
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      826 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/ods.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      569 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/configurable.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/docx.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/rtf.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      562 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/mailinglooptemplate.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      534 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/style.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      483 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/pdf.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      568 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/xls.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      515 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/subtemplate.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/nok.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/odt.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      823 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/ok.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      487 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/podtemplate.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6170 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      819 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/templates_listing.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/overrides.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/resources/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/resources/css/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      777 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/browser/resources/css/documentgenerator.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2952 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/AT_renderer.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      161 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/manual.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13410 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/fr/LC_MESSAGES/collective.documentgenerator.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      579 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9096 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/collective.documentgenerator.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      225 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/documentgenerator/locales/update.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/src/collective/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      390 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      198 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/travis.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2080 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6501 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/bootstrap.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18335 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/buildout.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1867 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/.travis.yml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      869 2019-10-14 11:59:36.000000 collective.documentgenerator-3.9/Makefile
```

### Comparing `collective.documentgenerator-3.8/docs/LICENSE.rst` & `collective.documentgenerator-3.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/docs/LICENSE.GPL` & `collective.documentgenerator-3.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/docs/technical.rst` & `collective.documentgenerator-3.9/docs/technical.rst`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/docs/user.rst` & `collective.documentgenerator-3.9/docs/user.rst`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/docs/images/AddPODTTemplateMenu.png` & `collective.documentgenerator-3.9/docs/images/AddPODTTemplateMenu.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/docs/images/addPloneSite.png` & `collective.documentgenerator-3.9/docs/images/addPloneSite.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/docs/images/viewlet.png` & `collective.documentgenerator-3.9/docs/images/viewlet.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/docs/images/demoInstal.png` & `collective.documentgenerator-3.9/docs/images/demoInstal.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/README.rst` & `collective.documentgenerator-3.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/PKG-INFO` & `collective.documentgenerator-3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.documentgenerator
-Version: 3.8
+Version: 3.9
 Summary: Desktop document generation (.odt, .pdf, .doc, ...) based on appy framework (http://appyframework.org) and OpenOffice/LibreOffice
 Home-page: http://pypi.python.org/pypi/collective.documentgenerator
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL
 Description: .. image:: https://travis-ci.org/collective/collective.documentgenerator.svg?branch=master
            :target: https://travis-ci.org/collective/collective.documentgenerator
@@ -105,31 +105,29 @@
         
         * `Source code @ GitHub <https://github.com/collective/collective.documentgenerator.git>`_
         * `Issues @ GitHub <https://github.com/collective/collective.documentgenerator/issues>`_
         * `Continuous Integration @ Travis CI <https://travis-ci.org/collective/collective.documentgenerator>`_
         * `Code Coverage @ Coveralls.io <https://coveralls.io/r/collective/collective.documentgenerator?branch=master>`_
         
         
-        Contributors
-        ============
-        
-        
-        - Simon Delcourt, simon.delcourt@imio.be
-        - Gauthier Bastien, gauthier.bastien@imio.be
-        - Vivian Antoine, vivian.antoine@imio.be
-        - André Nuyens, andre.nuyens@imio.be
-        - Franck NGAHA, franck.ngaha@imio.be
-        - Christophe Boulanger, christophe.boulanger@imio.be
-        - Cédric Messiant, cedricmessiant@ecreall.com
-        - Stephan Geulette, stephan.geulette@imio.be
-        
-        
         Changelog
         =========
         
+        3.9 (2019-10-14)
+        ----------------
+        
+        - context_var returns default when value is None.
+          [sgeulette]
+        - While reusing another POD template odt_file, make sure get_file will have
+          access to the POD template holding the odt_file by getting it unrestricted.
+          [gbastien]
+        - Fixed test `TestDexterityHelperViewMethods.test_display_date_method` as
+          translation format changed starting with `Plone 5.1.x`.
+          [gbastien]
+        
         3.8 (2019-08-13)
         ----------------
         
         - Added custom temporary directory 'CUSTOM_TMP' environment variable
           for appy's workspace.
           [odelaere]
         - Added ability to use an external server process for LibreOffice.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/PKG-INFO` & `collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.documentgenerator
-Version: 3.8
+Version: 3.9
 Summary: Desktop document generation (.odt, .pdf, .doc, ...) based on appy framework (http://appyframework.org) and OpenOffice/LibreOffice
 Home-page: http://pypi.python.org/pypi/collective.documentgenerator
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL
 Description: .. image:: https://travis-ci.org/collective/collective.documentgenerator.svg?branch=master
            :target: https://travis-ci.org/collective/collective.documentgenerator
@@ -105,31 +105,29 @@
         
         * `Source code @ GitHub <https://github.com/collective/collective.documentgenerator.git>`_
         * `Issues @ GitHub <https://github.com/collective/collective.documentgenerator/issues>`_
         * `Continuous Integration @ Travis CI <https://travis-ci.org/collective/collective.documentgenerator>`_
         * `Code Coverage @ Coveralls.io <https://coveralls.io/r/collective/collective.documentgenerator?branch=master>`_
         
         
-        Contributors
-        ============
-        
-        
-        - Simon Delcourt, simon.delcourt@imio.be
-        - Gauthier Bastien, gauthier.bastien@imio.be
-        - Vivian Antoine, vivian.antoine@imio.be
-        - André Nuyens, andre.nuyens@imio.be
-        - Franck NGAHA, franck.ngaha@imio.be
-        - Christophe Boulanger, christophe.boulanger@imio.be
-        - Cédric Messiant, cedricmessiant@ecreall.com
-        - Stephan Geulette, stephan.geulette@imio.be
-        
-        
         Changelog
         =========
         
+        3.9 (2019-10-14)
+        ----------------
+        
+        - context_var returns default when value is None.
+          [sgeulette]
+        - While reusing another POD template odt_file, make sure get_file will have
+          access to the POD template holding the odt_file by getting it unrestricted.
+          [gbastien]
+        - Fixed test `TestDexterityHelperViewMethods.test_display_date_method` as
+          translation format changed starting with `Plone 5.1.x`.
+          [gbastien]
+        
         3.8 (2019-08-13)
         ----------------
         
         - Added custom temporary directory 'CUSTOM_TMP' environment variable
           for appy's workspace.
           [odelaere]
         - Added ability to use an external server process for LibreOffice.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `collective.documentgenerator-3.8/src/collective.documentgenerator.egg-info/SOURCES.txt` & `collective.documentgenerator-3.9/src/collective.documentgenerator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .coveragerc
 .travis.yml
 CHANGES.rst
-CONTRIBUTORS.rst
 MANIFEST.in
 Makefile
 README.rst
 bootstrap.py
 buildout.cfg
 jenkins.cfg
 setup.py
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/DX_renderer.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/DX_renderer.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/controlpanel.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/PODTemplate.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/PODTemplate.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/ConfigurablePODTemplate.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/ConfigurablePODTemplate.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/SubTemplate.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/SubTemplate.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/StyleTemplate.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/StyleTemplate.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/base/types/MailingLoopTemplate.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/base/types/MailingLoopTemplate.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/testing/types/member.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/testing/types/member.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/possibly_mailed_model.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/possibly_mailed_model.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/styles_2.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/styles_2.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/modele_general.ods` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/modele_general.ods`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/mailing.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/mailing.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/modele_general.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/modele_general.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/sub_template.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/sub_template.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/styles.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/styles.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/demo/templates/modèle_collection.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/demo/templates/modèle_collection.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles/plone5/registry.xml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles/plone5/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/utils.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/utils.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/helper/__init__.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/helper/archetypes.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/helper/archetypes.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/helper/dexterity.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/helper/dexterity.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/helper/configure.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/helper/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/helper/base.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/helper/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             wtool = api.portal.get_tool('portal_workflow')
             state = wtool.getTitleForStateOnType(state, obj.portal_type)
         return state
 
     def context_var(self, name, default=''):
         """ Test if a context variable is defined and return it or return default """
         ctx = self.appy_renderer.contentParser.env.context
-        if name in ctx:
+        if name in ctx and ctx[name] is not None:
             return ctx[name]
         else:
             return default
 
     def mailing_list(self, gen_context=None):  # pragma: no cover
         """
             Return a mailing list (that will be added to generation context in "loop" view) to loop on.
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/generationlinks.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/generationlinks.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/generationlinks.pt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/generationlinks.pt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/viewlets/configure.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/demo/helper.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/demo/helper.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/demo/configure.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/demo/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/events/pod_templates_events.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/events/pod_templates_events.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/events/styles_events.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/events/styles_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,34 +67,33 @@
 
 
 def _update_template_styles(pod_template, style_template_filename):
     """
     Update template pod_template by templateStyle.
     """
     # we check if the pod_template has been modified except by style only
-    style_changes_only = pod_template.style_modification_md5 and\
-                         pod_template.current_md5 == pod_template.style_modification_md5
+    style_changes_only = \
+        pod_template.style_modification_md5 and pod_template.current_md5 == pod_template.style_modification_md5
     # save in temporary file, the template
     temp_file = create_temporary_file(pod_template.odt_file, 'pod_template.odt')
     new_template = open(temp_file.name, 'w')
     new_template.write(pod_template.odt_file.data)
     new_template.close()
 
     # merge style from templateStyle in template
     cmd = '{path} {script} {tmp_file} {extension} -e ' \
-          '{libreoffice_host} -p {port} -t {style_template} -v -a {stream}'.format(
-        path=config.get_uno_path(),
-        script=CONVSCRIPT,
-        tmp_file=temp_file.name,
-        extension='odt',
-        libreoffice_host=config.get_oo_server(),
-        port=config.get_oo_port(),
-        style_template=style_template_filename,
-        stream=config.get_use_stream(),
-    )
+          '{libreoffice_host} -p {port} ' \
+          '-t {style_template} -v -a {stream}'.format(path=config.get_uno_path(),
+                                                      script=CONVSCRIPT,
+                                                      tmp_file=temp_file.name,
+                                                      extension='odt',
+                                                      libreoffice_host=config.get_oo_server(),
+                                                      port=config.get_oo_port(),
+                                                      style_template=style_template_filename,
+                                                      stream=config.get_use_stream())
     (stdout, stderr) = executeCommand(cmd.split())
     if stderr:
         logger.error("Error during command '%s'" % cmd)
         logger.error("Error is '%s'" % stderr)
         portal = api.portal.get()
         request = portal.REQUEST
         try:
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/events/configure.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/file_representation.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/file_representation.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/style_template.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/style_template.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/pod_template.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/pod_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,20 @@
 
     def get_file(self):
         """
         Method used in renderer in order to retrieve the odt_file to be used.
         :return: an odt_file field.
         """
         if self.pod_template_to_use:
-            return api.content.get(UID=self.pod_template_to_use).odt_file
+            # make sure we get the POD template holding the odt_file
+            # by searching it unrestrictedly
+            catalog = api.portal.get_tool('portal_catalog')
+            brains = catalog.unrestrictedSearchResults(UID=self.pod_template_to_use)
+            obj = brains[0]._unrestrictedGetObject()
+            return obj.odt_file
         return self.odt_file
 
     def __setattr__(self, key, value):
         if key == 'pod_template_to_use':
             if hasattr(self, 'pod_template_to_use') and self.pod_template_to_use != value:
                 if self.pod_template_to_use:
                     self.del_parent_pod_annotation()
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/condition.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/condition.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/vocabulary.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/document_factory.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/document_factory.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/conditions.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/conditions.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/file_representation.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/file_representation.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/configure.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/content/vocabulary.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/content/vocabulary.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,30 +90,30 @@
         vocabulary = SimpleVocabulary(voc_terms)
 
         return vocabulary
 
 
 class ConfigColumnModifierVocabularyFactory(object):
     """
-    Vocabulary factory for 'optimize_tables' field.
+    Vocabulary factory for control panel 'column_modifier' field.
     """
 
     def __call__(self, context):
         voc_terms = [
             SimpleTerm('disabled', 0, _('Disabled')),
             SimpleTerm('nothing', 1, _('Nothing')),
             SimpleTerm('optimize', 2, _('Optimize')),
             SimpleTerm('distribute', 3, _('Distribute'))]
 
         return SimpleVocabulary(voc_terms)
 
 
 class PodColumnModifierVocabularyFactory(object):
     """
-    Vocabulary factory for 'optimize_tables' field.
+    Vocabulary factory for pod template 'column_modifier' field.
     """
 
     def __call__(self, context):
         # adapt first term value depending on global configuration value
         # get term from global value vocabulary
         vocabulary = queryUtility(
             IVocabularyFactory, 'collective.documentgenerator.ConfigColumnModifier')
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/testing.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/testing.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/interfaces.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/renderer.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/renderer.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_3.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_3.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_7.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_7.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_8.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_8.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_6.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_6.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_5.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_5.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/migrations/migrate_to_9.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/migrations/migrate_to_9.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_setup.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_base_helper_view.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_base_helper_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,21 @@
         generation_context = view._get_generation_context(helper_view, pod_template=pod_template)
         renderer = appy.pod.renderer.Renderer(StringIO(document_template.data), generation_context, 'dummy.odt')
         helper_view._set_appy_renderer(renderer)
 
         # unknown variable
         self.assertEqual(helper_view.context_var('dexter', 'undefined'), 'undefined')
 
+        # None value (after edition, an empty value is replaced by None)
+        pod_template.context_variables = [{'name': u'dexter', 'value': None}]
+        generation_context = view._get_generation_context(helper_view, pod_template=pod_template)
+        renderer = appy.pod.renderer.Renderer(StringIO(document_template.data), generation_context, 'dummy.odt')
+        helper_view._set_appy_renderer(renderer)
+        self.assertEqual(helper_view.context_var('dexter'), '')  # default is '' by default
+
         # add a context variable on pod template
         pod_template.context_variables = [{'name': u'dexter', 'value': u'1'}]
         generation_context = view._get_generation_context(helper_view, pod_template=pod_template)
         renderer = appy.pod.renderer.Renderer(StringIO(document_template.data), generation_context, 'dummy.odt')
         helper_view._set_appy_renderer(renderer)
         self.assertEqual(helper_view.context_var('dexter', 'undefined'), u'1')
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/failing_template.odt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/failing_template.odt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_config.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_DX_helper_view.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_DX_helper_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from collective.documentgenerator.config import HAS_PLONE_5_1
 from collective.documentgenerator.testing import DexterityIntegrationTests
 from plone import api
 from plone.app.testing import login
 from plone.app.textfield.value import RichTextValue
 from plone.autoform.interfaces import READ_PERMISSIONS_KEY
 from plone.behavior.interfaces import IBehavior
 from Products.CMFPlone.utils import safe_unicode
@@ -126,32 +127,42 @@
         result = self.view.display_date(field_name=effective_field_name, time_only=True)
         self.assertEqual(expected_date, result)
         result = self.view.display_date(date=self.content.birth_datetime, time_only=True)
         self.assertEqual(expected_date, result)
 
         # custom_format
         expected_date = '18 yolo 09 yolo 1986'
-        result = self.view.display_date(field_name=effective_field_name, custom_format='%d yolo %m yolo %Y')
+        result = self.view.display_date(
+            field_name=effective_field_name, custom_format='%d yolo %m yolo %Y')
         self.assertEqual(expected_date, result)
-        result = self.view.display_date(date=self.content.birth_datetime, custom_format='%d yolo %m yolo %Y')
+        result = self.view.display_date(
+            date=self.content.birth_datetime, custom_format='%d yolo %m yolo %Y')
         self.assertEqual(expected_date, result)
 
-        expected_date = u'jeu 18 sep 1986'
-        result = self.view.display_date(field_name=effective_field_name, custom_format='%a %d %b %Y',
-                                        target_language='fr')
+        # translation format has changed in Plone5.1+
+        if HAS_PLONE_5_1:
+            expected_date = u'jeu. 18 sept. 1986'
+        else:
+            # Plone4
+            expected_date = u'jeu 18 sep 1986'
+        result = self.view.display_date(
+            field_name=effective_field_name, custom_format='%a %d %b %Y',
+            target_language='fr')
         self.assertEqual(expected_date, result)
 
         expected_date = u'jeudi 18 Septembre 1986'
-        result = self.view.display_date(field_name=effective_field_name, custom_format='%A %d %B %Y',
-                                        target_language='fr', month_lc=False)
+        result = self.view.display_date(
+            field_name=effective_field_name, custom_format='%A %d %B %Y',
+            target_language='fr', month_lc=False)
         self.assertEqual(expected_date, result)
 
         expected_date = u'%Jeudi 18 %B 1986'
-        result = self.view.display_date(field_name=effective_field_name, custom_format='%%%A %d %%B %Y',
-                                        target_language='fr', day_lc=False)
+        result = self.view.display_date(
+            field_name=effective_field_name, custom_format='%%%A %d %%B %Y',
+            target_language='fr', day_lc=False)
         self.assertEqual(expected_date, result)
 
         # date
         self.content.birth_datetime = datetime.date(1986, 9, 18)
         expected_date = u'18/09/1986'
         result = self.view.display_date(field_name=effective_field_name)
         self.assertEqual(expected_date, result)
@@ -168,17 +179,19 @@
         result = self.view.display_date(field_name=effective_field_name, time_only=True)
         self.assertEqual(expected_date, result)
         result = self.view.display_date(date=self.content.birth_datetime, time_only=True)
         self.assertEqual(expected_date, result)
 
         # custom_format
         expected_date = '18 yolo 09 yolo 1986'
-        result = self.view.display_date(field_name=effective_field_name, custom_format='%d yolo %m yolo %Y')
+        result = self.view.display_date(
+            field_name=effective_field_name, custom_format='%d yolo %m yolo %Y')
         self.assertEqual(expected_date, result)
-        result = self.view.display_date(date=self.content.birth_datetime, custom_format='%d yolo %m yolo %Y')
+        result = self.view.display_date(
+            date=self.content.birth_datetime, custom_format='%d yolo %m yolo %Y')
         self.assertEqual(expected_date, result)
 
     def test_display_voc_method(self):
         field_name = 'languages'
         to_set = ('en', 'fr')
         expected = u'English|Français'
         self.content.languages = to_set
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_demo_profile.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_demo_profile.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_generation_view.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_generation_view.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_mailing_loop_template.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_mailing_loop_template.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_vocabulary.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_pod_template.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_pod_template.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_templates_listing_view.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_templates_listing_view.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_events.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_sub_template.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_sub_template.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_configurable_pod_template.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_configurable_pod_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
+
 from Acquisition import aq_base
 from collective.documentgenerator.content.pod_template import IConfigurablePODTemplate
 from collective.documentgenerator.content.pod_template import PodFormatsValidator
 from collective.documentgenerator.interfaces import IPODTemplateCondition
 from collective.documentgenerator.testing import ConfigurablePODTemplateIntegrationTest
 from collective.documentgenerator.testing import TEST_INSTALL_INTEGRATION
 from plone import api
+from Products.CMFCore.permissions import View
+from Products.CMFCore.utils import _checkPermission
 from zope.component import queryMultiAdapter
 from zope.i18n import translate
 from zope.interface import Invalid
 
 import unittest
 
 
@@ -109,14 +112,29 @@
         self.test_podtemplate.odt_file = None
         self.assertEqual(self.test_podtemplate.get_file(), reusable_template.odt_file, msg)
         self.assertEqual(reusable_template.get_file(), reusable_template.odt_file, msg)
         # basic case without reuse
         self.test_podtemplate.pod_template_to_use = None
         self.assertEqual(self.test_podtemplate.get_file(), self.test_podtemplate.odt_file, msg)
 
+    def test_get_file_is_unrestricted(self):
+        """When reusing another POD template odt_file, we will get
+           the odt_file unrestricted in case user would not have access to the POD template."""
+        reusable_template = self.portal.podtemplates.get('test_template_reusable')
+        self.test_podtemplate.pod_template_to_use = reusable_template.UID()
+
+        # make reusable template not accessible
+        reusable_template.manage_permission(View, 'Manager')
+        reusable_template.reindexObjectSecurity()
+
+        # get_file will correctly return the odt_file
+        self.assertFalse(_checkPermission(View, reusable_template))
+        self.assertFalse(self.portal.portal_catalog(UID=reusable_template.UID()))
+        self.assertEqual(self.test_podtemplate.get_file(), reusable_template.odt_file)
+
     def test_generation_condition_registration(self):
         from collective.documentgenerator.content.condition import ConfigurablePODTemplateCondition
 
         context = self.portal
         condition_obj = queryMultiAdapter(
             (self.test_podtemplate, context),
             IPODTemplateCondition,
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_utils.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_robot.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_AT_helper_view.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_AT_helper_view.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/tests/test_style_template.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/tests/test_style_template.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/setuphandlers.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/profiles.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/config.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 POD_FORMATS = ODS_FORMATS + ODT_FORMATS + NEUTRAL_FORMATS
 
 DEFAULT_PYTHON_UNO_PATH = u'/usr/bin/python'
 
 VIEWLET_TYPES = ['PODTemplate', 'ConfigurablePODTemplate']
 
 HAS_PLONE_5 = api.env.plone_version().startswith('5')
+HAS_PLONE_5_1 = api.env.plone_version() > '5.1'
 
 
 def get_uno_path():
     return api.portal.get_registry_record(
         'collective.documentgenerator.browser.controlpanel.IDocumentGeneratorControlPanelSchema.uno_path'
     )
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/configure.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/views.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/children_pod_template.pt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/children_pod_template.pt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/table.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/table.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/generation_view.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/generation_view.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/controlpanel.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/controlpanel.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     )
 
     use_stream = schema.Bool(
         title=_(u'Force communication via in/out stream with LibreOffice.'),
         description=_(u'If enabled, this will force using stream to communicate witth LibreOffice server. '
                       u'This must be true if the LO server is not on localhost or is in a docker container.'),
         required=True,
-        default=True
+        default=bool(os.getenv('USE_STREAM', False) == 'True'),
     )
 
 
 class DocumentGeneratorControlPanelEditForm(RegistryEditForm):
     implements(IDocumentGeneratorSettings)
 
     schema = IDocumentGeneratorControlPanelSchema
```

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/doc.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/doc.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/libreoffice_icon.xcf` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/libreoffice_icon.xcf`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/ods.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/ods.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/configurable.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/configurable.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/docx.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/docx.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/mailinglooptemplate.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/mailinglooptemplate.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/style.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/style.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/xls.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/xls.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/subtemplate.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/subtemplate.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/nok.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/nok.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/odt.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/odt.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/static/ok.png` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/static/ok.png`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/configure.zcml` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/templates_listing.pt` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/templates_listing.pt`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/browser/resources/css/documentgenerator.css` & `collective.documentgenerator-3.9/src/collective/documentgenerator/browser/resources/css/documentgenerator.css`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/AT_renderer.py` & `collective.documentgenerator-3.9/src/collective/documentgenerator/AT_renderer.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/locales/plone.pot` & `collective.documentgenerator-3.9/src/collective/documentgenerator/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/locales/fr/LC_MESSAGES/collective.documentgenerator.po` & `collective.documentgenerator-3.9/src/collective/documentgenerator/locales/fr/LC_MESSAGES/collective.documentgenerator.po`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/locales/fr/LC_MESSAGES/plone.po` & `collective.documentgenerator-3.9/src/collective/documentgenerator/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/src/collective/documentgenerator/locales/collective.documentgenerator.pot` & `collective.documentgenerator-3.9/src/collective/documentgenerator/locales/collective.documentgenerator.pot`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/.coveragerc` & `collective.documentgenerator-3.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/setup.py` & `collective.documentgenerator-3.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,20 @@
 """Installer for the collective.documentgenerator package."""
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 long_description = (
-    open('README.rst').read()
-    + '\n\n' +
-    'Contributors\n'
-    '============\n'
-    + '\n\n' +
-    open('CONTRIBUTORS.rst').read()
-    + '\n\n' +
-    open('CHANGES.rst').read()
-    + '\n\n')
+    open('README.rst').read() + '\n\n' + open('CHANGES.rst').read() + '\n\n')
 
 
 setup(
     name='collective.documentgenerator',
-    version='3.8',
+    version='3.9',
     description="Desktop document generation (.odt, .pdf, .doc, ...) based on appy framework (http://appyframework.org) and OpenOffice/LibreOffice",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `collective.documentgenerator-3.8/bootstrap.py` & `collective.documentgenerator-3.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.documentgenerator-3.8/CHANGES.rst` & `collective.documentgenerator-3.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog
 =========
 
+3.9 (2019-10-14)
+----------------
+
+- context_var returns default when value is None.
+  [sgeulette]
+- While reusing another POD template odt_file, make sure get_file will have
+  access to the POD template holding the odt_file by getting it unrestricted.
+  [gbastien]
+- Fixed test `TestDexterityHelperViewMethods.test_display_date_method` as
+  translation format changed starting with `Plone 5.1.x`.
+  [gbastien]
+
 3.8 (2019-08-13)
 ----------------
 
 - Added custom temporary directory 'CUSTOM_TMP' environment variable
   for appy's workspace.
   [odelaere]
 - Added ability to use an external server process for LibreOffice.
```

### Comparing `collective.documentgenerator-3.8/.travis.yml` & `collective.documentgenerator-3.9/.travis.yml`

 * *Files 16% similar despite different names*

```diff
@@ -33,32 +33,33 @@
   - mkdir $HOME/tmp
   - chmod 777 $HOME/tmp
   - export TMPDIR=$HOME/tmp
   - sed -ie "s#travis-5#travis-$PLONE_VERSION#" travis.cfg
   - pip install lxml --no-binary lxml
   - python -V
   - pip install -r requirements.txt
-  - python bootstrap.py --version=2.11.4
+  - python bootstrap.py --version=2.12.0
   - bin/buildout -N -c travis.cfg annotate
   - bin/buildout -Nt 5 -c travis.cfg
 
 before_script:
   - docker run -p 127.0.0.1:2002:8997 -d --rm --name="oo_server" xcgd/libreoffice:5.1
   - bin/translation-manage -c
 
 script:
   - docker ps
-  - bin/test
+  - env USE_STREAM=True bin/test
   - docker stop oo_server
   - docker run -p 127.0.0.1:2002:8997 -d --rm --name="oo_server" xcgd/libreoffice:latest
   - docker ps
-  - bin/test
+  - env USE_STREAM=True bin/test
   - docker stop oo_server
   - /usr/bin/soffice --invisible --headless --nologo --nofirststartwizard --accept="socket,host=localhost,port=2002;urp" & > /dev/null 2>&1
-  - bin/test
+  - env USE_STREAM=False bin/test
+  - env USE_STREAM=True bin/test
 
 after_success:
   - bin/createcoverage -d htmlcov
   - pip install --upgrade pip
   - pip install -q coveralls==0.5
   - coveralls
```

### Comparing `collective.documentgenerator-3.8/Makefile` & `collective.documentgenerator-3.9/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 lo_version=latest
 
 all: run
 
 .PHONY: bootstrap buildout run test cleanall startlibreoffice stoplibreoffice
 bootstrap:
 	virtualenv-2.7 .
-	pip install -r requirements.txt
-	./bin/python bootstrap.py --version=2.11.4
+	bin/pip install -r requirements.txt
+	./bin/python bootstrap.py --version=2.12.0
 
 buildout:
 	if ! test -f bin/buildout;then make bootstrap;fi
 	bin/buildout -Nt 5
 
 run:
 	if ! test -f bin/instance;then make buildout;fi
@@ -31,8 +31,8 @@
 	rm -fr bin develop-eggs htmlcov include .installed.cfg lib .mr.developer.cfg parts downloads eggs
 
 startlibreoffice:
 	make stoplibreoffice
 	docker run -p 2002:8997 -d --rm --name="oo_server" xcgd/libreoffice:$(lo_version)
 
 stoplibreoffice:
-	if docker ps | grep oo_server;then docker stop oo_server;fi
+	if docker ps | grep oo_server;then docker stop oo_server;fi
```

