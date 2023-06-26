# Comparing `tmp/taxonomy-connector-1.8.0.tar.gz` & `tmp/taxonomy-connector-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxonomy-connector-1.8.0.tar", last modified: Mon Apr 12 07:27:15 2021, max compression
+gzip compressed data, was "taxonomy-connector-1.9.0.tar", last modified: Wed Apr 14 07:02:48 2021, max compression
```

## Comparing `taxonomy-connector-1.8.0.tar` & `taxonomy-connector-1.9.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3833 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    34523 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     8508 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.156855 taxonomy-connector-1.8.0/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/base.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/constraints.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      701 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/dev.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     7027 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/pip-tools.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      324 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/pip-tools.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/test.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2806 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/travis.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      837 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/requirements/travis.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3151 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.156855 taxonomy-connector-1.8.0/taxonomy/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1779 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2893 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9583 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/emsi_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1914 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      519 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.156855 taxonomy-connector-1.8.0/taxonomy/management/
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/management/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.156855 taxonomy-connector-1.8.0/taxonomy/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/management/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2662 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/management/commands/populate_job_names.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3436 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/management/commands/refresh_course_skills.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3594 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/management/commands/refresh_job_postings_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3402 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/management/commands/refresh_job_skills.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/taxonomy/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3141 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2104 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0002_job_jobskills.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2135 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0003_auto_20200916_1019.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      659 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0004_auto_20210113_0452.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0005_blacklistedcourseskill.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      569 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0006_auto_20210128_0135.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0007_delete_all_records.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1337 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0008_auto_20210216_0710.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      465 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0009_skill_description.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      715 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/0010_auto_20210409_0256.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/migrations_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9367 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/taxonomy/providers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      134 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/providers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1490 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/providers/course_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      833 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/providers/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/taxonomy/signals/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/signals/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      570 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/signals/handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/signals/signals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      825 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6860 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/taxonomy/validators/
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/validators/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2150 2021-04-12 07:25:52.000000 taxonomy-connector-1.8.0/taxonomy/validators/course_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-12 07:27:15.160855 taxonomy-connector-1.8.0/taxonomy_connector.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8508 2021-04-12 07:27:15.000000 taxonomy-connector-1.8.0/taxonomy_connector.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1763 2021-04-12 07:27:15.000000 taxonomy-connector-1.8.0/taxonomy_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-12 07:27:15.000000 taxonomy-connector-1.8.0/taxonomy_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2021-04-12 07:27:15.000000 taxonomy-connector-1.8.0/taxonomy_connector.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-04-12 07:27:15.000000 taxonomy-connector-1.8.0/taxonomy_connector.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.964844 taxonomy-connector-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3968 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/CHANGELOG.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34523 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8683 2021-04-14 07:02:48.964844 taxonomy-connector-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.956843 taxonomy-connector-1.9.0/requirements/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      107 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/base.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/constraints.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      701 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/dev.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7027 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/pip-tools.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      324 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/pip-tools.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/test.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2806 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/test.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/travis.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      837 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/requirements/travis.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      118 2021-04-14 07:02:48.964844 taxonomy-connector-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3151 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.960844 taxonomy-connector-1.9.0/taxonomy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1781 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/admin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2893 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9583 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/emsi_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1914 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      519 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.960844 taxonomy-connector-1.9.0/taxonomy/management/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/management/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.960844 taxonomy-connector-1.9.0/taxonomy/management/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/management/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2662 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/management/commands/populate_job_names.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3436 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/management/commands/refresh_course_skills.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3594 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/management/commands/refresh_job_postings_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3402 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/management/commands/refresh_job_skills.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.960844 taxonomy-connector-1.9.0/taxonomy/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3141 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2104 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0002_job_jobskills.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2135 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0003_auto_20200916_1019.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      659 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0004_auto_20210113_0452.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0005_blacklistedcourseskill.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      569 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0006_auto_20210128_0135.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      335 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0007_delete_all_records.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1337 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0008_auto_20210216_0710.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      465 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0009_skill_description.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      715 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0010_auto_20210409_0256.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0011_auto_20210412_0241.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      616 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/0012_auto_20210412_0424.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      382 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/migrations_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9285 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.964844 taxonomy-connector-1.9.0/taxonomy/providers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      134 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/providers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1490 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/providers/course_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      833 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/providers/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.964844 taxonomy-connector-1.9.0/taxonomy/signals/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/signals/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      570 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/signals/handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      155 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/signals/signals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      825 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/tasks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6865 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.964844 taxonomy-connector-1.9.0/taxonomy/validators/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      140 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/validators/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2150 2021-04-14 07:01:26.000000 taxonomy-connector-1.9.0/taxonomy/validators/course_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-14 07:02:48.964844 taxonomy-connector-1.9.0/taxonomy_connector.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8683 2021-04-14 07:02:48.000000 taxonomy-connector-1.9.0/taxonomy_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2021-04-14 07:02:48.000000 taxonomy-connector-1.9.0/taxonomy_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-14 07:02:48.000000 taxonomy-connector-1.9.0/taxonomy_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      107 2021-04-14 07:02:48.000000 taxonomy-connector-1.9.0/taxonomy_connector.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-04-14 07:02:48.000000 taxonomy-connector-1.9.0/taxonomy_connector.egg-info/top_level.txt
```

### Comparing `taxonomy-connector-1.8.0/CHANGELOG.rst` & `taxonomy-connector-1.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,19 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 --------------------
 
