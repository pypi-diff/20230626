# Comparing `tmp/vss-cli-2023.6.1.dev2.tar.gz` & `tmp/vss-cli-2023.6.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-cli-2023.6.1.dev2.tar", last modified: Thu Jun 22 19:27:45 2023, max compression
+gzip compressed data, was "vss-cli-2023.6.1.dev3.tar", last modified: Mon Jun 26 14:06:56 2023, max compression
```

## Comparing `vss-cli-2023.6.1.dev2.tar` & `vss-cli-2023.6.1.dev3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.519332 vss-cli-2023.6.1.dev2/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12464 2023-06-22 19:27:45.519332 vss-cli-2023.6.1.dev2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-22 19:27:45.519332 vss-cli-2023.6.1.dev2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3827 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.503332 vss-cli-2023.6.1.dev2/vss_cli/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18320 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     7453 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    62562 2023-06-22 19:26:47.000000 vss-cli-2023.6.1.dev2/vss_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    13887 2023-06-22 19:26:47.000000 vss-cli-2023.6.1.dev2/vss_cli/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.507331 vss-cli-2023.6.1.dev2/vss_cli/data/
--rw-rw-rw-   0 root         (0) root         (0)     4524 2023-06-22 19:26:47.000000 vss-cli-2023.6.1.dev2/vss_cli/data/clib.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4070 2023-06-22 19:26:47.000000 vss-cli-2023.6.1.dev2/vss_cli/data/clone.yaml
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/data/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/data/image.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-06-22 19:26:47.000000 vss-cli-2023.6.1.dev2/vss_cli/data/shell.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-06-22 19:26:47.000000 vss-cli-2023.6.1.dev2/vss_cli/data/template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25272 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/hcio.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.511331 vss-cli-2023.6.1.dev2/vss_cli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 19:27:41.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15976 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/completion.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.515332 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/contentlib.py
--rw-rw-rw-   0 root         (0) root         (0)     2838 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/floppy.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/iso.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/os.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/rel_args.py
--rw-rw-rw-   0 root         (0) root         (0)     9402 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/template.py
--rw-rw-rw-   0 root         (0) root         (0)   141322 2023-06-22 19:26:47.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/vmdks.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/key.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/ovf.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.519332 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/change.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/export.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/new.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/retirement.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/vmdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/status.py
--rw-rw-rw-   0 root         (0) root         (0)     6761 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/stor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/token.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/plugins/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/sstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.519332 vss-cli-2023.6.1.dev2/vss_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75203 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/utils/emoji.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/utils/threading.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/vss.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/vssconst.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-14 16:00:18.000000 vss-cli-2023.6.1.dev2/vss_cli/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:27:45.507331 vss-cli-2023.6.1.dev2/vss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12464 2023-06-22 19:27:45.000000 vss-cli-2023.6.1.dev2/vss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2388 2023-06-22 19:27:45.000000 vss-cli-2023.6.1.dev2/vss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:27:45.000000 vss-cli-2023.6.1.dev2/vss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-22 19:27:45.000000 vss-cli-2023.6.1.dev2/vss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:27:45.000000 vss-cli-2023.6.1.dev2/vss_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-22 19:27:45.000000 vss-cli-2023.6.1.dev2/vss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 19:27:45.000000 vss-cli-2023.6.1.dev2/vss_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.934823 vss-cli-2023.6.1.dev3/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12464 2023-06-26 14:06:56.934823 vss-cli-2023.6.1.dev3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-26 14:06:56.934823 vss-cli-2023.6.1.dev3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.914823 vss-cli-2023.6.1.dev3/vss_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18320 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7453 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    62562 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    13887 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.918823 vss-cli-2023.6.1.dev3/vss_cli/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/data/clib.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4070 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/data/clone.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/data/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/data/image.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/data/shell.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/data/template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    25272 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/hcio.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.922823 vss-cli-2023.6.1.dev3/vss_cli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 14:06:53.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/completion.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.926823 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/contentlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/floppy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/iso.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/rel_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     9402 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)   141316 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/vmdks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/key.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/ovf.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.934823 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/new.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/retirement.py
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/vmdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     6761 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/stor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/plugins/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/sstatus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.934823 vss-cli-2023.6.1.dev3/vss_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75203 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/utils/emoji.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/utils/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/vss.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/vssconst.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-26 14:06:02.000000 vss-cli-2023.6.1.dev3/vss_cli/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:06:56.918823 vss-cli-2023.6.1.dev3/vss_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12464 2023-06-26 14:06:56.000000 vss-cli-2023.6.1.dev3/vss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-06-26 14:06:56.000000 vss-cli-2023.6.1.dev3/vss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:06:56.000000 vss-cli-2023.6.1.dev3/vss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-26 14:06:56.000000 vss-cli-2023.6.1.dev3/vss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:06:56.000000 vss-cli-2023.6.1.dev3/vss_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-26 14:06:56.000000 vss-cli-2023.6.1.dev3/vss_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-26 14:06:56.000000 vss-cli-2023.6.1.dev3/vss_cli.egg-info/top_level.txt
```

### Comparing `vss-cli-2023.6.1.dev2/LICENSE` & `vss-cli-2023.6.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/PKG-INFO` & `vss-cli-2023.6.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2023.6.1.dev2
+Version: 2023.6.1.dev3
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.1-dev2.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.1-dev3.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
```

### Comparing `vss-cli-2023.6.1.dev2/README.md` & `vss-cli-2023.6.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/setup.cfg` & `vss-cli-2023.6.1.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/setup.py` & `vss-cli-2023.6.1.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/autocompletion.py` & `vss-cli-2023.6.1.dev3/vss_cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/cli.py` & `vss-cli-2023.6.1.dev3/vss_cli/cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/config.py` & `vss-cli-2023.6.1.dev3/vss_cli/config.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/const.py` & `vss-cli-2023.6.1.dev3/vss_cli/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants used by VSS CLI (vss-cli)."""
 import os
 
 import pkg_resources
 
 PACKAGE_NAME = "vss_cli"
 
-__version__ = "2023.6.1-dev2"
+__version__ = "2023.6.1-dev3"
 
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://cloud-api.eis.utoronto.ca"
 DEFAULT_ENDPOINT_NAME = "cloud-api"
 DEFAULT_S3_SERVER = "https://vskey-stor.eis.utoronto.ca"
 _LEGACY_CONFIG = ("~", ".vss-cli", "config.json")
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/data/clib.yaml` & `vss-cli-2023.6.1.dev3/vss_cli/data/clib.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from CLib 2023.6.1-dev2             #
+#     VSS-CLI Spec from CLib 2023.6.1-dev3             #
 ####################################################
 built: clib               # Required: Do not remove.
 machine:
   item: ubuntu-22.04      # Required: Source content library id OVF.
   cpu: 1                  # Optional: CPU count (Default: 1).
   memory: 1               # Optional: Memory in GB (Default: 1GB).
   name: &name Vm-Name     # Required: Target virtual machine name.
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/data/clone.yaml` & `vss-cli-2023.6.1.dev3/vss_cli/data/clone.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Clone 2023.6.1-dev2             #
+#     VSS-CLI Spec from Clone 2023.6.1-dev3             #
 ####################################################
 built: clone              # Required: Do not remove.
 machine:
   source: SourceVM        # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   disks:
     - capacity_gb: 40     # Optional: Disk capacity in GB (Default: source vm disk capacity)
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/data/config.yaml` & `vss-cli-2023.6.1.dev3/vss_cli/data/config.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/data/image.yaml` & `vss-cli-2023.6.1.dev3/vss_cli/data/image.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/data/shell.yaml` & `vss-cli-2023.6.1.dev3/vss_cli/data/shell.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec shell VM v2023.6.1-dev2             #
+#     VSS-CLI Spec shell VM v2023.6.1-dev3             #
 ####################################################
 built: os_install         # Required: Do not remove.
 machine:
   name: Vm-Name            # Required: Target virtual machine name.
   os: ubuntu64Guest              # Required: Guest Operating System name or Id.
   cpu: 1                   # Optional: CPU count (Default: 1).
   memory: 1                # Optional: Memory in GB (Default: 1GB).
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/data/template.yaml` & `vss-cli-2023.6.1.dev3/vss_cli/data/template.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Template v2023.6.1-dev2         #
+#     VSS-CLI Spec from Template v2023.6.1-dev3         #
 ####################################################
 built: template           # Required: Do not remove.
 machine:
   source: NixSource                # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   folder: MyFolder       # Optional: Folder name, path or ID (Default: source vm folder)
   disks:
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/data_types.py` & `vss-cli-2023.6.1.dev3/vss_cli/data_types.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/hcio.py` & `vss-cli-2023.6.1.dev3/vss_cli/hcio.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/helper.py` & `vss-cli-2023.6.1.dev3/vss_cli/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/account.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/account.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/completion.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/completion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/callbacks.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/contentlib.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/contentlib.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/domain.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 
 @cli.group('domain', short_help='List compute domains.')
 @pass_context
 def cli(ctx: Configuration):
     """Domain command.
 
