# Comparing `tmp/dvc-3.2.1.tar.gz` & `tmp/dvc-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-3.2.1.tar", last modified: Fri Jun 23 03:38:23 2023, max compression
+gzip compressed data, was "dvc-3.2.2.tar", last modified: Mon Jun 26 05:12:22 2023, max compression
```

## Comparing `dvc-3.2.1.tar` & `dvc-3.2.2.tar`

### file list

```diff
@@ -1,665 +1,666 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.658466 dvc-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-23 03:38:06.000000 dvc-3.2.1/.dvcignore
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-23 03:38:06.000000 dvc-3.2.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-23 03:38:06.000000 dvc-3.2.1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-23 03:38:06.000000 dvc-3.2.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-23 03:38:06.000000 dvc-3.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.594466 dvc-3.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.594466 dvc-3.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/ISSUE_TEMPLATE/epic_story.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.594466 dvc-3.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/workflows/packages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/workflows/plugin_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-23 03:38:06.000000 dvc-3.2.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-23 03:38:06.000000 dvc-3.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-23 03:38:06.000000 dvc-3.2.1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-23 03:38:06.000000 dvc-3.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-23 03:38:06.000000 dvc-3.2.1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-23 03:38:06.000000 dvc-3.2.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-23 03:38:06.000000 dvc-3.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-23 03:38:06.000000 dvc-3.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-23 03:38:06.000000 dvc-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-23 03:38:23.654466 dvc-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-06-23 03:38:06.000000 dvc-3.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.598466 dvc-3.2.1/dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-23 03:38:10.000000 dvc-3.2.1/dvc/_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-23 03:38:23.000000 dvc-3.2.1/dvc/_dvc_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.598466 dvc-3.2.1/dvc/api/
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/api/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/api/experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/api/scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    11924 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/api/show.py
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/cachemgr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.598466 dvc-3.2.1/dvc/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     7614 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.602466 dvc-3.2.1/dvc/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/commands/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/exec_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3672 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/install.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/ls/ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/commands/queue/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/queue/kill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/queue/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/queue/start.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/queue/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/queue/stop.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/repro.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/compare.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    11039 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/dagascii.py
--rw-r--r--   0 runner    (1001) docker     (122)    11333 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/data_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5148 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/dependency/param.py
--rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/dependency/repo.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/env.py
--rw-r--r--   0 runner    (1001) docker     (122)     9622 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/fs/
--rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/fs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/fs/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    13922 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/fs/dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/fs/git.py
--rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/machine/
--rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/machine/backend/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/machine/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/machine/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/machine/backend/terraform.py
--rw-r--r--   0 runner    (1001) docker     (122)    46033 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)    15488 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/parsing/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/parsing/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.606466 dvc-3.2.1/dvc/render/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/render/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.610466 dvc-3.2.1/dvc/render/converter/
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/render/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/render/converter/image.py
--rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/render/converter/vega.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/render/match.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.614466 dvc-3.2.1/dvc/repo/
--rw-r--r--   0 runner    (1001) docker     (122)    18691 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.614466 dvc-3.2.1/dvc/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.614466 dvc-3.2.1/dvc/repo/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25373 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/executor/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/executor/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/push.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.618466 dvc-3.2.1/dvc/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/queue/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/refs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/stash.py
--rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/get.py
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    23105 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/index.py
--rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/ls_url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.618466 dvc-3.2.1/dvc/repo/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/metrics/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/metrics/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     8230 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/open_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.618466 dvc-3.2.1/dvc/repo/params/
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/params/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/params/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.618466 dvc-3.2.1/dvc/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/plots/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/repo/worktree.py
--rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     4310 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.618466 dvc-3.2.1/dvc/stage/
--rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9221 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     7462 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/params.py
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/stage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.618466 dvc-3.2.1/dvc/testing/
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4128 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/api_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.618466 dvc-3.2.1/dvc/testing/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.622466 dvc-3.2.1/dvc/testing/benchmarks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.622466 dvc-3.2.1/dvc/testing/benchmarks/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.622466 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_exp_show.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_help.py
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_push.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.622466 dvc-3.2.1/dvc/testing/benchmarks/cli/stories/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/stories/test_modify_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.622466 dvc-3.2.1/dvc/testing/benchmarks/cli/stories/use_cases/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/benchmarks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/path_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/remote_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/tmp_dir.py
--rw-r--r--   0 runner    (1001) docker     (122)    12070 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/testing/workspace_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.622466 dvc-3.2.1/dvc/ui/
--rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/ui/_rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/ui/pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/ui/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.626466 dvc-3.2.1/dvc/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.626466 dvc-3.2.1/dvc/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/serialize/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/serialize/_py.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/serialize/_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/serialize/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/utils/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-23 03:38:06.000000 dvc-3.2.1/dvc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.598466 dvc-3.2.1/dvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-23 03:38:23.000000 dvc-3.2.1/dvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16599 2023-06-23 03:38:23.000000 dvc-3.2.1/dvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 03:38:23.000000 dvc-3.2.1/dvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-23 03:38:23.000000 dvc-3.2.1/dvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1507 2023-06-23 03:38:23.000000 dvc-3.2.1/dvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-23 03:38:23.000000 dvc-3.2.1/dvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8681 2023-06-23 03:38:06.000000 dvc-3.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.626466 dvc-3.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/build-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      226 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/build_package.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.626466 dvc-3.2.1/scripts/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/build.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.626466 dvc-3.2.1/scripts/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-asyncssh.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-dvc.system.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-fsspec.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-23 03:38:06.000000 dvc-3.2.1/scripts/pyinstaller/hooks/hook-pydrive2.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-23 03:38:23.658466 dvc-3.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.626466 dvc-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/dir_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.634466 dvc-3.2.1/tests/func/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.634466 dvc-3.2.1/tests/func/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8061 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/api/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/api/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/api/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.634466 dvc-3.2.1/tests/func/artifacts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/artifacts/test_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.634466 dvc-3.2.1/tests/func/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.634466 dvc-3.2.1/tests/func/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3425 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/data/db/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/executor/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    26341 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)    13854 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_save.py
--rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_set_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_stash_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/machine/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/machine/test_machine_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/machine/test_machine_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7730 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/metrics/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/metrics/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/params/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/params/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/params/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10114 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/parsing/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    15835 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/parsing/test_foreach.py
--rw-r--r--   0 runner    (1001) docker     (122)     9670 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/parsing/test_interpolated_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/parsing/test_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/plots/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/plots/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/repro/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/repro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    33460 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/repro/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/repro/test_repro_allow_missing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/repro/test_repro_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)    30224 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    22833 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    16589 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_data_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    19044 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    12234 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     7976 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)    10535 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    21031 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    17911 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_merge_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_move.py
--rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_root.py
--rw-r--r--   0 runner    (1001) docker     (122)    20611 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_run_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_stage_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_used_objs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/test_virtual_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/func/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/utils/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/func/utils/test_strict_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.638466 dvc-3.2.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.642466 dvc-3.2.1/tests/integration/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/integration/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/integration/plots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13823 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/integration/plots/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/integration/plots/test_repo_plots_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/integration/test_studio_live_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.642466 dvc-3.2.1/tests/remotes/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/remotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.642466 dvc-3.2.1/tests/remotes/git-init/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/remotes/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/remotes/git_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/remotes/user.key
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/remotes/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/remotes_env.sample
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.642466 dvc-3.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.642466 dvc-3.2.1/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/cli/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.646466 dvc-3.2.1/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.646466 dvc-3.2.1/tests/unit/command/ls/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/ls/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/ls/test_ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_compat_flag.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)    11250 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    11272 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/command/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.646466 dvc-3.2.1/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.646466 dvc-3.2.1/tests/unit/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/data/db/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.646466 dvc-3.2.1/tests/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/dependency/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/dependency/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.650466 dvc-3.2.1/tests/unit/fs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    19226 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_dvc_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/fs/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.650466 dvc-3.2.1/tests/unit/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.650466 dvc-3.2.1/tests/unit/output/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/output/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/output/test_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/output/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/output/test_output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.650466 dvc-3.2.1/tests/unit/remote/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/remote/test_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/remote/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/remote/test_webdav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/remote/test_webhdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.650466 dvc-3.2.1/tests/unit/render/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/render/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/render/test_image_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/render/test_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/render/test_vega_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.650466 dvc-3.2.1/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.650466 dvc-3.2.1/tests/unit/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/unit/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/queue/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/queue/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/test_executor_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/unit/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/test_open_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/test_reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/repo/test_scm_context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/unit/scm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/scm/test_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/unit/stage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6074 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/test_loader_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/test_serialize_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/test_serialize_pipeline_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/stage/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_hashinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     8740 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4168 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_tabular_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/unit/ui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/ui/test_console.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/ui/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/ui/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/unit/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/serialize/test_python.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/serialize/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/serialize/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/test_cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:38:23.654466 dvc-3.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-23 03:38:06.000000 dvc-3.2.1/tests/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.989667 dvc-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-26 05:12:05.000000 dvc-3.2.2/.dvcignore
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-26 05:12:05.000000 dvc-3.2.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-26 05:12:05.000000 dvc-3.2.2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-26 05:12:05.000000 dvc-3.2.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-26 05:12:05.000000 dvc-3.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.909666 dvc-3.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.909666 dvc-3.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/ISSUE_TEMPLATE/epic_story.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.909666 dvc-3.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/workflows/packages.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/workflows/plugin_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-26 05:12:05.000000 dvc-3.2.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-26 05:12:05.000000 dvc-3.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-26 05:12:05.000000 dvc-3.2.2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-26 05:12:05.000000 dvc-3.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-26 05:12:05.000000 dvc-3.2.2/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-26 05:12:05.000000 dvc-3.2.2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-26 05:12:05.000000 dvc-3.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 05:12:05.000000 dvc-3.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-26 05:12:05.000000 dvc-3.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-26 05:12:22.989667 dvc-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-06-26 05:12:05.000000 dvc-3.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.917666 dvc-3.2.2/dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-26 05:12:08.000000 dvc-3.2.2/dvc/_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-26 05:12:22.000000 dvc-3.2.2/dvc/_dvc_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.917666 dvc-3.2.2/dvc/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/api/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/api/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/api/scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11924 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/api/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/cachemgr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.917666 dvc-3.2.2/dvc/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     7614 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.925666 dvc-3.2.2/dvc/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.925666 dvc-3.2.2/dvc/commands/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/exec_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3672 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/install.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.925666 dvc-3.2.2/dvc/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/ls/ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.925666 dvc-3.2.2/dvc/commands/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/queue/kill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/queue/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/queue/start.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/queue/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/queue/stop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11039 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/dagascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11333 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/data_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.929666 dvc-3.2.2/dvc/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5148 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/dependency/param.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/dependency/repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9622 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.929666 dvc-3.2.2/dvc/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4280 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/fs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/fs/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13922 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/fs/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/fs/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.929666 dvc-3.2.2/dvc/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.929666 dvc-3.2.2/dvc/machine/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/machine/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/machine/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/machine/backend/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46033 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.929666 dvc-3.2.2/dvc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)    15488 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/parsing/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/parsing/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.929666 dvc-3.2.2/dvc/render/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/render/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.929666 dvc-3.2.2/dvc/render/converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/render/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/render/converter/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/render/converter/vega.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/render/match.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.933666 dvc-3.2.2/dvc/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)    18691 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.937667 dvc-3.2.2/dvc/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11317 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.937667 dvc-3.2.2/dvc/repo/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25373 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/executor/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9647 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/executor/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/push.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.941666 dvc-3.2.2/dvc/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/queue/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/refs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/stash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23105 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/ls_url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.941666 dvc-3.2.2/dvc/repo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/metrics/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/metrics/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8230 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/open_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.941666 dvc-3.2.2/dvc/repo/params/
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/params/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/params/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.941666 dvc-3.2.2/dvc/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/plots/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/repo/worktree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4310 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.941666 dvc-3.2.2/dvc/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9221 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7462 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/stage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.945667 dvc-3.2.2/dvc/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4128 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/api_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.945667 dvc-3.2.2/dvc/testing/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.945667 dvc-3.2.2/dvc/testing/benchmarks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.945667 dvc-3.2.2/dvc/testing/benchmarks/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.949667 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_exp_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.949667 dvc-3.2.2/dvc/testing/benchmarks/cli/stories/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/stories/test_modify_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.949667 dvc-3.2.2/dvc/testing/benchmarks/cli/stories/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/benchmarks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/path_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/remote_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/tmp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12070 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/testing/workspace_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.949667 dvc-3.2.2/dvc/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/ui/_rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/ui/pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/ui/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.949667 dvc-3.2.2/dvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.949667 dvc-3.2.2/dvc/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/serialize/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/serialize/_py.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/serialize/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/serialize/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/utils/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-26 05:12:05.000000 dvc-3.2.2/dvc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.917666 dvc-3.2.2/dvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-26 05:12:22.000000 dvc-3.2.2/dvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16643 2023-06-26 05:12:22.000000 dvc-3.2.2/dvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 05:12:22.000000 dvc-3.2.2/dvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-26 05:12:22.000000 dvc-3.2.2/dvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1507 2023-06-26 05:12:22.000000 dvc-3.2.2/dvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-26 05:12:22.000000 dvc-3.2.2/dvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8681 2023-06-26 05:12:05.000000 dvc-3.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.953667 dvc-3.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/build-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      226 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/build_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.953667 dvc-3.2.2/scripts/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/build.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.953667 dvc-3.2.2/scripts/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-asyncssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-dvc.system.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-26 05:12:05.000000 dvc-3.2.2/scripts/pyinstaller/hooks/hook-pydrive2.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 05:12:22.989667 dvc-3.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.953667 dvc-3.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/dir_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.961667 dvc-3.2.2/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.961667 dvc-3.2.2/tests/func/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8061 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/api/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/api/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/api/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.961667 dvc-3.2.2/tests/func/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/artifacts/test_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.961667 dvc-3.2.2/tests/func/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.961667 dvc-3.2.2/tests/func/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3425 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/data/db/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.965667 dvc-3.2.2/tests/func/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.965667 dvc-3.2.2/tests/func/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/executor/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26341 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13854 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_set_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_stash_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.965667 dvc-3.2.2/tests/func/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/machine/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/machine/test_machine_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/machine/test_machine_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.965667 dvc-3.2.2/tests/func/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7730 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/metrics/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/metrics/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.965667 dvc-3.2.2/tests/func/params/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/params/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/params/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.965667 dvc-3.2.2/tests/func/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10114 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/parsing/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15835 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/parsing/test_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9670 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/parsing/test_interpolated_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/parsing/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.965667 dvc-3.2.2/tests/func/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/plots/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/plots/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.969667 dvc-3.2.2/tests/func/repro/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/repro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33460 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/repro/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/repro/test_repro_allow_missing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/repro/test_repro_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30224 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22833 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16589 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_data_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19044 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12234 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7976 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10535 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21031 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17911 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_merge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20611 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_run_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_stage_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_used_objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/test_virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.969667 dvc-3.2.2/tests/func/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/utils/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/func/utils/test_strict_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.969667 dvc-3.2.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.969667 dvc-3.2.2/tests/integration/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/integration/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/integration/plots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13823 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/integration/plots/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/integration/plots/test_repo_plots_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/integration/test_studio_live_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.969667 dvc-3.2.2/tests/remotes/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/remotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.969667 dvc-3.2.2/tests/remotes/git-init/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/remotes/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/remotes/git_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/remotes/user.key
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/remotes/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/remotes_env.sample
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.973667 dvc-3.2.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.973667 dvc-3.2.2/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/cli/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.977667 dvc-3.2.2/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.977667 dvc-3.2.2/tests/unit/command/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/ls/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/ls/test_ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_compat_flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3941 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11250 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11272 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/command/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.977667 dvc-3.2.2/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.977667 dvc-3.2.2/tests/unit/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/data/db/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.977667 dvc-3.2.2/tests/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/dependency/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/dependency/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.977667 dvc-3.2.2/tests/unit/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19226 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_dvc_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/fs/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.981667 dvc-3.2.2/tests/unit/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.981667 dvc-3.2.2/tests/unit/output/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/output/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/output/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/output/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/output/test_output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.981667 dvc-3.2.2/tests/unit/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/remote/test_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/remote/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/remote/test_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/remote/test_webhdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.981667 dvc-3.2.2/tests/unit/render/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/render/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/render/test_image_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/render/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/render/test_vega_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.981667 dvc-3.2.2/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.981667 dvc-3.2.2/tests/unit/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/unit/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/queue/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/queue/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/test_executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/unit/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/test_open_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/test_reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/repo/test_scm_context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/unit/scm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/scm/test_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/unit/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6074 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/test_loader_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/test_serialize_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/test_serialize_pipeline_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/stage/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_hashinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8740 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4168 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_tabular_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/unit/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/ui/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/ui/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/ui/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/unit/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/serialize/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/serialize/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/serialize/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/test_cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 05:12:22.985667 dvc-3.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-26 05:12:05.000000 dvc-3.2.2/tests/utils/plots.py
```

### Comparing `dvc-3.2.1/.git-blame-ignore-revs` & `dvc-3.2.2/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `dvc-3.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.github/ISSUE_TEMPLATE/epic_story.md` & `dvc-3.2.2/.github/ISSUE_TEMPLATE/epic_story.md`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.github/workflows/codeql.yml` & `dvc-3.2.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.github/workflows/packages.yaml` & `dvc-3.2.2/.github/workflows/packages.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.github/workflows/plugin_tests.yaml` & `dvc-3.2.2/.github/workflows/plugin_tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.github/workflows/tests.yaml` & `dvc-3.2.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.pre-commit-config.yaml` & `dvc-3.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/.pre-commit-hooks.yaml` & `dvc-3.2.2/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/CODE_OF_CONDUCT.md` & `dvc-3.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/LICENSE` & `dvc-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/PKG-INFO` & `dvc-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.2.1
+Version: 3.2.2
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.2.1/README.rst` & `dvc-3.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/_debug.py` & `dvc-3.2.2/dvc/_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/analytics.py` & `dvc-3.2.2/dvc/analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/annotations.py` & `dvc-3.2.2/dvc/annotations.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/api/data.py` & `dvc-3.2.2/dvc/api/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/api/experiments.py` & `dvc-3.2.2/dvc/api/experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/api/scm.py` & `dvc-3.2.2/dvc/api/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/api/show.py` & `dvc-3.2.2/dvc/api/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/cachemgr.py` & `dvc-3.2.2/dvc/cachemgr.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/cli/__init__.py` & `dvc-3.2.2/dvc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/cli/command.py` & `dvc-3.2.2/dvc/cli/command.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/cli/completion.py` & `dvc-3.2.2/dvc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/cli/parser.py` & `dvc-3.2.2/dvc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/cli/utils.py` & `dvc-3.2.2/dvc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/add.py` & `dvc-3.2.2/dvc/commands/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/cache.py` & `dvc-3.2.2/dvc/commands/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/check_ignore.py` & `dvc-3.2.2/dvc/commands/check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/checkout.py` & `dvc-3.2.2/dvc/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/commit.py` & `dvc-3.2.2/dvc/commands/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/completion.py` & `dvc-3.2.2/dvc/commands/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/config.py` & `dvc-3.2.2/dvc/commands/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/daemon.py` & `dvc-3.2.2/dvc/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/dag.py` & `dvc-3.2.2/dvc/commands/dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/data.py` & `dvc-3.2.2/dvc/commands/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/data_sync.py` & `dvc-3.2.2/dvc/commands/data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/destroy.py` & `dvc-3.2.2/dvc/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/diff.py` & `dvc-3.2.2/dvc/commands/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/__init__.py` & `dvc-3.2.2/dvc/commands/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/apply.py` & `dvc-3.2.2/dvc/commands/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/branch.py` & `dvc-3.2.2/dvc/commands/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/clean.py` & `dvc-3.2.2/dvc/commands/experiments/clean.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/diff.py` & `dvc-3.2.2/dvc/commands/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/exec_run.py` & `dvc-3.2.2/dvc/commands/experiments/exec_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/ls.py` & `dvc-3.2.2/dvc/commands/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/pull.py` & `dvc-3.2.2/dvc/commands/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/push.py` & `dvc-3.2.2/dvc/commands/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/queue_worker.py` & `dvc-3.2.2/dvc/commands/experiments/queue_worker.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/remove.py` & `dvc-3.2.2/dvc/commands/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/run.py` & `dvc-3.2.2/dvc/commands/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/save.py` & `dvc-3.2.2/dvc/commands/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/experiments/show.py` & `dvc-3.2.2/dvc/commands/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/freeze.py` & `dvc-3.2.2/dvc/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/gc.py` & `dvc-3.2.2/dvc/commands/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/get.py` & `dvc-3.2.2/dvc/commands/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/get_url.py` & `dvc-3.2.2/dvc/commands/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/git_hook.py` & `dvc-3.2.2/dvc/commands/git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/imp.py` & `dvc-3.2.2/dvc/commands/imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/imp_url.py` & `dvc-3.2.2/dvc/commands/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/init.py` & `dvc-3.2.2/dvc/commands/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/install.py` & `dvc-3.2.2/dvc/commands/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/ls/__init__.py` & `dvc-3.2.2/dvc/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/ls/ls_colors.py` & `dvc-3.2.2/dvc/commands/ls/ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/ls_url.py` & `dvc-3.2.2/dvc/commands/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/machine.py` & `dvc-3.2.2/dvc/commands/machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/metrics.py` & `dvc-3.2.2/dvc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/move.py` & `dvc-3.2.2/dvc/commands/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/params.py` & `dvc-3.2.2/dvc/commands/params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/plots.py` & `dvc-3.2.2/dvc/commands/plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/queue/__init__.py` & `dvc-3.2.2/dvc/commands/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/queue/kill.py` & `dvc-3.2.2/dvc/commands/queue/kill.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/queue/logs.py` & `dvc-3.2.2/dvc/commands/queue/logs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/queue/remove.py` & `dvc-3.2.2/dvc/commands/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/queue/start.py` & `dvc-3.2.2/dvc/commands/queue/start.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/queue/status.py` & `dvc-3.2.2/dvc/commands/queue/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/queue/stop.py` & `dvc-3.2.2/dvc/commands/queue/stop.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/remote.py` & `dvc-3.2.2/dvc/commands/remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/remove.py` & `dvc-3.2.2/dvc/commands/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/repro.py` & `dvc-3.2.2/dvc/commands/repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/root.py` & `dvc-3.2.2/dvc/commands/root.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/stage.py` & `dvc-3.2.2/dvc/commands/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/status.py` & `dvc-3.2.2/dvc/commands/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/unprotect.py` & `dvc-3.2.2/dvc/commands/unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/update.py` & `dvc-3.2.2/dvc/commands/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/commands/version.py` & `dvc-3.2.2/dvc/commands/version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/compare.py` & `dvc-3.2.2/dvc/compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/config.py` & `dvc-3.2.2/dvc/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/config_schema.py` & `dvc-3.2.2/dvc/config_schema.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/daemon.py` & `dvc-3.2.2/dvc/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/dagascii.py` & `dvc-3.2.2/dvc/dagascii.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/data_cloud.py` & `dvc-3.2.2/dvc/data_cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/dependency/__init__.py` & `dvc-3.2.2/dvc/dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/dependency/base.py` & `dvc-3.2.2/dvc/dependency/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/dependency/param.py` & `dvc-3.2.2/dvc/dependency/param.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/dependency/repo.py` & `dvc-3.2.2/dvc/dependency/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/dirs.py` & `dvc-3.2.2/dvc/dirs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/dvcfile.py` & `dvc-3.2.2/dvc/dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/env.py` & `dvc-3.2.2/dvc/env.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/exceptions.py` & `dvc-3.2.2/dvc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/fs/__init__.py` & `dvc-3.2.2/dvc/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/fs/data.py` & `dvc-3.2.2/dvc/fs/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/fs/dvc.py` & `dvc-3.2.2/dvc/fs/dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/fs/git.py` & `dvc-3.2.2/dvc/fs/git.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/ignore.py` & `dvc-3.2.2/dvc/ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/info.py` & `dvc-3.2.2/dvc/info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/lock.py` & `dvc-3.2.2/dvc/lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/logger.py` & `dvc-3.2.2/dvc/logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/machine/__init__.py` & `dvc-3.2.2/dvc/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/machine/backend/base.py` & `dvc-3.2.2/dvc/machine/backend/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/machine/backend/terraform.py` & `dvc-3.2.2/dvc/machine/backend/terraform.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/output.py` & `dvc-3.2.2/dvc/output.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/parsing/__init__.py` & `dvc-3.2.2/dvc/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/parsing/context.py` & `dvc-3.2.2/dvc/parsing/context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/parsing/interpolate.py` & `dvc-3.2.2/dvc/parsing/interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/pathspec_math.py` & `dvc-3.2.2/dvc/pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/progress.py` & `dvc-3.2.2/dvc/progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Manages progress bars for DVC repo."""
 import logging
 import sys
 from threading import RLock
+from typing import TYPE_CHECKING
 
 from tqdm import tqdm
 
 from dvc.env import DVC_IGNORE_ISATTY
 from dvc.utils import env2bool
 
+if TYPE_CHECKING:
+    from dvc.fs.callbacks import TqdmCallback
+
 logger = logging.getLogger(__name__)
 tqdm.set_lock(RLock())
 
 
 class Tqdm(tqdm):
     """
     maximum-compatibility tqdm-based progressbars
