# Comparing `tmp/xklb-2.1.8.tar.gz` & `tmp/xklb-2.1.9.tar.gz`

## Comparing `xklb-2.1.8.tar` & `xklb-2.1.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.8/.gitattributes
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xklb-2.1.8/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.8/Windows.md
--rw-r--r--   0        0        0   490400 2020-02-02 00:00:00.000000 xklb-2.1.8/pdm.lock
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.8/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/books.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/consts.py
--rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/dl_config.py
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/gui.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/hn_extract.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/lb.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/media.py
--rw-r--r--   0        0        0    25566 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/play_actions.py
--rw-r--r--   0        0        0    36224 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/praw_extract.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/subtitle.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tube_backend.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tube_extract.py
--rw-r--r--   0        0        0    83354 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/usage.py
--rw-r--r--   0        0        0    41329 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.8/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.8/LICENSE
--rw-r--r--   0        0        0    94114 2020-02-02 00:00:00.000000 xklb-2.1.8/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    97740 2020-02-02 00:00:00.000000 xklb-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.9/.gitattributes
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xklb-2.1.9/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.9/Windows.md
+-rw-r--r--   0        0        0   490400 2020-02-02 00:00:00.000000 xklb-2.1.9/pdm.lock
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.9/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/books.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/consts.py
+-rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/dl_config.py
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/lb.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/media.py
+-rw-r--r--   0        0        0    25566 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/play_actions.py
+-rw-r--r--   0        0        0    36352 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/subtitle.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tube_extract.py
+-rw-r--r--   0        0        0    83354 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/usage.py
+-rw-r--r--   0        0        0    41329 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.9/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.9/LICENSE
+-rw-r--r--   0        0        0    94114 2020-02-02 00:00:00.000000 xklb-2.1.9/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0    97740 2020-02-02 00:00:00.000000 xklb-2.1.9/PKG-INFO
```

### Comparing `xklb-2.1.8/TODO` & `xklb-2.1.9/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/Windows.md` & `xklb-2.1.9/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/pdm.lock` & `xklb-2.1.9/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/readme.py` & `xklb-2.1.9/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.1.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/.github/workflows/push.yaml` & `xklb-2.1.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/av.py` & `xklb-2.1.9/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/books.py` & `xklb-2.1.9/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/consts.py` & `xklb-2.1.9/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/db.py` & `xklb-2.1.9/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/dl_config.py` & `xklb-2.1.9/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/dl_extract.py` & `xklb-2.1.9/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/fs_extract.py` & `xklb-2.1.9/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/gdl_backend.py` & `xklb-2.1.9/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/gdl_extract.py` & `xklb-2.1.9/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/gui.py` & `xklb-2.1.9/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/history.py` & `xklb-2.1.9/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/hn_extract.py` & `xklb-2.1.9/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/lb.py` & `xklb-2.1.9/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/media.py` & `xklb-2.1.9/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/play_actions.py` & `xklb-2.1.9/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/player.py` & `xklb-2.1.9/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,17 +410,18 @@
                 FROM media m
                 LEFT JOIN history h on h.media_id = m.id
                 GROUP BY m.id, m.path
             )
             SELECT
                 {args.select_sql}
                 , play_count
-            FROM {'m' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table} AS m
+            FROM m
             WHERE 1=1
                 and path like :candidate
+                {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else f'and m.id in (select id from {args.table})'}
                 {filter_args_sql(args, m_columns)}
                 {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
                 {"and path not in ({})".format(",".join([f":ignore_path{i}" for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
             ORDER BY play_count, path
             LIMIT 1000
             """
 
@@ -471,17 +472,18 @@
             FROM media m
             LEFT JOIN history h on h.media_id = m.id
             GROUP BY m.id, m.path
         )
         SELECT
             {args.select_sql}, rank
             , play_count
-        FROM {args.table} m
+        FROM m
         WHERE 1=1
             and path != :path
+            and m.id in (select id from {args.table})
             {filter_args_sql(args, m_columns)}
             {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
         ORDER BY play_count
             , m.path like "http%"
             , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank), {args.sort}'}
             , path
         {"LIMIT " + str(args.limit - 1) if args.limit else ""} {args.offset_sql}
@@ -523,16 +525,17 @@
             FROM media m
             LEFT JOIN history h on h.media_id = m.id
             GROUP BY m.id, m.path
         )
         SELECT
             {args.select_sql}
             , play_count
-        FROM {args.table} m
+        FROM m
         WHERE 1=1
+            and m.id in (select id from {args.table})
             {filter_args_sql(args, m_columns)}
             {filter_paths}
             {'' if args.related >= consts.DIRS_NO_FILTER else (" ".join(args.filter_sql) or '')}
         ORDER BY play_count
             , m.path LIKE "http%"
             {'' if 'sort' in args.defaults else ', ' + args.sort}
             , path
```

### Comparing `xklb-2.1.8/xklb/playlists.py` & `xklb-2.1.9/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/praw_extract.py` & `xklb-2.1.9/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/search.py` & `xklb-2.1.9/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/subtitle.py` & `xklb-2.1.9/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/tabs_actions.py` & `xklb-2.1.9/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/tabs_extract.py` & `xklb-2.1.9/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/tube_backend.py` & `xklb-2.1.9/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/tube_extract.py` & `xklb-2.1.9/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/usage.py` & `xklb-2.1.9/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/utils.py` & `xklb-2.1.9/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/bigdirs.py` & `xklb-2.1.9/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/block.py` & `xklb-2.1.9/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/christen.py` & `xklb-2.1.9/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/cluster_sort.py` & `xklb-2.1.9/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/copy_play_counts.py` & `xklb-2.1.9/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/dedupe.py` & `xklb-2.1.9/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/dedupe_db.py` & `xklb-2.1.9/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/download_status.py` & `xklb-2.1.9/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/history.py` & `xklb-2.1.9/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/merge_dbs.py` & `xklb-2.1.9/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/merge_online_local.py` & `xklb-2.1.9/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/move_list.py` & `xklb-2.1.9/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/optimize_db.py` & `xklb-2.1.9/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/playback_control.py` & `xklb-2.1.9/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/playlists.py` & `xklb-2.1.9/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/redownload.py` & `xklb-2.1.9/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/relmv.py` & `xklb-2.1.9/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/scatter.py` & `xklb-2.1.9/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/streaming_tab_loader.py` & `xklb-2.1.9/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/mining/data.py` & `xklb-2.1.9/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/mining/extract_links.py` & `xklb-2.1.9/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.1.9/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/mining/nouns.py` & `xklb-2.1.9/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/mining/pushshift.py` & `xklb-2.1.9/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.1.9/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/xklb/assets/kotobago.png` & `xklb-2.1.9/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/.gitignore` & `xklb-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/LICENSE` & `xklb-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/README.md` & `xklb-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/pyproject.toml` & `xklb-2.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.8/PKG-INFO` & `xklb-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.1.8
+Version: 2.1.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
```