+[1.9.0] - 2021-04-12
+--------------------
+
+* Replace the usages of old `course_id` in `CourseSkills` with the new `course_key` field.
+
 [1.8.0] - 2021-04-09
 --------------------
 
 * Added a new field named `course_key` in `CourseSkills` model to deprecate and replace the old `course_id` field in future.
 
 [1.7.0] - 2021-04-07
 --------------------
```

### Comparing `taxonomy-connector-1.8.0/LICENSE` & `taxonomy-connector-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/PKG-INFO` & `taxonomy-connector-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: taxonomy-connector
-Version: 1.8.0
+Version: 1.9.0
 Summary: Taxonomy connector
 Home-page: https://github.com/edx/taxonomy-connector
 Author: edX
 Author-email: oscm@edx.org
 License: MIT
 Description: Taxonomy
         ========
@@ -81,14 +81,19 @@
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         --------------------
         
+        [1.9.0] - 2021-04-12
+        --------------------
+        
+        * Replace the usages of old `course_id` in `CourseSkills` with the new `course_key` field.
+        
         [1.8.0] - 2021-04-09
         --------------------
         
         * Added a new field named `course_key` in `CourseSkills` model to deprecate and replace the old `course_id` field in future.
         
         [1.7.0] - 2021-04-07
         --------------------
```

### Comparing `taxonomy-connector-1.8.0/README.rst` & `taxonomy-connector-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/requirements/constraints.txt` & `taxonomy-connector-1.9.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/requirements/dev.in` & `taxonomy-connector-1.9.0/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/requirements/dev.txt` & `taxonomy-connector-1.9.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/requirements/test.in` & `taxonomy-connector-1.9.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/requirements/test.txt` & `taxonomy-connector-1.9.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/requirements/travis.txt` & `taxonomy-connector-1.9.0/requirements/travis.txt`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/setup.py` & `taxonomy-connector-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/__init__.py` & `taxonomy-connector-1.9.0/taxonomy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 
 # taxonomy service follows semantic versioning specifications,
 # A version number is of the form `MAJOR.MINOR.PATCH`, where
 # 1. MAJOR version when you make incompatible API changes,
 # 2. MINOR version when you add functionality in a backwards compatible manner, and
 # 3. PATCH version when you make backwards compatible bug fixes.
 # More details can be found at https://semver.org/
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 
 default_app_config = 'taxonomy.apps.TaxonomyConfig'  # pylint: disable=invalid-name
```

### Comparing `taxonomy-connector-1.8.0/taxonomy/admin.py` & `taxonomy-connector-1.9.0/taxonomy/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
 @admin.register(CourseSkills)
 class CourseSkillsTitleAdmin(admin.ModelAdmin):
     """
     Administrative view for Course Skills.
     """
 
-    list_display = ('id', 'course_id', 'created', 'modified')
-    search_fields = ('course_id',)
+    list_display = ('id', 'course_key', 'created', 'modified')
+    search_fields = ('course_key',)
 
     def save_model(self, request, obj, form, change):
         """
-        Set `course_key` to the same value as `course_id` before saving the model.
+        Set `course_id` to the same value as `course_key` before saving the model.
         """