@@ -154,7 +158,12 @@
         if ncols_left:
             d["ncols_desc"] = d["ncols_info"] = ncols_left
         else:
             # work-around for zero-width description
             d["ncols_desc"] = d["ncols_info"] = 1
             d["prefix"] = ""
         return d
+
+    def as_callback(self) -> "TqdmCallback":
+        from dvc.fs.callbacks import TqdmCallback
+
+        return TqdmCallback(progress_bar=self)
```

### Comparing `dvc-3.2.1/dvc/prompt.py` & `dvc-3.2.2/dvc/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/render/convert.py` & `dvc-3.2.2/dvc/render/convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/render/converter/__init__.py` & `dvc-3.2.2/dvc/render/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/render/converter/image.py` & `dvc-3.2.2/dvc/render/converter/image.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/render/converter/vega.py` & `dvc-3.2.2/dvc/render/converter/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/render/match.py` & `dvc-3.2.2/dvc/render/match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/__init__.py` & `dvc-3.2.2/dvc/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/add.py` & `dvc-3.2.2/dvc/repo/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/artifacts.py` & `dvc-3.2.2/dvc/repo/artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/brancher.py` & `dvc-3.2.2/dvc/repo/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/checkout.py` & `dvc-3.2.2/dvc/repo/checkout.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from dvc.exceptions import (
     CheckoutError,
     CheckoutErrorSuggestGit,
     DvcException,
     NoOutputOrStageError,
 )
