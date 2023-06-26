# Comparing `tmp/magic-folder-23.5.0.tar.gz` & `tmp/magic-folder-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-folder-23.5.0.tar", last modified: Tue May  2 18:45:15 2023, max compression
+gzip compressed data, was "magic-folder-23.6.0.tar", last modified: Mon Jun 26 06:33:02 2023, max compression
```

## Comparing `magic-folder-23.5.0.tar` & `magic-folder-23.6.0.tar`

### file list

```diff
@@ -1,672 +1,680 @@
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      207 2022-02-03 01:05:52.000000 magic-folder-23.5.0/.coveragerc
--rw-r--r--   0 meejah    (1000) meejah    (1000)      324 2022-09-20 06:29:38.000000 magic-folder-23.5.0/.flake8
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.193878 magic-folder-23.5.0/.github/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:36:41.000000 magic-folder-23.5.0/.github/pull_request_template.md
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.193878 magic-folder-23.5.0/.github/workflows/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      935 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/codechecks.yml
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4319 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/linux.yml
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3192 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/macos.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3231 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/windows.yml
--rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2022-08-04 09:11:55.000000 magic-folder-23.5.0/.gitignore
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24277 2020-02-04 18:00:11.000000 magic-folder-23.5.0/COPYING.GPL
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17300 2020-02-04 18:00:11.000000 magic-folder-23.5.0/COPYING.TGPPL.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4840 2020-02-04 18:00:11.000000 magic-folder-23.5.0/CREDITS
--rw-r--r--   0 meejah    (1000) meejah    (1000)    10046 2023-03-16 04:36:41.000000 magic-folder-23.5.0/DEVELOPERS
--rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2022-09-20 06:29:38.000000 magic-folder-23.5.0/MANIFEST.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2242 2023-05-02 18:43:42.000000 magic-folder-23.5.0/Makefile
--rw-r--r--   0 meejah    (1000) meejah    (1000)    25457 2023-05-02 18:45:12.000000 magic-folder-23.5.0/NEWS.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7592 2021-07-26 20:37:49.000000 magic-folder-23.5.0/NOTES.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-05-02 18:45:15.309878 magic-folder-23.5.0/PKG-INFO
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5496 2023-02-07 22:05:58.000000 magic-folder-23.5.0/README.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/.hypothesis/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/.hypothesis/examples/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/25667fd10de02221/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.5.0/docs/.hypothesis/examples/25667fd10de02221/394341b7182cd227
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/26099471863eabde/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:34.000000 magic-folder-23.5.0/docs/.hypothesis/examples/26099471863eabde/394341b7182cd227
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/26b950c63ef40743/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:27.000000 magic-folder-23.5.0/docs/.hypothesis/examples/26b950c63ef40743/2cd852709fc7beda
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/27a267c0b163fc05/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:31.000000 magic-folder-23.5.0/docs/.hypothesis/examples/27a267c0b163fc05/2cd852709fc7beda
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/2bdd697e3cea2a04/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2023-03-16 04:52:44.000000 magic-folder-23.5.0/docs/.hypothesis/examples/2bdd697e3cea2a04/f4644a30270a4ea6
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/3674e9cecacd98c9/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:28.000000 magic-folder-23.5.0/docs/.hypothesis/examples/3674e9cecacd98c9/2cd852709fc7beda
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/532c4ead6274d000/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      212 2023-03-16 04:52:28.000000 magic-folder-23.5.0/docs/.hypothesis/examples/532c4ead6274d000/42e9ca500f868ebd
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/5ac28ffd404dc215/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        5 2023-03-16 04:52:38.000000 magic-folder-23.5.0/docs/.hypothesis/examples/5ac28ffd404dc215/68e09c5bfbe3cdbe
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/704d1edf754e9033/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       20 2023-03-16 04:52:39.000000 magic-folder-23.5.0/docs/.hypothesis/examples/704d1edf754e9033/d0ff8af3e4baa190
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/9e68e03a9abe82a7/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       11 2023-03-16 04:52:30.000000 magic-folder-23.5.0/docs/.hypothesis/examples/9e68e03a9abe82a7/d271b3d8c89fbe5f
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/b069c007d3e9f6fb/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       24 2023-03-16 04:52:38.000000 magic-folder-23.5.0/docs/.hypothesis/examples/b069c007d3e9f6fb/eaef33fe07ad3597
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/c06175530ec95812/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      238 2023-03-16 04:52:45.000000 magic-folder-23.5.0/docs/.hypothesis/examples/c06175530ec95812/fd83ff26e80c6fad
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/e1ab432a194b3b87/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.5.0/docs/.hypothesis/examples/e1ab432a194b3b87/394341b7182cd227
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/.hypothesis/unicode_data/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/unicode_data/13.0.0/
--rw-------   0 meejah    (1000) meejah    (1000)    20988 2023-03-16 04:52:30.000000 magic-folder-23.5.0/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/CODE_OF_CONDUCT.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      634 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/Makefile
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/_build/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.209878 magic-folder-23.5.0/docs/_build/doctrees/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14226 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/CODE_OF_CONDUCT.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9338 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/backdoors.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    38021 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/config.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    43869 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/datamodel.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    31814 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/development.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    33138 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/downloader.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)  1261313 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13136 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/index.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    66571 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/interface.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    54817 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/invites.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    59020 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/leif-design.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11222 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/limitations.doctree
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.209878 magic-folder-23.5.0/docs/_build/doctrees/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18815 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/conflict-api.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4250 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/index.doctree
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.209878 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18656 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)   178832 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    32883 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19020 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/recovery.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    37513 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/scanning-for-changes.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11826 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/release-process.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)   182197 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/releases.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23355 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/snapshots.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    42464 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/usage.doctree
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.213878 magic-folder-23.5.0/docs/_build/html/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      230 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/.buildinfo
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11411 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/CODE_OF_CONDUCT.html
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.213878 magic-folder-23.5.0/docs/_build/html/_images/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    27173 2023-03-16 20:16:58.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model--high-level.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)    30197 2023-03-17 00:18:54.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24088 2023-03-16 21:22:18.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)   436150 2023-03-17 00:06:11.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model.svg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_sources/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.5.0/docs/_build/html/_sources/backdoors.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7226 2023-03-16 08:24:55.000000 magic-folder-23.5.0/docs/_build/html/_sources/config.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11620 2023-03-17 00:18:36.000000 magic-folder-23.5.0/docs/_build/html/_sources/datamodel.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/_build/html/_sources/development.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.5.0/docs/_build/html/_sources/downloader.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2023-03-16 20:41:52.000000 magic-folder-23.5.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15051 2023-03-16 08:24:55.000000 magic-folder-23.5.0/docs/_build/html/_sources/interface.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-02-16 06:39:44.000000 magic-folder-23.5.0/docs/_build/html/_sources/invites.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17077 2023-03-16 20:45:29.000000 magic-folder-23.5.0/docs/_build/html/_sources/leif-design.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/_build/html/_sources/limitations.rst.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_sources/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/conflict-api.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      612 2023-03-16 20:41:30.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/index.rst.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/recovery.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/release-process.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/releases.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/snapshots.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-03-16 20:45:54.000000 magic-folder-23.5.0/docs/_build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_static/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14813 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.225878 magic-folder-23.5.0/docs/_build/html/_static/css/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3229 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.229878 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    87624 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)    67312 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)    86288 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)    66444 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   165742 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 meejah    (1000) meejah    (1000)   444379 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)   165548 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 meejah    (1000) meejah    (1000)    98024 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)    77160 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   323344 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   193308 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   309728 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   184912 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   328412 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   195704 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   309192 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   182708 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   135235 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/_build/html/_static/custom.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4472 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)      418 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)      286 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/file.png
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.229878 magic-folder-23.5.0/docs/_build/html/_static/js/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      934 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4370 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2734 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5023 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4758 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4846 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18215 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4712 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8183 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/backdoors.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19001 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/config.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23764 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/datamodel.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20860 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/development.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18079 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/downloader.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5143 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/genindex.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11167 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/index.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    44501 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/interface.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    35282 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/invites.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    30106 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/leif-design.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7597 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/limitations.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1120 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/objects.inv
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.229878 magic-folder-23.5.0/docs/_build/html/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16640 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/conflict-api.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8297 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/index.html
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14301 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/filesystem-integration.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    73834 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20764 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/user-interface-design.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16041 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/recovery.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19921 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/scanning-for-changes.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9495 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/release-process.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    51586 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/releases.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5542 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/search.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    63003 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/searchindex.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15500 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/snapshots.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    29531 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/usage.html
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_static/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/_static/.empty
--rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/_static/custom.css
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_templates/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/_templates/.empty
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_trial_temp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/_trial_marker
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/file
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/file
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/file
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      284 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      289 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      285 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_client_endpoint
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        6 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/h87a74R8VavQbimAtmp
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      273 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      275 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       12 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/api_client_endpoint
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       10 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      448 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      447 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      434 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.265878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      451 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.265878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:57.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:57.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      437 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.185878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/tahoe.cfg
--rw-r--r--   0 meejah    (1000) meejah    (1000)       41 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/test.log
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.5.0/docs/backdoors.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9480 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/conf.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7228 2023-05-02 17:54:21.000000 magic-folder-23.5.0/docs/config.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/development.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.5.0/docs/downloader.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)   664833 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/eliot.log
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2973 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/index.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14816 2023-05-02 17:54:21.000000 magic-folder-23.5.0/docs/interface.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14482 2022-11-11 00:40:27.000000 magic-folder-23.5.0/docs/invite-diagram-readonly.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1230 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/invite-diagram-readonly.seqdiag
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16247 2023-01-07 21:02:05.000000 magic-folder-23.5.0/docs/invite-diagram.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1229 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/invite-diagram.seqdiag
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-02-16 06:39:44.000000 magic-folder-23.5.0/docs/invites.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/limitations.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.277878 magic-folder-23.5.0/docs/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24834 2021-06-11 15:26:48.000000 magic-folder-23.5.0/docs/proposed/LightweightDesignscanfornewfiles.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/proposed/conflict-api.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      659 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/proposed/index.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.277878 magic-folder-23.5.0/docs/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/proposed/magic-folder/filesystem-integration.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18174 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/proposed/magic-folder/multi-party-conflict-detection.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.5.0/docs/proposed/magic-folder/remote-to-local-sync.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/proposed/magic-folder/user-interface-design.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)   257416 2021-06-11 16:23:59.000000 magic-folder-23.5.0/docs/proposed/markdown
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/proposed/recovery.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/proposed/scanning-for-changes.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/release-process.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/releases.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/snapshots.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/usage.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/integration/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-07-26 20:37:49.000000 magic-folder-23.5.0/integration/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2021-06-22 06:43:35.000000 magic-folder-23.5.0/integration/bar
--rw-r--r--   0 meejah    (1000) meejah    (1000)    12174 2023-04-29 14:16:49.000000 magic-folder-23.5.0/integration/conftest.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9445 2020-06-25 22:39:41.000000 magic-folder-23.5.0/integration/conftest.py.orig
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2110 2021-06-22 06:43:20.000000 magic-folder-23.5.0/integration/foo
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1780 2021-12-21 23:52:48.000000 magic-folder-23.5.0/integration/log.integ
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-06-22 06:45:13.000000 magic-folder-23.5.0/integration/pytest.log
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4271 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/test_add.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2758 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/test_general_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2802 2023-02-16 06:39:44.000000 magic-folder-23.5.0/integration/test_invite.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3363 2023-05-02 17:54:21.000000 magic-folder-23.5.0/integration/test_kitties.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2312 2023-02-07 22:05:58.000000 magic-folder-23.5.0/integration/test_list.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      592 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/test_magic_folder.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16384 2020-06-25 22:17:40.000000 magic-folder-23.5.0/integration/test_magic_folder.py.orig
--rw-r--r--   0 meejah    (1000) meejah    (1000)    10302 2020-06-25 22:39:42.000000 magic-folder-23.5.0/integration/test_magic_folder.py.rej
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5711 2023-05-02 18:43:42.000000 magic-folder-23.5.0/integration/test_multiuser.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2846 2023-05-02 17:54:21.000000 magic-folder-23.5.0/integration/test_same_files.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1977 2023-05-02 17:54:21.000000 magic-folder-23.5.0/integration/test_status.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23667 2023-04-18 02:49:28.000000 magic-folder-23.5.0/integration/test_synchronize.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4367 2023-02-07 22:05:58.000000 magic-folder-23.5.0/integration/test_tahoe_objects.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    47467 2023-05-02 18:43:42.000000 magic-folder-23.5.0/integration/util.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23625 2020-06-25 22:17:40.000000 magic-folder-23.5.0/integration/util.py.orig
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5425 2020-06-25 22:39:43.000000 magic-folder-23.5.0/integration/util.py.rej
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.185878 magic-folder-23.5.0/misc/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/misc/build_helpers/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2889 2022-08-04 09:11:55.000000 magic-folder-23.5.0/misc/build_helpers/platform-pins.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3919 2021-11-25 22:22:35.000000 magic-folder-23.5.0/misc/build_helpers/run-deprecations.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      228 2021-11-25 22:22:35.000000 magic-folder-23.5.0/misc/build_helpers/sqlite_version.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2475 2023-01-20 00:19:51.000000 magic-folder-23.5.0/misc/build_helpers/update-version.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/misc/coding_tools/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      807 2021-07-26 20:37:49.000000 magic-folder-23.5.0/misc/coding_tools/check-debugging.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/newsfragments/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2022-09-20 06:29:38.000000 magic-folder-23.5.0/newsfragments/.keep-directory
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1455 2022-09-20 06:29:38.000000 magic-folder-23.5.0/pyproject.toml
--rw-r--r--   0 meejah    (1000) meejah    (1000)      287 2021-08-27 20:55:28.000000 magic-folder-23.5.0/pytest.ini
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.289878 magic-folder-23.5.0/requirements/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      443 2021-11-25 22:22:35.000000 magic-folder-23.5.0/requirements/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2023-01-30 21:42:35.000000 magic-folder-23.5.0/requirements/base.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)    44868 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/base.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      254 2022-09-20 06:29:38.000000 magic-folder-23.5.0/requirements/build.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11012 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/build.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3489 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/platform.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2022-09-20 06:29:38.000000 magic-folder-23.5.0/requirements/tahoe-integration-1.17.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/tahoe-integration-1.18.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       67 2021-07-26 20:37:49.000000 magic-folder-23.5.0/requirements/tahoe-integration-master.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      827 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/test.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16621 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/test.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       48 2022-08-04 09:11:55.000000 magic-folder-23.5.0/requirements/tox.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)      949 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/tox.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       38 2023-05-02 18:45:15.309878 magic-folder-23.5.0/setup.cfg
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2661 2022-09-20 06:29:38.000000 magic-folder-23.5.0/setup.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.189878 magic-folder-23.5.0/src/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.297878 magic-folder-23.5.0/src/magic_folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      123 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      152 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/__main__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1171 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/_coverage.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1670 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/_endpoint_parser.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5780 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/_schema.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      162 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder/_version.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20176 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/api_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    38333 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13666 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/client.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5264 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    78056 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/config.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    22660 2023-05-02 18:43:42.000000 magic-folder-23.5.0/src/magic_folder/downloader.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2741 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/endpoints.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1611 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/initialize.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20672 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/invite.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/join.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2173 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/list.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    47419 2023-05-02 18:43:42.000000 magic-folder-23.5.0/src/magic_folder/magic_file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18012 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/magic_folder.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      539 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/magicpath.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2786 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/migrate.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13438 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/participants.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4142 2023-01-20 00:19:51.000000 magic-folder-23.5.0/src/magic_folder/pid.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9328 2023-02-08 01:51:42.000000 magic-folder-23.5.0/src/magic_folder/scanner.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18416 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/service.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1286 2023-02-16 06:39:44.000000 magic-folder-23.5.0/src/magic_folder/show_config.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23391 2023-04-21 21:55:43.000000 magic-folder-23.5.0/src/magic_folder/snapshot.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    21598 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/status.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14506 2023-02-17 18:23:28.000000 magic-folder-23.5.0/src/magic_folder/tahoe_client.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/test/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3189 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      849 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/agentutil.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/test/cli/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.5.0/src/magic_folder/test/cli/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6104 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/cli/common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4451 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/cli/test_api_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24283 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/cli/test_magic_folder.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6801 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4962 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/eliotutil.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16684 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/fixtures.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5130 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/matchers.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/test/plugins/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      334 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/plugins/magic_folder_tests_dropin.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    12527 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/strategies.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    26838 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_api_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    22808 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4839 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_client.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4663 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    49601 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_config.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    73041 2023-05-02 18:43:42.000000 magic-folder-23.5.0/src/magic_folder/test/test_download.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5476 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_eliotutil.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1281 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_endpoints.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1188 2022-03-15 06:53:54.000000 magic-folder-23.5.0/src/magic_folder/test/test_foo.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    28373 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_invite.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11803 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_local_snapshot.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    10182 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_magic_file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8112 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_magic_folder_service.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1199 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_magicpath.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17352 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_participants.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4646 2023-01-20 00:19:51.000000 magic-folder-23.5.0/src/magic_folder/test/test_pid.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15544 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_scanner.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7004 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/test/test_schema.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8026 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_service.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18979 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_snapshot.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    10854 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_status.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2040 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_strategies.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    12958 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_tahoe_client.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5832 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_testing.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    25929 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_upload.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2532 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_util_database.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4535 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_util_file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6446 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_util_twisted.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    80071 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_web.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/testing/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-07-07 16:51:27.000000 magic-folder-23.5.0/src/magic_folder/testing/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18739 2023-01-30 21:42:35.000000 magic-folder-23.5.0/src/magic_folder/testing/web.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    12645 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/uploader.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/util/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.5.0/src/magic_folder/util/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6852 2023-04-22 08:12:52.000000 magic-folder-23.5.0/src/magic_folder/util/capabilities.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5603 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/database.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9471 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/eliotutil.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      617 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/encoding.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2473 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1403 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/observer.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6547 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/twisted.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2176 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/wrap.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    30795 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/web.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.297878 magic-folder-23.5.0/src/magic_folder.egg-info/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/PKG-INFO
--rw-r--r--   0 meejah    (1000) meejah    (1000)    31307 2023-05-02 18:45:15.000000 magic-folder-23.5.0/src/magic_folder.egg-info/SOURCES.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)        1 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/dependency_links.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      104 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/entry_points.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      532 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/requires.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       21 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/top_level.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.189878 magic-folder-23.5.0/src/twisted/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/twisted/plugins/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      301 2021-07-26 20:37:49.000000 magic-folder-23.5.0/src/twisted/plugins/magic_folder_dropin.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5616 2023-02-07 22:05:58.000000 magic-folder-23.5.0/tox.ini
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.393074 magic-folder-23.6.0/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      207 2022-02-03 01:05:52.000000 magic-folder-23.6.0/.coveragerc
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      324 2022-09-20 06:29:38.000000 magic-folder-23.6.0/.flake8
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.265075 magic-folder-23.6.0/.github/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:27:27.000000 magic-folder-23.6.0/.github/pull_request_template.md
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.265075 magic-folder-23.6.0/.github/workflows/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      935 2023-06-26 06:27:27.000000 magic-folder-23.6.0/.github/workflows/codechecks.yml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4319 2023-06-26 06:27:27.000000 magic-folder-23.6.0/.github/workflows/linux.yml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3192 2023-06-26 06:27:27.000000 magic-folder-23.6.0/.github/workflows/macos.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3231 2023-06-26 06:27:27.000000 magic-folder-23.6.0/.github/workflows/windows.yml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2022-08-04 09:11:55.000000 magic-folder-23.6.0/.gitignore
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      365 2023-06-26 06:27:27.000000 magic-folder-23.6.0/.readthedocs.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24277 2020-02-04 18:00:11.000000 magic-folder-23.6.0/COPYING.GPL
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17300 2020-02-04 18:00:11.000000 magic-folder-23.6.0/COPYING.TGPPL.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4840 2020-02-04 18:00:11.000000 magic-folder-23.6.0/CREDITS
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10046 2023-06-26 06:27:27.000000 magic-folder-23.6.0/DEVELOPERS
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2022-09-20 06:29:38.000000 magic-folder-23.6.0/MANIFEST.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2275 2023-06-26 06:28:21.000000 magic-folder-23.6.0/Makefile
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    26342 2023-06-26 06:33:00.000000 magic-folder-23.6.0/NEWS.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7592 2021-07-26 20:37:49.000000 magic-folder-23.6.0/NOTES.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-06-26 06:33:02.393074 magic-folder-23.6.0/PKG-INFO
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5496 2023-06-26 06:27:27.000000 magic-folder-23.6.0/README.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.229075 magic-folder-23.6.0/docs/.hypothesis/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.229075 magic-folder-23.6.0/docs/.hypothesis/examples/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/25667fd10de02221/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.6.0/docs/.hypothesis/examples/25667fd10de02221/394341b7182cd227
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/26099471863eabde/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:34.000000 magic-folder-23.6.0/docs/.hypothesis/examples/26099471863eabde/394341b7182cd227
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/26b950c63ef40743/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:27.000000 magic-folder-23.6.0/docs/.hypothesis/examples/26b950c63ef40743/2cd852709fc7beda
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/27a267c0b163fc05/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:31.000000 magic-folder-23.6.0/docs/.hypothesis/examples/27a267c0b163fc05/2cd852709fc7beda
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/2bdd697e3cea2a04/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2023-03-16 04:52:44.000000 magic-folder-23.6.0/docs/.hypothesis/examples/2bdd697e3cea2a04/f4644a30270a4ea6
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/3674e9cecacd98c9/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:28.000000 magic-folder-23.6.0/docs/.hypothesis/examples/3674e9cecacd98c9/2cd852709fc7beda
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/532c4ead6274d000/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      212 2023-03-16 04:52:28.000000 magic-folder-23.6.0/docs/.hypothesis/examples/532c4ead6274d000/42e9ca500f868ebd
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/5ac28ffd404dc215/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        5 2023-03-16 04:52:38.000000 magic-folder-23.6.0/docs/.hypothesis/examples/5ac28ffd404dc215/68e09c5bfbe3cdbe
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/704d1edf754e9033/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       20 2023-03-16 04:52:39.000000 magic-folder-23.6.0/docs/.hypothesis/examples/704d1edf754e9033/d0ff8af3e4baa190
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/9e68e03a9abe82a7/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       11 2023-03-16 04:52:30.000000 magic-folder-23.6.0/docs/.hypothesis/examples/9e68e03a9abe82a7/d271b3d8c89fbe5f
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/b069c007d3e9f6fb/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       24 2023-03-16 04:52:38.000000 magic-folder-23.6.0/docs/.hypothesis/examples/b069c007d3e9f6fb/eaef33fe07ad3597
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/c06175530ec95812/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      238 2023-03-16 04:52:45.000000 magic-folder-23.6.0/docs/.hypothesis/examples/c06175530ec95812/fd83ff26e80c6fad
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/examples/e1ab432a194b3b87/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.6.0/docs/.hypothesis/examples/e1ab432a194b3b87/394341b7182cd227
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.229075 magic-folder-23.6.0/docs/.hypothesis/unicode_data/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.277075 magic-folder-23.6.0/docs/.hypothesis/unicode_data/13.0.0/
+-rw-------   0 meejah    (1000) meejah    (1000)    20988 2023-03-16 04:52:30.000000 magic-folder-23.6.0/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      634 2020-07-06 21:59:25.000000 magic-folder-23.6.0/docs/Makefile
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.233075 magic-folder-23.6.0/docs/_build/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.285075 magic-folder-23.6.0/docs/_build/doctrees/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14226 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/CODE_OF_CONDUCT.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9338 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/backdoors.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    38021 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/config.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    43869 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/datamodel.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    31814 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/development.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    33138 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/downloader.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)  1261313 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13136 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    66571 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/interface.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    54817 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/invites.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    59020 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/leif-design.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11222 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/limitations.doctree
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.285075 magic-folder-23.6.0/docs/_build/doctrees/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18815 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/proposed/conflict-api.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4250 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/proposed/index.doctree
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.285075 magic-folder-23.6.0/docs/_build/doctrees/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18656 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   178832 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    32883 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19020 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/proposed/recovery.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    37513 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/proposed/scanning-for-changes.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11826 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/release-process.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   182197 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/releases.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23355 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/snapshots.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    42464 2023-03-17 00:18:57.000000 magic-folder-23.6.0/docs/_build/doctrees/usage.doctree
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.293075 magic-folder-23.6.0/docs/_build/html/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      230 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/.buildinfo
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11411 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/CODE_OF_CONDUCT.html
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.293075 magic-folder-23.6.0/docs/_build/html/_images/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    27173 2023-03-16 20:16:58.000000 magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model--high-level.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30197 2023-03-17 00:18:54.000000 magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24088 2023-03-16 21:22:18.000000 magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model-abstract.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   436150 2023-03-17 00:06:11.000000 magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model.svg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.297075 magic-folder-23.6.0/docs/_build/html/_sources/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-03-16 04:36:41.000000 magic-folder-23.6.0/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.6.0/docs/_build/html/_sources/backdoors.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7226 2023-03-16 08:24:55.000000 magic-folder-23.6.0/docs/_build/html/_sources/config.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11620 2023-03-17 00:18:36.000000 magic-folder-23.6.0/docs/_build/html/_sources/datamodel.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.6.0/docs/_build/html/_sources/development.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.6.0/docs/_build/html/_sources/downloader.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2023-03-16 20:41:52.000000 magic-folder-23.6.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15051 2023-03-16 08:24:55.000000 magic-folder-23.6.0/docs/_build/html/_sources/interface.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-02-16 06:39:44.000000 magic-folder-23.6.0/docs/_build/html/_sources/invites.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17077 2023-03-16 20:45:29.000000 magic-folder-23.6.0/docs/_build/html/_sources/leif-design.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-02-07 22:05:58.000000 magic-folder-23.6.0/docs/_build/html/_sources/limitations.rst.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.297075 magic-folder-23.6.0/docs/_build/html/_sources/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-03-16 04:36:41.000000 magic-folder-23.6.0/docs/_build/html/_sources/proposed/conflict-api.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      612 2023-03-16 20:41:30.000000 magic-folder-23.6.0/docs/_build/html/_sources/proposed/index.rst.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.297075 magic-folder-23.6.0/docs/_build/html/_sources/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.6.0/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.6.0/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.6.0/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-03-16 04:36:41.000000 magic-folder-23.6.0/docs/_build/html/_sources/proposed/recovery.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.6.0/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-03-16 04:36:41.000000 magic-folder-23.6.0/docs/_build/html/_sources/release-process.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-03-16 04:36:41.000000 magic-folder-23.6.0/docs/_build/html/_sources/releases.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-03-16 04:36:41.000000 magic-folder-23.6.0/docs/_build/html/_sources/snapshots.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-03-16 20:45:54.000000 magic-folder-23.6.0/docs/_build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.301075 magic-folder-23.6.0/docs/_build/html/_static/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14813 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.301075 magic-folder-23.6.0/docs/_build/html/_static/css/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3229 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.313074 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    87624 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    67312 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    86288 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    66444 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   165742 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   444379 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   165548 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    98024 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    77160 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   323344 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   193308 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   309728 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   184912 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   328412 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   195704 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   309192 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   182708 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   135235 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.6.0/docs/_build/html/_static/custom.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4472 2023-03-08 00:43:20.000000 magic-folder-23.6.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      418 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      286 2023-03-08 00:43:20.000000 magic-folder-23.6.0/docs/_build/html/_static/file.png
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.313074 magic-folder-23.6.0/docs/_build/html/_static/js/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      934 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4370 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2734 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5023 2023-03-08 00:44:09.000000 magic-folder-23.6.0/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4758 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.6.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.6.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4846 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18215 2023-03-08 00:43:20.000000 magic-folder-23.6.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4712 2023-03-08 00:43:20.000000 magic-folder-23.6.0/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8183 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/backdoors.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19001 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/config.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23764 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/datamodel.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20860 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/development.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18079 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/downloader.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5143 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/genindex.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11167 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/index.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    44501 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/interface.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    35282 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/invites.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30106 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/leif-design.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7597 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/limitations.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1120 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/objects.inv
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.313074 magic-folder-23.6.0/docs/_build/html/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16640 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/proposed/conflict-api.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8297 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/proposed/index.html
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.313074 magic-folder-23.6.0/docs/_build/html/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14301 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/proposed/magic-folder/filesystem-integration.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    73834 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20764 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/proposed/magic-folder/user-interface-design.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16041 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/proposed/recovery.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19921 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/proposed/scanning-for-changes.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9495 2023-03-17 00:18:58.000000 magic-folder-23.6.0/docs/_build/html/release-process.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    51586 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/releases.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5542 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/search.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    63003 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/searchindex.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15500 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/snapshots.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    29531 2023-03-17 00:18:59.000000 magic-folder-23.6.0/docs/_build/html/usage.html
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.313074 magic-folder-23.6.0/docs/_static/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.6.0/docs/_static/.empty
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.6.0/docs/_static/custom.css
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.313074 magic-folder-23.6.0/docs/_templates/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.6.0/docs/_templates/.empty
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.313074 magic-folder-23.6.0/docs/_trial_temp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:53.000000 magic-folder-23.6.0/docs/_trial_temp/_trial_marker
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.233075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.233075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/file
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/file
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.237075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/file
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.241075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.241075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.241075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      284 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.317074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.321075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.241075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.321075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.321075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.325075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      289 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.241075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.325075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      285 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.325075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.325075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.241075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.325075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.325075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_client_endpoint
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.241075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        6 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/h87a74R8VavQbimAtmp
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.329074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.245075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      273 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.333074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.337074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      275 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.337074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       12 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/api_client_endpoint
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.337074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       10 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.337074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.249075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.341074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.341074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.341074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.341074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.341074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      448 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.341074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.341074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      447 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.253075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.345075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.345075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.345075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.345075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      434 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.345075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.345075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      451 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.345075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:57.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:57.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      437 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.257075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.261075 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.349074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.353074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.353074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.353074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.353074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.357074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.357074 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/tahoe.cfg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       41 2023-03-16 04:52:53.000000 magic-folder-23.6.0/docs/_trial_temp/test.log
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.6.0/docs/backdoors.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9480 2021-07-26 20:37:49.000000 magic-folder-23.6.0/docs/conf.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7228 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/config.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12907 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/datamodel.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.6.0/docs/development.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.6.0/docs/downloader.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   664833 2023-03-16 04:53:01.000000 magic-folder-23.6.0/docs/eliot.log
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/index.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14816 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/interface.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14482 2022-11-11 00:40:27.000000 magic-folder-23.6.0/docs/invite-diagram-readonly.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1230 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/invite-diagram-readonly.seqdiag
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16247 2023-01-07 21:02:05.000000 magic-folder-23.6.0/docs/invite-diagram.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1229 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/invite-diagram.seqdiag
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/invites.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17077 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/leif-design.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/limitations.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    25859 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/magic-folder-data-model--high-level.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30197 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/magic-folder-data-model-abstract--conflict.plain.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30583 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/magic-folder-data-model-abstract--conflict.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    22449 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/magic-folder-data-model-abstract.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   430340 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/magic-folder-data-model.svg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.357074 magic-folder-23.6.0/docs/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24834 2021-06-11 15:26:48.000000 magic-folder-23.6.0/docs/proposed/LightweightDesignscanfornewfiles.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/proposed/conflict-api.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      612 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/proposed/index.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.357074 magic-folder-23.6.0/docs/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.6.0/docs/proposed/magic-folder/filesystem-integration.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.6.0/docs/proposed/magic-folder/remote-to-local-sync.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.6.0/docs/proposed/magic-folder/user-interface-design.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   257416 2021-06-11 16:23:59.000000 magic-folder-23.6.0/docs/proposed/markdown
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/proposed/recovery.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.6.0/docs/proposed/scanning-for-changes.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/release-process.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/releases.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/snapshots.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-06-26 06:27:27.000000 magic-folder-23.6.0/docs/usage.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.361074 magic-folder-23.6.0/integration/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2022-09-20 06:29:38.000000 magic-folder-23.6.0/integration/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-07-26 20:37:49.000000 magic-folder-23.6.0/integration/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2021-06-22 06:43:35.000000 magic-folder-23.6.0/integration/bar
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12174 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/conftest.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9445 2020-06-25 22:39:41.000000 magic-folder-23.6.0/integration/conftest.py.orig
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2110 2021-06-22 06:43:20.000000 magic-folder-23.6.0/integration/foo
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1780 2021-12-21 23:52:48.000000 magic-folder-23.6.0/integration/log.integ
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-06-22 06:45:13.000000 magic-folder-23.6.0/integration/pytest.log
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4271 2023-06-22 01:52:57.000000 magic-folder-23.6.0/integration/test_add.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2758 2022-09-20 06:29:38.000000 magic-folder-23.6.0/integration/test_general_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2802 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/test_invite.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3363 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/test_kitties.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2312 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/test_list.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      592 2022-09-20 06:29:38.000000 magic-folder-23.6.0/integration/test_magic_folder.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16384 2020-06-25 22:17:40.000000 magic-folder-23.6.0/integration/test_magic_folder.py.orig
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10302 2020-06-25 22:39:42.000000 magic-folder-23.6.0/integration/test_magic_folder.py.rej
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5711 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/test_multiuser.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2846 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/test_same_files.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1977 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/test_status.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23667 2023-06-13 18:10:42.000000 magic-folder-23.6.0/integration/test_synchronize.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4367 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/test_tahoe_objects.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    47467 2023-06-26 06:27:27.000000 magic-folder-23.6.0/integration/util.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23625 2020-06-25 22:17:40.000000 magic-folder-23.6.0/integration/util.py.orig
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5425 2020-06-25 22:39:43.000000 magic-folder-23.6.0/integration/util.py.rej
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.261075 magic-folder-23.6.0/misc/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.365074 magic-folder-23.6.0/misc/build_helpers/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1482 2023-05-16 00:42:34.000000 magic-folder-23.6.0/misc/build_helpers/ann.toml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2889 2022-08-04 09:11:55.000000 magic-folder-23.6.0/misc/build_helpers/platform-pins.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3919 2021-11-25 22:22:35.000000 magic-folder-23.6.0/misc/build_helpers/run-deprecations.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      228 2021-11-25 22:22:35.000000 magic-folder-23.6.0/misc/build_helpers/sqlite_version.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2475 2023-06-26 06:27:27.000000 magic-folder-23.6.0/misc/build_helpers/update-version.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.365074 magic-folder-23.6.0/misc/coding_tools/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      807 2021-07-26 20:37:49.000000 magic-folder-23.6.0/misc/coding_tools/check-debugging.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.365074 magic-folder-23.6.0/newsfragments/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2022-09-20 06:29:38.000000 magic-folder-23.6.0/newsfragments/.keep-directory
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1455 2022-09-20 06:29:38.000000 magic-folder-23.6.0/pyproject.toml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      287 2021-08-27 20:55:28.000000 magic-folder-23.6.0/pytest.ini
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.365074 magic-folder-23.6.0/requirements/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      443 2021-11-25 22:22:35.000000 magic-folder-23.6.0/requirements/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/base.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    51070 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/base.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      254 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/build.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10627 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/build.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3489 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/platform.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2022-09-20 06:29:38.000000 magic-folder-23.6.0/requirements/tahoe-integration-1.17.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/tahoe-integration-1.18.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       67 2021-07-26 20:37:49.000000 magic-folder-23.6.0/requirements/tahoe-integration-master.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      827 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/test.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16658 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/test.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       48 2022-08-04 09:11:55.000000 magic-folder-23.6.0/requirements/tox.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1158 2023-06-26 06:27:27.000000 magic-folder-23.6.0/requirements/tox.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       38 2023-06-26 06:33:02.393074 magic-folder-23.6.0/setup.cfg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2661 2022-09-20 06:29:38.000000 magic-folder-23.6.0/setup.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.261075 magic-folder-23.6.0/src/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.377074 magic-folder-23.6.0/src/magic_folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      123 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      152 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/__main__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1171 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/_coverage.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1670 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/_endpoint_parser.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5780 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/_schema.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      162 2023-06-26 06:33:02.000000 magic-folder-23.6.0/src/magic_folder/_version.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20176 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/api_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    38483 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13666 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/client.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5264 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    78056 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/config.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    22725 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/downloader.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2741 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/endpoints.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1611 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/initialize.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20672 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/invite.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/join.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2173 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/list.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    48125 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/magic_file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18012 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/magic_folder.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      539 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/magicpath.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2786 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/migrate.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13785 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/participants.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4142 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/pid.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9335 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/scanner.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18416 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/service.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1286 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/show_config.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23391 2023-05-12 07:52:05.000000 magic-folder-23.6.0/src/magic_folder/snapshot.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    21598 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/status.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14506 2023-06-22 01:52:57.000000 magic-folder-23.6.0/src/magic_folder/tahoe_client.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.385074 magic-folder-23.6.0/src/magic_folder/test/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3189 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      849 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/agentutil.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.389074 magic-folder-23.6.0/src/magic_folder/test/cli/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.6.0/src/magic_folder/test/cli/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6104 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/cli/common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4451 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/cli/test_api_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24283 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/cli/test_magic_folder.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6801 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4962 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/eliotutil.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16684 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/fixtures.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5130 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/matchers.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.389074 magic-folder-23.6.0/src/magic_folder/test/plugins/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      334 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/plugins/magic_folder_tests_dropin.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12527 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/strategies.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    26838 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_api_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    22960 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4839 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_client.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4663 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    49601 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_config.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    73643 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_download.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5476 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_eliotutil.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1281 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_endpoints.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1188 2022-03-15 06:53:54.000000 magic-folder-23.6.0/src/magic_folder/test/test_foo.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    28373 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_invite.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11803 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_local_snapshot.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10605 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_magic_file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8112 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_magic_folder_service.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1199 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_magicpath.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17352 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_participants.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4646 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_pid.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18378 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_scanner.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7004 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_schema.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8026 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_service.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18979 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_snapshot.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10854 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_status.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2040 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_strategies.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12958 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_tahoe_client.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5832 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_testing.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    26060 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_upload.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2532 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_util_database.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4535 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_util_file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6446 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/test/test_util_twisted.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    80071 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/test/test_web.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.389074 magic-folder-23.6.0/src/magic_folder/testing/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-07-07 16:51:27.000000 magic-folder-23.6.0/src/magic_folder/testing/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18739 2023-01-30 21:42:35.000000 magic-folder-23.6.0/src/magic_folder/testing/web.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12645 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/uploader.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.393074 magic-folder-23.6.0/src/magic_folder/util/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.6.0/src/magic_folder/util/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6852 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/util/capabilities.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5603 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/util/database.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9471 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/util/eliotutil.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      617 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/util/encoding.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2473 2023-05-19 07:49:40.000000 magic-folder-23.6.0/src/magic_folder/util/file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1403 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/util/observer.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6547 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/util/twisted.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2176 2022-09-20 06:29:38.000000 magic-folder-23.6.0/src/magic_folder/util/wrap.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30795 2023-06-26 06:27:27.000000 magic-folder-23.6.0/src/magic_folder/web.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.377074 magic-folder-23.6.0/src/magic_folder.egg-info/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-06-26 06:33:02.000000 magic-folder-23.6.0/src/magic_folder.egg-info/PKG-INFO
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    31561 2023-06-26 06:33:02.000000 magic-folder-23.6.0/src/magic_folder.egg-info/SOURCES.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        1 2023-06-26 06:33:02.000000 magic-folder-23.6.0/src/magic_folder.egg-info/dependency_links.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      104 2023-06-26 06:33:02.000000 magic-folder-23.6.0/src/magic_folder.egg-info/entry_points.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      532 2023-06-26 06:33:02.000000 magic-folder-23.6.0/src/magic_folder.egg-info/requires.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       21 2023-06-26 06:33:02.000000 magic-folder-23.6.0/src/magic_folder.egg-info/top_level.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.261075 magic-folder-23.6.0/src/twisted/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-06-26 06:33:02.393074 magic-folder-23.6.0/src/twisted/plugins/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      301 2021-07-26 20:37:49.000000 magic-folder-23.6.0/src/twisted/plugins/magic_folder_dropin.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5616 2023-06-26 06:27:27.000000 magic-folder-23.6.0/tox.ini
```

### Comparing `magic-folder-23.5.0/.github/workflows/codechecks.yml` & `magic-folder-23.6.0/.github/workflows/codechecks.yml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/.github/workflows/linux.yml` & `magic-folder-23.6.0/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/.github/workflows/macos.yaml` & `magic-folder-23.6.0/.github/workflows/macos.yaml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/.github/workflows/windows.yml` & `magic-folder-23.6.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/COPYING.GPL` & `magic-folder-23.6.0/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/COPYING.TGPPL.rst` & `magic-folder-23.6.0/COPYING.TGPPL.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/CREDITS` & `magic-folder-23.6.0/CREDITS`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/DEVELOPERS` & `magic-folder-23.6.0/DEVELOPERS`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/Makefile` & `magic-folder-23.6.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,14 @@
 	testmf_venv/bin/pip uninstall -y magic_folder
 	testmf_venv/bin/pip install dist/magic-folder-`git describe --abbrev=0`.tar.gz
 	testmf_venv/bin/magic-folder --version
 	testmf_venv/bin/magic-folder-api --version
 	rm -rf testmf_venv
 
 release-upload:
-	twine upload dist/magic_folder-`git describe --abbrev=0`-py3-none-any.whl dist/magic_folder-`git describe --abbrev=0`-py3-none-any.whl.asc dist/magic-folder-`git describe --abbrev=0`.tar.gz dist/magic-folder-`git describe --abbrev=0`.tar.gz.asc
+	twine upload --config-file pypirc-magicfolder dist/magic_folder-`git describe --abbrev=0`-py3-none-any.whl dist/magic_folder-`git describe --abbrev=0`-py3-none-any.whl.asc dist/magic-folder-`git describe --abbrev=0`.tar.gz dist/magic-folder-`git describe --abbrev=0`.tar.gz.asc
 
 coverage:
 	-coverage erase
 	MAGIC_FOLDER_HYPOTHESIS_PROFILE=magic-folder-fast coverage run -m twisted.trial magic_folder
 	coverage combine
 	git diff main.. | cuv diff -
```

### Comparing `magic-folder-23.5.0/NEWS.rst` & `magic-folder-23.6.0/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 ﻿.. -*- coding: utf-8-with-signature -*-
 
 .. towncrier start line
+Magic_Folder 23.6.0 (2023-06-26)
+''''''''''''''''''''''''''''''''
+
+No significant changes.
+
+
+Magic_Folder 23.6.0 (2023-06-26)
+''''''''''''''''''''''''''''''''
+
+Features
+--------
+
+- Added a description of the datamodel to the documentation (`#702 <https://github.com/LeastAuthority/magic-folder/issues/702>`_)
+- Conflict files now named after the Participant (not Author) (`#711 <https://github.com/LeastAuthority/magic-folder/issues/711>`_)
+
+
+Bug Fixes
+---------
+
+- "magic-folder status" properly parses scan/poll events (`#717 <https://github.com/LeastAuthority/magic-folder/issues/717>`_)
+- Handle updates to conflicted files more robustly (`#719 <https://github.com/LeastAuthority/magic-folder/issues/719>`_)
+
+
+Other Changes
+-------------
+
+- Bump dependencies, including security-relevant cryptography library (`#716 <https://github.com/LeastAuthority/magic-folder/issues/716>`_)
+
+
 Magic_Folder 23.5.0 (2023-05-02)
 ''''''''''''''''''''''''''''''''
 
 Backwards Incompatible Changes
 ------------------------------
 
 - The /status endpoint now produces event-based output
```

### Comparing `magic-folder-23.5.0/NOTES.rst` & `magic-folder-23.6.0/NOTES.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/PKG-INFO` & `magic-folder-23.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-folder
-Version: 23.5.0
+Version: 23.6.0
 Summary: Tahoe-LAFS-based file synchronization
 Home-page: https://github.com/LeastAuthority/magic-folder/
 Author: the Tahoe-LAFS developers, the Magic-Folder developers
 Author-email: tahoe-dev@tahoe-lafs.org
 License: GNU GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `magic-folder-23.5.0/README.rst` & `magic-folder-23.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz` & `magic-folder-23.6.0/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/CODE_OF_CONDUCT.rst` & `magic-folder-23.6.0/docs/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/Makefile` & `magic-folder-23.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/CODE_OF_CONDUCT.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/CODE_OF_CONDUCT.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/backdoors.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/backdoors.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/config.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/config.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/datamodel.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/datamodel.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/development.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/development.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/downloader.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/downloader.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/environment.pickle` & `magic-folder-23.6.0/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/index.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/interface.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/interface.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/invites.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/invites.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/leif-design.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/leif-design.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/limitations.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/limitations.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/proposed/conflict-api.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/proposed/conflict-api.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/proposed/index.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/proposed/index.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/proposed/recovery.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/proposed/recovery.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/proposed/scanning-for-changes.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/proposed/scanning-for-changes.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/release-process.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/release-process.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/releases.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/releases.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/snapshots.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/snapshots.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/doctrees/usage.doctree` & `magic-folder-23.6.0/docs/_build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/CODE_OF_CONDUCT.html` & `magic-folder-23.6.0/docs/_build/html/CODE_OF_CONDUCT.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model--high-level.svg` & `magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model--high-level.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg` & `magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract.svg` & `magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model-abstract.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model.svg` & `magic-folder-23.6.0/docs/_build/html/_images/magic-folder-data-model.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/backdoors.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/backdoors.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/config.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/config.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/datamodel.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/datamodel.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/development.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/development.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/downloader.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/downloader.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/index.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/interface.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/interface.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/invites.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/invites.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/leif-design.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/leif-design.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/limitations.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/limitations.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/proposed/conflict-api.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/proposed/conflict-api.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/proposed/index.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/proposed/index.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/proposed/recovery.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/proposed/recovery.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/release-process.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/release-process.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/snapshots.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/snapshots.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_sources/usage.rst.txt` & `magic-folder-23.6.0/docs/_build/html/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/basic.css` & `magic-folder-23.6.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/badge_only.css` & `magic-folder-23.6.0/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `magic-folder-23.6.0/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/css/theme.css` & `magic-folder-23.6.0/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/doctools.js` & `magic-folder-23.6.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/js/badge_only.js` & `magic-folder-23.6.0/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `magic-folder-23.6.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv.min.js` & `magic-folder-23.6.0/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/js/theme.js` & `magic-folder-23.6.0/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/language_data.js` & `magic-folder-23.6.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/pygments.css` & `magic-folder-23.6.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/searchtools.js` & `magic-folder-23.6.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/_static/sphinx_highlight.js` & `magic-folder-23.6.0/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/backdoors.html` & `magic-folder-23.6.0/docs/_build/html/backdoors.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/config.html` & `magic-folder-23.6.0/docs/_build/html/config.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/datamodel.html` & `magic-folder-23.6.0/docs/_build/html/datamodel.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/development.html` & `magic-folder-23.6.0/docs/_build/html/development.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/downloader.html` & `magic-folder-23.6.0/docs/_build/html/downloader.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/genindex.html` & `magic-folder-23.6.0/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/index.html` & `magic-folder-23.6.0/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/interface.html` & `magic-folder-23.6.0/docs/_build/html/interface.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/invites.html` & `magic-folder-23.6.0/docs/_build/html/invites.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/leif-design.html` & `magic-folder-23.6.0/docs/_build/html/leif-design.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/limitations.html` & `magic-folder-23.6.0/docs/_build/html/limitations.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/objects.inv` & `magic-folder-23.6.0/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/proposed/conflict-api.html` & `magic-folder-23.6.0/docs/_build/html/proposed/conflict-api.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/proposed/index.html` & `magic-folder-23.6.0/docs/_build/html/proposed/index.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/filesystem-integration.html` & `magic-folder-23.6.0/docs/_build/html/proposed/magic-folder/filesystem-integration.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html` & `magic-folder-23.6.0/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/user-interface-design.html` & `magic-folder-23.6.0/docs/_build/html/proposed/magic-folder/user-interface-design.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/proposed/recovery.html` & `magic-folder-23.6.0/docs/_build/html/proposed/recovery.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/proposed/scanning-for-changes.html` & `magic-folder-23.6.0/docs/_build/html/proposed/scanning-for-changes.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/release-process.html` & `magic-folder-23.6.0/docs/_build/html/release-process.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/releases.html` & `magic-folder-23.6.0/docs/_build/html/releases.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/search.html` & `magic-folder-23.6.0/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/searchindex.js` & `magic-folder-23.6.0/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/snapshots.html` & `magic-folder-23.6.0/docs/_build/html/snapshots.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_build/html/usage.html` & `magic-folder-23.6.0/docs/_build/html/usage.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite` & `magic-folder-23.6.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/backdoors.rst` & `magic-folder-23.6.0/docs/backdoors.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/conf.py` & `magic-folder-23.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/config.rst` & `magic-folder-23.6.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/development.rst` & `magic-folder-23.6.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/downloader.rst` & `magic-folder-23.6.0/docs/downloader.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/eliot.log` & `magic-folder-23.6.0/docs/eliot.log`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/index.rst` & `magic-folder-23.6.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -79,10 +79,12 @@
    limitations
    releases
    backdoors
    development
    interface
    config
    snapshots
