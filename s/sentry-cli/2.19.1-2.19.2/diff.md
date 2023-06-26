# Comparing `tmp/sentry_cli-2.19.1.tar.gz` & `tmp/sentry_cli-2.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.19.1.tar", last modified: Thu Jun 15 07:53:02 2023, max compression
+gzip compressed data, was "sentry_cli-2.19.2.tar", last modified: Mon Jun 26 09:06:10 2023, max compression
```

## Comparing `sentry_cli-2.19.1.tar` & `sentry_cli-2.19.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/
--rw-r--r--   0 runner    (1001) docker     (123)    80839 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.038466 sentry_cli-2.19.1/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.038466 sentry_cli-2.19.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87192 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    38886 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.795359 sentry_cli-2.19.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    80979 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-26 09:06:10.795359 sentry_cli-2.19.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.779359 sentry_cli-2.19.2/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-26 09:06:10.000000 sentry_cli-2.19.2/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-26 09:06:10.000000 sentry_cli-2.19.2/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:06:10.000000 sentry_cli-2.19.2/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:06:10.000000 sentry_cli-2.19.2/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 09:06:10.795359 sentry_cli-2.19.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.783359 sentry_cli-2.19.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87192 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.783359 sentry_cli-2.19.2/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.783359 sentry_cli-2.19.2/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.783359 sentry_cli-2.19.2/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.783359 sentry_cli-2.19.2/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.787359 sentry_cli-2.19.2/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.791359 sentry_cli-2.19.2/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.791359 sentry_cli-2.19.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.795359 sentry_cli-2.19.2/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:06:10.795359 sentry_cli-2.19.2/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    38886 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-06-26 09:05:55.000000 sentry_cli-2.19.2/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.19.1/Cargo.lock` & `sentry_cli-2.19.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -564,15 +564,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c26bbb078acf09bc1ecda02d4223f03bdd28bd4874edcb0379138efc499ce971"
@@ -581,15 +581,15 @@
 name = "cxxbridge-macro"
 version = "1.0.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "357f40d1f06a24b60ae1fe122542c1fb05d28d32acb2aed064e84bc2ad1e252e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "data-encoding"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d8666cb01533c39dde32bcbab8e227b4ed6679b2c925eba05feabea39508fb"
@@ -699,17 +699,17 @@
 checksum = "3efd4742acf458718a6456e0adf0b4d734d6b783e452bbf1ac36bf31f4085cb3"
 dependencies = [
  "string_cache",
 ]
 
 [[package]]
 name = "elsa"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b4b5d23ed6b6948d68240aafa4ac98e568c9a020efd9d4201a6288bc3006e09"