+from dvc.ui import ui
 from dvc.utils import relpath
 
 from . import locked
 
 if TYPE_CHECKING:
     from dvc_data.index import BaseDataIndex, DataIndexEntry
     from dvc_objects.fs.base import FileSystem
@@ -102,15 +103,14 @@
     with_deps=False,
     force=False,
     relink=False,
     recursive=False,
     allow_missing=False,
     **kwargs,
 ):
-    from dvc.fs.callbacks import Callback
     from dvc.repo.index import build_data_index
     from dvc.stage.exceptions import StageFileBadNameError, StageFileDoesNotExistError
     from dvc_data.index.checkout import ADD, DELETE, MODIFY, apply, compare
 
     stats: Dict[str, List[str]] = {
         "added": [],
         "deleted": [],
@@ -138,54 +138,58 @@
     view = self.index.targets_view(
         targets,
         recursive=recursive,
         with_deps=with_deps,
         onerror=onerror,
     )
 
-    with Callback.as_tqdm_callback(
+    with ui.progress(
         unit="entry",
         desc="Building data index",
-    ) as cb:
+    ) as pb:
         old = build_data_index(
-            view, self.root_dir, self.fs, compute_hash=True, callback=cb
+            view,
+            self.root_dir,
+            self.fs,
+            compute_hash=True,
+            callback=pb.as_callback(),
         )
 
     new = view.data["repo"]
 
-    with Callback.as_tqdm_callback(
+    with ui.progress(
         desc="Comparing indexes",
         unit="entry",
-    ) as cb:
-        diff = compare(old, new, relink=relink, delete=True, callback=cb)
+    ) as pb:
+        diff = compare(old, new, relink=relink, delete=True, callback=pb.as_callback())
 
     if not force:
         _check_can_delete(diff.files_delete, new, self.root_dir, self.fs)
 
     failed = set()
     out_paths = [out.fs_path for out in view.outs if out.use_cache and out.is_in_repo]
 
     def checkout_onerror(src_path, dest_path, _exc):
         logger.debug(
-            "failed to create {%s} from {%s}", dest_path, src_path, exc_info=True
+            "failed to create '%s' from '%s'", dest_path, src_path, exc_info=True
         )
 
         for out_path in out_paths:
             if self.fs.path.isin_or_eq(dest_path, out_path):
                 failed.add(out_path)
 
-    with Callback.as_tqdm_callback(
+    with ui.progress(
         unit="file",
         desc="Checkout",
-    ) as cb:
+    ) as pb:
         apply(
             diff,
             self.root_dir,
             self.fs,
-            callback=cb,
+            callback=pb.as_callback(),
             update_meta=False,
             onerror=checkout_onerror,
             state=self.state,
             **kwargs,
         )
 
     out_changes = _build_out_changes(view, diff.changes)
```

### Comparing `dvc-3.2.1/dvc/repo/collect.py` & `dvc-3.2.2/dvc/repo/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/commit.py` & `dvc-3.2.2/dvc/repo/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/data.py` & `dvc-3.2.2/dvc/repo/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import posixpath
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, TypedDict, Union
 
+from dvc.fs.callbacks import DEFAULT_CALLBACK
 from dvc.ui import ui
 
 if TYPE_CHECKING:
+    from dvc.fs.callbacks import Callback
     from dvc.repo import Repo
     from dvc.scm import Git, NoSCM
     from dvc_data.index import DataIndex
     from dvc_data.index.diff import Change
 
 
 def posixpath_to_os_path(path: str) -> str:
@@ -46,14 +48,15 @@
     old: "DataIndex",
     new: "DataIndex",
     *,
     granular: bool = False,
     not_in_cache: bool = False,
     not_in_remote: bool = False,
     remote_refresh: bool = False,
+    callback: "Callback" = DEFAULT_CALLBACK,
 ) -> Dict[str, List[str]]:
     from dvc_data.index import StorageError
     from dvc_data.index.diff import UNCHANGED, UNKNOWN, diff
 
     ret: Dict[str, List[str]] = {}
 
     def _add_change(typ, change):