+   datamodel
    downloader
    release-process
+   leif-design
    proposed/index
```

### Comparing `magic-folder-23.5.0/docs/interface.rst` & `magic-folder-23.6.0/docs/interface.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/invite-diagram-readonly.png` & `magic-folder-23.6.0/docs/invite-diagram-readonly.png`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/invite-diagram-readonly.seqdiag` & `magic-folder-23.6.0/docs/invite-diagram-readonly.seqdiag`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/invite-diagram.png` & `magic-folder-23.6.0/docs/invite-diagram.png`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/invite-diagram.seqdiag` & `magic-folder-23.6.0/docs/invite-diagram.seqdiag`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/invites.rst` & `magic-folder-23.6.0/docs/invites.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/limitations.rst` & `magic-folder-23.6.0/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/LightweightDesignscanfornewfiles.html` & `magic-folder-23.6.0/docs/proposed/LightweightDesignscanfornewfiles.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/conflict-api.rst` & `magic-folder-23.6.0/docs/proposed/conflict-api.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/index.rst` & `magic-folder-23.6.0/docs/proposed/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -14,9 +14,8 @@
    :maxdepth: 1
 
    conflict-api
    recovery
    magic-folder/filesystem-integration
    magic-folder/remote-to-local-sync
    magic-folder/user-interface-design
-   magic-folder/multi-party-conflict-detection
    scanning-for-changes
```

### Comparing `magic-folder-23.5.0/docs/proposed/magic-folder/filesystem-integration.rst` & `magic-folder-23.6.0/docs/proposed/magic-folder/filesystem-integration.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/magic-folder/multi-party-conflict-detection.rst` & `magic-folder-23.6.0/docs/leif-design.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,37 @@
+.. _leif-design:
+
+The Leif Design: synchronization model
+======================================
+
+Originally proposed by Tahoe-LAFS contributor Leif Ryge, this design of magic-folder synchronization is ofter referred to as "the Leif model".
+
+This document is of interest to magic-folder contributors or experts wishing to understand the history of the synchronization model.
+
+.. WARNING::
+
+   This document is largely for historical purposes.
+   Details have changed and some of the terminology in here dates from when magic-folder was part of the Tahoe-LAFS codebase and a subcommand of ``tahoe``.
+
+
 Multi-party Conflict Detection
-==============================
+------------------------------
 
 The current Magic-Folder remote conflict detection design does not properly detect remote conflicts
 for groups of three or more parties. This design is specified in the "Fire Dragon" section of this document:
 https://github.com/tahoe-lafs/tahoe-lafs/blob/2551.wip.2/docs/proposed/magic-folder/remote-to-local-sync.rst#fire-dragons-distinguishing-conflicts-from-overwrites
 
 This Tahoe-LAFS trac ticket comment outlines a scenario with
 three parties in which a remote conflict is falsely detected:
 
 .. _`ticket comment`: https://tahoe-lafs.org/trac/tahoe-lafs/ticket/2551#comment:22
 
 
 Summary and definitions
-=======================
+-----------------------
 
 Abstract file: a file being shared by a Magic Folder.
 
 Local file: a file in a client's local filesystem corresponding to an abstract file.
 
 Relative path: the path of an abstract or local file relative to the Magic Folder root.
 
@@ -40,58 +55,55 @@
 
 * if a client Bob currently has version V of a file at relative path F, and it sees a new version V'
   of that file in another client Alice's DMD, such that V' follows V, then the write of the new version
   is initially an overwrite and should be to the same filename.
 * if, in the same situation, V' does not follow V, then the write of the new version should be
   classified as a conflict.
 
-The existing :doc:`remote-to-local-sync` document defines when an initial
+The existing :doc:`proposed/magic-folder/remote-to-local-sync` document defines when an initial
 overwrite should be reclassified as a conflict.
 
 The above definitions completely specify the desired solution of the false
 conflict behaviour described in the `ticket comment`_. However, they do not give
 a concrete algorithm to compute the follows relation, or a representation in the
 Tahoe-LAFS file store of the metadata needed to compute it.
 
 We will consider two alternative designs, proposed by Leif Ryge and
 Zooko Wilcox-O'Hearn, that aim to fill this gap.
 
 
 
 Leif's Proposal: Magic-Folder "single-file" snapshot design
-===========================================================
+-----------------------------------------------------------
 
 Abstract
---------
+````````
 
 We propose a relatively simple modification to the initial Magic Folder design which
 adds merkle DAGs of immutable historical snapshots for each file. The full history
 does not necessarily need to be retained, and the choice of how much history to retain
 can potentially be made on a per-file basis.
 
-Motivation:
------------
-
-no SPOFs, no admins
-```````````````````
+Motivation:n o SPOFs, no admins
+```````````````````````````````
 
 Additionally, the initial design had two cases of excess authority:
 
 1. The magic folder administrator (inviter) has everyone's write-caps and is thus essentially "root"
 2. Each client shares ambient authority and can delete anything or everything and
    (assuming there is not a conflict) the data will be deleted from all clients. So, each client
    is effectively "root" too.
 
 Thus, while it is useful for file synchronization, the initial design is a much less safe place
 to store data than in a single mutable tahoe directory (because more client computers have the
 possibility to delete it).
 
 
 Glossary
---------
+````````
 
 - merkle DAG: like a merkle tree but with multiple roots, and with each node potentially having multiple parents
 - magic folder: a logical directory that can be synchronized between many clients
   (devices, users, ...) using a Tahoe-LAFS storage grid
 - client: a Magic-Folder-enabled Tahoe-LAFS client instance that has access to a magic folder
 - DMD: "distributed mutable directory", a physical Tahoe-LAFS mutable directory.
   Each client has the write cap to their own DMD, and read caps to all other client's DMDs
@@ -107,15 +119,15 @@
 - capability: a Tahoe-LAFS diminishable cryptographic capability
 - cap: short for capability
 - conflict: the situation when another client's current snapshot for a file is different than our current snapshot, and is not a descendant of ours.
 - overwrite: the situation when another client's current snapshot for a file is a (not necessarily direct) descendant of our current snapshot.
 
 
 Overview
---------
+````````
 
 This new design will track the history of each file using "snapshots" which are
 created at each upload. Each snapshot will specify one or more parent snapshots,
 forming a directed acyclic graph. A Magic-Folder user's DMD uses a flattened directory
 hierarchy naming scheme, as in the original design. But, instead of pointing directly
 at file contents, each file name will link to that user's latest snapshot for that file.
 
@@ -144,15 +156,15 @@
 created which has two parents - the client's snapshot prior to the conflict, and the
 new conflicting snapshot. If multiple .conflict files are deleted or renamed in a short
 period of time, a single conflict-resolving snapshot with more than two parents can be created.
 
 ! I think this behavior will confuse users. 
 
 Tahoe-LAFS snapshot objects
----------------------------
+```````````````````````````
 
 These Tahoe-LAFS snapshot objects only track the history of a single file, not a directory hierarchy.
 Snapshot objects contain only two field types:
 - ``Content``: an immutable capability of the file contents (omitted if deletion snapshot)
 - ``Parent0..N``: immutable capabilities representing parent snapshots
 
 Therefore in this system an interesting side effect of this Tahoe snapshot object is that there is no
@@ -161,27 +173,27 @@
 The snapshot object is an immutable directory which looks like this:
 content -> immutable cap to file content
 parent0 -> immutable cap to a parent snapshot object
 parent1..N -> more parent snapshots
 
 
 Snapshot Author Identity
-------------------------
+````````````````````````
 
 Snapshot identity might become an important feature so that bad actors
 can be recognized and other clients can stop "subscribing" to (polling for) updates from them.
 
 Perhaps snapshots could be signed by the user's Magic-Folder write key for this purpose? Probably a bad idea to reuse the write-cap key for this. Better to introduce ed25519 identity keys which can (optionally) sign snapshot contents and store the signature as another member of the immutable directory.
 
 
 Conflict Resolution
--------------------
+```````````````````
 
 detection of conflicts
-``````````````````````
+~~~~~~~~~~~~~~~~~~~~~~
 
 A Magic-Folder client updates a given file's current snapshot link to a snapshot which is a descendent
 of the previous snapshot. For a given file, let's say "file1", Alice can detect that Bob's DMD has a "file1"
 that links to a snapshot which conflicts. Two snapshots conflict if one is not an ancestor of the other.
 
 
 a possible UI for resolving conflicts
@@ -195,15 +207,15 @@
 choose the other version then she moves it into place:
 
    mv file1.conflicted.previous file1
 
 
 This scheme works for N number of conflicts. Bob for instance could choose
 the same resolution for the conflict, like this:
-   
+
    mv file1.Alice file1
 
 
 Deletion propagation and eventual Garbage Collection
 ----------------------------------------------------
 
 When a user deletes a file, this is represented by a link from their DMD file
@@ -285,15 +297,15 @@
 
 Bob can in fact, set a pre-existing directory (with files) as his new Magic-Folder directory, resulting
 in a merge of the Magic-Folder with Bob's local directory. Filename collisions will result in conflicts
 because Bob's new snapshots are not descendent's of the existing Magic-Folder file snapshots.
 
 
 Example: simultaneous update with four parties:
-    
+
 1. A, B, C, D are in sync for file "foo" at snapshot X
 2. A and B simultaneously change the file, creating snapshots XA and XB (both descendants of X).
 3. C hears about XA first, and D hears about XB first. Both accept an overwrite.
 4. All four parties hear about the other update they hadn't heard about yet.
 5. Result:
     - everyone's local file "foo" has the content pointed to by the snapshot in their DMD's "foo" entry
     - A and C's DMDs each have the "foo" entry pointing at snapshot XA
@@ -325,49 +337,7 @@
 
     - The conflict files on A, B, and C disappear, and everyone's local file "foo" contains D's manually-merged content.
 
 
 Daira: I think it is too complicated to include multiple nicknames in the .conflict files
 (e.g. "foo.conflict-B,D"). It should be sufficient to have one file for each other client,
 reflecting that client's latest version, regardless of who else it conflicts with.
-
-
-Zooko's Design (as interpreted by Daira)
-========================================
-
-A version map is a mapping from client nickname to version number.
-
-Definition: a version map M' strictly-follows a mapping M iff for every entry c->v
-in M, there is an entry c->v' in M' such that v' > v.
-
-
-Each client maintains a 'local version map' and a 'conflict version map' for each file
-in its magic folder db.
-If it has never written the file, then the entry for its own nickname in the local version
-map is zero. The conflict version map only contains entries for nicknames B where
-"$FILENAME.conflict-$B" exists.
-
-When a client A uploads a file, it increments the version for its own nickname in its
-local version map for the file, and includes that map as metadata with its upload.
-
-A download by client A from client B is an overwrite iff the downloaded version map
-strictly-follows A's local version map for that file; in this case A replaces its local
-version map with the downloaded version map. Otherwise it is a conflict, and the
-download is put into "$FILENAME.conflict-$B"; in this case A's
-local version map remains unchanged, and the entry B->v taken from the downloaded
-version map is added to its conflict version map.
-
-If client A deletes or renames a conflict file "$FILENAME.conflict-$B", then A copies
-the entry for B from its conflict version map to its local version map, deletes
-the entry for B in its conflict version map, and performs another upload (with
-incremented version number) of $FILENAME.
-
-
-Example:
-    A, B, C = (10, 20, 30) everyone agrees.
-    A updates: (11, 20, 30)
-    B updates: (10, 21, 30)
-
-C will see either A or B first. Both would be an overwrite, if considered alone.
-
-
-
```

### Comparing `magic-folder-23.5.0/docs/proposed/magic-folder/remote-to-local-sync.rst` & `magic-folder-23.6.0/docs/proposed/magic-folder/remote-to-local-sync.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/magic-folder/user-interface-design.rst` & `magic-folder-23.6.0/docs/proposed/magic-folder/user-interface-design.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/markdown` & `magic-folder-23.6.0/docs/proposed/markdown`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/recovery.rst` & `magic-folder-23.6.0/docs/proposed/recovery.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/proposed/scanning-for-changes.rst` & `magic-folder-23.6.0/docs/proposed/scanning-for-changes.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/release-process.rst` & `magic-folder-23.6.0/docs/release-process.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/snapshots.rst` & `magic-folder-23.6.0/docs/snapshots.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/docs/usage.rst` & `magic-folder-23.6.0/docs/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Using Magic Folder
 ==================
 
 Magic-Folder is used in two ways.
 
 The first way is to interact with the running daemon (including its
 configuration) is via the ``magic-folder`` command line tool (which
-uses the :ref:`HTTP API`). The following sections detail different
+uses the :ref:`http-api`). The following sections detail different
 subcommands available.  For additional information see `Magic Folder
 CLI design`_. See :ref:`config` for more on how configuration is kept.
 
 .. _`Magic Folder CLI design`: ../proposed/magic-folder/user-interface-design
 
 The second way is to interact with content, use your normal
 filesystem-based tools.  The folder which Magic-Folder synchronizes is
```

### Comparing `magic-folder-23.5.0/integration/README` & `magic-folder-23.6.0/integration/README`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/bar` & `magic-folder-23.6.0/integration/bar`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/conftest.py` & `magic-folder-23.6.0/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/conftest.py.orig` & `magic-folder-23.6.0/integration/conftest.py.orig`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/foo` & `magic-folder-23.6.0/integration/foo`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/log.integ` & `magic-folder-23.6.0/integration/log.integ`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_add.py` & `magic-folder-23.6.0/integration/test_add.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_general_cli.py` & `magic-folder-23.6.0/integration/test_general_cli.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_invite.py` & `magic-folder-23.6.0/integration/test_invite.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_kitties.py` & `magic-folder-23.6.0/integration/test_kitties.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_list.py` & `magic-folder-23.6.0/integration/test_list.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_magic_folder.py` & `magic-folder-23.6.0/integration/test_magic_folder.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_magic_folder.py.orig` & `magic-folder-23.6.0/integration/test_magic_folder.py.orig`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_magic_folder.py.rej` & `magic-folder-23.6.0/integration/test_magic_folder.py.rej`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_multiuser.py` & `magic-folder-23.6.0/integration/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_same_files.py` & `magic-folder-23.6.0/integration/test_same_files.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_status.py` & `magic-folder-23.6.0/integration/test_status.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_synchronize.py` & `magic-folder-23.6.0/integration/test_synchronize.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/test_tahoe_objects.py` & `magic-folder-23.6.0/integration/test_tahoe_objects.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/util.py` & `magic-folder-23.6.0/integration/util.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/util.py.orig` & `magic-folder-23.6.0/integration/util.py.orig`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/integration/util.py.rej` & `magic-folder-23.6.0/integration/util.py.rej`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/misc/build_helpers/platform-pins.py` & `magic-folder-23.6.0/misc/build_helpers/platform-pins.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/misc/build_helpers/run-deprecations.py` & `magic-folder-23.6.0/misc/build_helpers/run-deprecations.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/misc/build_helpers/update-version.py` & `magic-folder-23.6.0/misc/build_helpers/update-version.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/misc/coding_tools/check-debugging.py` & `magic-folder-23.6.0/misc/coding_tools/check-debugging.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/pyproject.toml` & `magic-folder-23.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/requirements/base.in` & `magic-folder-23.6.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/requirements/base.txt` & `magic-folder-23.6.0/requirements/base.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 #
 appdirs==1.4.4 \
     --hash=sha256:7d5d0167b2b1ba821647616af46a749d1c653740dd0d2415100fe26e27afdf41 \
     --hash=sha256:a841dacd6b99318a741b166adb07e19ee71a274450e68237b4650ca1055ab128
     # via
     #   -r requirements/base.in
     #   twisted
-attrs==22.2.0 \
-    --hash=sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836 \
-    --hash=sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99
+attrs==23.1.0 \
+    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
+    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
     # via
     #   -r requirements/base.in
     #   autobahn
     #   automat
     #   klein
     #   magic-wormhole
     #   service-identity
@@ -63,17 +63,17 @@
     --hash=sha256:b57adba8a1444faf784394de3436233728a1ecaeb6e07e8c22c8848f179b893c \
     --hash=sha256:bf4fa8b2ca74381bb5442c089350f09a3f17797829d958fad058d6e44d9eb83c \
     --hash=sha256:ca3204d00d3cb2dfed07f2d74a25f12fc12f73e606fcaa6975d1f7ae69cacbb2 \
     --hash=sha256:cbb03eec97496166b704ed663a53680ab57c5084b2fc98ef23291987b525cb7d \
     --hash=sha256:e9a51bbfe7e9802b5f3508687758b564069ba937748ad7b9e890086290d2f79e \
     --hash=sha256:fbdaec13c5105f0c4e5c52614d04f0bca5f5af007910daa8b6b12095edaa67b3
     # via twisted
-boltons==21.0.0 \
-    --hash=sha256:65e70a79a731a7fe6e98592ecfb5ccf2115873d01dbc576079874629e5c90f13 \
-    --hash=sha256:b9bb7b58b2b420bbe11a6025fdef6d3e5edc9f76a42fb467afe7ca212ef9948b
+boltons==23.0.0 \
+    --hash=sha256:8c50a71829525835ca3c849c7ed2511610c972b4dddfcd41a4a5447222beb4b0 \
+    --hash=sha256:f716a1b57698a5b19062f3146cb5ce3549904028a2f267c2c0cf584eea3ad75b
     # via eliot
 cbor2==5.4.6 \
     --hash=sha256:0b956f19e93ba3180c336282cd1b6665631f2d3a196a9c19b29a833bf979e7a4 \
     --hash=sha256:0bd12c54a48949d11f5ffc2fa27f5df1b4754111f5207453e5fae3512ebb3cab \
     --hash=sha256:0d2b926b024d3a1549b819bc82fdc387062bbd977b0299dd5fa5e0ea3267b98b \
     --hash=sha256:1618d16e310f7ffed141762b0ff5d8bb6b53ad449406115cc465bf04213cefcf \
     --hash=sha256:181ac494091d1f9c5bb373cd85514ce1eb967a8cf3ec298e8dfa8878aa823956 \
@@ -177,54 +177,123 @@
     --hash=sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6 \
     --hash=sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b \
     --hash=sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01 \
     --hash=sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==2.1.1 \
-    --hash=sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845 \
-    --hash=sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f
+charset-normalizer==3.1.0 \
+    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
+    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
+    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
+    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
+    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
+    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
+    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
+    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
+    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
+    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
+    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
+    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
+    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
+    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
+    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
+    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
+    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
+    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
+    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
+    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
+    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
+    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
+    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
+    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
+    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
+    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
+    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
+    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
+    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
+    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
+    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
+    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
+    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
+    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
+    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
+    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
+    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
+    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
+    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
+    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
+    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
+    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
+    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
+    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
+    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
+    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
+    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
+    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
+    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
+    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
+    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
+    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
+    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
+    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
+    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
+    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
+    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
+    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
+    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
+    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
+    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
+    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
+    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
+    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
+    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
+    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
+    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
+    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
+    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
+    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
+    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
+    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
+    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
+    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
+    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via magic-wormhole
 collections-extended==2.0.2 \
     --hash=sha256:bc096dda430b9455f51287943f7f63fbe53a4de78c444cc38c44e996af306ac5 \
     --hash=sha256:d68ebd1e2208444e392aa0016e5c085bd897f89296f5c1860787de5935994114
     # via tahoe-lafs
 constantly==15.1.0 \
     --hash=sha256:586372eb92059873e29eba4f9dec8381541b4d3834660707faf8ba59146dfc35 \
     --hash=sha256:dd2fa9d6b1a51a83f0d7dd76293d734046aa176e384bf6e33b7e44880eb37c5d
     # via twisted
-cryptography==39.0.0 \
-    --hash=sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b \
-    --hash=sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f \
-    --hash=sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190 \
-    --hash=sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f \
-    --hash=sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f \
-    --hash=sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb \
-    --hash=sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c \
-    --hash=sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773 \
-    --hash=sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72 \
-    --hash=sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8 \
-    --hash=sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717 \
-    --hash=sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9 \
-    --hash=sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856 \
-    --hash=sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96 \
-    --hash=sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288 \
-    --hash=sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39 \
-    --hash=sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e \
-    --hash=sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce \
-    --hash=sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1 \
-    --hash=sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de \
-    --hash=sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df \
-    --hash=sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf \
-    --hash=sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458
+cryptography==40.0.2 \
+    --hash=sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440 \
+    --hash=sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288 \
+    --hash=sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b \
+    --hash=sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958 \
+    --hash=sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b \
+    --hash=sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d \
+    --hash=sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a \
+    --hash=sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404 \
+    --hash=sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b \
+    --hash=sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e \
+    --hash=sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2 \
+    --hash=sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c \
+    --hash=sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b \
+    --hash=sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9 \
+    --hash=sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b \
+    --hash=sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636 \
+    --hash=sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99 \
+    --hash=sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e \
+    --hash=sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9
     # via
     #   -r requirements/base.in
     #   autobahn
     #   pyopenssl
     #   service-identity
     #   tahoe-lafs
     #   twisted
@@ -235,35 +304,35 @@
     # via tahoe-lafs
 eliot==1.14.0 \
     --hash=sha256:adc9c05263aa5527f1679e9af65728a06df1485f5a5e1ea94bc6f7081c14e479 \
     --hash=sha256:c2f099a3e8d5ecfc22745766e7cc664a48db64b6b89d986dff270491d8683149
     # via
     #   -r requirements/base.in
     #   tahoe-lafs
-filelock==3.9.0 \
-    --hash=sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de \
-    --hash=sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d
+filelock==3.12.0 \
+    --hash=sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9 \
+    --hash=sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718
     # via
     #   -r requirements/base.in
     #   tahoe-lafs
-foolscap==21.7.0 \
-    --hash=sha256:7520d5a2b6b2ac0b55d1c41c8bc1cdef65a611bbffc48ce0d1adcbd252e81e54 \
-    --hash=sha256:e9d18553860d9358e85d7662d9cd8bf3826d51b4ecd480a05dfbf4fc45363f84
+foolscap==23.3.0 \
+    --hash=sha256:56eee85c2d5baec801c2bdaae7d4c0831f23d401516e2e668d13485994db9145 \
+    --hash=sha256:c125982c80423a6c000fd8fd976972a14db8537f527f29403dacb44c7176a33e
     # via tahoe-lafs
-future==0.18.2 \
-    --hash=sha256:b1bead90b70cf6ec3f0710ae53a525360fa360d306a86583adc6bf83a4db537d
+future==0.18.3 \
+    --hash=sha256:34a17436ed1e96697a86f9de3d15a3b0be01d8bc8de9c1dffd59fb8234ed5307
     # via tahoe-lafs
 hkdf==0.0.3 \
     --hash=sha256:622a31c634bc185581530a4b44ffb731ed208acf4614f9c795bdd70e77991dca
     # via
     #   magic-wormhole
     #   spake2
-humanize==4.4.0 \
-    --hash=sha256:8830ebf2d65d0395c1bd4c79189ad71e023f277c2c7ae00f263124432e6f2ffa \
-    --hash=sha256:efb2584565cc86b7ea87a977a15066de34cdedaf341b11c851cfcfd2b964779c
+humanize==4.6.0 \
+    --hash=sha256:401201aca462749773f02920139f302450cb548b70489b9b4b92be39fe3c3c50 \
+    --hash=sha256:5f1f22bc65911eb1a6ffe7659bd6598e33dcfeeb904eb16ee1e705a09bf75916
     # via
     #   -r requirements/base.in
     #   magic-wormhole
 hyperlink==21.0.0 \
     --hash=sha256:427af957daa58bc909471c6c40f74c5450fa123dd093fc53efd2e91d2705a56b \
     --hash=sha256:e6b14c37ecb73e89c77d78cdb4c2cc8f3fb59a885c5b3f819ff4ed80f25af1b4
     # via
@@ -283,65 +352,75 @@
     --hash=sha256:912feeb5e0f7e0188e6f42241d2f450002e11bbc0937c65865045854c24c0bd0 \
     --hash=sha256:b864a1f30885ee72c5ac2835a761b8fe8aa9c28b9395cacf27286602688d3e51
     # via
     #   klein
     #   treq
     #   twisted
     #   txtorcon