-    A fault domain consists of one or more ESXI hosts and
+    A domain consists of one or more ESXI hosts and
     Datastore Clusters grouped together according to their
     physical location in the datacenter.
     """
 
 
-@cli.command('ls', short_help='list fault domains')
+@cli.command('ls', short_help='list domains')
 @so.filter_opt
 @so.all_opt
 @so.page_opt
 @so.sort_opt
 @so.count_opt
 @pass_context
 def domain_ls(ctx: Configuration, filter_by, show_all, sort, page, count):
-    """List available fault domains."""
+    """List available domains."""
     columns = ctx.columns or const.COLUMNS_MOREF
     params = dict(expand=1, sort='name,asc')
     if all(filter_by):
         params['filter'] = ';'.join(filter_by)
     if all(sort):
         params['sort'] = ';'.join(sort)
     # query
@@ -57,15 +57,15 @@
     'name_or_moref',
     type=click.STRING,
     required=True,
     shell_complete=autocompletion.domains,
 )
 @pass_context
 def domain_get(ctx: Configuration, name_or_moref):
-    """Get fault domain information."""
+    """Get domain information."""
     _domain = ctx.get_domain_by_name_or_moref(name_or_moref)
     ctx.moref = _domain[0]['moref']
     if click.get_current_context().invoked_subcommand is None:
         columns = ctx.columns or const.COLUMNS_MOREF
         with ctx.spinner(disable=ctx.debug):
             obj = ctx.get_domain(ctx.moref)
         ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
@@ -73,15 +73,15 @@
 
 @domain_get.command('vms', help='Given domain vms.')
 @click.option(
     '-p', '--page', is_flag=True, help='page results in a less-like format'
 )
 @pass_context
 def domain_get_vms(ctx: Configuration, page):
-    """Get VMs in given fault domain."""
+    """Get VMs in given domain."""
     with ctx.spinner(disable=ctx.debug):
         obj = ctx.get_vms_by_domain(ctx.moref)
     if not obj:
         raise VssCliError(
             f'Either domain {ctx.moref} does not exist, '
             f'or you do not have permission to access.'
         )
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/floppy.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/floppy.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/folder.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/helper.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/image.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/inventory.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/iso.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/iso.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/net.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/net.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/os.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/os.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/rel_args.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/rel_args.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/rel_opts.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/template.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/template.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/vm.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/vm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1807,15 +1807,15 @@
     '--force',
     is_flag=True,
     help='Shut down or power off before migration.',
 )
 @click.option('-o', '--on', is_flag=True, help='Power of after migrating')
 @pass_context
 def compute_vm_set_domain(ctx: Configuration, name_or_moref, force, on):
-    """Migrate a virtual machine to another fault domain.
+    """Migrate a virtual machine to another domain.
 
     In order to proceed with the virtual machine relocation,
     in some cases the VM is required to be in a powered off state.
 
     The `force` flag will send a shutdown signal anf if times out,
     will perform a power off task. After migration completes, the `on` flag
     indicates to power on the virtual machine.
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/compute_plugins/vmdks.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/compute_plugins/vmdks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/configure.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/configure.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/key.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/key.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/message.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/message.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/misc.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/ovf.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/ovf.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/plugins.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/raw.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/raw.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/change.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/change.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/export.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/export.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/folder.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/image.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/inventory.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/new.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/new.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/retirement.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/retirement.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/snapshot.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/snapshot.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/request_plugins/vmdk.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/request_plugins/vmdk.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/service.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/service.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/shell.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/status.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/status.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/stor.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/stor.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/token.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/token.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/plugins/upgrade.py` & `vss-cli-2023.6.1.dev3/vss_cli/plugins/upgrade.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/rel_opts.py` & `vss-cli-2023.6.1.dev3/vss_cli/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/sstatus.py` & `vss-cli-2023.6.1.dev3/vss_cli/sstatus.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/utils/emoji.py` & `vss-cli-2023.6.1.dev3/vss_cli/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/utils/threading.py` & `vss-cli-2023.6.1.dev3/vss_cli/utils/threading.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/validators.py` & `vss-cli-2023.6.1.dev3/vss_cli/validators.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/vss.py` & `vss-cli-2023.6.1.dev3/vss_cli/vss.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli/yaml.py` & `vss-cli-2023.6.1.dev3/vss_cli/yaml.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli.egg-info/PKG-INFO` & `vss-cli-2023.6.1.dev3/vss_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2023.6.1.dev2
+Version: 2023.6.1.dev3
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.1-dev2.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.1-dev3.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
```

### Comparing `vss-cli-2023.6.1.dev2/vss_cli.egg-info/SOURCES.txt` & `vss-cli-2023.6.1.dev3/vss_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.1.dev2/vss_cli.egg-info/requires.txt` & `vss-cli-2023.6.1.dev3/vss_cli.egg-info/requires.txt`

 * *Files identical despite different names*