@@ -66,14 +69,15 @@
     for change in diff(
         old,
         new,
         with_unchanged=True,
         shallow=not granular,
         hash_only=True,
         with_unknown=True,
+        callback=callback,
     ):
         if (
             change.typ == UNCHANGED
             and (not change.old or not change.old.hash_info)
             and (not change.new or not change.new.hash_info)
         ):
             # NOTE: emulating previous behaviour
@@ -145,38 +149,52 @@
         is_dirty=any([staged, unstaged, untracked]),
     )
 
 
 def _diff_index_to_wtree(repo: "Repo", **kwargs: Any) -> Dict[str, List[str]]:
     from .index import build_data_index
 
-    with ui.status("Building workspace index"):
+    with ui.progress(
+        desc="Building workspace index",
+        unit="entry",
+    ) as pb:
         workspace = build_data_index(
-            repo.index, repo.root_dir, repo.fs, compute_hash=True
+            repo.index,
+            repo.root_dir,
+            repo.fs,
+            compute_hash=True,
+            callback=pb.as_callback(),
         )
 
-    with ui.status("Calculating diff between index/workspace"):
+    with ui.progress(
+        desc="Calculating diff between index/workspace",
+        unit="entry",
+    ) as pb:
         return _diff(
             repo.index.data["repo"],
             workspace,
             not_in_cache=True,
+            callback=pb.as_callback(),
             **kwargs,
         )
 
 
 def _diff_head_to_index(
     repo: "Repo", head: str = "HEAD", **kwargs: Any
 ) -> Dict[str, List[str]]:
     index = repo.index.data["repo"]
 
     with repo.switch(head):
         head_index = repo.index.data["repo"]
 