-        obj.course_key = obj.course_id
+        obj.course_id = obj.course_key
         super().save_model(request, obj, form, change)
 
 
 @admin.register(Job)
 class JobAdmin(admin.ModelAdmin):
     """
     Administrative view for Jobs.
```

### Comparing `taxonomy-connector-1.8.0/taxonomy/constants.py` & `taxonomy-connector-1.9.0/taxonomy/constants.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/emsi_client.py` & `taxonomy-connector-1.9.0/taxonomy/emsi_client.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/enums.py` & `taxonomy-connector-1.9.0/taxonomy/enums.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/exceptions.py` & `taxonomy-connector-1.9.0/taxonomy/exceptions.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/management/commands/populate_job_names.py` & `taxonomy-connector-1.9.0/taxonomy/management/commands/populate_job_names.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/management/commands/refresh_course_skills.py` & `taxonomy-connector-1.9.0/taxonomy/management/commands/refresh_course_skills.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/management/commands/refresh_job_postings_data.py` & `taxonomy-connector-1.9.0/taxonomy/management/commands/refresh_job_postings_data.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/management/commands/refresh_job_skills.py` & `taxonomy-connector-1.9.0/taxonomy/management/commands/refresh_job_skills.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0001_initial.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0002_job_jobskills.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0002_job_jobskills.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0003_auto_20200916_1019.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0003_auto_20200916_1019.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0004_auto_20210113_0452.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0004_auto_20210113_0452.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0005_blacklistedcourseskill.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0005_blacklistedcourseskill.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0006_auto_20210128_0135.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0006_auto_20210128_0135.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0008_auto_20210216_0710.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0008_auto_20210216_0710.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/migrations/0010_auto_20210409_0256.py` & `taxonomy-connector-1.9.0/taxonomy/migrations/0010_auto_20210409_0256.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/models.py` & `taxonomy-connector-1.9.0/taxonomy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,20 +97,15 @@
         blank=False,
         help_text=_(
             'The ID of the course whose text was used for skills extraction.'
         )
     )
     course_key = models.CharField(
         max_length=255,
-        blank=True,
-        null=True,
-        editable=False,
-        help_text=_(
-            'The key of the course whose text was used for skills extraction.'
-        )
+        help_text=_('The key of the course whose text was used for skills extraction.')
     )
     skill = models.ForeignKey(
         Skill,
         blank=False,
         null=False,
         on_delete=models.deletion.CASCADE,
         help_text=_(
@@ -133,21 +128,21 @@
         Meta configuration for CourseSkills model.
         """
 
         verbose_name = 'Course Skill'
         verbose_name_plural = 'Course Skills'
         ordering = ('created', )
         app_label = 'taxonomy'
-        unique_together = ('course_id', 'skill')
+        unique_together = ('course_key', 'skill')
 
     def __str__(self):
         """
         Create a human-readable string representation of the object.
         """
-        return '<CourseSkills name="{}" course_id="{}">'.format(self.skill.name, self.course_id)
+        return '<CourseSkills name="{}" course_key="{}">'.format(self.skill.name, self.course_key)
 
     def __repr__(self):
         """
         Create a unique string representation of the object.
         """
         return '<CourseSkills id="{0}" skill="{1!r}">'.format(self.id, self.skill)
```

### Comparing `taxonomy-connector-1.8.0/taxonomy/providers/course_metadata.py` & `taxonomy-connector-1.9.0/taxonomy/providers/course_metadata.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/providers/utils.py` & `taxonomy-connector-1.9.0/taxonomy/providers/utils.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/signals/handlers.py` & `taxonomy-connector-1.9.0/taxonomy/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/tasks.py` & `taxonomy-connector-1.9.0/taxonomy/tasks.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy/utils.py` & `taxonomy-connector-1.9.0/taxonomy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     """
     Persist the skills data in the database.
     """
     skill, __ = Skill.objects.update_or_create(external_id=skill_external_id, defaults=skill_data)
 
     if not is_course_skill_blacklisted(course_key, skill.id):
         CourseSkills.objects.update_or_create(
-            course_id=course_key,
+            course_key=course_key,
             skill=skill,
             defaults={
                 'confidence': confidence,
-                'course_key': course_key,
+                'course_id': course_key,
             },
         )
 
 
 def process_skills_data(course, course_skills, should_commit_to_db):
     """
     Process skills data returned by the EMSI service and update databased.
@@ -116,29 +116,29 @@
     Blacklist a course skill.
 
     Arguments:
         course_key (CourseKey): CourseKey object pointing to the course whose skill need to be black-listed.
         skill_id (int): Primary key identifier of the skill that need to be blacklisted.
     """
     CourseSkills.objects.filter(
-        course_id=course_key,
+        course_key=course_key,
         skill_id=skill_id,
     ).update(is_blacklisted=True)
 
 
 def remove_course_skill_from_blacklist(course_key, skill_id):
     """
     Remove a course skill from the blacklist.
 
     Arguments:
         course_key (CourseKey): CourseKey object pointing to the course whose skill need to be black-listed.
         skill_id (int): Primary key identifier of the skill that need to be blacklisted.
     """
     CourseSkills.objects.filter(
-        course_id=course_key,
+        course_key=course_key,
         skill_id=skill_id,
     ).update(is_blacklisted=False)
 
 
 def is_course_skill_blacklisted(course_key, skill_id):
     """
     Return the black listed status of a course skill.
@@ -147,15 +147,15 @@
         course_key (CourseKey): CourseKey object pointing to the course whose skill need to be checked.
         skill_id (int): Primary key identifier of the skill that need to be checked.
 
     Returns:
         (bool): True if course-skill (identified by the arguments) is black-listed, False otherwise.
     """
     return CourseSkills.objects.filter(
-        course_id=course_key,
+        course_key=course_key,
         skill_id=skill_id,
         is_blacklisted=True,
     ).exists()
 
 
 def get_whitelisted_course_skills(course_key, prefetch_skills=True):
     """
@@ -164,15 +164,15 @@
     Arguments:
         course_key (str): Key of the course whose course skills need to be returned.
         prefetch_skills (bool): If True, Prefetch related skills in a single query using Django's select_related.
 
     Returns:
         (list<CourseSkills>): A list of all the course skills that are not blacklisted.
     """