-klein==21.8.0 \
-    --hash=sha256:5231df96787d13b498fbd75b37d4fb3920f8249364d06159c687ede4b8a2464d \
-    --hash=sha256:901dae754366e0a655d67afa02b4fb6c825de4bb26d7a3784b1634907e6dfed6
+klein==23.5.0 \
+    --hash=sha256:75e484974352783cf19cdc553eb60ff043b8d234d1b3c387cdbb1c53d646f5c3 \
+    --hash=sha256:906912b7ab410d9a7f351202839c3cd73a2ac077bd0071c861c31f0eef760287
     # via
     #   -r requirements/base.in
     #   tahoe-lafs
 magic-wormhole==0.12.0 \
     --hash=sha256:1b0fd8a334da978f3dd96b620fa9b9348cabedf26a87f74baac7a37052928160 \
     --hash=sha256:7c9a8d2a6e89314878dda23efc14c78398f1b6eb80e6c86c895c001c888d086e
     # via tahoe-lafs
-markupsafe==2.1.1 \
-    --hash=sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003 \
-    --hash=sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88 \
-    --hash=sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5 \
-    --hash=sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7 \
-    --hash=sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a \
-    --hash=sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603 \
-    --hash=sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1 \
-    --hash=sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135 \
-    --hash=sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247 \
-    --hash=sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6 \
-    --hash=sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601 \
-    --hash=sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77 \
-    --hash=sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02 \
-    --hash=sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e \
-    --hash=sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63 \
-    --hash=sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f \
-    --hash=sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980 \
-    --hash=sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b \
-    --hash=sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812 \
-    --hash=sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff \
-    --hash=sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96 \
-    --hash=sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1 \
-    --hash=sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925 \
-    --hash=sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a \
-    --hash=sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6 \
-    --hash=sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e \
-    --hash=sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f \
-    --hash=sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4 \
-    --hash=sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f \
-    --hash=sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3 \
-    --hash=sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c \
-    --hash=sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a \
-    --hash=sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417 \
-    --hash=sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a \
-    --hash=sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a \
-    --hash=sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37 \
-    --hash=sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452 \
-    --hash=sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933 \
-    --hash=sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a \
-    --hash=sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7
+markupsafe==2.1.2 \
+    --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
+    --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
+    --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
+    --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
+    --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
+    --hash=sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0 \
+    --hash=sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1 \
+    --hash=sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa \
+    --hash=sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03 \
+    --hash=sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323 \
+    --hash=sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65 \
+    --hash=sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013 \
+    --hash=sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036 \
+    --hash=sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f \
+    --hash=sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4 \
+    --hash=sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419 \
+    --hash=sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2 \
+    --hash=sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619 \
+    --hash=sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a \
+    --hash=sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a \
+    --hash=sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd \
+    --hash=sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7 \
+    --hash=sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666 \
+    --hash=sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65 \
+    --hash=sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859 \
+    --hash=sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625 \
+    --hash=sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff \
+    --hash=sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156 \
+    --hash=sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd \
+    --hash=sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba \
+    --hash=sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f \
+    --hash=sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1 \
+    --hash=sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094 \
+    --hash=sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a \
+    --hash=sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513 \
+    --hash=sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed \
+    --hash=sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d \
+    --hash=sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3 \
+    --hash=sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147 \
+    --hash=sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c \
+    --hash=sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603 \
+    --hash=sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601 \
+    --hash=sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a \
+    --hash=sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1 \
+    --hash=sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d \
+    --hash=sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3 \
+    --hash=sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54 \
+    --hash=sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2 \
+    --hash=sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6 \
+    --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
     # via werkzeug
 netifaces==0.11.0 \
     --hash=sha256:043a79146eb2907edf439899f262b3dfe41717d34124298ed281139a8b93ca32 \
     --hash=sha256:08e3f102a59f9eaef70948340aeb6c89bd09734e0dca0f3b82720305729f63ea \
     --hash=sha256:0f6133ac02521270d9f7c490f0c8c60638ff4aec8338efeff10a1b51506abe85 \
     --hash=sha256:18917fbbdcb2d4f897153c5ddbb56b31fa6dd7c3fa9608b7e3c3a663df8206b5 \
     --hash=sha256:2479bb4bb50968089a7c045f24d120f37026d7e802ec134c4490eae994c729b5 \
@@ -367,42 +446,42 @@
     --hash=sha256:c92ff9ac7c2282009fe0dcb67ee3cd17978cffbe0c8f4b471c00fe4325c9b4d4 \
     --hash=sha256:c9a3a47cd3aaeb71e93e681d9816c56406ed755b9442e981b07e3618fb71d2ac \
     --hash=sha256:cb925e1ca024d6f9b4f9b01d83215fd00fe69d095d0255ff3f64bffda74025c8 \
     --hash=sha256:d07b01c51b0b6ceb0f09fc48ec58debd99d2c8430b09e56651addeaf5de48048 \
     --hash=sha256:e76c7f351e0444721e85f975ae92718e21c1f361bda946d60a214061de1f00a1 \
     --hash=sha256:eb4813b77d5df99903af4757ce980a98c4d702bbcb81f32a0b305a1537bdf0b1
     # via tahoe-lafs
-psutil==5.9.4 \
-    --hash=sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff \
-    --hash=sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1 \
-    --hash=sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62 \
-    --hash=sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549 \
-    --hash=sha256:54c0d3d8e0078b7666984e11b12b88af2db11d11249a8ac8920dd5ef68a66e08 \
-    --hash=sha256:54d5b184728298f2ca8567bf83c422b706200bcbbfafdc06718264f9393cfeb7 \
-    --hash=sha256:6001c809253a29599bc0dfd5179d9f8a5779f9dffea1da0f13c53ee568115e1e \
-    --hash=sha256:68908971daf802203f3d37e78d3f8831b6d1014864d7a85937941bb35f09aefe \
-    --hash=sha256:6b92c532979bafc2df23ddc785ed116fced1f492ad90a6830cf24f4d1ea27d24 \
-    --hash=sha256:852dd5d9f8a47169fe62fd4a971aa07859476c2ba22c2254d4a1baa4e10b95ad \
-    --hash=sha256:9120cd39dca5c5e1c54b59a41d205023d436799b1c8c4d3ff71af18535728e94 \
-    --hash=sha256:c1ca331af862803a42677c120aff8a814a804e09832f166f226bfd22b56feee8 \
-    --hash=sha256:efeae04f9516907be44904cc7ce08defb6b665128992a56957abc9b61dca94b7 \
-    --hash=sha256:fd8522436a6ada7b4aad6638662966de0d61d241cb821239b2ae7013d41a43d4
+psutil==5.9.5 \
+    --hash=sha256:104a5cc0e31baa2bcf67900be36acde157756b9c44017b86b2c049f11957887d \
+    --hash=sha256:3c6f686f4225553615612f6d9bc21f1c0e305f75d7d8454f9b46e901778e7217 \
+    --hash=sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4 \
+    --hash=sha256:5410638e4df39c54d957fc51ce03048acd8e6d60abc0f5107af51e5fb566eb3c \
+    --hash=sha256:5b9b8cb93f507e8dbaf22af6a2fd0ccbe8244bf30b1baad6b3954e935157ae3f \
+    --hash=sha256:7a7dd9997128a0d928ed4fb2c2d57e5102bb6089027939f3b722f3a210f9a8da \
+    --hash=sha256:89518112647f1276b03ca97b65cc7f64ca587b1eb0278383017c2a0dcc26cbe4 \
+    --hash=sha256:8c5f7c5a052d1d567db4ddd231a9d27a74e8e4a9c3f44b1032762bd7b9fdcd42 \
+    --hash=sha256:ab8ed1a1d77c95453db1ae00a3f9c50227ebd955437bcf2a574ba8adbf6a74d5 \
+    --hash=sha256:acf2aef9391710afded549ff602b5887d7a2349831ae4c26be7c807c0a39fac4 \
+    --hash=sha256:b258c0c1c9d145a1d5ceffab1134441c4c5113b2417fafff7315a917a026c3c9 \
+    --hash=sha256:be8929ce4313f9f8146caad4272f6abb8bf99fc6cf59344a3167ecd74f4f203f \
+    --hash=sha256:c607bb3b57dc779d55e1554846352b4e358c10fff3abf3514a7a6601beebdb30 \
+    --hash=sha256:ea8518d152174e1249c4f2a1c89e3e6065941df2fa13a1ab45327716a23c2b48
     # via
     #   -r requirements/base.in
     #   tahoe-lafs
-pyasn1==0.4.8 \
-    --hash=sha256:39c7e2ec30515947ff4e87fb6f456dfc6e84857d34be479c9d4a4ba4bf46aa5d \
-    --hash=sha256:aef77c9fb94a3ac588e87841208bdec464471d9871bd5050a287cc9a475cd0ba
+pyasn1==0.5.0 \
+    --hash=sha256:87a2121042a1ac9358cabcaf1d07680ff97ee6404333bacca15f76aa8ad01a57 \
+    --hash=sha256:97b7290ca68e62a832558ec3976f15cbf911bf5d7c7039d8b861c2a0ece69fde
     # via
     #   pyasn1-modules
     #   service-identity
     #   twisted
-pyasn1-modules==0.2.8 \
-    --hash=sha256:905f84c712230b2c592c19470d3ca8d552de726050d1d1716282a1f6146be65e \
-    --hash=sha256:a50b808ffeb97cb3601dd25981f6b016cbb3d31fbf57a8b8a87428e6158d0c74
+pyasn1-modules==0.3.0 \
+    --hash=sha256:5bd01446b736eb9d31512a30d46c1ac3395d676c6f3cafa4c03eb54b9925631c \
+    --hash=sha256:d3ccd6ed470d9ffbc716be08bd90efbd44d0734bc9303818f7336070984a162d
     # via service-identity
 pycddl==0.4.0 \
     --hash=sha256:07d4c8d89ba58998fe7bae29f365c7d196de799b8ad6ebd9d318539f5063c5ef \
     --hash=sha256:29beb3665e4c0e115ead58641f4b7ab4885a74b6084e9522fd64ffb3362731b1 \
     --hash=sha256:2f6ba8aea040f7e3271dab4fc4d43da6d0c07806d8f62ef7129d37b6feff2f46 \
     --hash=sha256:37c21e2b2da26f80d923f2a0247028ccbcf3db58664f0e0b0469eac9ad9a1c88 \
     --hash=sha256:3d15788607051ae91aad3a299a7105713f038a958419e6bfb970dc045f0d982d \
@@ -437,17 +516,17 @@
     --hash=sha256:52cb72a79269189d4e0dc537556f4740f7f0a9ec41c1322598799b0bdad4ef92 \
     --hash=sha256:61f642bf2378713e2c2e1de73444a3778e5f0a38be6fee0fe532fe30060282ff \
     --hash=sha256:8ac7448f09ab85811607bdd21ec2464495ac8b7c66d146bf545b0f08fb9220ba \
     --hash=sha256:a36d4a9dda1f19ce6e03c9a784a2921a4b726b02e1c736600ca9c22029474394 \
     --hash=sha256:a422368fc821589c228f4c49438a368831cb5bbc0eab5ebe1d7fac9dded6567b \
     --hash=sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543
     # via magic-wormhole
-pyopenssl==23.0.0 \
-    --hash=sha256:c1cc5f86bcacefc84dada7d31175cae1b1518d5f60d3d0bb595a67822a868a6f \
-    --hash=sha256:df5fc28af899e74e19fccb5510df423581047e10ab6f1f4ba1763ff5fde844c0
+pyopenssl==23.1.1 \
+    --hash=sha256:841498b9bec61623b1b6c47ebbc02367c07d60e0e195f19790817f10cc8db0b7 \
+    --hash=sha256:9e0c526404a210df9d2b18cd33364beadb0dc858a739b885677bc65e105d4a4c
     # via
     #   foolscap
     #   twisted
 pyrsistent==0.19.3 \
     --hash=sha256:016ad1afadf318eb7911baa24b049909f7f3bb2c5b1ed7b6a8f21db21ea3faa8 \
     --hash=sha256:1a2994773706bbb4995c31a97bc94f1418314923bd1048c6d964837040376440 \
     --hash=sha256:20460ac0ea439a3e79caa1dbd560344b64ed75e85d8703943e0b66c2a6150e4a \
@@ -474,16 +553,16 @@
     --hash=sha256:e42296a09e83028b3476f7073fcb69ffebac0e66dbbfd1bd847d61f74db30f19 \
     --hash=sha256:e8f2b814a3dc6225964fa03d8582c6e0b6650d68a232df41e3cc1b66a5d2f8d1 \
     --hash=sha256:f0774bf48631f3a20471dd7c5989657b639fd2d285b861237ea9e82c36a415a9 \
     --hash=sha256:f0e7c4b2f77593871e918be000b96c8107da48444d57005b6a6bc61fb4331b2c
     # via
     #   eliot
     #   tahoe-lafs
-pyutil==3.3.0 \
-    --hash=sha256:8c4d4bf668c559186389bb9bce99e4b1b871c09ba252a756ccaacd2b8f401848
+pyutil==3.3.6 \
+    --hash=sha256:5dc3d6bb9c5bababb5d0b773e094045d75712e8b34af2d29b0e28602668267c0
     # via
     #   -r requirements/base.in
     #   tahoe-lafs
 pyyaml==6.0 \
     --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
     --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
     --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
@@ -521,25 +600,25 @@
     --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
     --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
     --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
     --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
     --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
     --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
     # via tahoe-lafs
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+requests==2.30.0 \
+    --hash=sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294 \
+    --hash=sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4
     # via treq
 service-identity==21.1.0 \
     --hash=sha256:6e6c6086ca271dc11b033d17c3a8bea9f24ebff920c587da090afc9519419d34 \
     --hash=sha256:f0b0caac3d40627c3c04d7a51b6e06721857a0e10a8775f2d1d7e72901b3a7db
     # via twisted
-setuptools==65.6.3 \
-    --hash=sha256:57f6f22bde4e042978bcd50176fdb381d7c21a9efa4041202288d3737a0c6a54 \
-    --hash=sha256:a7620757bf984b58deaf32fc8a4577a9bbc0850cf92c20e1ce41c38c19e5fb75
+setuptools==67.7.2 \
+    --hash=sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b \
+    --hash=sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990
     # via
     #   autobahn
     #   tahoe-lafs
     #   zope-interface
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
@@ -555,17 +634,17 @@
     --hash=sha256:c17a614b29ee4126206e22181f70a406c618d3c6c62ca6d6779bce95e9c926f4 \
     --hash=sha256:ce80705f8516c54364931f3b2c9a917ba001500d7f2fc76a0e8cf3bcaf0e30f7
     # via magic-wormhole
 tahoe-lafs==1.18.0 \
     --hash=sha256:3db9b215602b374bbf8027bdaed1d9853d0a330226ab1ecfdf19b72c87501146 \
     --hash=sha256:717a470df34edd31ad6b94467dabaa1caedd7f2f5233b04b89d8cfe936e317fe
     # via -r requirements/base.in
-tqdm==4.64.1 \
-    --hash=sha256:5f4f682a004951c1b450bc753c710e9280c5746ce6ffedee253ddbcbf54cf1e4 \
-    --hash=sha256:6fee160d6ffcd1b1c68c65f14c829c22832bc401726335ce92c52d395944a6a1
+tqdm==4.65.0 \
+    --hash=sha256:1871fb68a86b8fb3b59ca4cdd3dcccbc7e6d613eeed31f4c332531977b89beb5 \
+    --hash=sha256:c4f53a17fe37e132815abceec022631be8ffe1b9381c2e6e30aa70edc99e9671
     # via magic-wormhole
 treq==22.2.0 \
     --hash=sha256:27d95b07c5c14be3e7b280416139b036087617ad5595be913b1f9b3ce981b9b2 \
     --hash=sha256:df757e3f141fc782ede076a604521194ffcb40fa2645cf48e5a37060307f52ec
     # via
     #   -r requirements/base.in
     #   tahoe-lafs
@@ -581,33 +660,33 @@
     #   foolscap
     #   klein
     #   magic-wormhole
     #   tahoe-lafs
     #   treq
     #   tubes
     #   txtorcon
-txaio==22.2.1 \
-    --hash=sha256:2e4582b70f04b2345908254684a984206c0d9b50e3074a24a4c55aba21d24d01 \
-    --hash=sha256:41223af4a9d5726e645a8ee82480f413e5e300dd257db94bc38ae12ea48fb2e5
+txaio==23.1.1 \
+    --hash=sha256:aaea42f8aad50e0ecfb976130ada140797e9dcb85fad2cf72b0f37f8cefcb490 \
+    --hash=sha256:f9a9216e976e5e3246dfd112ad7ad55ca915606b60b84a757ac769bd404ff704
     # via autobahn
-txtorcon==22.0.0 \
-    --hash=sha256:824b5df1977bedabfc1c49c9523b8fa1b7cff11d6fee78015df1ce133685779c \
-    --hash=sha256:89a1b65e32a4b369d67e6c166387fbc468cc5d05227448d239a5e7e9718aa053
+txtorcon==23.0.0 \
+    --hash=sha256:0225ffad67689137849ad9ad34adb569b0d88f9af0450300067a5f901e994325 \
+    --hash=sha256:bd7739573cf159b2ac0ac314329f45dd91a7245a4f141258aa5fa23117421869
     # via magic-wormhole
-typing-extensions==4.4.0 \
-    --hash=sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa \
-    --hash=sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e
+typing-extensions==4.5.0 \
+    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
+    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via twisted
-urllib3==1.26.13 \
-    --hash=sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc \
-    --hash=sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8
+urllib3==2.0.2 \
+    --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
+    --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
     # via requests
-werkzeug==2.2.2 \
-    --hash=sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f \
-    --hash=sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5
+werkzeug==2.3.3 \
+    --hash=sha256:4866679a0722de00796a74086238bb3b98d90f423f05de039abb09315487254a \
+    --hash=sha256:a987caf1092edc7523edb139edb20c70571c4a8d5eed02e0b547b4739174d091
     # via
     #   klein
     #   tahoe-lafs
 zfec==1.5.7.2 \
     --hash=sha256:01b47b1144940a620393d38d12d381a6f3e6522e96d834d658e095422876fdc8 \
     --hash=sha256:07f0a7862b21cd3e2484cf774310b7aadb7e440cae1fb646fe1fe3706b5072de \
     --hash=sha256:08e3d2c815ab4c92809dadee6b286ea48d5a2b190128275bb6734d4327ff9132 \
@@ -642,51 +721,45 @@
     --hash=sha256:bbac2e34ef9c4aad8da02112c67926f8b473616f49f2738adf1a29bd36e8abf1 \
     --hash=sha256:bd243cf9f76a4d9250f90900b3acd7b4403984618148f7c08c5dec974418166f \
     --hash=sha256:c4fcbd28b2a04d59301a60381ffd6bb2db65be1d15c7928da0c11d57683c5e86 \
     --hash=sha256:e6a2325ff4d4a30e6b92a2c25241120639c39697d6514906559b45387e937233 \
     --hash=sha256:e8736aee43bee6684741542e21de6db4cb6dc639c8e9e7d6258eacf4fe34085d \
     --hash=sha256:eb54b0ab948a82e35f25a972a7ecdcef12d2d201a38d0308a21ea64442d41a7d
     # via tahoe-lafs
-zope-interface==5.5.2 \
-    --hash=sha256:008b0b65c05993bb08912f644d140530e775cf1c62a072bf9340c2249e613c32 \
-    --hash=sha256:0217a9615531c83aeedb12e126611b1b1a3175013bbafe57c702ce40000eb9a0 \
-    --hash=sha256:0fb497c6b088818e3395e302e426850f8236d8d9f4ef5b2836feae812a8f699c \
-    --hash=sha256:17ebf6e0b1d07ed009738016abf0d0a0f80388e009d0ac6e0ead26fc162b3b9c \
-    --hash=sha256:311196634bb9333aa06f00fc94f59d3a9fddd2305c2c425d86e406ddc6f2260d \
-    --hash=sha256:3218ab1a7748327e08ef83cca63eea7cf20ea7e2ebcb2522072896e5e2fceedf \
-    --hash=sha256:404d1e284eda9e233c90128697c71acffd55e183d70628aa0bbb0e7a3084ed8b \
-    --hash=sha256:4087e253bd3bbbc3e615ecd0b6dd03c4e6a1e46d152d3be6d2ad08fbad742dcc \
-    --hash=sha256:40f4065745e2c2fa0dff0e7ccd7c166a8ac9748974f960cd39f63d2c19f9231f \
-    --hash=sha256:5334e2ef60d3d9439c08baedaf8b84dc9bb9522d0dacbc10572ef5609ef8db6d \
-    --hash=sha256:604cdba8f1983d0ab78edc29aa71c8df0ada06fb147cea436dc37093a0100a4e \
-    --hash=sha256:6373d7eb813a143cb7795d3e42bd8ed857c82a90571567e681e1b3841a390d16 \
-    --hash=sha256:655796a906fa3ca67273011c9805c1e1baa047781fca80feeb710328cdbed87f \
-    --hash=sha256:65c3c06afee96c654e590e046c4a24559e65b0a87dbff256cd4bd6f77e1a33f9 \
-    --hash=sha256:696f3d5493eae7359887da55c2afa05acc3db5fc625c49529e84bd9992313296 \
-    --hash=sha256:6e972493cdfe4ad0411fd9abfab7d4d800a7317a93928217f1a5de2bb0f0d87a \
-    --hash=sha256:7579960be23d1fddecb53898035a0d112ac858c3554018ce615cefc03024e46d \
-    --hash=sha256:765d703096ca47aa5d93044bf701b00bbce4d903a95b41fff7c3796e747b1f1d \
-    --hash=sha256:7e66f60b0067a10dd289b29dceabd3d0e6d68be1504fc9d0bc209cf07f56d189 \
-    --hash=sha256:8a2ffadefd0e7206adc86e492ccc60395f7edb5680adedf17a7ee4205c530df4 \
-    --hash=sha256:959697ef2757406bff71467a09d940ca364e724c534efbf3786e86eee8591452 \
-    --hash=sha256:9d783213fab61832dbb10d385a319cb0e45451088abd45f95b5bb88ed0acca1a \
-    --hash=sha256:a16025df73d24795a0bde05504911d306307c24a64187752685ff6ea23897cb0 \
-    --hash=sha256:a2ad597c8c9e038a5912ac3cf166f82926feff2f6e0dabdab956768de0a258f5 \
-    --hash=sha256:bfee1f3ff62143819499e348f5b8a7f3aa0259f9aca5e0ddae7391d059dce671 \
-    --hash=sha256:d169ccd0756c15bbb2f1acc012f5aab279dffc334d733ca0d9362c5beaebe88e \
-    --hash=sha256:d514c269d1f9f5cd05ddfed15298d6c418129f3f064765295659798349c43e6f \
-    --hash=sha256:d692374b578360d36568dd05efb8a5a67ab6d1878c29c582e37ddba80e66c396 \
-    --hash=sha256:dbaeb9cf0ea0b3bc4b36fae54a016933d64c6d52a94810a63c00f440ecb37dd7 \
-    --hash=sha256:dc26c8d44472e035d59d6f1177eb712888447f5799743da9c398b0339ed90b1b \
-    --hash=sha256:e1574980b48c8c74f83578d1e77e701f8439a5d93f36a5a0af31337467c08fcf \
-    --hash=sha256:e74a578172525c20d7223eac5f8ad187f10940dac06e40113d62f14f3adb1e8f \
-    --hash=sha256:e945de62917acbf853ab968d8916290548df18dd62c739d862f359ecd25842a6 \
-    --hash=sha256:f0980d44b8aded808bec5059018d64692f0127f10510eca71f2f0ace8fb11188 \
-    --hash=sha256:f98d4bd7bbb15ca701d19b93263cc5edfd480c3475d163f137385f49e5b3a3a7 \
-    --hash=sha256:fb68d212efd057596dee9e6582daded9f8ef776538afdf5feceb3059df2d2e7b
+zope-interface==6.0 \
+    --hash=sha256:042f2381118b093714081fd82c98e3b189b68db38ee7d35b63c327c470ef8373 \
+    --hash=sha256:0ec9653825f837fbddc4e4b603d90269b501486c11800d7c761eee7ce46d1bbb \
+    --hash=sha256:12175ca6b4db7621aedd7c30aa7cfa0a2d65ea3a0105393e05482d7a2d367446 \
+    --hash=sha256:1592f68ae11e557b9ff2bc96ac8fc30b187e77c45a3c9cd876e3368c53dc5ba8 \
+    --hash=sha256:23ac41d52fd15dd8be77e3257bc51bbb82469cf7f5e9a30b75e903e21439d16c \
+    --hash=sha256:424d23b97fa1542d7be882eae0c0fc3d6827784105264a8169a26ce16db260d8 \
+    --hash=sha256:4407b1435572e3e1610797c9203ad2753666c62883b921318c5403fb7139dec2 \
+    --hash=sha256:48f4d38cf4b462e75fac78b6f11ad47b06b1c568eb59896db5b6ec1094eb467f \
+    --hash=sha256:4c3d7dfd897a588ec27e391edbe3dd320a03684457470415870254e714126b1f \
+    --hash=sha256:5171eb073474a5038321409a630904fd61f12dd1856dd7e9d19cd6fe092cbbc5 \
+    --hash=sha256:5a158846d0fca0a908c1afb281ddba88744d403f2550dc34405c3691769cdd85 \
+    --hash=sha256:6ee934f023f875ec2cfd2b05a937bd817efcc6c4c3f55c5778cbf78e58362ddc \
+    --hash=sha256:790c1d9d8f9c92819c31ea660cd43c3d5451df1df61e2e814a6f99cebb292788 \
+    --hash=sha256:809fe3bf1a91393abc7e92d607976bbb8586512913a79f2bf7d7ec15bd8ea518 \
+    --hash=sha256:87b690bbee9876163210fd3f500ee59f5803e4a6607d1b1238833b8885ebd410 \
+    --hash=sha256:89086c9d3490a0f265a3c4b794037a84541ff5ffa28bb9c24cc9f66566968464 \
+    --hash=sha256:99856d6c98a326abbcc2363827e16bd6044f70f2ef42f453c0bd5440c4ce24e5 \
+    --hash=sha256:aab584725afd10c710b8f1e6e208dbee2d0ad009f57d674cb9d1b3964037275d \
+    --hash=sha256:af169ba897692e9cd984a81cb0f02e46dacdc07d6cf9fd5c91e81f8efaf93d52 \
+    --hash=sha256:b39b8711578dcfd45fc0140993403b8a81e879ec25d53189f3faa1f006087dca \
+    --hash=sha256:b3f543ae9d3408549a9900720f18c0194ac0fe810cecda2a584fd4dca2eb3bb8 \
+    --hash=sha256:d0583b75f2e70ec93f100931660328965bb9ff65ae54695fb3fa0a1255daa6f2 \
+    --hash=sha256:dfbbbf0809a3606046a41f8561c3eada9db811be94138f42d9135a5c47e75f6f \
+    --hash=sha256:e538f2d4a6ffb6edfb303ce70ae7e88629ac6e5581870e66c306d9ad7b564a58 \
+    --hash=sha256:eba51599370c87088d8882ab74f637de0c4f04a6d08a312dce49368ba9ed5c2a \
+    --hash=sha256:ee4b43f35f5dc15e1fec55ccb53c130adb1d11e8ad8263d68b1284b66a04190d \
+    --hash=sha256:f2363e5fd81afb650085c6686f2ee3706975c54f331b426800b53531191fdf28 \
+    --hash=sha256:f299c020c6679cb389814a3b81200fe55d428012c5e76da7e722491f5d205990 \
+    --hash=sha256:f72f23bab1848edb7472309e9898603141644faec9fd57a823ea6b4d1c4c8995 \
+    --hash=sha256:fa90bac61c9dc3e1a563e5babb3fd2c0c1c80567e815442ddbe561eadc803b30
     # via
     #   -r requirements/base.in
     #   autobahn
     #   eliot
     #   klein
     #   tahoe-lafs
     #   twisted