-    with ui.status("Calculating diff between head/index"):
-        return _diff(head_index, index, **kwargs)
+    with ui.progress(
+        desc="Calculating diff between head/index",
+        unit="entry",
+    ) as pb:
+        return _diff(head_index, index, callback=pb.as_callback(), **kwargs)
 
 
 class Status(TypedDict):
     not_in_cache: List[str]
     not_in_remote: List[str]
     committed: Dict[str, List[str]]
     uncommitted: Dict[str, List[str]]
```

### Comparing `dvc-3.2.1/dvc/repo/destroy.py` & `dvc-3.2.2/dvc/repo/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/diff.py` & `dvc-3.2.2/dvc/repo/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/__init__.py` & `dvc-3.2.2/dvc/repo/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/apply.py` & `dvc-3.2.2/dvc/repo/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/branch.py` & `dvc-3.2.2/dvc/repo/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/brancher.py` & `dvc-3.2.2/dvc/repo/experiments/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/cache.py` & `dvc-3.2.2/dvc/repo/experiments/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/collect.py` & `dvc-3.2.2/dvc/repo/experiments/collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     TYPE_CHECKING,
     Collection,
     Dict,
     Iterable,
     Iterator,
     List,
     Optional,
+    Tuple,
     Union,
 )
 
 from funcy import first
 from scmrepo.exceptions import SCMError as InnerSCMError
 
 from dvc.scm import Git, SCMError, iter_revs
@@ -365,16 +366,17 @@
             names[rev] = head_branch
         else:
             names[rev] = tags.get(rev) or branches.get(rev)
     return names
 
 
 def _sorted_ranges(exp_ranges: Iterable["ExpRange"]) -> List["ExpRange"]:
-    """Return list of ExpRange sorted by timestamp."""
+    """Return list of ExpRange sorted by (timestamp, rev)."""
 
-    def _head_timestamp(exp_range: "ExpRange") -> datetime:
+    def _head_timestamp(exp_range: "ExpRange") -> Tuple[datetime, str]:
         head_exp = first(exp_range.revs)
         if head_exp and head_exp.data and head_exp.data.timestamp:
-            return head_exp.data.timestamp
-        return datetime.fromtimestamp(0)
+            return head_exp.data.timestamp, head_exp.rev
+
+        return datetime.fromtimestamp(0), ""
 
     return sorted(exp_ranges, key=_head_timestamp, reverse=True)
```

### Comparing `dvc-3.2.1/dvc/repo/experiments/diff.py` & `dvc-3.2.2/dvc/repo/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/exceptions.py` & `dvc-3.2.2/dvc/repo/experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/executor/base.py` & `dvc-3.2.2/dvc/repo/experiments/executor/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/executor/local.py` & `dvc-3.2.2/dvc/repo/experiments/executor/local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/executor/ssh.py` & `dvc-3.2.2/dvc/repo/experiments/executor/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,16 +206,15 @@
 
     def collect_cache(
         self, repo: "Repo", exp_ref: "ExpRefInfo", run_cache: bool = True
     ):
         """Collect DVC cache."""
         from dvc.repo.experiments.pull import _pull_cache
 