+checksum = "b5e0aca8dce8856e420195bd13b6a64de3334235ccc9214e824b86b12bf26283"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
@@ -893,17 +893,17 @@
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.27.1"
+version = "0.27.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "221996f774192f0f718773def8201c4ae31f02616a54ccfc2d358bb0e5cefdec"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
 dependencies = [
  "fallible-iterator",
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "git2"
@@ -935,17 +935,17 @@
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
 name = "goblin"
-version = "0.6.0"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572564d6cba7d09775202c8e7eebc4d534d5ae36578ab402fb21e182a0ac9505"
+checksum = "0d6b4de4a8eb6c46a8c77e1d3be942cb9a8bf073c22374578e5ba4b08ed0ff68"
 dependencies = [
  "log",
  "plain",
  "scroll 0.11.0",
 ]
 
 [[package]]
@@ -1229,20 +1229,14 @@
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
-name = "lazycell"
-version = "1.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
-
-[[package]]
 name = "leb128"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "884e2677b40cc8c339eaefcb701c32ef1fd2493d71118dc0ca4b6a736c93bd67"
 
 [[package]]
 name = "libc"
@@ -1348,17 +1342,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
-version = "0.5.8"
+version = "0.5.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b182332558b18d807c4ce1ca8ca983b34c3ee32765e47b3f0f69b90355cc1dc"
+checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.7.1"
@@ -1497,17 +1491,17 @@
 checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
@@ -1707,15 +1701,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b27bd18aa01d91c8ed2b61ea23406a676b42d82609c6e2581fba42f0c15f17f"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "pest_meta"
 version = "2.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f02b677c1859756359fc9983c2e56a0237f18624a3789528804406b7e915e5d"
@@ -1810,17 +1804,17 @@
  "lazy_static",
  "term",
  "unicode-width",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.50"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proguard"
 version = "5.0.0"
@@ -1838,17 +1832,17 @@
 checksum = "7f50b1c63b38611e7d4d7f68b82d3ad0cc71a2ad2e7f61fc10f1328d917c93cd"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "r2d2"
 version = "0.8.10"
@@ -2118,26 +2112,26 @@
 name = "scroll_derive"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aaaae8f38bb311444cfb7f1979af0bc9240d95795f75f9ceddf6a59b79ceffa0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "scroll_derive"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdbda6ac5cd1321e724fa9cee216f3a61885889b896f073b8f82322789c5250e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "semver"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d7eb9ef2c18661902cc47e535f9bc51b78acd254da71d375c2f6720d9a40403"
@@ -2191,15 +2185,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.19.1"
+version = "2.19.2"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
@@ -2306,37 +2300,37 @@
  "time 0.3.17",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.93"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa 1.0.5",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2518,56 +2512,56 @@
 name = "subtle"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
 
 [[package]]
 name = "symbolic"
-version = "12.0.0"
+version = "12.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c8842a52dc500c0d997b525747ea4514b1bdf7d652e0d1287d0aef9111d2c02"
+checksum = "0d311bfa722c01294e838091c455ed4e63c96ea7b8fb65b7fd7acdc72a4b0309"
 dependencies = [
  "symbolic-common",
  "symbolic-debuginfo",
  "symbolic-il2cpp",
  "symbolic-symcache",
 ]
 
 [[package]]
 name = "symbolic-common"
-version = "12.0.0"
+version = "12.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87abaf26f8fe1ffbcabcdcb5c090cba8da4a82803456bb05b5663fcbca2cd877"
+checksum = "0eb6682826c7186b16c5c0ed2a68f419609f8af62f070c688871caae4911432d"
 dependencies = [
  "debugid",
  "memmap2",
  "serde",
  "stable_deref_trait",
  "uuid",
 ]
 
 [[package]]
 name = "symbolic-debuginfo"
-version = "12.0.0"
+version = "12.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a3e3d193c41fa790c8d913ac642bbfcb0c4e356a95ebf4f1baa8be2a8474c82"
+checksum = "222363f4ca5fb00cdd4915afba4a6aa18549d3438b27c048db2c41f0ea7a1e58"
 dependencies = [
  "bitvec",
  "debugid",
  "dmsort",
  "elementtree",
  "elsa",
  "fallible-iterator",
  "flate2",
  "gimli",
  "goblin",
  "lazy_static",
- "lazycell",
  "nom",
  "nom-supreme",
+ "once_cell",
  "parking_lot",
  "pdb-addr2line",
  "regex",
  "scroll 0.11.0",
  "serde",
  "serde_json",
  "smallvec",
@@ -2576,44 +2570,44 @@
  "thiserror",
  "wasmparser",
  "zip",
 ]
 
 [[package]]
 name = "symbolic-il2cpp"
-version = "12.0.0"
+version = "12.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44853ca2c7f9da1960178bccef8ea16593b5d2f0a8a5c3ddc36eadae096b82fd"
+checksum = "ffa4db538300bbac1e849bf0ffb3d8f555e76b3a55a7fb88e840832b03e75d8e"
 dependencies = [
  "indexmap",
  "serde_json",
  "symbolic-common",
  "symbolic-debuginfo",
 ]
 
 [[package]]
 name = "symbolic-ppdb"
-version = "12.0.0"
+version = "12.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5660b66c748cdddb30e12e3748b5241a72e9a19b555396b3555042b5f31ca27b"
+checksum = "1e3c9b6cc654de90c05d841af02f3dd37415278538fa23534cbcb58a1a74ae8b"
 dependencies = [
  "flate2",
  "indexmap",
  "serde_json",
  "symbolic-common",
  "thiserror",
  "uuid",
  "watto",
 ]
 
 [[package]]
 name = "symbolic-symcache"
-version = "12.0.0"
+version = "12.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4805e6fddf325b9770a089b59bd3d523fbca0ca036525394807eb56d77e645c8"
+checksum = "90eb533854b83630874a393c2e2048a5f9fe0b38ce6d000afe7b58f0a28cc511"
 dependencies = [
  "indexmap",
  "symbolic-common",
  "symbolic-debuginfo",
  "symbolic-il2cpp",
  "thiserror",
  "tracing",
@@ -2628,14 +2622,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "tempfile"
@@ -2679,30 +2684,30 @@
 dependencies = [
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
@@ -2801,15 +2806,15 @@
 name = "tracing-attributes"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
@@ -2990,15 +2995,15 @@
 checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3012,30 +3017,30 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
 
 [[package]]
 name = "wasmparser"
-version = "0.95.0"
+version = "0.102.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2ea896273ea99b15132414be1da01ab0d8836415083298ecaffbe308eaac87a"
+checksum = "48134de3d7598219ab9eaf6b91b15d8e50d31da76b8519fe4ecfcec2cf35104b"
 dependencies = [
  "indexmap",
  "url",
 ]
 
 [[package]]
 name = "watto"
```

### Comparing `sentry_cli-2.19.1/Cargo.toml` & `sentry_cli-2.19.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.19.1"
+version = "2.19.2"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
@@ -62,15 +62,15 @@
   "curl",
   "contexts",
 ] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 sha1_smol = { version = "1.0.0", features = ["serde"] }
 sourcemap = { version = "6.2.3", features = ["ram_bundle"] }
-symbolic = { version = "12.0.0", features = ["debuginfo-serde", "il2cpp"] }
+symbolic = { version = "12.1.5", features = ["debuginfo-serde", "il2cpp"] }
 thiserror = "1.0.38"
 url = "2.3.1"
 username = "0.2.0"
 uuid = { version = "1.3.0", features = ["v4", "serde"] }
 walkdir = "2.3.2"
 which = "4.4.0"
 zip = "0.6.4"
```

### Comparing `sentry_cli-2.19.1/LICENSE` & `sentry_cli-2.19.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/PKG-INFO` & `sentry_cli-2.19.2/sentry_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sentry_cli
-Version: 2.19.1
+Name: sentry-cli
+Version: 2.19.2
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.19.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.19.2 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.19.1/README.md` & `sentry_cli-2.19.2/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/build.rs` & `sentry_cli-2.19.2/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.19.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sentry-cli
-Version: 2.19.1
+Name: sentry_cli
+Version: 2.19.2
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.19.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.19.2 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.19.1/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.19.2/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/setup.cfg` & `sentry_cli-2.19.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/setup.py` & `sentry_cli-2.19.2/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/api.rs` & `sentry_cli-2.19.2/src/api.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/bashsupport.sh` & `sentry_cli-2.19.2/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/bash_hook.rs` & `sentry_cli-2.19.2/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.19.2/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.19.2/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/debug_files/check.rs` & `sentry_cli-2.19.2/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/debug_files/find.rs` & `sentry_cli-2.19.2/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/debug_files/mod.rs` & `sentry_cli-2.19.2/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.19.2/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/debug_files/upload.rs` & `sentry_cli-2.19.2/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/deploys/list.rs` & `sentry_cli-2.19.2/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/deploys/mod.rs` & `sentry_cli-2.19.2/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/deploys/new.rs` & `sentry_cli-2.19.2/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/events/list.rs` & `sentry_cli-2.19.2/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/events/mod.rs` & `sentry_cli-2.19.2/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/files/delete.rs` & `sentry_cli-2.19.2/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/files/list.rs` & `sentry_cli-2.19.2/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/files/mod.rs` & `sentry_cli-2.19.2/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/files/upload.rs` & `sentry_cli-2.19.2/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/info.rs` & `sentry_cli-2.19.2/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/issues/mod.rs` & `sentry_cli-2.19.2/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/issues/mute.rs` & `sentry_cli-2.19.2/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/issues/resolve.rs` & `sentry_cli-2.19.2/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/issues/unresolve.rs` & `sentry_cli-2.19.2/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/login.rs` & `sentry_cli-2.19.2/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/mod.rs` & `sentry_cli-2.19.2/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/monitors/list.rs` & `sentry_cli-2.19.2/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/monitors/mod.rs` & `sentry_cli-2.19.2/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/monitors/run.rs` & `sentry_cli-2.19.2/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/organizations/list.rs` & `sentry_cli-2.19.2/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/organizations/mod.rs` & `sentry_cli-2.19.2/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/projects/list.rs` & `sentry_cli-2.19.2/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/projects/mod.rs` & `sentry_cli-2.19.2/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/react_native/appcenter.rs` & `sentry_cli-2.19.2/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/react_native/gradle.rs` & `sentry_cli-2.19.2/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/react_native/mod.rs` & `sentry_cli-2.19.2/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/react_native/xcode.rs` & `sentry_cli-2.19.2/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/archive.rs` & `sentry_cli-2.19.2/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/delete.rs` & `sentry_cli-2.19.2/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/finalize.rs` & `sentry_cli-2.19.2/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/info.rs` & `sentry_cli-2.19.2/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/list.rs` & `sentry_cli-2.19.2/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/mod.rs` & `sentry_cli-2.19.2/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/new.rs` & `sentry_cli-2.19.2/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/restore.rs` & `sentry_cli-2.19.2/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/releases/set_commits.rs` & `sentry_cli-2.19.2/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/repos/list.rs` & `sentry_cli-2.19.2/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/repos/mod.rs` & `sentry_cli-2.19.2/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/send_envelope.rs` & `sentry_cli-2.19.2/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/send_event.rs` & `sentry_cli-2.19.2/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.19.2/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.19.2/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.19.2/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.19.2/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.19.2/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/uninstall.rs` & `sentry_cli-2.19.2/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/update.rs` & `sentry_cli-2.19.2/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/commands/upload_proguard.rs` & `sentry_cli-2.19.2/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/config.rs` & `sentry_cli-2.19.2/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/constants.rs` & `sentry_cli-2.19.2/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/android.rs` & `sentry_cli-2.19.2/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/appcenter.rs` & `sentry_cli-2.19.2/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/args.rs` & `sentry_cli-2.19.2/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/chunks.rs` & `sentry_cli-2.19.2/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/codepush.rs` & `sentry_cli-2.19.2/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/cordova.rs` & `sentry_cli-2.19.2/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/dif.rs` & `sentry_cli-2.19.2/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/dif_upload.rs` & `sentry_cli-2.19.2/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/enc.rs` & `sentry_cli-2.19.2/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/event.rs` & `sentry_cli-2.19.2/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/file_search.rs` & `sentry_cli-2.19.2/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/file_upload.rs` & `sentry_cli-2.19.2/src/utils/file_upload.rs`

 * *Files 10% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         )?;
     } else {
         bail!("This version of Sentry does not support artifact bundles. A release slug is required (provide with --release)");
     }
     Ok(())
 }
 
+#[derive(Debug, Clone)]
 pub struct UploadContext<'a> {
     pub org: &'a str,
     pub project: Option<&'a str>,
     pub release: Option<&'a str>,
     pub dist: Option<&'a str>,
     pub note: Option<&'a str>,
     pub wait: bool,
@@ -269,75 +270,48 @@
     pb.finish_and_clear();
 
     print_upload_context_details(context);
 
     Ok(())
 }
 
-fn upload_files_chunked(
+fn poll_assemble(
+    checksum: Digest,
+    chunks: &[Digest],
     context: &UploadContext,
-    files: &SourceFiles,
     options: &ChunkUploadOptions,
 ) -> Result<()> {
-    let archive = build_artifact_bundle(context, files, None)?;
-
-    let progress_style =
-        ProgressStyle::default_spinner().template("{spinner} Optimizing bundle for upload...");
-
-    let pb = ProgressBar::new_spinner();
-    pb.enable_steady_tick(100);
-    pb.set_style(progress_style);
-
-    let view = ByteView::open(archive.path())?;
-    let (checksum, checksums) = get_sha1_checksums(&view, options.chunk_size)?;
-    let chunks = view
-        .chunks(options.chunk_size as usize)
-        .zip(checksums.iter())
-        .map(|(data, checksum)| Chunk((*checksum, data)))
-        .collect::<Vec<_>>();
-
-    pb.finish_with_duration("Optimizing");
-
-    let progress_style = ProgressStyle::default_bar().template(&format!(
-        "{} Uploading files...\
-       \n{{wide_bar}}  {{bytes}}/{{total_bytes}} ({{eta}})",
-        style(">").dim(),
-    ));
-
-    upload_chunks(&chunks, options, progress_style)?;
-    println!("{} Uploaded files to Sentry", style(">").dim());
-
     let progress_style = ProgressStyle::default_spinner().template("{spinner} Processing files...");
 
     let pb = ProgressBar::new_spinner();
     pb.enable_steady_tick(100);
     pb.set_style(progress_style);
 
     let assemble_start = Instant::now();
     let max_wait = match options.max_wait {
         0 => DEFAULT_MAX_WAIT,
         secs => Duration::from_secs(secs),
     };
 
     let api = Api::current();
+    let use_artifact_bundle =
+        options.supports(ChunkUploadCapability::ArtifactBundles) && context.project.is_some();
     let response = loop {
         // prefer standalone artifact bundle upload over legacy release based upload
-        let response = if options.supports(ChunkUploadCapability::ArtifactBundles)
-            && context.project.is_some()
-        {
+        let response = if use_artifact_bundle {
             api.assemble_artifact_bundle(
                 context.org,
                 vec![context.project.unwrap().to_string()],
                 checksum,
-                &checksums,
+                chunks,
                 context.release,
                 context.dist,
             )?
         } else {
-            api.assemble_release_artifacts(context.org, context.release()?, checksum, &checksums)?
+            api.assemble_release_artifacts(context.org, context.release()?, checksum, chunks)?
         };
 
         // Poll until there is a response, unless the user has specified to skip polling. In
         // that case, we return the potentially partial response from the server. This might
         // still contain a cached error.
         if !context.wait || response.state.is_finished() {
             break response;
@@ -371,14 +345,74 @@
     }
 
     print_upload_context_details(context);
 
     Ok(())
 }
 
+fn upload_files_chunked(
+    context: &UploadContext,
+    files: &SourceFiles,
+    options: &ChunkUploadOptions,
+) -> Result<()> {
+    let archive = build_artifact_bundle(context, files, None)?;
+
+    let progress_style =
+        ProgressStyle::default_spinner().template("{spinner} Optimizing bundle for upload...");
+
+    let pb = ProgressBar::new_spinner();
+    pb.enable_steady_tick(100);
+    pb.set_style(progress_style);
+
+    let view = ByteView::open(archive.path())?;
+    let (checksum, checksums) = get_sha1_checksums(&view, options.chunk_size)?;
+    let mut chunks = view
+        .chunks(options.chunk_size as usize)
+        .zip(checksums.iter())
+        .map(|(data, checksum)| Chunk((*checksum, data)))
+        .collect::<Vec<_>>();
+
+    pb.finish_with_duration("Optimizing");
+
+    let progress_style = ProgressStyle::default_bar().template(&format!(
+        "{} Uploading files...\
+       \n{{wide_bar}}  {{bytes}}/{{total_bytes}} ({{eta}})",
+        style(">").dim(),
+    ));
+
+    // Filter out chunks that are already on the server. This only matters if we're in the
+    // `assemble_artifact_bundle` case; `assemble_release_artifacts` always returns `missing_chunks: []`,
+    // so there's no point querying the endpoint.
+    if options.supports(ChunkUploadCapability::ArtifactBundles) && context.project.is_some() {
+        let api = Api::current();
+        let response = api.assemble_artifact_bundle(
+            context.org,
+            vec![context.project.unwrap().to_string()],
+            checksum,
+            &checksums,
+            context.release,
+            context.dist,
+        )?;
+        chunks.retain(|Chunk((digest, _))| response.missing_chunks.contains(digest));
+    };
+
+    upload_chunks(&chunks, options, progress_style)?;
+
+    if !chunks.is_empty() {
+        println!("{} Uploaded files to Sentry", style(">").dim());
+        poll_assemble(checksum, &checksums, context, options)
+    } else {
+        println!(
+            "{} Nothing to upload, all files are on the server",
+            style(">").dim()
+        );
+        Ok(())
+    }
+}
+
 fn build_debug_id(files: &SourceFiles) -> DebugId {
     let mut sorted_files = Vec::from_iter(files);
     sorted_files.sort_by_key(|x| x.0);
 
     let mut hash = sha1_smol::Sha1::new();
     for (path, source_file) in sorted_files {
         hash.update(path.as_bytes());
@@ -432,15 +466,18 @@
     if let Some(release) = context.release {
         bundle.set_attribute("release".to_owned(), release.to_owned());
     }
     if let Some(dist) = context.dist {
         bundle.set_attribute("dist".to_owned(), dist.to_owned());
     }
 
-    for file in files.values() {
+    let mut files_sorted = files.values().collect::<Vec<_>>();
+    files_sorted.sort_by_key(|file| &file.url[..]);
+
+    for file in files_sorted {
         pb.inc(1);
         pb.set_message(&file.url);
 
         let mut info = SourceFileInfo::new();
         info.set_ty(file.ty);
         info.set_url(file.url.clone());
         for (k, v) in &file.headers {
@@ -526,31 +563,77 @@
     println!(
         "{} {}",
         style("> Upload type:").dim(),
         style(upload_type).yellow()
     );
 }
 
-#[test]
-fn test_url_to_bundle_path() {
-    assert_eq!(url_to_bundle_path("~/bar").unwrap(), "_/_/bar");
-    assert_eq!(url_to_bundle_path("~/foo/bar").unwrap(), "_/_/foo/bar");
-    assert_eq!(
-        url_to_bundle_path("~/dist/js/bundle.js.map").unwrap(),
-        "_/_/dist/js/bundle.js.map"
-    );
-    assert_eq!(
-        url_to_bundle_path("~/babel.config.js").unwrap(),
-        "_/_/babel.config.js"
-    );
+#[cfg(test)]
+mod tests {
+    use sha1_smol::Sha1;
+
+    use super::*;
+
+    #[test]
+    fn test_url_to_bundle_path() {
+        assert_eq!(url_to_bundle_path("~/bar").unwrap(), "_/_/bar");
+        assert_eq!(url_to_bundle_path("~/foo/bar").unwrap(), "_/_/foo/bar");
+        assert_eq!(
+            url_to_bundle_path("~/dist/js/bundle.js.map").unwrap(),
+            "_/_/dist/js/bundle.js.map"
+        );
+        assert_eq!(
+            url_to_bundle_path("~/babel.config.js").unwrap(),
+            "_/_/babel.config.js"
+        );
+
+        assert_eq!(url_to_bundle_path("~/#/bar").unwrap(), "_/_/#/bar");
+        assert_eq!(url_to_bundle_path("~/foo/#/bar").unwrap(), "_/_/foo/#/bar");
+        assert_eq!(
+            url_to_bundle_path("~/dist/#js/bundle.js.map").unwrap(),
+            "_/_/dist/#js/bundle.js.map"
+        );
+        assert_eq!(
+            url_to_bundle_path("~/#foo/babel.config.js").unwrap(),
+            "_/_/#foo/babel.config.js"
+        );
+    }
+
+    #[test]
+    fn build_artifact_bundle_deterministic() {
+        let context = UploadContext {
+            org: "wat-org",
+            project: Some("wat-project"),
+            release: None,
+            dist: None,
+            note: None,
+            wait: false,
+            dedupe: true,
+            chunk_upload_options: None,
+        };
 
-    assert_eq!(url_to_bundle_path("~/#/bar").unwrap(), "_/_/#/bar");
-    assert_eq!(url_to_bundle_path("~/foo/#/bar").unwrap(), "_/_/foo/#/bar");
-    assert_eq!(
-        url_to_bundle_path("~/dist/#js/bundle.js.map").unwrap(),
-        "_/_/dist/#js/bundle.js.map"
-    );
-    assert_eq!(
-        url_to_bundle_path("~/#foo/babel.config.js").unwrap(),
-        "_/_/#foo/babel.config.js"
-    );
+        let source_files = ["bundle.min.js.map", "vendor.min.js.map"]
+            .into_iter()
+            .map(|name| {
+                let file = SourceFile {
+                    url: format!("~/{name}"),
+                    path: format!("tests/integration/_fixtures/{name}").into(),
+                    contents: std::fs::read(format!("tests/integration/_fixtures/{name}")).unwrap(),
+                    ty: SourceFileType::SourceMap,
+                    headers: Default::default(),
+                    messages: Default::default(),
+                    already_uploaded: false,
+                };
+                (format!("~/{name}"), file)
+            })
+            .collect();
+
+        let file = build_artifact_bundle(&context, &source_files, None).unwrap();
+
+        let buf = std::fs::read(file.path()).unwrap();
+        let hash = Sha1::from(buf);
+        assert_eq!(
+            hash.digest().to_string(),
+            "3f1ae634a707ec4bc01cf227589e24e4deac4a19"
+        );
+    }
 }
```

### Comparing `sentry_cli-2.19.1/src/utils/formatting.rs` & `sentry_cli-2.19.2/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/fs.rs` & `sentry_cli-2.19.2/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/http.rs` & `sentry_cli-2.19.2/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/logging.rs` & `sentry_cli-2.19.2/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/progress.rs` & `sentry_cli-2.19.2/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/releases.rs` & `sentry_cli-2.19.2/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/retry.rs` & `sentry_cli-2.19.2/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.19.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.19.2/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/sourcemaps.rs` & `sentry_cli-2.19.2/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/system.rs` & `sentry_cli-2.19.2/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/ui.rs` & `sentry_cli-2.19.2/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/update.rs` & `sentry_cli-2.19.2/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/vcs.rs` & `sentry_cli-2.19.2/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.1/src/utils/xcode.rs` & `sentry_cli-2.19.2/src/utils/xcode.rs`

 * *Files identical despite different names*