```

### Comparing `magic-folder-23.5.0/requirements/build.txt` & `magic-folder-23.6.0/requirements/build.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,100 +2,89 @@
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-bleach==5.0.1 \
-    --hash=sha256:085f7f33c15bd408dd9b17a4ad77c577db66d76203e5984b1bd59baeee948b2a \
-    --hash=sha256:0d03255c47eb9bd2f26aa9bb7f2107732e7e8fe195ca2f64709fcf3b0a4a085c
+bleach==6.0.0 \
+    --hash=sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414 \
+    --hash=sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4
     # via readme-renderer
 click-default-group==1.2.2 \
     --hash=sha256:d9560e8e8dfa44b3562fbc9425042a0fd6d21956fcc2db0077f63f34253ab904
     # via towncrier
-commonmark==0.9.1 \
-    --hash=sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60 \
-    --hash=sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9
-    # via rich
 docutils==0.19 \
     --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
     --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
     # via readme-renderer
-dulwich==0.20.50 \
-    --hash=sha256:06775c5713cfeda778c7c67d4422b5e7554d3a7f644f1dde646cdf486a30285a \
-    --hash=sha256:0c61c193d02c0e1e0d758cdd57ae76685c368d09a01f00d704ba88bd96767cfe \
-    --hash=sha256:0e4862f318d99cc8a500e3622a89613a88c07d957a0f628cdc2ed86addff790f \
-    --hash=sha256:0f9c4f2455f966cad94648278fa9972e4695b35d04f82792fa58e1ea15dd83f0 \
-    --hash=sha256:11b180b80363b4fc70664197028181a17ae4c52df9965a29b62a6c52e40c2dbe \
-    --hash=sha256:2644466270267270f2157ea6f1c0aa224f6f3bf06a307fc39954e6b4b3d82bae \
-    --hash=sha256:2aa2a4a84029625bf9c63771f8a628db1f3be2d2ea3cb8b17942cd4317797152 \
-    --hash=sha256:322ff8ff6aa4d6d36294cd36de1c84767eb1903c7db3e7b4475ad091febf5363 \
-    --hash=sha256:3b1964fa80cafd5a1fd71615b0313daf6f3295c6ab05656ea0c1d2423539904a \
-    --hash=sha256:3fb35cedb1243bc420d885ef5b4afd642c6ac8f07ddfc7fdbca1becf9948bf7e \
-    --hash=sha256:4842e22ed863a776b36ef8ffe9ed7b772eb452b42c8d02975c29d27e3bc50ab4 \
-    --hash=sha256:49f66f1c057c18d7d60363f461f4ab8329320fbe1f02a7a33c255864a7d3c942 \
-    --hash=sha256:4aa1d0861517ebbbe0e0084cc9ab4f7ab720624a3eda2bd10e45f774ab858db8 \
-    --hash=sha256:4bb23a9cec63e16c0e432335f068169b73dd44fa9318dd7cd7a4ca83607ff367 \
-    --hash=sha256:4e541cd690a5e3d55082ed51732d755917e933cddeb4b0204f2a5ec5d5d7b60b \
-    --hash=sha256:50a941796b2c675be39be728d540c16b5b7ce77eb9e1b3f855650ece6832d2be \
-    --hash=sha256:519b627d49d273e2fd01c79d09e578675ca6cd05193c1787e9ef165c9a1d66ea \
-    --hash=sha256:5267619b34ddaf8d9a6b841492cd17a971fd25bf9a5657f2de928385c3a08b94 \
-    --hash=sha256:5411d0f1092152e1c0bb916ae490fe181953ae1b8d13f4e68661253e10b78dbb \
-    --hash=sha256:57bff9bde0b6b05b00c6acbb1a94357caddb2908ed7026a48c715ff50d220335 \
-    --hash=sha256:583c6bbc27f13fe2e41a19f6987a42681c6e4f6959beae0a6e5bb033b8b081a8 \
-    --hash=sha256:5d3290a45651c8e534f8e83ae2e30322aefdd162f0f338bae2e79a6ee5a87513 \
-    --hash=sha256:6343569f998ce429e2a5d813c56768ac51b496522401db950f0aa44240bfa901 \
-    --hash=sha256:6a75cab01b909c4c683c2083e060e378bc01701b7366b5a7d9846ef6d3b9e3d5 \
-    --hash=sha256:6d409a282f8848fd6c8d7c7545ad2f75c16de5d5977de202642f1d50fdaac554 \
-    --hash=sha256:7301773e5cc16d521bc6490e73772a86a4d1d0263de506f08b54678cc4e2f061 \
-    --hash=sha256:731e7f319b34251fadeb362ada1d52cc932369d9cdfa25c0e41150cda28773d0 \
-    --hash=sha256:78c388ad421199000fb7b5ed5f0c7b509b3e31bd7cad303786a4d0bf89b82f60 \
-    --hash=sha256:790e4a641284a7fb4d56ebdaf8b324a5826fbbb9c54307c06f586f9f6a5e56db \
-    --hash=sha256:7aaabb8e4beadd53f75f853a981caaadef3ef130e5645c902705704eaf136daa \
-    --hash=sha256:80ab07131a6e68594441f5c4767e9e44e87fceafc3e347e541c928a18c679bd8 \
-    --hash=sha256:80e8750ee2fa0ab2784a095956077758e5f6107de27f637c4b9d18406652c22c \
-    --hash=sha256:8cc6092a4f0bbbff2e553e87a9c6325955b64ea43fca21297c8182e19ae8a43c \
-    --hash=sha256:8f3af857f94021cae1322d86925bfc0dd31e501e885ab5db275473bfac0bb39d \
-    --hash=sha256:9091f1d53a3c0747cbf0bd127c64e7f09b770264d8fb53e284383fcdf69154e7 \
-    --hash=sha256:9163fbb021a8ad9c35a0814a5eedf45a8eb3a0b764b865d7016d901fc5a947fc \
-    --hash=sha256:97f02f8d500d4af08dc022d697c56e8539171acc3f575c2fe9acf3b078e5c8c9 \
-    --hash=sha256:a24a3893108f3b97beb958670d5f3f2a3bec73a1fe18637a572a85abd949a1c4 \
-    --hash=sha256:a344230cadfc5d315752add6ce9d4cfcfc6c85e36bbf57fce9444bcc7c6ea8fb \
-    --hash=sha256:a405cd236766060894411614a272cfb86fe86cde5ca73ef264fc4fa5a715fff4 \
-    --hash=sha256:a6ec7c8fea2b44187a3b545e6c11ab9947ffb122647b07abcdb7cc3aaa770c0e \
-    --hash=sha256:af4adac92fb95671ea3a24f2f8e5e5e8f638711ce9c33a3ca6cd68bf1ff7d99f \
-    --hash=sha256:b4d11d44176e5d2fa8271fc86ad1e0a8731b9ad8f77df64c12846b30e16135eb \
-    --hash=sha256:b70106580ed11f45f4c32d2831d0c9c9f359bc2415fff4a6be443e3a36811398 \
-    --hash=sha256:c075f69c2de19d9fd97e3b70832d2b42c6a4a5d909b3ffd1963b67d86029f95f \
-    --hash=sha256:c2edbff3053251985f10702adfafbee118298d383ef5b5b432a5f22d1f1915df \
-    --hash=sha256:c3dc9f97ec8d3db08d9723b9fd06f3e52c15b84c800d153cfb59b0a3dc8b8d40 \
-    --hash=sha256:c7542a72c5640dd0620862d6df8688f02a6c336359b5af9b3fcfe11b7fa6652f \
-    --hash=sha256:c83e7840d9d0a94d7033bc109efe0c22dfcdcd816bcd4469085e42809e3bf5ba \
-    --hash=sha256:c96e3fb9d48c0454dc242c7accc7819780c9a7f29e441a9eff12361ed0fa35f9 \
-    --hash=sha256:cb194c53109131bcbcd1ca430fcd437cdaf2d33e204e45fbe121c47eaa43e9af \
-    --hash=sha256:d2f7df39bd1378d3b0bfb3e7fc930fd0191924af1f0ef587bcd9946afe076c06 \
-    --hash=sha256:d3ee45001411b638641819b7b3b33f31f13467c84066e432256580fcab7d8815 \
-    --hash=sha256:d4629635a97e3af1b5da48071e00c8e70fad85f3266fadabe1f5a8f49172c507 \
-    --hash=sha256:dd9fa00971ecf059bb358085a942ecac5be4ff71acdf299f44c8cbc45c18659f \
-    --hash=sha256:df3562dde3079d57287c233d45b790bc967c5aae975c9a7b07ca30e60e055512 \
-    --hash=sha256:e1ae18d5805f0c0c5dac65795f8d48660437166b12ee2c0ffea95bfdbf9c1051 \
-    --hash=sha256:e29a3c2037761fa816aa556e78364dfc8e3f44b873db2d17aed96f9b06ac83a3 \
-    --hash=sha256:ea8ffe26d91dbcd5580dbd5a07270a12ea57b091604d77184da0a0d9fad50ed3 \
-    --hash=sha256:ee0f9b02019c0ea84cdd31c00a0c283669b771c85612997a911715cf84e33d99 \
-    --hash=sha256:eefe786a6010f8546baac4912113eeed4e397ddb8c433a345b548a04d4176496 \
-    --hash=sha256:f08406b6b789dea5c95ba1130a0801d8748a67f18be940fe7486a8b481fde875 \
-    --hash=sha256:fbb6368f18451dc44c95c55e1a609d1a01d3821f7ed480b22b2aea1baca0f4a7
+dulwich==0.21.5 \
+    --hash=sha256:0aa44b812d978fc22a04531f5090c3c369d5facd03fa6e0501d460a661800c7f \
+    --hash=sha256:0ab86d6d42e385bf3438e70f3c9b16de68018bd88929379e3484c0ef7990bd3c \
+    --hash=sha256:1b20a3656b48c941d49c536824e1e5278a695560e8de1a83b53a630143c4552e \
+    --hash=sha256:1cc0c9ba19ac1b2372598802bc9201a9c45e5d6f1f7a80ec40deeb10acc4e9ae \
+    --hash=sha256:1e39b7c2c9bda6acae83b25054650a8bb7e373e886e2334721d384e1479bf04b \
+    --hash=sha256:26456dba39d1209fca17187db06967130e27eeecad2b3c2bbbe63467b0bf09d6 \
+    --hash=sha256:281310644e02e3aa6d76bcaffe2063b9031213c4916b5f1a6e68c25bdecfaba4 \
+    --hash=sha256:2aba0fdad2a19bd5bb3aad6882580cb33359c67b48412ccd4cfccd932012b35e \
+    --hash=sha256:32493a456358a3a6c15bbda07106fc3d4cc50834ee18bc7717968d18be59b223 \
+    --hash=sha256:3800cdc17d144c1f7e114972293bd6c46688f5bcc2c9228ed0537ded72394082 \
+    --hash=sha256:3932b5e17503b265a85f1eda77ede647681c3bab53bc9572955b6b282abd26ea \
+    --hash=sha256:3e68b162af2aae995355e7920f89d50d72b53d56021e5ac0a546d493b17cbf7e \
+    --hash=sha256:3e8f6d4f4f4d01dd1d3c968e486d4cd77f96f772da7265941bc506de0944ddb9 \
+    --hash=sha256:45d6198e804b539708b73a003419e48fb42ff2c3c6dd93f63f3b134dff6dd259 \
+    --hash=sha256:4814ca3209dabe0fe7719e9545fbdad7f8bb250c5a225964fe2a31069940c4cf \
+    --hash=sha256:494024f74c2eef9988adb4352b3651ac1b6c0466176ec62b69d3d3672167ba68 \
+    --hash=sha256:4db330fb59fe3b9d253bdf0e49a521739db83689520c4921ab1c5242aaf77b82 \
+    --hash=sha256:5e56b2c1911c344527edb2bf1a4356e2fb7e086b1ba309666e1e5c2224cdca8a \
+    --hash=sha256:5e8a79c1ed7166f32ad21974fa98d11bf6fd74e94a47e754c777c320e01257c6 \
+    --hash=sha256:6155ab7388ee01c670f7c5d8003d4e133eebebc7085a856c007989f0ba921b36 \
+    --hash=sha256:61e10242b5a7a82faa8996b2c76239cfb633620b02cdd2946e8af6e7eb31d651 \
+    --hash=sha256:6616132d219234580de88ceb85dd51480dc43b1bdc05887214b8dd9cfd4a9d40 \
+    --hash=sha256:684c52cff867d10c75a7238151ca307582b3d251bbcd6db9e9cffbc998ef804e \
+    --hash=sha256:6f46bcb6777e5f9f4af24a2bd029e88b77316269d24ce66be590e546a0d8f7b7 \
+    --hash=sha256:70955e4e249ddda6e34a4636b90f74e931e558f993b17c52570fa6144b993103 \
+    --hash=sha256:7dc358c2ee727322a09b7c6da43d47a1026049dbd3ad8d612eddca1f9074b298 \
+    --hash=sha256:7f357639b56146a396f48e5e0bc9bbaca3d6d51c8340bd825299272b588fff5f \
+    --hash=sha256:7fe62685bf356bfb4d0738f84a3fcf0d1fc9e11fee152e488a20b8c66a52429e \
+    --hash=sha256:823091d6b6a1ea07dc4839c9752198fb39193213d103ac189c7669736be2eaff \
+    --hash=sha256:82cdf482f8f51fcc965ffad66180b54a9abaea9b1e985a32e1acbfedf6e0e363 \
+    --hash=sha256:82f632afb9c7c341a875d46aaa3e6c5e586c7a64ce36c9544fa400f7e4f29754 \
+    --hash=sha256:85d3401d08b1ec78c7d58ae987c4bb7b768a438f3daa74aeb8372bebc7fb16fa \
+    --hash=sha256:8864719bc176cdd27847332a2059127e2f7bab7db2ff99a999873cb7fff54116 \
+    --hash=sha256:891d5c73e2b66d05dbb502e44f027dc0dbbd8f6198bc90dae348152e69d0befc \
+    --hash=sha256:9019189d7a8f7394df6a22cd5b484238c5776e42282ad5d6d6c626b4c5f43597 \
+    --hash=sha256:90479608e49db93d8c9e4323bc0ec5496678b535446e29d8fd67dc5bbb5d51bf \
+    --hash=sha256:a605e10d72f90a39ea2e634fbfd80f866fc4df29a02ea6db52ae92e5fd4a2003 \
+    --hash=sha256:a917fd3b4493db3716da2260f16f6b18f68d46fbe491d851d154fc0c2d984ae4 \
+    --hash=sha256:aae448da7d80306dda4fc46292fed7efaa466294571ab3448be16714305076f1 \
+    --hash=sha256:aeb736d777ee21f2117a90fc453ee181aa7eedb9e255b5ef07c51733f3fe5cb6 \
+    --hash=sha256:b24cb1fad0525dba4872e9381bc576ea2a6dcdf06b0ed98f8e953e3b1d719b89 \
+    --hash=sha256:b2c9931b657f2206abec0964ec2355ee2c1e04d05f8864e823ffa23c548c4548 \
+    --hash=sha256:b943517e30bd651fbc275a892bb96774f3893d95fe5a4dedd84496a98eaaa8ab \
+    --hash=sha256:baecef0d8b9199822c7912876a03a1af17833f6c0d461efb62decebd45897e49 \
+    --hash=sha256:be12a46f73023970125808a4a78f610c055373096c1ecea3280edee41613eba8 \
+    --hash=sha256:c2a565d4e704d7f784cdf9637097141f6d47129c8fffc2fac699d57cb075a169 \
+    --hash=sha256:c8ded43dc0bd2e65420eb01e778034be5ca7f72e397a839167eda7dcb87c4248 \
+    --hash=sha256:c922a4573267486be0ef85216f2da103fb38075b8465dc0e90457843884e4860 \
+    --hash=sha256:daa607370722c3dce99a0022397c141caefb5ed32032a4f72506f4817ea6405b \
+    --hash=sha256:e2f676bfed8146966fe934ee734969d7d81548fbd250a8308582973670a9dab1 \
+    --hash=sha256:e52b20c4368171b7d32bd3ab0f1d2402e76ad4f2ea915ff9aa73bc9fa2b54d6d \
+    --hash=sha256:eaf6c7fb6b13495c19c9aace88821c2ade3c8c55b4e216cd7cc55d3e3807d7fa \
+    --hash=sha256:f2eeca6d61366cf5ee8aef45bed4245a67d4c0f0d731dc2383eabb80fa695683 \
+    --hash=sha256:f9a6bf99f57bcac4c77fc60a58f1b322c91cc4d8c65dc341f76bf402622f89cb \
+    --hash=sha256:f9b6ac1b1c67fc6083c42b7b6cd3b211292c8a6517216c733caf23e8b103ab6d \
+    --hash=sha256:fd4ad079758514375f11469e081723ba8831ce4eaa1a64b41f06a3a866d5ac34
     # via -r requirements/build.in
 gpg==1.10.0 \
     --hash=sha256:349214a866c84aa548bc35ed14eccd2ec9085b3958d5753a63a19a71a1f523ca
     # via -r requirements/build.in
-importlib-metadata==6.0.0 \
-    --hash=sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad \
-    --hash=sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d
+importlib-metadata==6.6.0 \
+    --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
+    --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3 \
     --hash=sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158 \
     --hash=sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a
     # via keyring
@@ -109,49 +98,57 @@
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
     # via towncrier
 keyring==23.13.1 \
     --hash=sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd \
     --hash=sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678
     # via twine
-more-itertools==9.0.0 \
-    --hash=sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41 \
-    --hash=sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab
+markdown-it-py==2.2.0 \
+    --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
+    --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
+    # via rich
+mdurl==0.1.2 \
+    --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
+    --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
+    # via markdown-it-py
+more-itertools==9.1.0 \
+    --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
+    --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
     # via jaraco-classes
-packaging==23.0 \
-    --hash=sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2 \
-    --hash=sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97
+packaging==23.1 \
+    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
+    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via setuptools-scm
 pkginfo==1.9.6 \
     --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
     --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
     # via twine
-pygments==2.14.0 \
-    --hash=sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297 \
-    --hash=sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717
+pygments==2.15.1 \
+    --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
+    --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via
     #   readme-renderer
     #   rich
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via
     #   -r requirements/build.in
     #   twine
-requests-toolbelt==0.10.1 \
-    --hash=sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7 \
-    --hash=sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d
+requests-toolbelt==1.0.0 \
+    --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
+    --hash=sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06
     # via twine
 rfc3986==2.0.0 \
     --hash=sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd \
     --hash=sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c
     # via twine
-rich==13.0.1 \
-    --hash=sha256:25f83363f636995627a99f6e4abc52ed0970ebbd544960cc63cbb43aaac3d6f0 \
-    --hash=sha256:41fe1d05f433b0f4724cda8345219213d2bfa472ef56b2f64f415b5b94d51b04
+rich==13.3.5 \
+    --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
+    --hash=sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704
     # via twine
 secretstorage==3.3.3 \
     --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
     --hash=sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99
     # via keyring
 setuptools-scm==7.1.0 \
     --hash=sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27 \
@@ -171,15 +168,15 @@
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
     # via -r requirements/build.in
 webencodings==0.5.1 \
     --hash=sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78 \
     --hash=sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923
     # via bleach
-wheel==0.38.4 \
-    --hash=sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac \
-    --hash=sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8
-    # via -r requirements/build.in
-zipp==3.11.0 \
-    --hash=sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa \
-    --hash=sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766
+wheel==0.40.0 \
+    --hash=sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873 \
+    --hash=sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247
+    # via -r requirements/build.in
+zipp==3.15.0 \
+    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
+    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
     # via importlib-metadata
```

### Comparing `magic-folder-23.5.0/requirements/platform.txt` & `magic-folder-23.6.0/requirements/platform.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/requirements/test.in` & `magic-folder-23.6.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/requirements/test.txt` & `magic-folder-23.6.0/requirements/test.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,99 @@
-# SHA1:a8c8542a688b0f0536686bca85d0e10566072c05
+# SHA1:37361896904be50f54e60c721e99ff39f798096c
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-cachetools==5.2.1 \
-    --hash=sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe \
-    --hash=sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da
+cachetools==5.3.0 \
+    --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
+    --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
     # via tox
 chardet==5.1.0 \
     --hash=sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5 \
     --hash=sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9
     # via tox
 click-default-group==1.2.2 \
     --hash=sha256:d9560e8e8dfa44b3562fbc9425042a0fd6d21956fcc2db0077f63f34253ab904
     # via towncrier
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via
     #   -r requirements/test.in
     #   tox