-        with self.get_odb() as odb:
-            _pull_cache(repo, exp_ref, run_cache=run_cache, odb=odb)
+        _pull_cache(repo, exp_ref, run_cache=run_cache)
 
     @contextmanager
     def get_odb(self):
         from dvc.cachemgr import CacheManager, get_odb
 
         cache_path = posixpath.join(
             self._repo_abspath,
```

### Comparing `dvc-3.2.1/dvc/repo/experiments/ls.py` & `dvc-3.2.2/dvc/repo/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/pull.py` & `dvc-3.2.2/dvc/repo/experiments/pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,13 @@
 
 def _pull_cache(
     repo,
     refs: Union[ExpRefInfo, Iterable["ExpRefInfo"]],
     dvc_remote=None,
     jobs=None,
     run_cache=False,
-    odb=None,
 ):
     if isinstance(refs, ExpRefInfo):
         refs = [refs]
     revs = list(exp_commits(repo.scm, refs))
     logger.debug("dvc fetch experiment '%s'", refs)
-    repo.fetch(jobs=jobs, remote=dvc_remote, run_cache=run_cache, revs=revs, odb=odb)
+    repo.fetch(jobs=jobs, remote=dvc_remote, run_cache=run_cache, revs=revs)
```

### Comparing `dvc-3.2.1/dvc/repo/experiments/push.py` & `dvc-3.2.2/dvc/repo/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/queue/base.py` & `dvc-3.2.2/dvc/repo/experiments/queue/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/queue/celery.py` & `dvc-3.2.2/dvc/repo/experiments/queue/celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/queue/remove.py` & `dvc-3.2.2/dvc/repo/experiments/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/queue/tasks.py` & `dvc-3.2.2/dvc/repo/experiments/queue/tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/queue/tempdir.py` & `dvc-3.2.2/dvc/repo/experiments/queue/tempdir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/queue/utils.py` & `dvc-3.2.2/dvc/repo/experiments/queue/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/queue/workspace.py` & `dvc-3.2.2/dvc/repo/experiments/queue/workspace.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/refs.py` & `dvc-3.2.2/dvc/repo/experiments/refs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/remove.py` & `dvc-3.2.2/dvc/repo/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/run.py` & `dvc-3.2.2/dvc/repo/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/save.py` & `dvc-3.2.2/dvc/repo/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/serialize.py` & `dvc-3.2.2/dvc/repo/experiments/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/show.py` & `dvc-3.2.2/dvc/repo/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/stash.py` & `dvc-3.2.2/dvc/repo/experiments/stash.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/experiments/utils.py` & `dvc-3.2.2/dvc/repo/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/fetch.py` & `dvc-3.2.2/dvc/repo/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/gc.py` & `dvc-3.2.2/dvc/repo/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/get.py` & `dvc-3.2.2/dvc/repo/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/get_url.py` & `dvc-3.2.2/dvc/repo/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/graph.py` & `dvc-3.2.2/dvc/repo/graph.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/imp_url.py` & `dvc-3.2.2/dvc/repo/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/imports.py` & `dvc-3.2.2/dvc/repo/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/index.py` & `dvc-3.2.2/dvc/repo/index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/init.py` & `dvc-3.2.2/dvc/repo/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/install.py` & `dvc-3.2.2/dvc/repo/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/ls.py` & `dvc-3.2.2/dvc/repo/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/ls_url.py` & `dvc-3.2.2/dvc/repo/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/metrics/diff.py` & `dvc-3.2.2/dvc/repo/metrics/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/metrics/show.py` & `dvc-3.2.2/dvc/repo/metrics/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/move.py` & `dvc-3.2.2/dvc/repo/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/open_repo.py` & `dvc-3.2.2/dvc/repo/open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/params/diff.py` & `dvc-3.2.2/dvc/repo/params/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/params/show.py` & `dvc-3.2.2/dvc/repo/params/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/plots/__init__.py` & `dvc-3.2.2/dvc/repo/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/plots/diff.py` & `dvc-3.2.2/dvc/repo/plots/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/pull.py` & `dvc-3.2.2/dvc/repo/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/push.py` & `dvc-3.2.2/dvc/repo/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/remove.py` & `dvc-3.2.2/dvc/repo/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/reproduce.py` & `dvc-3.2.2/dvc/repo/reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/run.py` & `dvc-3.2.2/dvc/repo/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/scm_context.py` & `dvc-3.2.2/dvc/repo/scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/stage.py` & `dvc-3.2.2/dvc/repo/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/status.py` & `dvc-3.2.2/dvc/repo/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/trie.py` & `dvc-3.2.2/dvc/repo/trie.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/update.py` & `dvc-3.2.2/dvc/repo/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/repo/worktree.py` & `dvc-3.2.2/dvc/repo/worktree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/rwlock.py` & `dvc-3.2.2/dvc/rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/schema.py` & `dvc-3.2.2/dvc/schema.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/scm.py` & `dvc-3.2.2/dvc/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/__init__.py` & `dvc-3.2.2/dvc/stage/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/cache.py` & `dvc-3.2.2/dvc/stage/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/decorators.py` & `dvc-3.2.2/dvc/stage/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/exceptions.py` & `dvc-3.2.2/dvc/stage/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/imports.py` & `dvc-3.2.2/dvc/stage/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/loader.py` & `dvc-3.2.2/dvc/stage/loader.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/run.py` & `dvc-3.2.2/dvc/stage/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/serialize.py` & `dvc-3.2.2/dvc/stage/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/stage/utils.py` & `dvc-3.2.2/dvc/stage/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/README.rst` & `dvc-3.2.2/dvc/testing/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/api_tests.py` & `dvc-3.2.2/dvc/testing/api_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_checkout.py` & `dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_data_status.py` & `dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/benchmarks/cli/commands/test_plots.py` & `dvc-3.2.2/dvc/testing/benchmarks/cli/commands/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/benchmarks/cli/stories/test_modify_data.py` & `dvc-3.2.2/dvc/testing/benchmarks/cli/stories/test_modify_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/benchmarks/fixtures.py` & `dvc-3.2.2/dvc/testing/benchmarks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/benchmarks/plugin.py` & `dvc-3.2.2/dvc/testing/benchmarks/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/cloud.py` & `dvc-3.2.2/dvc/testing/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/fixtures.py` & `dvc-3.2.2/dvc/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/path_info.py` & `dvc-3.2.2/dvc/testing/path_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/plugin.py` & `dvc-3.2.2/dvc/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/remote_tests.py` & `dvc-3.2.2/dvc/testing/remote_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/tmp_dir.py` & `dvc-3.2.2/dvc/testing/tmp_dir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/testing/workspace_tests.py` & `dvc-3.2.2/dvc/testing/workspace_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/ui/__init__.py` & `dvc-3.2.2/dvc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/ui/_rich_progress.py` & `dvc-3.2.2/dvc/ui/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/ui/pager.py` & `dvc-3.2.2/dvc/ui/pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/ui/table.py` & `dvc-3.2.2/dvc/ui/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/updater.py` & `dvc-3.2.2/dvc/updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/__init__.py` & `dvc-3.2.2/dvc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/cli_parse.py` & `dvc-3.2.2/dvc/utils/cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/collections.py` & `dvc-3.2.2/dvc/utils/collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/diff.py` & `dvc-3.2.2/dvc/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/fs.py` & `dvc-3.2.2/dvc/utils/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/humanize.py` & `dvc-3.2.2/dvc/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/hydra.py` & `dvc-3.2.2/dvc/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/serialize/__init__.py` & `dvc-3.2.2/dvc/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/serialize/_common.py` & `dvc-3.2.2/dvc/utils/serialize/_common.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/serialize/_json.py` & `dvc-3.2.2/dvc/utils/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/serialize/_py.py` & `dvc-3.2.2/dvc/utils/serialize/_py.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/serialize/_toml.py` & `dvc-3.2.2/dvc/utils/serialize/_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/serialize/_yaml.py` & `dvc-3.2.2/dvc/utils/serialize/_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/strictyaml.py` & `dvc-3.2.2/dvc/utils/strictyaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/studio.py` & `dvc-3.2.2/dvc/utils/studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/table.py` & `dvc-3.2.2/dvc/utils/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc/utils/threadpool.py` & `dvc-3.2.2/dvc/utils/threadpool.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/dvc.egg-info/PKG-INFO` & `dvc-3.2.2/dvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.2.1
+Version: 3.2.2
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.2.1/dvc.egg-info/SOURCES.txt` & `dvc-3.2.2/dvc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -539,14 +539,15 @@
 tests/unit/repo/__init__.py
 tests/unit/repo/test_open_repo.py
 tests/unit/repo/test_repo.py
 tests/unit/repo/test_reproduce.py
 tests/unit/repo/test_scm_context.py
 tests/unit/repo/experiments/__init__.py
 tests/unit/repo/experiments/conftest.py
+tests/unit/repo/experiments/test_collect.py
 tests/unit/repo/experiments/test_executor_status.py
 tests/unit/repo/experiments/test_remove.py
 tests/unit/repo/experiments/test_utils.py
 tests/unit/repo/experiments/queue/__init__.py
 tests/unit/repo/experiments/queue/test_celery.py
 tests/unit/repo/experiments/queue/test_remove.py
 tests/unit/repo/plots/__init__.py
```

### Comparing `dvc-3.2.1/dvc.egg-info/requires.txt` & `dvc-3.2.2/dvc.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/pyproject.toml` & `dvc-3.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/scripts/pyinstaller/build.py` & `dvc-3.2.2/scripts/pyinstaller/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/scripts/pyinstaller/hooks/hook-dvc.py` & `dvc-3.2.2/scripts/pyinstaller/hooks/hook-dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/conftest.py` & `dvc-3.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/dir_helpers.py` & `dvc-3.2.2/tests/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/api/test_data.py` & `dvc-3.2.2/tests/func/api/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/api/test_experiments.py` & `dvc-3.2.2/tests/func/api/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/api/test_scm.py` & `dvc-3.2.2/tests/func/api/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/api/test_show.py` & `dvc-3.2.2/tests/func/api/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/artifacts/test_artifacts.py` & `dvc-3.2.2/tests/func/artifacts/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/data/db/test_index.py` & `dvc-3.2.2/tests/func/data/db/test_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/conftest.py` & `dvc-3.2.2/tests/func/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/executor/test_ssh.py` & `dvc-3.2.2/tests/func/experiments/executor/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_apply.py` & `dvc-3.2.2/tests/func/experiments/test_apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_diff.py` & `dvc-3.2.2/tests/func/experiments/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_experiments.py` & `dvc-3.2.2/tests/func/experiments/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_queue.py` & `dvc-3.2.2/tests/func/experiments/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_remote.py` & `dvc-3.2.2/tests/func/experiments/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_remove.py` & `dvc-3.2.2/tests/func/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_save.py` & `dvc-3.2.2/tests/func/experiments/test_save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_set_params.py` & `dvc-3.2.2/tests/func/experiments/test_set_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_show.py` & `dvc-3.2.2/tests/func/experiments/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_stash_exp.py` & `dvc-3.2.2/tests/func/experiments/test_stash_exp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/experiments/test_utils.py` & `dvc-3.2.2/tests/func/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/machine/conftest.py` & `dvc-3.2.2/tests/func/machine/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/machine/test_machine_config.py` & `dvc-3.2.2/tests/func/machine/test_machine_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/machine/test_machine_status.py` & `dvc-3.2.2/tests/func/machine/test_machine_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/metrics/test_diff.py` & `dvc-3.2.2/tests/func/metrics/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/metrics/test_show.py` & `dvc-3.2.2/tests/func/metrics/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/params/test_diff.py` & `dvc-3.2.2/tests/func/params/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/params/test_show.py` & `dvc-3.2.2/tests/func/params/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/parsing/__init__.py` & `dvc-3.2.2/tests/func/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/parsing/test_errors.py` & `dvc-3.2.2/tests/func/parsing/test_errors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/parsing/test_foreach.py` & `dvc-3.2.2/tests/func/parsing/test_foreach.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/parsing/test_interpolated_entry.py` & `dvc-3.2.2/tests/func/parsing/test_interpolated_entry.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/parsing/test_resolver.py` & `dvc-3.2.2/tests/func/parsing/test_resolver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/plots/test_diff.py` & `dvc-3.2.2/tests/func/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/plots/test_modify.py` & `dvc-3.2.2/tests/func/plots/test_modify.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/plots/test_show.py` & `dvc-3.2.2/tests/func/plots/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/repro/test_repro.py` & `dvc-3.2.2/tests/func/repro/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/repro/test_repro_allow_missing.py` & `dvc-3.2.2/tests/func/repro/test_repro_allow_missing.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/repro/test_repro_pull.py` & `dvc-3.2.2/tests/func/repro/test_repro_pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_add.py` & `dvc-3.2.2/tests/func/test_add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_analytics.py` & `dvc-3.2.2/tests/func/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_check_ignore.py` & `dvc-3.2.2/tests/func/test_check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_checkout.py` & `dvc-3.2.2/tests/func/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_cli.py` & `dvc-3.2.2/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_commit.py` & `dvc-3.2.2/tests/func/test_commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_config.py` & `dvc-3.2.2/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_data_cloud.py` & `dvc-3.2.2/tests/func/test_data_cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_data_status.py` & `dvc-3.2.2/tests/func/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_diff.py` & `dvc-3.2.2/tests/func/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_dvcfile.py` & `dvc-3.2.2/tests/func/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_external_repo.py` & `dvc-3.2.2/tests/func/test_external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_fs.py` & `dvc-3.2.2/tests/func/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_gc.py` & `dvc-3.2.2/tests/func/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_get.py` & `dvc-3.2.2/tests/func/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_get_url.py` & `dvc-3.2.2/tests/func/test_get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_ignore.py` & `dvc-3.2.2/tests/func/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_import.py` & `dvc-3.2.2/tests/func/test_import.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_import_url.py` & `dvc-3.2.2/tests/func/test_import_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_init.py` & `dvc-3.2.2/tests/func/test_init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_install.py` & `dvc-3.2.2/tests/func/test_install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_lock.py` & `dvc-3.2.2/tests/func/test_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_lockfile.py` & `dvc-3.2.2/tests/func/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_ls.py` & `dvc-3.2.2/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_merge_driver.py` & `dvc-3.2.2/tests/func/test_merge_driver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_move.py` & `dvc-3.2.2/tests/func/test_move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_odb.py` & `dvc-3.2.2/tests/func/test_odb.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_remote.py` & `dvc-3.2.2/tests/func/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_remove.py` & `dvc-3.2.2/tests/func/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_repo.py` & `dvc-3.2.2/tests/func/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_repo_index.py` & `dvc-3.2.2/tests/func/test_repo_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_run.py` & `dvc-3.2.2/tests/func/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_run_cache.py` & `dvc-3.2.2/tests/func/test_run_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_scm.py` & `dvc-3.2.2/tests/func/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_scm_context.py` & `dvc-3.2.2/tests/func/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_stage.py` & `dvc-3.2.2/tests/func/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_stage_load.py` & `dvc-3.2.2/tests/func/test_stage_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_state.py` & `dvc-3.2.2/tests/func/test_state.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_status.py` & `dvc-3.2.2/tests/func/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_unprotect.py` & `dvc-3.2.2/tests/func/test_unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_update.py` & `dvc-3.2.2/tests/func/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_used_objs.py` & `dvc-3.2.2/tests/func/test_used_objs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_utils.py` & `dvc-3.2.2/tests/func/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_version.py` & `dvc-3.2.2/tests/func/test_version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/test_virtual_directory.py` & `dvc-3.2.2/tests/func/test_virtual_directory.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/utils/test_hydra.py` & `dvc-3.2.2/tests/func/utils/test_hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/func/utils/test_strict_yaml.py` & `dvc-3.2.2/tests/func/utils/test_strict_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/integration/plots/conftest.py` & `dvc-3.2.2/tests/integration/plots/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/integration/plots/test_plots.py` & `dvc-3.2.2/tests/integration/plots/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/integration/plots/test_repo_plots_api.py` & `dvc-3.2.2/tests/integration/plots/test_repo_plots_api.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/integration/test_studio_live_experiments.py` & `dvc-3.2.2/tests/integration/test_studio_live_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/remotes/git_server.py` & `dvc-3.2.2/tests/remotes/git_server.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/remotes/user.key` & `dvc-3.2.2/tests/remotes/user.key`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/remotes_env.sample` & `dvc-3.2.2/tests/remotes_env.sample`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/scripts.py` & `dvc-3.2.2/tests/scripts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/cli/test_main.py` & `dvc-3.2.2/tests/unit/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/ls/test_ls.py` & `dvc-3.2.2/tests/unit/command/ls/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/ls/test_ls_colors.py` & `dvc-3.2.2/tests/unit/command/ls/test_ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_add.py` & `dvc-3.2.2/tests/unit/command/test_add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_cache.py` & `dvc-3.2.2/tests/unit/command/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_checkout.py` & `dvc-3.2.2/tests/unit/command/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_compat_flag.py` & `dvc-3.2.2/tests/unit/command/test_compat_flag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_config.py` & `dvc-3.2.2/tests/unit/command/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_dag.py` & `dvc-3.2.2/tests/unit/command/test_dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_data_status.py` & `dvc-3.2.2/tests/unit/command/test_data_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,31 +71,31 @@
     out, err = capsys.readouterr()
     assert out.rstrip() == json.dumps(omit(mocked_status, [*to_omit, "git"]))
     assert not err
 
 
 def test_no_changes_repo(dvc, scm, capsys):
     assert main(["data", "status"]) == 0
-    assert capsys.readouterr() == ("No changes.\n", "")
+    out, _ = capsys.readouterr()
+    assert out == "No changes.\n"
 
 
 def test_empty_scm_repo(tmp_dir, capsys):
     tmp_dir.init(scm=True)
     Repo.init()
 
     assert main(["data", "status"]) == 0
-    out, err = capsys.readouterr()
+    out, _ = capsys.readouterr()
     assert (
         out
         == """\
 No changes in an empty git repo.
 (there are changes not tracked by dvc, use "git status" to see)
 """
     )
-    assert not err
 
 
 @pytest.mark.parametrize(
     "args",
     [
         ("--untracked-files",),
         ("--unchanged",),
```

### Comparing `dvc-3.2.1/tests/unit/command/test_data_sync.py` & `dvc-3.2.2/tests/unit/command/test_data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_diff.py` & `dvc-3.2.2/tests/unit/command/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_experiments.py` & `dvc-3.2.2/tests/unit/command/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_gc.py` & `dvc-3.2.2/tests/unit/command/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_get.py` & `dvc-3.2.2/tests/unit/command/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_git_hook.py` & `dvc-3.2.2/tests/unit/command/test_git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_imp.py` & `dvc-3.2.2/tests/unit/command/test_imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_imp_url.py` & `dvc-3.2.2/tests/unit/command/test_imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_ls_url.py` & `dvc-3.2.2/tests/unit/command/test_ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_machine.py` & `dvc-3.2.2/tests/unit/command/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_metrics.py` & `dvc-3.2.2/tests/unit/command/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_params.py` & `dvc-3.2.2/tests/unit/command/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_plots.py` & `dvc-3.2.2/tests/unit/command/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_queue.py` & `dvc-3.2.2/tests/unit/command/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_repro.py` & `dvc-3.2.2/tests/unit/command/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_stage.py` & `dvc-3.2.2/tests/unit/command/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_status.py` & `dvc-3.2.2/tests/unit/command/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/command/test_update.py` & `dvc-3.2.2/tests/unit/command/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/data/db/test_local.py` & `dvc-3.2.2/tests/unit/data/db/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/dependency/test_params.py` & `dvc-3.2.2/tests/unit/dependency/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_azure.py` & `dvc-3.2.2/tests/unit/fs/test_azure.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_data.py` & `dvc-3.2.2/tests/unit/fs/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_dvc.py` & `dvc-3.2.2/tests/unit/fs/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_dvc_info.py` & `dvc-3.2.2/tests/unit/fs/test_dvc_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_fs.py` & `dvc-3.2.2/tests/unit/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_path.py` & `dvc-3.2.2/tests/unit/fs/test_path.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_s3.py` & `dvc-3.2.2/tests/unit/fs/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/fs/test_tree.py` & `dvc-3.2.2/tests/unit/fs/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/machine/test_machine.py` & `dvc-3.2.2/tests/unit/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/output/test_load.py` & `dvc-3.2.2/tests/unit/output/test_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/output/test_local.py` & `dvc-3.2.2/tests/unit/output/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/output/test_output.py` & `dvc-3.2.2/tests/unit/output/test_output.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/remote/test_oss.py` & `dvc-3.2.2/tests/unit/remote/test_oss.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/remote/test_remote.py` & `dvc-3.2.2/tests/unit/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/remote/test_webdav.py` & `dvc-3.2.2/tests/unit/remote/test_webdav.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/remote/test_webhdfs.py` & `dvc-3.2.2/tests/unit/remote/test_webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/render/test_convert.py` & `dvc-3.2.2/tests/unit/render/test_convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/render/test_image_converter.py` & `dvc-3.2.2/tests/unit/render/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/render/test_match.py` & `dvc-3.2.2/tests/unit/render/test_match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/render/test_vega_converter.py` & `dvc-3.2.2/tests/unit/render/test_vega_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/experiments/conftest.py` & `dvc-3.2.2/tests/unit/repo/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/experiments/queue/test_celery.py` & `dvc-3.2.2/tests/unit/repo/experiments/queue/test_celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/experiments/queue/test_remove.py` & `dvc-3.2.2/tests/unit/repo/experiments/queue/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/experiments/test_executor_status.py` & `dvc-3.2.2/tests/unit/repo/experiments/test_executor_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/experiments/test_remove.py` & `dvc-3.2.2/tests/unit/repo/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/experiments/test_utils.py` & `dvc-3.2.2/tests/unit/repo/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/plots/test_diff.py` & `dvc-3.2.2/tests/unit/repo/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/test_open_repo.py` & `dvc-3.2.2/tests/unit/repo/test_open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/test_repo.py` & `dvc-3.2.2/tests/unit/repo/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/test_reproduce.py` & `dvc-3.2.2/tests/unit/repo/test_reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/repo/test_scm_context.py` & `dvc-3.2.2/tests/unit/repo/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/scm/test_scm.py` & `dvc-3.2.2/tests/unit/scm/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/stage/test_cache.py` & `dvc-3.2.2/tests/unit/stage/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/stage/test_loader_pipeline_file.py` & `dvc-3.2.2/tests/unit/stage/test_loader_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/stage/test_run.py` & `dvc-3.2.2/tests/unit/stage/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/stage/test_serialize_pipeline_file.py` & `dvc-3.2.2/tests/unit/stage/test_serialize_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/stage/test_serialize_pipeline_lock.py` & `dvc-3.2.2/tests/unit/stage/test_serialize_pipeline_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/stage/test_stage.py` & `dvc-3.2.2/tests/unit/stage/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/stage/test_utils.py` & `dvc-3.2.2/tests/unit/stage/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_analytics.py` & `dvc-3.2.2/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_collect.py` & `dvc-3.2.2/tests/unit/test_collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_compare.py` & `dvc-3.2.2/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_config.py` & `dvc-3.2.2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_context.py` & `dvc-3.2.2/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_daemon.py` & `dvc-3.2.2/tests/unit/test_daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_dvcfile.py` & `dvc-3.2.2/tests/unit/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_ignore.py` & `dvc-3.2.2/tests/unit/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_imports.py` & `dvc-3.2.2/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_info.py` & `dvc-3.2.2/tests/unit/test_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_interpolate.py` & `dvc-3.2.2/tests/unit/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_lockfile.py` & `dvc-3.2.2/tests/unit/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_logger.py` & `dvc-3.2.2/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_metrics.py` & `dvc-3.2.2/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_params.py` & `dvc-3.2.2/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_pathspec_math.py` & `dvc-3.2.2/tests/unit/test_pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_progress.py` & `dvc-3.2.2/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_rwlock.py` & `dvc-3.2.2/tests/unit/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_tabular_data.py` & `dvc-3.2.2/tests/unit/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/test_updater.py` & `dvc-3.2.2/tests/unit/test_updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/ui/test_console.py` & `dvc-3.2.2/tests/unit/ui/test_console.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/ui/test_pager.py` & `dvc-3.2.2/tests/unit/ui/test_pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/ui/test_table.py` & `dvc-3.2.2/tests/unit/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/serialize/test_python.py` & `dvc-3.2.2/tests/unit/utils/serialize/test_python.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/serialize/test_toml.py` & `dvc-3.2.2/tests/unit/utils/serialize/test_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/serialize/test_yaml.py` & `dvc-3.2.2/tests/unit/utils/serialize/test_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/test_cli_parse.py` & `dvc-3.2.2/tests/unit/utils/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/test_collections.py` & `dvc-3.2.2/tests/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/test_executors.py` & `dvc-3.2.2/tests/unit/utils/test_executors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/test_fs.py` & `dvc-3.2.2/tests/unit/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/test_humanize.py` & `dvc-3.2.2/tests/unit/utils/test_humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/test_studio.py` & `dvc-3.2.2/tests/unit/utils/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/unit/utils/test_utils.py` & `dvc-3.2.2/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/utils/__init__.py` & `dvc-3.2.2/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.2.1/tests/utils/asserts.py` & `dvc-3.2.2/tests/utils/asserts.py`

 * *Files identical despite different names*