-    qs = CourseSkills.objects.filter(course_id=course_key, is_blacklisted=False)
+    qs = CourseSkills.objects.filter(course_key=course_key, is_blacklisted=False)
     if prefetch_skills:
         qs = qs.select_related('skill')
     return qs.all()
 
 
 def get_blacklisted_course_skills(course_key, prefetch_skills=True):
     """
@@ -181,11 +181,11 @@
     Arguments:
         course_key (str): Key of the course whose course skills need to be returned.
         prefetch_skills (bool): If True, Prefetch related skills in a single query using Django's select_related.
 
     Returns:
         (list<CourseSkills>): A list of all the course skills that are blacklisted.
     """
-    qs = CourseSkills.objects.filter(course_id=course_key, is_blacklisted=True)
+    qs = CourseSkills.objects.filter(course_key=course_key, is_blacklisted=True)
     if prefetch_skills:
         qs = qs.select_related('skill')
     return qs.all()
```

### Comparing `taxonomy-connector-1.8.0/taxonomy/validators/course_metadata.py` & `taxonomy-connector-1.9.0/taxonomy/validators/course_metadata.py`

 * *Files identical despite different names*

### Comparing `taxonomy-connector-1.8.0/taxonomy_connector.egg-info/PKG-INFO` & `taxonomy-connector-1.9.0/taxonomy_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: taxonomy-connector
-Version: 1.8.0
+Version: 1.9.0
 Summary: Taxonomy connector
 Home-page: https://github.com/edx/taxonomy-connector
 Author: edX
 Author-email: oscm@edx.org
 License: MIT
 Description: Taxonomy
         ========
@@ -81,14 +81,19 @@
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         --------------------
         
+        [1.9.0] - 2021-04-12
+        --------------------
+        
+        * Replace the usages of old `course_id` in `CourseSkills` with the new `course_key` field.
+        
         [1.8.0] - 2021-04-09
         --------------------
         
         * Added a new field named `course_key` in `CourseSkills` model to deprecate and replace the old `course_id` field in future.
         
         [1.7.0] - 2021-04-07
         --------------------
```

### Comparing `taxonomy-connector-1.8.0/taxonomy_connector.egg-info/SOURCES.txt` & `taxonomy-connector-1.9.0/taxonomy_connector.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 taxonomy/migrations/0004_auto_20210113_0452.py
 taxonomy/migrations/0005_blacklistedcourseskill.py
 taxonomy/migrations/0006_auto_20210128_0135.py
 taxonomy/migrations/0007_delete_all_records.py
 taxonomy/migrations/0008_auto_20210216_0710.py
 taxonomy/migrations/0009_skill_description.py
 taxonomy/migrations/0010_auto_20210409_0256.py
+taxonomy/migrations/0011_auto_20210412_0241.py
+taxonomy/migrations/0012_auto_20210412_0424.py
 taxonomy/migrations/__init__.py
 taxonomy/providers/__init__.py
 taxonomy/providers/course_metadata.py
 taxonomy/providers/utils.py
 taxonomy/signals/__init__.py
 taxonomy/signals/handlers.py
 taxonomy/signals/signals.py
```