-coverage==7.0.4 \
-    --hash=sha256:0322354757b47640535daabd2d56384ff3cad2896248fc84d328c5fad4922d5c \
-    --hash=sha256:053cdc47cae08257051d7e934a0de4d095b60eb8a3024fa9f1b2322fa1547137 \
-    --hash=sha256:0815a09b32384e8ff00a5939ec9cd10efce8742347e019c2daca1a32f5ac2aae \
-    --hash=sha256:1791e5f74c5b52f76e83fe9f4bb9571cf76d40ee0c51952ee1e4ee935b7e98b9 \
-    --hash=sha256:1ba5cc54baf3c322c4388de2a43cc95f7809366f0600e743e5aae8ea9d1038b2 \
-    --hash=sha256:1e9e94f2612ee549a4b3ee79cbc61bceed77e69cf38cfa05858bae939a886d16 \
-    --hash=sha256:22d8ef6865cb6834cab2b72fff20747a55c714b57b675f7e11c9624fe4f7cb45 \
-    --hash=sha256:260854160083f8275a9d9d49a05ab0ffc7a1f08f2ccccbfaec94a18aae9f407c \
-    --hash=sha256:2904d7a0388911c61e7e3beefe48c29dfccaba938fc1158f63190101a21e04c2 \
-    --hash=sha256:2b5936b624fbe711ed02dfd86edd678822e5ee68da02b6d231e5c01090b64590 \
-    --hash=sha256:2b854f7985b48122b6fe346631e86d67b63293f8255cb59a93d79e3d9f1574e3 \
-    --hash=sha256:2dfbee0bf0d633be3a2ab068f5a5731a70adf147d0ba17d9f9932b46c7c5782b \
-    --hash=sha256:2e59aef3fba5758059208c9eff10ae7ded3629e797972746ec33b56844f69411 \
-    --hash=sha256:32dc010713455ac0fe2fddb0e48aa43875cc7eb7b09768df10bad8ce45f9c430 \
-    --hash=sha256:34c0457e1ba450ae8b22dc8ea2fd36ada1010af61291e4c96963cd9d9633366f \
-    --hash=sha256:3d9201cfa5a98652b9cef36ab202f17fe3ea83f497b4ba2a8ed39399dfb8fcd4 \
-    --hash=sha256:4665a714af31f160403c2e448fb2fef330719d2e04e836b08d60d612707c1041 \
-    --hash=sha256:4e8267466662aff93d66fa72b9591d02122dfc8a729b0a43dd70e0fb07ed9b37 \
-    --hash=sha256:55121fe140d7e42cb970999b93cf1c2b24484ce028b32bbd00238bb25c13e34a \
-    --hash=sha256:5caa9dd91dcc5f054350dc57a02e053d79633907b9ccffff999568d13dcd19f8 \
-    --hash=sha256:6abc91f6f8b3cc0ae1034e2c03f38769fba1952ab70d0b26953aa01691265c39 \
-    --hash=sha256:6c5554d55668381e131577f20e8f620d4882b04ad558f7e7f3f1f55b3124c379 \
-    --hash=sha256:70c294bb15ba576fb96b580db35895bf03749d683df044212b74e938a7f6821f \
-    --hash=sha256:73bc6114aab7753ca784f87bcd3b7613bc797aa255b5bca45e5654070ae9acfb \
-    --hash=sha256:92f135d370fcd7a6fb9659fa2eb716dd2ca364719cbb1756f74d90a221bca1a7 \
-    --hash=sha256:9cb88a3019ad042eaa69fc7639ef077793fedbf313e89207aa82fefe92c97ebd \
-    --hash=sha256:9dafdba3b2b9010abab08cb8c0dc6549bfca6e1630fe14d47b01dca00d39e694 \
-    --hash=sha256:a63922765ee49d5b4c32afb2cd5516812c8665f3b78e64a0dd005bdfabf991b1 \
-    --hash=sha256:a78a80d131c067d67d8a6f9bd3d3f7ea7eac82c1c7259f97d7ab73f723da9d55 \
-    --hash=sha256:b75aff2c35ceaa299691e772f7bf7c8aeab25f46acea2be3dd04cccb914a9860 \
-    --hash=sha256:b84076e3de192fba0f95e279ac017b64c7c6ecd4f09f36f13420f5bed898a9c7 \
-    --hash=sha256:b8dfb5fed540f77e814bf4ec79619c241af6b4578fa1093c5e3389bbb7beab3f \
-    --hash=sha256:bc74b64bfa89e2f862ea45dd6ac1def371d7cc883b76680d20bdd61a6f3daa20 \
-    --hash=sha256:bc9c77004970a364a1e5454cf7cb884e4277592b959c287689b2a0fd027ef552 \
-    --hash=sha256:c027fbb83a8c78a6e06a0302ea1799fdb70e5cda9845a5e000545b8e2b47ea39 \
-    --hash=sha256:c06046f54e719da21c79f98ecc0962581d1aee0b3798dc6b12b1217da8bf93f4 \
-    --hash=sha256:c58921fcd9914b56444292e7546fe183d079db99528142c809549ddeaeacd8e9 \
-    --hash=sha256:c82f34fafaf5bc05d222fcf84423d6e156432ca35ca78672d4affd0c09c6ef6c \
-    --hash=sha256:caf82db5b7f16b51ec32fe0bd2da0805b177c807aa8bfb478c7e6f893418c284 \
-    --hash=sha256:cb8cfa3bf3a9f18211279458917fef5edeb5e1fdebe2ea8b11969ec2ebe48884 \
-    --hash=sha256:d68f2f7bddb3acdd3b36ef7f334b9d14f30b93e094f808fbbd8d288b8f9e2f9b \
-    --hash=sha256:daf91db39324e9939a9db919ee4fb42a1a23634a056616dae891a030e89f87ba \
-    --hash=sha256:dcfbf8ffc046f20d75fd775a92c378f6fc7b9bded6c6f2ab88b6b9cb5805a184 \
-    --hash=sha256:e44b60b0b49aa85d548d392a2dca2c6a581cd4084e72e9e16bd58bd86ec20816 \
-    --hash=sha256:ea45f0dba5a993e93b158f1a9dcfff2770e3bcabf2b80dbe7aa15dce0bcb3bf3 \
-    --hash=sha256:ee32a080bab779b71c4d09a3eb5254bfca43ee88828a683dab27dfe8f582516e \
-    --hash=sha256:efc200fa75d9634525b40babc7a16342bd21c101db1a58ef84dc14f4bf6ac0fd \
-    --hash=sha256:f092d9f2ddaa30235d33335fbdb61eb8f3657af519ef5f9dd6bdae65272def11 \
-    --hash=sha256:f3d485e6ec6e09857bf2115ece572d666b7c498377d4c70e66bb06c63ed177c2 \
-    --hash=sha256:f684d88eb4924ed0630cf488fd5606e334c6835594bb5fe36b50a509b10383ed \
-    --hash=sha256:f6c4ad409a0caf7e2e12e203348b1a9b19c514e7d078520973147bf2d3dcbc6f
+coverage==7.2.5 \
+    --hash=sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3 \
+    --hash=sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a \
+    --hash=sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813 \
+    --hash=sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0 \
+    --hash=sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a \
+    --hash=sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd \
+    --hash=sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139 \
+    --hash=sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b \
+    --hash=sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252 \
+    --hash=sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790 \
+    --hash=sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045 \
+    --hash=sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce \
+    --hash=sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200 \
+    --hash=sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718 \
+    --hash=sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b \
+    --hash=sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f \
+    --hash=sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5 \
+    --hash=sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade \
+    --hash=sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5 \
+    --hash=sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a \
+    --hash=sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8 \
+    --hash=sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33 \
+    --hash=sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e \
+    --hash=sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c \
+    --hash=sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3 \
+    --hash=sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969 \
+    --hash=sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068 \
+    --hash=sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2 \
+    --hash=sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771 \
+    --hash=sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed \
+    --hash=sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212 \
+    --hash=sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614 \
+    --hash=sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88 \
+    --hash=sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3 \
+    --hash=sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c \
+    --hash=sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84 \
+    --hash=sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11 \
+    --hash=sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1 \
+    --hash=sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1 \
+    --hash=sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e \
+    --hash=sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1 \
+    --hash=sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd \
+    --hash=sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47 \
+    --hash=sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a \
+    --hash=sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c \
+    --hash=sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31 \
+    --hash=sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5 \
+    --hash=sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6 \
+    --hash=sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303 \
+    --hash=sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5 \
+    --hash=sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47
     # via -r requirements/test.in
 decorator==5.1.1 \
     --hash=sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330 \
     --hash=sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186
     # via pytest-twisted
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
     # via virtualenv
-exceptiongroup==1.1.0 \
-    --hash=sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e \
-    --hash=sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23
+exceptiongroup==1.1.1 \
+    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
+    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
     # via
     #   hypothesis
     #   pytest
-extras==1.0.0 \
-    --hash=sha256:132e36de10b9c91d5d4cc620160a476e0468a88f16c9431817a6729611a81b4e \
-    --hash=sha256:f689f08df47e2decf76aa6208c081306e7bd472630eb1ec8a875c67de2366e87
-    # via testtools
 fixtures==4.0.1 \
     --hash=sha256:d2758826400d095b79666cf93a32a84f50ff8cd179831927efb48cd1e3ca7466
     # via
     #   -r requirements/test.in
     #   testtools
 flake8==3.9.2 \
     --hash=sha256:07528381786f2a6237b061f6e96610a4167b226cb926e2aa2b6b1d78057c576b \
@@ -105,112 +101,116 @@
     # via
     #   -r requirements/test.in
     #   flake8-future-import
 flake8-future-import==0.4.7 \
     --hash=sha256:7ecb1b89f5e026afb0cfdb8642d150bf56efbb6fb86a713ea4568398142f47ae \
     --hash=sha256:ed826cca28fd4b55c486d69c4bfb32e9a052efc66714bf22bf471f50ecf8e0de
     # via -r requirements/test.in
-greenlet==2.0.1 \
-    --hash=sha256:0109af1138afbfb8ae647e31a2b1ab030f58b21dd8528c27beaeb0093b7938a9 \
-    --hash=sha256:0459d94f73265744fee4c2d5ec44c6f34aa8a31017e6e9de770f7bcf29710be9 \
-    --hash=sha256:04957dc96669be041e0c260964cfef4c77287f07c40452e61abe19d647505581 \
-    --hash=sha256:0722c9be0797f544a3ed212569ca3fe3d9d1a1b13942d10dd6f0e8601e484d26 \
-    --hash=sha256:097e3dae69321e9100202fc62977f687454cd0ea147d0fd5a766e57450c569fd \
-    --hash=sha256:0b493db84d124805865adc587532ebad30efa68f79ad68f11b336e0a51ec86c2 \
-    --hash=sha256:13ba6e8e326e2116c954074c994da14954982ba2795aebb881c07ac5d093a58a \
-    --hash=sha256:13ebf93c343dd8bd010cd98e617cb4c1c1f352a0cf2524c82d3814154116aa82 \
-    --hash=sha256:1407fe45246632d0ffb7a3f4a520ba4e6051fc2cbd61ba1f806900c27f47706a \
-    --hash=sha256:1bf633a50cc93ed17e494015897361010fc08700d92676c87931d3ea464123ce \
-    --hash=sha256:2d0bac0385d2b43a7bd1d651621a4e0f1380abc63d6fb1012213a401cbd5bf8f \
-    --hash=sha256:3001d00eba6bbf084ae60ec7f4bb8ed375748f53aeaefaf2a37d9f0370558524 \
-    --hash=sha256:356e4519d4dfa766d50ecc498544b44c0249b6de66426041d7f8b751de4d6b48 \
-    --hash=sha256:38255a3f1e8942573b067510f9611fc9e38196077b0c8eb7a8c795e105f9ce77 \
-    --hash=sha256:3d75b8d013086b08e801fbbb896f7d5c9e6ccd44f13a9241d2bf7c0df9eda928 \
-    --hash=sha256:41b825d65f31e394b523c84db84f9383a2f7eefc13d987f308f4663794d2687e \
-    --hash=sha256:42e602564460da0e8ee67cb6d7236363ee5e131aa15943b6670e44e5c2ed0f67 \
-    --hash=sha256:4aeaebcd91d9fee9aa768c1b39cb12214b30bf36d2b7370505a9f2165fedd8d9 \
-    --hash=sha256:4c8b1c43e75c42a6cafcc71defa9e01ead39ae80bd733a2608b297412beede68 \
-    --hash=sha256:4d37990425b4687ade27810e3b1a1c37825d242ebc275066cfee8cb6b8829ccd \
-    --hash=sha256:4f09b0010e55bec3239278f642a8a506b91034f03a4fb28289a7d448a67f1515 \
-    --hash=sha256:505138d4fa69462447a562a7c2ef723c6025ba12ac04478bc1ce2fcc279a2db5 \
-    --hash=sha256:5067920de254f1a2dee8d3d9d7e4e03718e8fd2d2d9db962c8c9fa781ae82a39 \
-    --hash=sha256:56961cfca7da2fdd178f95ca407fa330c64f33289e1804b592a77d5593d9bd94 \
-    --hash=sha256:5a8e05057fab2a365c81abc696cb753da7549d20266e8511eb6c9d9f72fe3e92 \
-    --hash=sha256:659f167f419a4609bc0516fb18ea69ed39dbb25594934bd2dd4d0401660e8a1e \
-    --hash=sha256:662e8f7cad915ba75d8017b3e601afc01ef20deeeabf281bd00369de196d7726 \
-    --hash=sha256:6f61d71bbc9b4a3de768371b210d906726535d6ca43506737682caa754b956cd \
-    --hash=sha256:72b00a8e7c25dcea5946692a2485b1a0c0661ed93ecfedfa9b6687bd89a24ef5 \
-    --hash=sha256:811e1d37d60b47cb8126e0a929b58c046251f28117cb16fcd371eed61f66b764 \
-    --hash=sha256:81b0ea3715bf6a848d6f7149d25bf018fd24554a4be01fcbbe3fdc78e890b955 \
-    --hash=sha256:88c8d517e78acdf7df8a2134a3c4b964415b575d2840a2746ddb1cc6175f8608 \
-    --hash=sha256:8dca09dedf1bd8684767bc736cc20c97c29bc0c04c413e3276e0962cd7aeb148 \
-    --hash=sha256:974a39bdb8c90a85982cdb78a103a32e0b1be986d411303064b28a80611f6e51 \
-    --hash=sha256:9e112e03d37987d7b90c1e98ba5e1b59e1645226d78d73282f45b326f7bddcb9 \
-    --hash=sha256:9e9744c657d896c7b580455e739899e492a4a452e2dd4d2b3e459f6b244a638d \
-    --hash=sha256:9ed358312e63bf683b9ef22c8e442ef6c5c02973f0c2a939ec1d7b50c974015c \
-    --hash=sha256:9f2c221eecb7ead00b8e3ddb913c67f75cba078fd1d326053225a3f59d850d72 \
-    --hash=sha256:a20d33124935d27b80e6fdacbd34205732660e0a1d35d8b10b3328179a2b51a1 \
-    --hash=sha256:a4c0757db9bd08470ff8277791795e70d0bf035a011a528ee9a5ce9454b6cba2 \
-    --hash=sha256:afe07421c969e259e9403c3bb658968702bc3b78ec0b6fde3ae1e73440529c23 \
-    --hash=sha256:b1992ba9d4780d9af9726bbcef6a1db12d9ab1ccc35e5773685a24b7fb2758eb \
-    --hash=sha256:b23d2a46d53210b498e5b701a1913697671988f4bf8e10f935433f6e7c332fb6 \
-    --hash=sha256:b5e83e4de81dcc9425598d9469a624826a0b1211380ac444c7c791d4a2137c19 \
-    --hash=sha256:be35822f35f99dcc48152c9839d0171a06186f2d71ef76dc57fa556cc9bf6b45 \
-    --hash=sha256:be9e0fb2ada7e5124f5282d6381903183ecc73ea019568d6d63d33f25b2a9000 \
-    --hash=sha256:c140e7eb5ce47249668056edf3b7e9900c6a2e22fb0eaf0513f18a1b2c14e1da \
-    --hash=sha256:c6a08799e9e88052221adca55741bf106ec7ea0710bca635c208b751f0d5b617 \
-    --hash=sha256:cb242fc2cda5a307a7698c93173d3627a2a90d00507bccf5bc228851e8304963 \
-    --hash=sha256:cce1e90dd302f45716a7715517c6aa0468af0bf38e814ad4eab58e88fc09f7f7 \
-    --hash=sha256:cd4ccc364cf75d1422e66e247e52a93da6a9b73cefa8cad696f3cbbb75af179d \
-    --hash=sha256:d21681f09e297a5adaa73060737e3aa1279a13ecdcfcc6ef66c292cb25125b2d \
-    --hash=sha256:d38ffd0e81ba8ef347d2be0772e899c289b59ff150ebbbbe05dc61b1246eb4e0 \
-    --hash=sha256:d566b82e92ff2e09dd6342df7e0eb4ff6275a3f08db284888dcd98134dbd4243 \
-    --hash=sha256:d5b0ff9878333823226d270417f24f4d06f235cb3e54d1103b71ea537a6a86ce \
-    --hash=sha256:d6ee1aa7ab36475035eb48c01efae87d37936a8173fc4d7b10bb02c2d75dd8f6 \
-    --hash=sha256:db38f80540083ea33bdab614a9d28bcec4b54daa5aff1668d7827a9fc769ae0a \
-    --hash=sha256:ea688d11707d30e212e0110a1aac7f7f3f542a259235d396f88be68b649e47d1 \
-    --hash=sha256:f6327b6907b4cb72f650a5b7b1be23a2aab395017aa6f1adb13069d66360eb3f \
-    --hash=sha256:fb412b7db83fe56847df9c47b6fe3f13911b06339c2aa02dcc09dce8bbf582cd
+greenlet==2.0.2 \
+    --hash=sha256:03a8f4f3430c3b3ff8d10a2a86028c660355ab637cee9333d63d66b56f09d52a \
+    --hash=sha256:0bf60faf0bc2468089bdc5edd10555bab6e85152191df713e2ab1fcc86382b5a \
+    --hash=sha256:18a7f18b82b52ee85322d7a7874e676f34ab319b9f8cce5de06067384aa8ff43 \
+    --hash=sha256:18e98fb3de7dba1c0a852731c3070cf022d14f0d68b4c87a19cc1016f3bb8b33 \
+    --hash=sha256:1a819eef4b0e0b96bb0d98d797bef17dc1b4a10e8d7446be32d1da33e095dbb8 \
+    --hash=sha256:26fbfce90728d82bc9e6c38ea4d038cba20b7faf8a0ca53a9c07b67318d46088 \
+    --hash=sha256:2780572ec463d44c1d3ae850239508dbeb9fed38e294c68d19a24d925d9223ca \
+    --hash=sha256:283737e0da3f08bd637b5ad058507e578dd462db259f7f6e4c5c365ba4ee9343 \
+    --hash=sha256:2d4686f195e32d36b4d7cf2d166857dbd0ee9f3d20ae349b6bf8afc8485b3645 \
+    --hash=sha256:2dd11f291565a81d71dab10b7033395b7a3a5456e637cf997a6f33ebdf06f8db \
+    --hash=sha256:30bcf80dda7f15ac77ba5af2b961bdd9dbc77fd4ac6105cee85b0d0a5fcf74df \
+    --hash=sha256:32e5b64b148966d9cccc2c8d35a671409e45f195864560829f395a54226408d3 \
+    --hash=sha256:36abbf031e1c0f79dd5d596bfaf8e921c41df2bdf54ee1eed921ce1f52999a86 \
+    --hash=sha256:3a06ad5312349fec0ab944664b01d26f8d1f05009566339ac6f63f56589bc1a2 \
+    --hash=sha256:3a51c9751078733d88e013587b108f1b7a1fb106d402fb390740f002b6f6551a \
+    --hash=sha256:3c9b12575734155d0c09d6c3e10dbd81665d5c18e1a7c6597df72fd05990c8cf \
+    --hash=sha256:3f6ea9bd35eb450837a3d80e77b517ea5bc56b4647f5502cd28de13675ee12f7 \
+    --hash=sha256:4b58adb399c4d61d912c4c331984d60eb66565175cdf4a34792cd9600f21b394 \
+    --hash=sha256:4d2e11331fc0c02b6e84b0d28ece3a36e0548ee1a1ce9ddde03752d9b79bba40 \
+    --hash=sha256:5454276c07d27a740c5892f4907c86327b632127dd9abec42ee62e12427ff7e3 \
+    --hash=sha256:561091a7be172ab497a3527602d467e2b3fbe75f9e783d8b8ce403fa414f71a6 \
+    --hash=sha256:6c3acb79b0bfd4fe733dff8bc62695283b57949ebcca05ae5c129eb606ff2d74 \
+    --hash=sha256:703f18f3fda276b9a916f0934d2fb6d989bf0b4fb5a64825260eb9bfd52d78f0 \
+    --hash=sha256:7492e2b7bd7c9b9916388d9df23fa49d9b88ac0640db0a5b4ecc2b653bf451e3 \
+    --hash=sha256:76ae285c8104046b3a7f06b42f29c7b73f77683df18c49ab5af7983994c2dd91 \
+    --hash=sha256:7cafd1208fdbe93b67c7086876f061f660cfddc44f404279c1585bbf3cdc64c5 \
+    --hash=sha256:7efde645ca1cc441d6dc4b48c0f7101e8d86b54c8530141b09fd31cef5149ec9 \
+    --hash=sha256:88d9ab96491d38a5ab7c56dd7a3cc37d83336ecc564e4e8816dbed12e5aaefc8 \
+    --hash=sha256:8eab883b3b2a38cc1e050819ef06a7e6344d4a990d24d45bc6f2cf959045a45b \
+    --hash=sha256:910841381caba4f744a44bf81bfd573c94e10b3045ee00de0cbf436fe50673a6 \
+    --hash=sha256:9190f09060ea4debddd24665d6804b995a9c122ef5917ab26e1566dcc712ceeb \
+    --hash=sha256:937e9020b514ceedb9c830c55d5c9872abc90f4b5862f89c0887033ae33c6f73 \
+    --hash=sha256:94c817e84245513926588caf1152e3b559ff794d505555211ca041f032abbb6b \
+    --hash=sha256:971ce5e14dc5e73715755d0ca2975ac88cfdaefcaab078a284fea6cfabf866df \
+    --hash=sha256:9d14b83fab60d5e8abe587d51c75b252bcc21683f24699ada8fb275d7712f5a9 \
+    --hash=sha256:9f35ec95538f50292f6d8f2c9c9f8a3c6540bbfec21c9e5b4b751e0a7c20864f \
+    --hash=sha256:a1846f1b999e78e13837c93c778dcfc3365902cfb8d1bdb7dd73ead37059f0d0 \
+    --hash=sha256:acd2162a36d3de67ee896c43effcd5ee3de247eb00354db411feb025aa319857 \
+    --hash=sha256:b0ef99cdbe2b682b9ccbb964743a6aca37905fda5e0452e5ee239b1654d37f2a \
+    --hash=sha256:b80f600eddddce72320dbbc8e3784d16bd3fb7b517e82476d8da921f27d4b249 \
+    --hash=sha256:b864ba53912b6c3ab6bcb2beb19f19edd01a6bfcbdfe1f37ddd1778abfe75a30 \
+    --hash=sha256:b9ec052b06a0524f0e35bd8790686a1da006bd911dd1ef7d50b77bfbad74e292 \
+    --hash=sha256:ba2956617f1c42598a308a84c6cf021a90ff3862eddafd20c3333d50f0edb45b \
+    --hash=sha256:bdfea8c661e80d3c1c99ad7c3ff74e6e87184895bbaca6ee8cc61209f8b9b85d \
+    --hash=sha256:be4ed120b52ae4d974aa40215fcdfde9194d63541c7ded40ee12eb4dda57b76b \
+    --hash=sha256:c4302695ad8027363e96311df24ee28978162cdcdd2006476c43970b384a244c \
+    --hash=sha256:c48f54ef8e05f04d6eff74b8233f6063cb1ed960243eacc474ee73a2ea8573ca \
+    --hash=sha256:c9c59a2120b55788e800d82dfa99b9e156ff8f2227f07c5e3012a45a399620b7 \
+    --hash=sha256:cd021c754b162c0fb55ad5d6b9d960db667faad0fa2ff25bb6e1301b0b6e6a75 \
+    --hash=sha256:d27ec7509b9c18b6d73f2f5ede2622441de812e7b1a80bbd446cb0633bd3d5ae \
+    --hash=sha256:d5508f0b173e6aa47273bdc0a0b5ba055b59662ba7c7ee5119528f466585526b \
+    --hash=sha256:d75209eed723105f9596807495d58d10b3470fa6732dd6756595e89925ce2470 \
+    --hash=sha256:db1a39669102a1d8d12b57de2bb7e2ec9066a6f2b3da35ae511ff93b01b5d564 \
+    --hash=sha256:dbfcfc0218093a19c252ca8eb9aee3d29cfdcb586df21049b9d777fd32c14fd9 \
+    --hash=sha256:e0f72c9ddb8cd28532185f54cc1453f2c16fb417a08b53a855c4e6a418edd099 \
+    --hash=sha256:e7c8dc13af7db097bed64a051d2dd49e9f0af495c26995c00a9ee842690d34c0 \
+    --hash=sha256:ea9872c80c132f4663822dd2a08d404073a5a9b5ba6155bea72fb2a79d1093b5 \
+    --hash=sha256:eff4eb9b7eb3e4d0cae3d28c283dc16d9bed6b193c2e1ace3ed86ce48ea8df19 \
+    --hash=sha256:f82d4d717d8ef19188687aa32b8363e96062911e63ba22a0cff7802a8e58e5f1 \
+    --hash=sha256:fc3a569657468b6f3fb60587e48356fe512c1754ca05a564f11366ac9e306526
     # via pytest-twisted
-hypothesis==6.62.0 \
-    --hash=sha256:76f1141e8237f6dd0780a171bec5d6aec873208ccc27b5f9753d4cccd8904272 \
-    --hash=sha256:e250da77878460f74b53039493a7a18d6fc137b0b77791b382b6a0f4ada9144e
+hypothesis==6.75.2 \
+    --hash=sha256:29fee1fabf764eb021665d20e633ef7ba931c5841de20f9ff3e01e8a512d6a4d \
+    --hash=sha256:50c270b38d724ce0fefa71b8e3511d123f7a31a9af9ea003447d4e1489292fbc
     # via -r requirements/test.in
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
     # via towncrier
+magic-wormhole-mailbox-server==0.4.1 \
+    --hash=sha256:1af10592909caaf519c00e706eac842c5e77f8d4356215fe9c61c7b2258a88fb \
+    --hash=sha256:1bf47755dba25dbfce99335f393b8a157515e098de6b5ed25324f679c3a5350e
+    # via -r requirements/test.in
 mccabe==0.6.1 \
     --hash=sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42 \
     --hash=sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f
     # via flake8
-mock==5.0.1 \
-    --hash=sha256:c41cfb1e99ba5d341fbcc5308836e7d7c9786d302f995b2c271ce2144dece9eb \
-    --hash=sha256:e3ea505c03babf7977fd21674a69ad328053d414f05e6433c30d8fa14a534a6b
+mock==5.0.2 \
+    --hash=sha256:06f18d7d65b44428202b145a9a36e99c2ee00d1eb992df0caf881d4664377891 \
+    --hash=sha256:0e0bc5ba78b8db3667ad636d964eb963dc97a59f04c6f6214c5f0e4a8f726c56
     # via -r requirements/test.in
-packaging==23.0 \
-    --hash=sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2 \
-    --hash=sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97
+packaging==23.1 \
+    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
+    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via
     #   pyproject-api
     #   pytest
     #   tox
-pbr==5.11.0 \
-    --hash=sha256:b97bc6695b2aff02144133c2e7399d5885223d42b7912ffaec2ca3898e673bfe \
-    --hash=sha256:db2317ff07c84c4c63648c9064a79fe9d9f5c7ce85a9099d4b6258b3db83225a
+pbr==5.11.1 \
+    --hash=sha256:567f09558bae2b3ab53cb3c1e2e33e726ff3338e7bae3db5dc954b3a44eef12b \
+    --hash=sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3
     # via
     #   fixtures
     #   testtools
-platformdirs==2.6.2 \
-    --hash=sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490 \
-    --hash=sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2
+platformdirs==3.5.0 \
+    --hash=sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4 \
+    --hash=sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0 \
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
     # via
@@ -220,21 +220,21 @@
     --hash=sha256:514f76d918fcc0b55c6680472f0a37970994e07bbb80725808c17089be302068 \
     --hash=sha256:c389c1d06bf7904078ca03399a4816f974a1d590090fecea0c63ec26ebaf1cef
     # via flake8
 pyflakes==2.3.1 \
     --hash=sha256:7893783d01b8a89811dd72d7dfd4d84ff098e5eed95cfa8905b22bbffe52efc3 \
     --hash=sha256:f5bc8ecabc05bb9d291eb5203d6810b49040f6ff446a756326104746cc00c1db
     # via flake8
-pyproject-api==1.4.0 \
-    --hash=sha256:ac85c1f82e0291dbae5a7739dbb9a990e11ee4034c9b5599ea714f07a24ecd71 \
-    --hash=sha256:c34226297781efdd1ba4dfb74ce21076d9a8360e2125ea31803c1a02c76b2460
+pyproject-api==1.5.1 \
+    --hash=sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9 \
+    --hash=sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43
     # via tox
-pytest==7.2.0 \
-    --hash=sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71 \
-    --hash=sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59
+pytest==7.3.1 \
+    --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
+    --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
     # via
     #   -r requirements/test.in
     #   pytest-lazy-fixture
     #   pytest-twisted
 pytest-lazy-fixture==0.6.3 \
     --hash=sha256:0e7d0c7f74ba33e6e80905e9bfd81f9d15ef9a790de97993e34213deb5ad10ac \
     --hash=sha256:e0b379f38299ff27a653f03eaa69b08a6fd4484e46fd1c9907d984b9f9daeda6
@@ -243,31 +243,31 @@
     --hash=sha256:1b63b73182bd1b995f30826a1d870c9ac0d08244ab0c871eb8bd0c8243acfb3d \
     --hash=sha256:209bf5a6452cfbfb61de8f015902c14ec8126400911507074bb2ee4ce8dfe313
     # via -r requirements/test.in
 sortedcontainers==2.4.0 \
     --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
     --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
     # via hypothesis
-testtools==2.5.0 \
-    --hash=sha256:57c13433d94f9ffde3be6534177d10fb0c1507cc499319128958ca91a65cb23f \
-    --hash=sha256:798525999f053e4df4e352c0c198baeb9f5079f34bad5bd57a44e97a54fa0330
+testtools==2.6.0 \
+    --hash=sha256:28b65e14c0f2d3ecbbfb5f55c9dcde5e4faa80ac16a37a823909a1fe3cbcb30a \
+    --hash=sha256:cae7b2c2f459e448e0bb22c017fa1e7b4ba534b6e623d9f7ec0e0312aac8f7e8
     # via -r requirements/test.in
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   pyproject-api
     #   pytest
     #   towncrier
     #   tox
 towncrier==22.12.0 \
     --hash=sha256:9767a899a4d6856950f3598acd9e8f08da2663c49fdcda5ea0f9e6ba2afc8eea \
     --hash=sha256:9c49d7e75f646a9aea02ae904c0bc1639c8fd14a01292d2b123b8d307564034d
     # via -r requirements/test.in
-tox==4.2.6 \
-    --hash=sha256:ecf224a4f3a318adcdd71aa8fe15ffd31f14afd6a9845a43ffd63950a7325538 \
-    --hash=sha256:fb79b3e4b788491949576a9c80c2d56419eac994567c3591e24bb2788b5901d0
+tox==4.5.1 \
+    --hash=sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56 \
+    --hash=sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046
     # via -r requirements/test.in
-virtualenv==20.17.1 \
-    --hash=sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4 \
-    --hash=sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058
+virtualenv==20.23.0 \
+    --hash=sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e \
+    --hash=sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924
     # via tox
```

### Comparing `magic-folder-23.5.0/requirements/tox.txt` & `magic-folder-23.6.0/requirements/tox.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r test.txt
-pip==22.3.1 \
-    --hash=sha256:65fd48317359f3af8e593943e6ae1506b66325085ea64b706a998c6e83eeaf38 \
-    --hash=sha256:908c78e6bc29b676ede1c4d57981d490cb892eb45cd8c214ab6298125119e077
+extras==1.0.0 \
+    --hash=sha256:132e36de10b9c91d5d4cc620160a476e0468a88f16c9431817a6729611a81b4e \
+    --hash=sha256:f689f08df47e2decf76aa6208c081306e7bd472630eb1ec8a875c67de2366e87
+    # via python-subunit
+pip==23.1.2 \
+    --hash=sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba \
+    --hash=sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18
     # via -r requirements/tox.in
 python-subunit==1.4.2 \
     --hash=sha256:2988d324d55ec35dd037e502e3f74ac38f4e457bd44ee0edf5e898f7ee1134d4 \
     --hash=sha256:c08d6de7e09bf6ac69dcd8e4e57a247a267d1e786493ba559cfb744747d82c8c
     # via subunitreporter
 subunitreporter==22.2.0 \
     --hash=sha256:ef5f8c7d3d3bf2548a39d3e6994fd83a22737e619fae0584aedcc11bcf9e0023
     # via -r requirements/tox.in
-wheel==0.38.4 \
-    --hash=sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac \
-    --hash=sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8
+wheel==0.40.0 \
+    --hash=sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873 \
+    --hash=sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247
     # via -r requirements/tox.in
```

### Comparing `magic-folder-23.5.0/setup.py` & `magic-folder-23.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/_coverage.py` & `magic-folder-23.6.0/src/magic_folder/_coverage.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/_endpoint_parser.py` & `magic-folder-23.6.0/src/magic_folder/_endpoint_parser.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/_schema.py` & `magic-folder-23.6.0/src/magic_folder/_schema.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/api_cli.py` & `magic-folder-23.6.0/src/magic_folder/api_cli.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/cli.py` & `magic-folder-23.6.0/src/magic_folder/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,19 +388,24 @@
         "tahoe": {
             "happy": False,
             "connected": None,
             "desired": None,
         },
     }
 
-    # lambdas can't assign things
+    # helper because lambdas can't assign things
     def copy_state(dest, src, keys):
         for k in keys:
             dest[k] = src[k]
 
+    # helper because lambdas can't assign things
+    def assign(dest, dest_key, value):
+        dest[dest_key] = value
+
+
     def error(e):
         """
         Handle a kind=error message
         """
         state["folders"][e["folder"]]["errors"].append({
             "timestamp": e["timestamp"],
             "summary": e["summary"],
@@ -458,16 +463,16 @@
                     humanize.naturaldelta(now - f["last-updated"]),
                 ),
                 file=out,
             )
 
     # based on the "kind" of event, we update our state
     updates = {
-        "scan-completed": lambda e: copy_state(state["folders"][e["folder"]], e, {"last-scan"}),
-        "poll-completed": lambda e: copy_state(state["folders"][e["folder"]], e, {"last-poll"}),
+        "scan-completed": lambda e: assign(state["folders"][e["folder"]], "last-scan", e["timestamp"]),
+        "poll-completed": lambda e: assign(state["folders"][e["folder"]], "last-poll", e["timestamp"]),
         "tahoe-connection-changed": lambda e: copy_state(state["tahoe"], e, {"happy", "connected", "desired"}),
         "error-occurred": error,
         "folder-added": lambda _: None,
         "folder-deleted": lambda _: None,
         "upload-queued": upload,
         "upload-started": upload,
         "upload-finished": upload,
```

### Comparing `magic-folder-23.5.0/src/magic_folder/client.py` & `magic-folder-23.6.0/src/magic_folder/client.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/common.py` & `magic-folder-23.6.0/src/magic_folder/common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/config.py` & `magic-folder-23.6.0/src/magic_folder/config.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/downloader.py` & `magic-folder-23.6.0/src/magic_folder/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,25 +567,25 @@
                     if participant.is_self:
                         # we don't download from ourselves
                         continue
                     files = yield participant.files()
                     for relpath, file_data in files.items():
                         if self._is_remote_update(relpath, file_data.snapshot_cap):
                             self._status.download_queued(self._config.name, relpath)
-                            updates.append((relpath, file_data.snapshot_cap))
+                            updates.append((relpath, file_data.snapshot_cap, participant))
 
             # allow for parallel downloads
             # (we could de-duplicate snapshots here, but the state-machine has to anyway)
             yield gatherResults([
-                self._process_snapshot(relpath, snapshot_cap)
-                for relpath, snapshot_cap in updates
+                self._process_snapshot(relpath, snapshot_cap, participant)
+                for relpath, snapshot_cap, participant in updates
             ])
 
     @inline_callbacks
-    def _process_snapshot(self, relpath, snapshot_cap):
+    def _process_snapshot(self, relpath, snapshot_cap, participant):
         """
         Internal helper.
 
         Does the work of caching and acting on a single remote
         Snapshot.
 
         :returns Deferred: fires with None upon completion
@@ -615,8 +615,8 @@
             if our_snapshot_cap is not None \
                and self._remote_snapshot_cache.is_ancestor_of(snapshot.capability, our_snapshot_cap):
                 Message.log(
                     message_type=u"downloader:redundant-update",
                     relpath=snapshot.relpath,
                 )
             else:
-                yield maybeDeferred(mf.found_new_remote, snapshot)
+                yield maybeDeferred(mf.found_new_remote, snapshot, participant)
```

### Comparing `magic-folder-23.5.0/src/magic_folder/endpoints.py` & `magic-folder-23.6.0/src/magic_folder/endpoints.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/initialize.py` & `magic-folder-23.6.0/src/magic_folder/initialize.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/invite.py` & `magic-folder-23.6.0/src/magic_folder/invite.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/list.py` & `magic-folder-23.6.0/src/magic_folder/list.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/magic_file.py` & `magic-folder-23.6.0/src/magic_folder/magic_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,25 +240,37 @@
         Eventually, the snapshot will be uploaded. Even if our process
         re-starts, the LocalSnapshot will be recovered from local
         state and further attempts to upload will be made.
 
         :returns Deferred: fires with None when our local state is
             persisted. This is before the upload has occurred.
         """
-        return self._local_update()
+        d = maybeDeferred(self._local_update)
 
-    def found_new_remote(self, remote_snapshot):
+        def is_empty(arg):
+            """
+            The state-machine can return 'no outputs' -- which is an empty
+            list -- if we go conflict -> conflict. Here we translate
+            that to None
+            """
+            if not arg:
+                return None
+            return arg
+        d.addCallback(is_empty)
+        return d
+
+    def found_new_remote(self, remote_snapshot, participant):
         """
         A RemoteSnapshot that doesn't match our existing database entry
         has been found. It will be downloaded and applied (possibly
         resulting in conflicts).
 
         :param RemoteSnapshot remote_snapshot: the newly-discovered remote
         """
-        self._remote_update(remote_snapshot)
+        self._remote_update(remote_snapshot, participant)
         return self.when_idle()
 
     def local_snapshot_exists(self, local_snapshot):
         """
         State describing a LocalSnapshot exists. This should be the
         'youngest' one if there are multiple snapshots for this file.
 
@@ -373,28 +385,28 @@
     @_machine.input()
     def _no_upload_work(self, snapshot):
         """
         We finished one upload and there is no more
         """
 
     @_machine.input()
-    def _download_mismatch(self, snapshot, staged_path):
+    def _download_mismatch(self, snapshot, staged_path, participant):
         """
         The local file does not match what we expect given database state
         """
 
     @_machine.input()
-    def _download_matches(self, snapshot, staged_path, local_pathstate):
+    def _download_matches(self, snapshot, staged_path, local_pathstate, participant):
         """
         The local file (if any) matches what we expect given database
         state
         """
 
     @_machine.input()
-    def _remote_update(self, snapshot):
+    def _remote_update(self, snapshot, participant):
         """
         The file has a remote update.
         """
 
     @_machine.input()
     def _existing_local_snapshot(self, snapshot):
         """
@@ -408,15 +420,15 @@
     def _existing_conflict(self):
         """
         This path is already conflicted. Used when initializing a fresh
         file from the database.
         """
 
     @_machine.input()
-    def _download_completed(self, snapshot, staged_path):
+    def _download_completed(self, snapshot, staged_path, participant):
         """
         A remote Snapshot has been downloaded
         """
 
     @_machine.input()
     def _snapshot_completed(self, snapshot):
         """
@@ -438,15 +450,15 @@
     @_machine.input()
     def _fatal_error_download(self, snapshot):
         """
         An error has occurred with no other recovery path.
         """
 
     @_machine.input()
-    def _queued_download(self, snapshot):
+    def _queued_download(self, snapshot, participant):
         """
         There is queued RemoteSnapshot work
         """
 
     @_machine.input()
     def _no_download_work(self, snapshot):
         """
@@ -456,21 +468,21 @@
     @_machine.input()
     def _conflict_resolution(self, snapshot):
         """
         A conflicted file has been resolved
         """
 
     @_machine.input()
-    def _ancestor_matches(self, snapshot, staged_path):
+    def _ancestor_matches(self, snapshot, staged_path, participant):
         """
         snapshot is our ancestor
         """
 
     @_machine.input()
-    def _ancestor_mismatch(self, snapshot, staged_path):
+    def _ancestor_mismatch(self, snapshot, staged_path, participant):
         """
         snapshot is not our ancestor
         """
 
     @_machine.input()
     def _ancestor_we_are_newer(self, snapshot, staged_path):
         """
@@ -480,20 +492,20 @@
     @_machine.input()
     def _cancel(self, snapshot):
         """
         We have been cancelled
         """
 
     @_machine.output()
-    def _begin_download(self, snapshot):
+    def _begin_download(self, snapshot, participant):
         """
         Download a given Snapshot (including its content)
         """
         def downloaded(staged_path):
-            self._call_later(self._download_completed, snapshot, staged_path)
+            self._call_later(self._download_completed, snapshot, staged_path, participant)
 
         retry_delay_sequence = _delay_sequence()
 
         def error(f):
             if f.check(CancelledError):
                 self._factory._folder_status.error_occurred(
                     "Cancelled: {}".format(self._relpath)
@@ -538,15 +550,15 @@
             d.addCallback(downloaded)
             d.addErrback(error)
             return d
 
         return perform_download()
 
     @_machine.output()
-    def _check_local_update(self, snapshot, staged_path):
+    def _check_local_update(self, snapshot, staged_path, participant):
         """
         Detect a 'last minute' change by comparing the state of our local
         file to that of the database.
 
         In case of a brand new file we've never seen: the database
         will have no entry, and there is no local file.
 
@@ -572,28 +584,28 @@
             assert False, "unexpected local snapshot; state-machine inconsistency?"
         except KeyError:
             pass
 
         # now, determine if we've found a local update
         if current_pathstate is None:
             if local_pathinfo.exists:
-                self._call_later(self._download_mismatch, snapshot, staged_path)
+                self._call_later(self._download_mismatch, snapshot, staged_path, participant)
                 return
         else:
             # we've seen this file before so its pathstate should
             # match what we expect according to the database .. or
             # else some update happened meantime.
             if current_pathstate != local_pathinfo.state:
-                self._call_later(self._download_mismatch, snapshot, staged_path)
+                self._call_later(self._download_mismatch, snapshot, staged_path, participant)
                 return
 
-        self._call_later(self._download_matches, snapshot, staged_path, local_pathinfo.state)
+        self._call_later(self._download_matches, snapshot, staged_path, local_pathinfo.state, participant)
 
     @_machine.output()
-    def _check_ancestor(self, snapshot, staged_path):
+    def _check_ancestor(self, snapshot, staged_path, participant):
         """
         Check if the ancestor for this remote update is correct or not.
         """
         try:
             remote_cap = self._factory._config.get_remotesnapshot(snapshot.relpath)
         except KeyError:
             remote_cap = None
@@ -608,21 +620,21 @@
                 # do because we are newer
                 if self._factory._remote_cache.is_ancestor_of(snapshot.capability, remote_cap):
                     self._call_later(self._ancestor_we_are_newer, snapshot, staged_path)
                     return
                 Message.log(
                     message_type="ancestor_mismatch",
                 )
-                self._call_later(self._ancestor_mismatch, snapshot, staged_path)
+                self._call_later(self._ancestor_mismatch, snapshot, staged_path, participant)
                 return
-        self._call_later(self._ancestor_matches, snapshot, staged_path)
+        self._call_later(self._ancestor_matches, snapshot, staged_path, participant)
         return
 
     @_machine.output()
-    def _perform_remote_update(self, snapshot, staged_path, local_pathstate):
+    def _perform_remote_update(self, snapshot, staged_path, local_pathstate, participant):
         """
         Resolve a remote update locally
 
         :param PathState local_pathstate: the PathState of the local
             file as it existed _right_ before we concluded it was fine
             (None if there was no local file before now)
         """
@@ -667,15 +679,15 @@
                 with self._action.context():
                     write_traceback()
                 # mark as a conflict -- we use the retained tmpfile as
                 # the original "staged" path here, causing "our"
                 # emergency data to be in the conflict file .. maybe
                 # this should just be the original tmpfile and we
                 # shouldn't mess with it further?
-                self._call_later(self._download_mismatch, snapshot, e.path)
+                self._call_later(self._download_mismatch, snapshot, e.path, participant)
                 return
 
         # Note, if we crash here (after moving the file into place but
         # before noting that in our database) then we could produce
         # LocalSnapshots referencing the wrong parent. We will no
         # longer produce snapshots with the wrong parent once we
         # re-run and get past this point.
@@ -760,15 +772,15 @@
     def _status_download_finished(self):
         self._factory._folder_status.download_finished(self._relpath)
 
     @_machine.output()
     def _cancel_queued_work(self):
         for d in self._queue_local:
             d.cancel()
-        for d in self._queue_remote:
+        for d, _, _ in self._queue_remote:
             d.cancel()
 
     @_machine.output()
     def _create_local_snapshot(self):
         """
         Create a LocalSnapshot for this update
         """
@@ -837,21 +849,21 @@
                 self._call_later(self._upload_completed, snapshot)
 
             d.addCallback(got_remote)
             d.addErrback(upload_error, snapshot)
             return d
 
     @_machine.output()
-    def _mark_download_conflict(self, snapshot, staged_path):
+    def _mark_download_conflict(self, snapshot, staged_path, participant):
         """
         Mark a conflict for this remote snapshot
         """
         conflict_path = "{}.conflict-{}".format(
             self._relpath,
-            snapshot.author.name
+            participant.name,
         )
         self._factory._magic_fs.mark_conflict(self._relpath, conflict_path, staged_path)
         self._factory._config.add_conflict(snapshot)
 
     @_machine.output()
     def _update_personal_dmd_upload(self, snapshot):
         """
@@ -944,26 +956,26 @@
         def got_snap(snap):
             ret_d.callback(snap)
             return snap
         d.addCallbacks(got_snap, failed)
         return ret_d
 
     @_machine.output()
-    def _queue_remote_update(self, snapshot):
+    def _queue_remote_update(self, snapshot, participant):
         """
         Save this remote snapshot for later processing (in _check_for_remote_work)
         """
         # skip queueing this download if we already have this snapshot
         # ahead in the queue
-        for _, queued_snap in self._queue_remote:
+        for _, queued_snap, _ in self._queue_remote:
             if snapshot == queued_snap:
                 # same return-value as _begin_download: None
                 return succeed(None)
         d = Deferred()
-        self._queue_remote.append((d, snapshot))
+        self._queue_remote.append((d, snapshot, participant))
         return d
 
     @_machine.output()
     def _check_for_local_work(self):
         """
         Inject any queued local updates
         """
@@ -979,20 +991,20 @@
 
     @_machine.output()
     def _check_for_remote_work(self):
         """
         Inject any saved remote updates.
         """
         if self._queue_remote:
-            d, snapshot = self._queue_remote.pop(0)
+            d, snapshot, participant = self._queue_remote.pop(0)
 
-            def do_remote_update(done_d, snap):
-                update_d = self._queued_download(snap)
+            def do_remote_update(done_d, snap, part):
+                update_d = self._queued_download(snap, part)
                 update_d.addBoth(done_d.callback)
-            self._call_later(do_remote_update, d, snapshot)
+            self._call_later(do_remote_update, d, snapshot, participant)
             return
         self._call_later(self._no_download_work, None)
 
     @_machine.output()
     def _working(self):
         """
         We are doing some work so this file is not currently updated.
```

### Comparing `magic-folder-23.5.0/src/magic_folder/magic_folder.py` & `magic-folder-23.6.0/src/magic_folder/magic_folder.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/magicpath.py` & `magic-folder-23.6.0/src/magic_folder/magicpath.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/migrate.py` & `magic-folder-23.6.0/src/magic_folder/migrate.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/participants.py` & `magic-folder-23.6.0/src/magic_folder/participants.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
 
 @implementer(IParticipant)
 @attr.s
 class _StaticParticipant(object):
     """
     An in-memory IParticipant provider
     """
+    name = attr.ib()
     my_files = attr.ib()  # dict: str -> SnapshotEntry
     _is_self = attr.ib(default=False)
 
     def files(self):
         return self.my_files
 
     def is_self(self):
@@ -159,39 +160,50 @@
     """
     writer = attr.ib()
     participants = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         if self.participants is None:
             self.participants = [
-                _StaticParticipant([], True),
+                _StaticParticipant("default", {}, True),
             ]
-        assert len([p.is_self() for p in self.participants]) == 1, "Must have exactly one 'self' participant"
+        assert len([p for p in self.participants if p.is_self()]) == 1, "Must have exactly one 'self' participant"
 
     def list(self):
         return self.participants
 
     def add(self, author, personal_dmd_cap):
         self.participants.append(
             _StaticParticipant(
                 author,
                 personal_dmd_cap,
             )
         )
 
 
-def static_participants(my_files=None, other_files=None):
+def static_participants(my_files=None, other_files=None, names=None):
     """
     An ``IParticipants`` provider. Usually for testing.
     """
     # XXX name, dircap, is_self for participants is public?
+    def name_generator():
+        number = 0
+        while True:
+            yield "name_{}".format(number)
+            number += 1
+    if names is None:
+        names = name_generator()
+    else:
+        # turn it into a generator too
+        names = (n for n in names)
+
     writer = _StaticWriteableParticipant()
-    reader = _StaticParticipant(my_files or [], True)
+    reader = _StaticParticipant(next(names), my_files or [], True)
     others = [
-        _StaticParticipant(files, False)
+        _StaticParticipant(next(names), files, False)
         for files in (other_files or [])
     ]
     return _StaticParticipants(writer, [reader] + others)
 
 
 def participants_from_collective(collective_dirnode, upload_dirnode, tahoe_client):
     """
```

### Comparing `magic-folder-23.5.0/src/magic_folder/pid.py` & `magic-folder-23.6.0/src/magic_folder/pid.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/scanner.py` & `magic-folder-23.6.0/src/magic_folder/scanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,21 +166,19 @@
             yield find_updated_files(
                 self._cooperator, self._config, process, self._status
             )
             yield find_deleted_files(
                 self._cooperator, self._config, process, self._status
             )
 
-        results = []
-
         def create_update(path):
             magic_file = self._file_factory.magic_file_for(path)
             d = magic_file.create_update()
-            assert d is not None, "Internal error: no snapshot produced"
-            d.addBoth(results.append)
+            # this will produce a LocalSnapshot instance or None when
+            # there is nothing to do -- for example, when conflicted.
             return d
 
         yield self._cooperator.coiterate(
             create_update(path)
             for path in updates
         )
```

### Comparing `magic-folder-23.5.0/src/magic_folder/service.py` & `magic-folder-23.6.0/src/magic_folder/service.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/show_config.py` & `magic-folder-23.6.0/src/magic_folder/show_config.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/snapshot.py` & `magic-folder-23.6.0/src/magic_folder/snapshot.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/status.py` & `magic-folder-23.6.0/src/magic_folder/status.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/tahoe_client.py` & `magic-folder-23.6.0/src/magic_folder/tahoe_client.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/__init__.py` & `magic-folder-23.6.0/src/magic_folder/test/__init__.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/agentutil.py` & `magic-folder-23.6.0/src/magic_folder/test/agentutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/cli/common.py` & `magic-folder-23.6.0/src/magic_folder/test/cli/common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/cli/test_api_cli.py` & `magic-folder-23.6.0/src/magic_folder/test/cli/test_api_cli.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/cli/test_magic_folder.py` & `magic-folder-23.6.0/src/magic_folder/test/cli/test_magic_folder.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/common.py` & `magic-folder-23.6.0/src/magic_folder/test/common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/eliotutil.py` & `magic-folder-23.6.0/src/magic_folder/test/eliotutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/fixtures.py` & `magic-folder-23.6.0/src/magic_folder/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/matchers.py` & `magic-folder-23.6.0/src/magic_folder/test/matchers.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/strategies.py` & `magic-folder-23.6.0/src/magic_folder/test/strategies.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_api_cli.py` & `magic-folder-23.6.0/src/magic_folder/test/test_api_cli.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_cli.py` & `magic-folder-23.6.0/src/magic_folder/test/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
 from ..client import (
     create_magic_folder_client,
 )
 from ..status import (
     StatusProtocol,
     EventsWebSocketStatusService,
     TahoeStatus,
+    ScannerStatus,
+    PollerStatus,
 )
 from magic_folder.util.observer import (
     ListenObserver,
 )
 from magic_folder.initialize import (
     magic_folder_initialize,
 )
@@ -590,14 +592,16 @@
             TahoeStatus(2, 2, True)
         )
         status_service.folder_added("a")
         status_service.upload_queued("a", "a-file")
         status_service.download_queued("a", "b-file")
         status_service.download_started("a", "b-file")
         status_service.error_occurred("a", "Some sort of error")
+        status_service.scan_status("a", ScannerStatus(0))
+        status_service.poll_status("a", PollerStatus(0))
 
         # now we build up enough infrastructure to serve this status
         # out
         status_service.startService()
         server_proto = StatusProtocol(status_service)
         agent = create_memory_agent(self.reactor, pump, lambda: server_proto)
```

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_client.py` & `magic-folder-23.6.0/src/magic_folder/test/test_client.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_common.py` & `magic-folder-23.6.0/src/magic_folder/test/test_common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_config.py` & `magic-folder-23.6.0/src/magic_folder/test/test_config.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_download.py` & `magic-folder-23.6.0/src/magic_folder/test/test_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 )
 from ..testing.web import (
     create_fake_tahoe_root,
     create_tahoe_treq_client,
 )
 from ..participants import (
     participants_from_collective,
+    static_participants,
 )
 from ..util.capabilities import (
     Capability,
     random_immutable,
 )
 from ..util.file import (
     PathState,
@@ -1133,14 +1134,22 @@
         self.remote_cache = self.file_factory._remote_cache
         self.state_path = self.alice.global_config._get_state_path("default")
         self.alice_config = self.alice.global_config.get_magic_folder("default")
         self.alice_author = self.alice_config.author
         self.filesystem = InMemoryMagicFolderFilesystem()
         self.file_factory._magic_fs = self.filesystem
 
+        self.participants = static_participants(
+            names=["alice", "carol"],
+            my_files=[],
+            other_files=[
+                [],
+            ],
+        )
+
         self.carol_author = create_local_author("carol")
 
     def tearDown(self):
         super(ConflictTests, self).tearDown()
         return self.alice.cleanup()
 
     @inline_callbacks
@@ -1179,15 +1188,15 @@
         )
         self.alice_config.store_currentsnapshot_state("foo", get_pathinfo(local_path).state)
 
         # tell the state-machine about the local, and then get it to
         # examine the remote-snapshot
         mf = self.file_factory.magic_file_for(local_path)
         yield mf.local_snapshot_exists(local0)
-        yield mf.found_new_remote(remote0)
+        yield mf.found_new_remote(remote0, self.participants.participants[1])
 
         yield mf.when_idle()
 
         # we have a local-snapshot for the same relpath as the incoming
         # remote, so this is a conflict
         self.assertThat(
             self.filesystem.actions,
@@ -1231,15 +1240,15 @@
             content_cap=random_immutable(),
             metadata_cap=random_immutable(),
         )
         self.remote_cache._cached_snapshots[cap0.danger_real_capability_string()] = remote0
 
         # tell the updater to examine the remote-snapshot
         mf = self.file_factory.magic_file_for(local_path)
-        yield mf.found_new_remote(remote0)
+        yield mf.found_new_remote(remote0, self.participants.participants[1])
         yield mf.when_idle()
 
         # we have a local-snapshot for the same relpath as the incoming
         # remote, so this is a conflict
 
         self.assertThat(
             self.filesystem.actions,
@@ -1277,15 +1286,15 @@
         # we've 'seen' this file before so we must have the path locally
         local_path.setContent(b"dummy")
         self.alice_config.store_downloaded_snapshot("foo", remotes[0], get_pathinfo(local_path).state)
 
         # tell the updater to examine the youngest remote
         youngest = remotes[-1]
         mf = self.file_factory.magic_file_for(local_path)
-        yield mf.found_new_remote(youngest)
+        yield mf.found_new_remote(youngest, self.participants.participants[0])
         yield mf.when_idle()
 
         # we have a common ancestor so this should be an update
         self.assertThat(
             self.filesystem.actions,
             Equals([
                 ("download", "foo", youngest.content_cap),
@@ -1339,15 +1348,15 @@
         self.alice_magic_path.child("foo").setContent(b"whatever")
         self.alice_config.store_downloaded_snapshot("foo", other, PathState(
             mtime_ns=0, ctime_ns=0, size=len("whatever"),
         ))
 
         # ...child->parent aren't related to "other"
         mf = self.file_factory.magic_file_for(self.alice_magic_path.child("foo"))
-        yield mf.found_new_remote(child)
+        yield mf.found_new_remote(child, self.participants.participants[0])
         yield mf.when_idle()
 
         # so, no common ancestor: a conflict
         self.assertThat(
             self.filesystem.actions,
             Equals([
                 ("download", "foo", child.content_cap),
@@ -1396,15 +1405,15 @@
             "foo",
             parent,
             get_pathinfo(self.alice_magic_path.child("foo")).state,
         )
 
         # deletion snapshot
         mf = self.file_factory.magic_file_for(self.alice_magic_path.child("foo"))
-        yield mf.found_new_remote(child)
+        yield mf.found_new_remote(child, self.participants.participants[0])
         yield mf.when_idle()
 
         self.assertThat(
             self.filesystem.actions,
             Equals([
                 ("delete", "foo"),
             ])
@@ -1444,15 +1453,15 @@
         # so "alice" has "child" already
         local_path = self.alice_magic_path.child("foo")
         local_path.setContent(b"whatever")
         self.alice_config.store_downloaded_snapshot("foo", child, get_pathinfo(local_path).state)
 
         # we update with the parent (so, it's old)
         mf = self.file_factory.magic_file_for(local_path)
-        yield mf.found_new_remote(parent)
+        yield mf.found_new_remote(parent, self.participants.participants[0])
         yield mf.when_idle()
 
         # XXX to fix this need to add another state in the
         # state-machine to "maybe bail out early" if the updater is
         # newer before _begin_download()
 
         # so we should do nothing
@@ -1707,14 +1716,18 @@
 
 
 class CancelTests(AsyncTestCase):
     """
     Tests relating to cancelling operations
     """
 
+    def setUp(self):
+        super(CancelTests, self).setUp()
+        self.participants = static_participants()
+
     # XXX NOTE if this name gets longer, the resulting temp-paths can
     # become "too long" on windows causing failures
     @inline_callbacks
     def test_cancel0(self):
         """
         An update arrives but one of the tahoe requests is cancelled
         """
@@ -1751,15 +1764,15 @@
             content_cap = random_immutable(directory=True)
             relpath = "some_file"  # match earlier relpath
         remote_snapshot = FakeRemoteSnapshot()
 
         mf = service.file_factory.magic_file_for(local)
         # when .stream_capability() is called it will receive an
         # already cancelled Deferred
-        yield mf.found_new_remote(remote_snapshot)
+        yield mf.found_new_remote(remote_snapshot, self.participants.participants[0])
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(carol.global_service.status_service._marshal_state()),
             ContainsDict({
                 "events": AfterPreprocessing(
@@ -1829,15 +1842,15 @@
         # arrange to cancel the Personal DMD update
         service.file_factory._write_participant = wrap_frozen(
             service.file_factory._write_participant,
             update_snapshot=cancelled,
         )
 
         mf = service.file_factory.magic_file_for(magic_path.child(relpath))
-        yield mf.found_new_remote(parent)
+        yield mf.found_new_remote(parent, self.participants.participants[0])
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(carol.global_service.status_service._marshal_state()),
             ContainsDict({
                 "events": AfterPreprocessing(
```

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_eliotutil.py` & `magic-folder-23.6.0/src/magic_folder/test/test_eliotutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_endpoints.py` & `magic-folder-23.6.0/src/magic_folder/test/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_foo.py` & `magic-folder-23.6.0/src/magic_folder/test/test_foo.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_invite.py` & `magic-folder-23.6.0/src/magic_folder/test/test_invite.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_local_snapshot.py` & `magic-folder-23.6.0/src/magic_folder/test/test_local_snapshot.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_magic_file.py` & `magic-folder-23.6.0/src/magic_folder/test/test_magic_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     DeferredList,
 )
 from twisted.application.service import (
     Service,
     MultiService,
 )
 
+from nacl.signing import (
+    VerifyKey,
+)
+
 from ..config import (
     create_testing_configuration,
 )
 from ..testing.web import (
     create_tahoe_treq_client,
 )
 from ..downloader import (
@@ -35,14 +39,15 @@
 )
 from ..participants import (
     SnapshotEntry,
     static_participants,
 )
 from ..snapshot import (
     create_local_author,
+    create_author,
     RemoteSnapshot,
 )
 from ..status import (
     FolderStatus,
     EventsWebSocketStatusService,
 )
 from ..util.capabilities import (
@@ -194,15 +199,15 @@
                 ("bar", local_cap),
             ])
         )
 
 
 class RemoteUpdateTests(AsyncTestCase):
     """
-    Correct operations of maybe_update_personal_dmd_to_local and helpers
+    Correct operation of remote updates
     """
 
     def setUp(self):
         super(RemoteUpdateTests, self).setUp()
         # avoid global import
         from twisted.internet import reactor
         self.reactor = reactor
@@ -315,11 +320,14 @@
             parents_raw=[],
             content_cap=random_immutable(),
             metadata_cap=random_immutable(),
         )
         self.remote_cache._cached_snapshots[cap0.danger_real_capability_string()] = remote0
         abspath = self.config.magic_path.preauthChild(relpath)
         mf = self.magic_file_factory.magic_file_for(abspath)
-        d0 = mf.found_new_remote(remote0)
-        d1 = mf.found_new_remote(remote0)
-        d2 = mf.found_new_remote(remote0)
+        self.participants.add(create_author("beth", VerifyKey(b"\xff" * 32)), random_dircap())
+        self.participants.add(create_author("callum", VerifyKey(b"\xee" * 32)), random_dircap())
+        self.participants.add(create_author("dawn", VerifyKey(b"\xee" * 32)), random_dircap())
+        d0 = mf.found_new_remote(remote0, self.participants.participants[1])
+        d1 = mf.found_new_remote(remote0, self.participants.participants[2])
+        d2 = mf.found_new_remote(remote0, self.participants.participants[3])
         yield DeferredList([d0, d1, d2])
```

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_magic_folder_service.py` & `magic-folder-23.6.0/src/magic_folder/test/test_magic_folder_service.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_magicpath.py` & `magic-folder-23.6.0/src/magic_folder/test/test_magicpath.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_participants.py` & `magic-folder-23.6.0/src/magic_folder/test/test_participants.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_pid.py` & `magic-folder-23.6.0/src/magic_folder/test/test_pid.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_scanner.py` & `magic-folder-23.6.0/src/magic_folder/test/test_scanner.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,30 @@
 from twisted.internet.task import Clock, Cooperator
 from twisted.python import runtime
 from twisted.python.filepath import FilePath
 
 from hyperlink import (
     DecodedURL,
 )
+from nacl.signing import (
+    VerifyKey,
+)
 
 from ..config import create_testing_configuration
 from ..magic_file import MagicFileFactory
 from ..scanner import (
     ScannerService,
     find_updated_files,
     find_deleted_files,
 )
 from ..snapshot import (
     LocalSnapshot,
     RemoteSnapshot,
     create_local_author,
+    create_author,
 )
 from ..status import (
     FolderStatus,
     EventsWebSocketStatusService,
 )
 from ..util.file import (
     PathState,
@@ -546,7 +550,100 @@
             service._loop(),
             succeeded(Always()),
         )
         self.assertThat(
             files,
             Equals([local])
         )
+
+    @given(
+        relative_paths(),
+    )
+    def test_scan_conflicted_file(self, relpath):
+        """
+        A locally conflicted file receives a remote update (which should
+        be ignored)
+        """
+        # make a conflict
+        # update same file, different participant
+        # (XXX how does the error manifest, exactly?)
+        self.setup_example()
+        other_author = create_author("radia", VerifyKey(b"\xaa" * 32))
+
+        # a snapshot we have seen already
+        snap0 = RemoteSnapshot(
+            relpath,
+            self.author,
+            metadata={
+                "modification_time": int(0),
+            },
+            capability=random_immutable(directory=True),
+            parents_raw=[],
+            content_cap=random_immutable(),
+            metadata_cap=random_immutable(),
+        )
+        self.config.store_downloaded_snapshot(
+            relpath,
+            snap0,
+            OLD_PATH_STATE,
+        )
+
+        # make it conflicted
+        snap1 = RemoteSnapshot(
+            relpath,
+            other_author,
+            metadata={
+                "modification_time": int(1),
+            },
+            capability=random_immutable(directory=True),
+            parents_raw=[],
+            content_cap=random_immutable(),
+            metadata_cap=random_immutable(),
+        )
+        self.config.store_downloaded_snapshot(
+            relpath,
+            snap1,
+            OLD_PATH_STATE,
+        )
+        self.config.add_conflict(snap1)
+
+        # now it is conflicted, start a scanner service and let it
+        # find an update.
+        local = self.magic_path.preauthChild(relpath)
+        local.parent().makedirs(ignoreExistingDirectory=True)
+        local.setContent(b"test_scanner conflicted content\n" * 10)
+
+        class SnapshotService(object):
+            def add_file(self, f):
+                assert False, "Should not actually add files"
+
+        class FakeUploader(object):
+            def upload_snapshot(self, snapshot):
+                return Deferred()
+
+        file_factory = MagicFileFactory(
+            self.config,
+            self.tahoe_client,
+            self.folder_status,
+            SnapshotService(),
+            FakeUploader(),
+            object(), # write_participant,
+            object(), # remote_cache,
+            object(), # filesystem,
+            synchronous=True,
+        )
+
+        service = ScannerService(
+            self.config,
+            file_factory,
+            object(),
+            cooperator=self.cooperator,
+            scan_interval=None,
+            clock=self.clock,
+        )
+        service.startService()
+        self.addCleanup(service.stopService)
+
+        self.assertThat(
+            service._loop(),
+            succeeded(Always()),
+        )
```

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_schema.py` & `magic-folder-23.6.0/src/magic_folder/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_service.py` & `magic-folder-23.6.0/src/magic_folder/test/test_service.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_snapshot.py` & `magic-folder-23.6.0/src/magic_folder/test/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_status.py` & `magic-folder-23.6.0/src/magic_folder/test/test_status.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_strategies.py` & `magic-folder-23.6.0/src/magic_folder/test/test_strategies.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_tahoe_client.py` & `magic-folder-23.6.0/src/magic_folder/test/test_tahoe_client.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_testing.py` & `magic-folder-23.6.0/src/magic_folder/test/test_testing.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_upload.py` & `magic-folder-23.6.0/src/magic_folder/test/test_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     DecodedURL,
 )
 
 from ..snapshot import (
     create_local_author,
     RemoteSnapshot,
 )
+from ..participants import (
+    static_participants,
+)
 from ..testing.web import (
     create_fake_tahoe_root,
     create_tahoe_treq_client,
 )
 from ..tahoe_client import (
     create_tahoe_client,
 )
@@ -300,15 +303,16 @@
                 "modification_time": int(1234),
             },
             capability=random_immutable(directory=True),
             parents_raw=[snap.capability.danger_real_capability_string()],
             content_cap=random_immutable(),
             metadata_cap=random_immutable(),
         )
-        mf.found_new_remote(child)
+        participants = static_participants()
+        mf.found_new_remote(child, participants.participants[0])
 
         self.assertThat(
             transitions,
             Equals([
                 ('_conflicted', '_remote_update', '_conflicted'),
             ])
         )
```

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_util_database.py` & `magic-folder-23.6.0/src/magic_folder/test/test_util_database.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_util_file.py` & `magic-folder-23.6.0/src/magic_folder/test/test_util_file.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_util_twisted.py` & `magic-folder-23.6.0/src/magic_folder/test/test_util_twisted.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/test/test_web.py` & `magic-folder-23.6.0/src/magic_folder/test/test_web.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/testing/web.py` & `magic-folder-23.6.0/src/magic_folder/testing/web.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/uploader.py` & `magic-folder-23.6.0/src/magic_folder/uploader.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/capabilities.py` & `magic-folder-23.6.0/src/magic_folder/util/capabilities.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/database.py` & `magic-folder-23.6.0/src/magic_folder/util/database.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/eliotutil.py` & `magic-folder-23.6.0/src/magic_folder/util/eliotutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/encoding.py` & `magic-folder-23.6.0/src/magic_folder/util/encoding.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/file.py` & `magic-folder-23.6.0/src/magic_folder/util/file.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/observer.py` & `magic-folder-23.6.0/src/magic_folder/util/observer.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/twisted.py` & `magic-folder-23.6.0/src/magic_folder/util/twisted.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/util/wrap.py` & `magic-folder-23.6.0/src/magic_folder/util/wrap.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder/web.py` & `magic-folder-23.6.0/src/magic_folder/web.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/src/magic_folder.egg-info/PKG-INFO` & `magic-folder-23.6.0/src/magic_folder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-folder
-Version: 23.5.0
+Version: 23.6.0
 Summary: Tahoe-LAFS-based file synchronization
 Home-page: https://github.com/LeastAuthority/magic-folder/
 Author: the Tahoe-LAFS developers, the Magic-Folder developers
 Author-email: tahoe-dev@tahoe-lafs.org
 License: GNU GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `magic-folder-23.5.0/src/magic_folder.egg-info/SOURCES.txt` & `magic-folder-23.6.0/src/magic_folder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .coveragerc
 .flake8
 .gitignore
+.readthedocs.yaml
 COPYING.GPL
 COPYING.TGPPL.rst
 CREDITS
 DEVELOPERS
 MANIFEST.in
 Makefile
 NEWS.rst
@@ -20,25 +21,32 @@
 .github/workflows/macos.yaml
 .github/workflows/windows.yml
 docs/CODE_OF_CONDUCT.rst
 docs/Makefile
 docs/backdoors.rst
 docs/conf.py
 docs/config.rst
+docs/datamodel.rst
 docs/development.rst
 docs/downloader.rst
 docs/eliot.log
 docs/index.rst
 docs/interface.rst
 docs/invite-diagram-readonly.png
 docs/invite-diagram-readonly.seqdiag
 docs/invite-diagram.png
 docs/invite-diagram.seqdiag
 docs/invites.rst
+docs/leif-design.rst
 docs/limitations.rst
+docs/magic-folder-data-model--high-level.svg
+docs/magic-folder-data-model-abstract--conflict.plain.svg
+docs/magic-folder-data-model-abstract--conflict.svg
+docs/magic-folder-data-model-abstract.svg
+docs/magic-folder-data-model.svg
 docs/release-process.rst
 docs/releases.rst
 docs/snapshots.rst
 docs/usage.rst
 docs/.hypothesis/examples/25667fd10de02221/394341b7182cd227
 docs/.hypothesis/examples/26099471863eabde/394341b7182cd227
 docs/.hypothesis/examples/26b950c63ef40743/2cd852709fc7beda
@@ -323,15 +331,14 @@
 docs/proposed/LightweightDesignscanfornewfiles.html
 docs/proposed/conflict-api.rst
 docs/proposed/index.rst
 docs/proposed/markdown
 docs/proposed/recovery.rst
 docs/proposed/scanning-for-changes.rst
 docs/proposed/magic-folder/filesystem-integration.rst
-docs/proposed/magic-folder/multi-party-conflict-detection.rst
 docs/proposed/magic-folder/remote-to-local-sync.rst
 docs/proposed/magic-folder/user-interface-design.rst
 integration/README
 integration/__init__.py
 integration/bar
 integration/conftest.py
 integration/conftest.py.orig
@@ -350,14 +357,15 @@
 integration/test_same_files.py
 integration/test_status.py
 integration/test_synchronize.py
 integration/test_tahoe_objects.py
 integration/util.py
 integration/util.py.orig
 integration/util.py.rej
+misc/build_helpers/ann.toml
 misc/build_helpers/platform-pins.py
 misc/build_helpers/run-deprecations.py
 misc/build_helpers/sqlite_version.py
 misc/build_helpers/update-version.py
 misc/coding_tools/check-debugging.py
 newsfragments/.keep-directory
 requirements/README
```

### Comparing `magic-folder-23.5.0/src/magic_folder.egg-info/requires.txt` & `magic-folder-23.6.0/src/magic_folder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.5.0/tox.ini` & `magic-folder-23.6.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 # your web browser.
 
 [testenv:docs]
 # we pin docutils because of https://sourceforge.net/p/docutils/bugs/301/
 # which asserts when it reads links to .svg files (e.g. about.rst)
 deps =
      sphinx
-     docutils==0.12
+     docutils==0.19
 # normal install is not needed for docs, and slows things down
 skip_install = True
 commands =
          sphinx-build -b html -d {toxinidir}/docs/_build/doctrees {toxinidir}/docs {toxinidir}/docs/_build/html
 
 [testenv:tarballs]
 deps =
```

