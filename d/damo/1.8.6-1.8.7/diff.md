# Comparing `tmp/damo-1.8.6.tar.gz` & `tmp/damo-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.6.tar", last modified: Mon Jun 19 21:07:26 2023, max compression
+gzip compressed data, was "damo-1.8.7.tar", last modified: Mon Jun 26 17:48:13 2023, max compression
```

## Comparing `damo-1.8.6.tar` & `damo-1.8.7.tar`

### file list

```diff
@@ -1,57 +1,55 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.797932 damo-1.8.6/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-19 21:07:26.797932 damo-1.8.6/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-19 21:07:22.000000 damo-1.8.6/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.6/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-19 21:07:26.797932 damo-1.8.6/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.6/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.781932 damo-1.8.6/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.797932 damo-1.8.6/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:22.000000 damo-1.8.6/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.6/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.6/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-17 18:34:52.000000 damo-1.8.6/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-05-29 19:08:47.000000 damo-1.8.6/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17097 2023-06-04 19:28:36.000000 damo-1.8.6/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    22860 2023-06-18 18:09:23.000000 damo-1.8.6/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-04 19:28:46.000000 damo-1.8.6/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3880 2023-06-10 21:05:04.000000 damo-1.8.6/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.6/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.6/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13386 2023-06-18 17:39:30.000000 damo-1.8.6/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.6/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5615 2023-06-04 19:26:26.000000 damo-1.8.6/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-06-18 17:31:57.000000 damo-1.8.6/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.6/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3376 2023-06-18 17:35:15.000000 damo-1.8.6/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.6/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      974 2023-06-11 18:40:28.000000 damo-1.8.6/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1653 2023-06-11 19:01:29.000000 damo-1.8.6/src/damo/damo_show_accesses.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      837 2023-06-11 18:26:23.000000 damo-1.8.6/src/damo/damo_show_snapshot.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-11 17:45:41.000000 damo-1.8.6/src/damo/damo_show_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.6/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1073 2023-06-10 21:05:04.000000 damo-1.8.6/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2956 2023-06-18 18:12:17.000000 damo-1.8.6/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1016 2023-06-10 21:05:04.000000 damo-1.8.6/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.6/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3930 2023-06-18 17:35:51.000000 damo-1.8.6/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-19 21:06:16.000000 damo-1.8.6/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-06-18 17:22:23.000000 damo-1.8.6/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.797932 damo-1.8.6/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1316 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.863841 damo-1.8.7/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-26 17:48:13.863841 damo-1.8.7/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-26 17:48:09.000000 damo-1.8.7/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.7/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-26 17:48:13.863841 damo-1.8.7/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.7/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.839842 damo-1.8.7/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.859841 damo-1.8.7/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:09.000000 damo-1.8.7/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.7/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.7/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-17 18:34:52.000000 damo-1.8.7/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-06-25 18:34:34.000000 damo-1.8.7/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.8.7/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    23604 2023-06-25 18:16:50.000000 damo-1.8.7/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-04 19:28:46.000000 damo-1.8.7/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3992 2023-06-25 17:52:33.000000 damo-1.8.7/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.7/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.7/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13386 2023-06-18 17:39:30.000000 damo-1.8.7/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.7/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5725 2023-06-25 17:13:05.000000 damo-1.8.7/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-06-18 17:31:57.000000 damo-1.8.7/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.7/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3766 2023-06-24 18:02:53.000000 damo-1.8.7/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.7/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5105 2023-06-25 18:54:44.000000 damo-1.8.7/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.7/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1058 2023-06-25 17:28:02.000000 damo-1.8.7/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2956 2023-06-18 18:12:17.000000 damo-1.8.7/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1001 2023-06-25 17:28:02.000000 damo-1.8.7/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-25 17:28:02.000000 damo-1.8.7/src/damo/damo_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.7/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3930 2023-06-18 17:35:51.000000 damo-1.8.7/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-26 17:47:10.000000 damo-1.8.7/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-06-18 17:22:23.000000 damo-1.8.7/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.859841 damo-1.8.7/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.6/PKG-INFO` & `damo-1.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.6
+Version: 1.8.7
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.6/README.md` & `damo-1.8.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -72,19 +72,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.6/setup.py` & `damo-1.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damo_deprecated.py` & `damo-1.8.7/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damo_deprecation_notice.py` & `damo-1.8.7/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damo_dist.py` & `damo-1.8.7/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damo_fmt_str.py` & `damo-1.8.7/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damo_fs.py` & `damo-1.8.7/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damo_paddr_layout.py` & `damo-1.8.7/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damo_subcmds.py` & `damo-1.8.7/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damon.py` & `damo-1.8.7/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damon_args.py` & `damo-1.8.7/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/_damon_dbgfs.py` & `damo-1.8.7/src/damo/_damon_dbgfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,31 +55,41 @@
 
     if feature_supported('init_regions'):
         string = ' '.join(['%s %d %d' % (tid, r.start, r.end) for r in
             target.regions])
         wops.append({debugfs_init_regions: string})
     return wops
 
+# note that DAMON debugfs interface is deprecated[1], and hence newer DAMOS
+# actions including _damon.damos_action_lru_prio and
+# _damon.damos_action_lru_deprio are not supported.
+#
+# [1] https://git.kernel.org/torvalds/c/5445fcbc4cda
 damos_action_to_int = {
         _damon.damos_action_willneed: 0,
         _damon.damos_action_cold: 1,
         _damon.damos_action_pageout: 2,
         _damon.damos_action_hugepage: 3,
         _damon.damos_action_nohugepage: 4,
         _damon.damos_action_stat: 5}
 
 damos_wmark_metric_to_int = {
         _damon.damos_wmarks_metric_none: 0,
         _damon.damos_wmarks_metric_free_mem_rate: 1}
 
 def damos_action_to_file_input(action_str):
-    return '%d' % damos_action_to_int[action_str]
+    if not action_str in damos_action_to_int:
+        raise Exception('\'%s\' DAMOS action is not supported' % action_str)
+    return damos_action_to_int[action_str]
 
 def damos_wmarks_metric_to_file_input(metric_str):
-    return '%d' % damos_wmark_metric_to_int[metric_str]
+    if not metric_str in damos_wmark_metric_to_int:
+        raise Exception('\'%s\' DAMOS watermark metric is not supported' %
+                metric_str)
+    return damos_wmark_metric_to_int[metric_str]
 
 def file_content_to_damos_action(action_file_content):
     for action_str in damos_action_to_int:
         if damos_action_to_int[action_str] == action_file_content:
             return action_str
 
 def file_content_to_damos_wmarks_metric(metric_file_content):
@@ -91,61 +101,50 @@
     pattern = damos.access_pattern.converted_for_units(
             _damon.unit_samples, _damon.unit_aggr_intervals,
             intervals)
     quotas = damos.quotas
     watermarks = damos.watermarks
 
     max_nr_accesses = intervals.aggr / intervals.sample
-    v0_scheme = '%d\t%d\t%d\t%d\t%d\t%d\t%s' % (
+    v0_scheme = '%d\t%d\t%d\t%d\t%d\t%d\t%d' % (
             pattern.sz_bytes[0], pattern.sz_bytes[1],
-            pattern.nr_acc_min_max[0].samples, pattern.nr_acc_min_max[1].samples,
-            pattern.age_min_max[0].aggr_intervals, pattern.age_min_max[1].aggr_intervals,
+            pattern.nr_acc_min_max[0].samples,
+            pattern.nr_acc_min_max[1].samples,
+            pattern.age_min_max[0].aggr_intervals,
+            pattern.age_min_max[1].aggr_intervals,
             damos_action_to_file_input(damos.action))
     if scheme_version == 0:
         return v0_scheme
 
-    v1_scheme = '%s\t%d\t%d' % (v0_scheme,
-            quotas.sz_bytes, quotas.reset_interval_ms)
-    if scheme_version == 1:
-        return v1_scheme
-
-    v2_scheme = '%s\t%d\t%d\t%d' % (v1_scheme,
-            quotas.weight_sz_permil, quotas.weight_nr_accesses_permil,
-            quotas.weight_age_permil)
-    if scheme_version == 2:
-        return v2_scheme
-
-    v3_scheme = '%s\t%s\t%d\t%d\t%d\t%d' % (v2_scheme,
-            damos_wmarks_metric_to_file_input(watermarks.metric),
-            watermarks.interval_us, watermarks.high_permil,
-            watermarks.mid_permil, watermarks.low_permil)
-    if scheme_version == 3:
-        return v3_scheme
-
-    v4_scheme = '%s\t' % v0_scheme + '\t'.join('%d' % x for x in [quotas.time_ms,
-        quotas.sz_bytes, quotas.reset_interval_ms, quotas.weight_sz_permil,
-        quotas.weight_nr_accesses_permil, quotas.weight_age_permil,
-        int(damos_wmarks_metric_to_file_input(watermarks.metric)),
-        watermarks.interval_us, watermarks.high_permil, watermarks.mid_permil,
-        watermarks.low_permil])
+    v4_scheme = '%s\t' % v0_scheme + '\t'.join(
+            '%d' % x for x in [
+                # quotas
+                quotas.time_ms, quotas.sz_bytes, quotas.reset_interval_ms,
+                quotas.weight_sz_permil, quotas.weight_nr_accesses_permil,
+                quotas.weight_age_permil,
+                # wmarks
+                damos_wmarks_metric_to_file_input(watermarks.metric),
+                watermarks.interval_us, watermarks.high_permil,
+                watermarks.mid_permil, watermarks.low_permil])
     if scheme_version == 4:
         return v4_scheme
 
     raise Exception('Unsupported scheme version: %d' % scheme_version)
 
 def get_scheme_version():
-    scheme_version = 0
+    '''Return the scheme version that the running kernel supports'''
+    scheme_version = 0      # 5.15-based DAMON implementation
     if feature_supported('schemes_speed_limit'):
-        scheme_version = 1
+        scheme_version = 1  # Non-mainlined implementation (deprecated)
     if feature_supported('schemes_prioritization'):
-        scheme_version = 2
+        scheme_version = 2  # Non-mainlined implementation (deprecated)
     if feature_supported('schemes_wmarks'):
-        scheme_version = 3
+        scheme_version = 3  # Non-mainlined implementation (deprecated)
     if feature_supported('schemes_quotas'):
-        scheme_version = 4
+        scheme_version = 4  # 5.16-based DAMON implementation
     return scheme_version
 
 def wops_for_schemes(schemes, intervals):
     scheme_file_input_lines = []
     for scheme in schemes:
         scheme_file_input_lines.append(damos_to_debugfs_input(scheme,
             intervals, get_scheme_version()))
@@ -181,15 +180,20 @@
         return write_contents
 
     write_contents += wops_for_schemes(ctx.schemes, ctx.intervals)
 
     return write_contents
 
 def stage_kdamonds(kdamonds):
-    return _damo_fs.write_files(wops_for_kdamonds(kdamonds))
+    '''Return error'''
+    try:
+        wops = wops_for_kdamonds(kdamonds)
+    except Exception as e:
+        return 'staging kdamond failed (%s)' % e
+    return _damo_fs.write_files(wops)
 
 # for current_kdamonds
 
 def debugfs_schemes_output_fields_to_access_pattern(fields, intervals_us):
     sz_bytes = fields[:2]
 
     # convert nr_accesses from sample intervals to percent
@@ -216,38 +220,14 @@
 
     access_pattern = debugfs_schemes_output_fields_to_access_pattern(fields,
             intervals_us)
     action = file_content_to_damos_action(fields[6])
 
     if len(fields) == 7:
         damos = _damon.Damos(access_pattern=access_pattern, action=action)
-    elif len(fields) == 9:
-        damos = _damon.Damos(access_pattern=access_pattern, action=action)
-        damos.quotas.sz_bytes = fields[7]
-        damos.quotas.reset_interval_ms = fields[8]
-    elif len(fields) == 12:
-        damos = _damon.Damos(access_pattern=access_pattern, action=action)
-        damos.quotas.sz_bytes = fields[7]
-        damos.quotas.reset_interval_ms = fields[8]
-        damos.quotas.weight_sz_permil = fields[9]
-        damos.quotas.weight_nr_accesses_permil = fields[10]
-        damos.quotas.weight_age_permil = fields[11]
-    elif len(fields) == 17:
-        damos = _damon.Damos(access_pattern=access_pattern, action=action)
-        damos.quotas.sz_bytes = fields[7]
-        damos.quotas.reset_interval_ms = fields[8]
-        damos.quotas.weight_sz_permil = fields[9]
-        damos.quotas.weight_nr_accesses_permil = fields[10]
-        damos.quotas.weight_age_permil = fields[11]
-        damos.watermarks.metric = file_content_to_damos_wmarks_metric(
-                fields[12])
-        damos.watermarks.interval_us = fields[13]
-        damos.watermarks.high_permil = fields[14]
-        damos.watermarks.mid_permil = fields[15]
-        damos.watermarks.low_permil = fields[16]
     elif len(fields) == 18:
         damos = _damon.Damos(access_pattern=access_pattern, action=action)
         damos.quotas.time_ms = fields[7]
         damos.quotas.sz_bytes = fields[8]
         damos.quotas.reset_interval_ms = fields[9]
         damos.quotas.weight_sz_permil = fields[10]
         damos.quotas.weight_nr_accesses_permil = fields[11]
@@ -453,10 +433,10 @@
             feature_supports['schemes_quotas'] = True
             feature_supports['schemes_stat_succ'] = True
             feature_supports['schemes_stat_qt_exceed'] = True
 
     if 0 < get_scheme_version() and get_scheme_version() < 4:
         _damo_deprecation_notice.deprecated(
                 feature='support of non-mainlined DAMOS implementation',
-                deadline='2023-Q2')
+                deadline='2023-Q2', do_exit=True)
 
     return None
```

### Comparing `damo-1.8.6/src/damo/_damon_result.py` & `damo-1.8.7/src/damo/_damon_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,28 +341,41 @@
                     stderr=subprocess.PIPE)
         except:
             err = 'perf record not working with "%s"' % PERF
     except:
         err = 'perf not found at "%s"' % PERF
     return err
 
+def parse_json(json_str):
+    kvpairs = json.loads(json_str)
+    return [DamonRecord.from_kvpairs(kvp) for kvp in kvpairs]
+
 def parse_json_compressed(result_file):
     with open(result_file, 'rb') as f:
         compressed = f.read()
     decompressed = zlib.decompress(compressed).decode()
-    kvpairs = json.loads(decompressed)
-    return [DamonRecord.from_kvpairs(kvp) for kvp in kvpairs]
+    return parse_json(decompressed)
+
+def parse_json_file(record_file):
+    with open(record_file) as f:
+        json_str = f.read()
+    return parse_json(json_str)
 
 def parse_records_file(result_file, monitoring_intervals=None):
     '''
     Return monitoring results records and error string
     '''
 
     file_type = subprocess.check_output(
             ['file', '-b', result_file]).decode().strip()
+    if file_type == 'JSON data':
+        try:
+            return parse_json_file(result_file), None
+        except Exception as e:
+            return None, 'failed parsing json file (%s)' % e
     if file_type == 'zlib compressed data':
         try:
             return parse_json_compressed(result_file), None
         except Exception as e:
             return None, 'failed parsing json compressed file (%s)' % e
 
     perf_script_output = None
@@ -387,14 +400,19 @@
 
 def write_json_compressed(records, file_path):
     json_str = json.dumps([r.to_kvpairs(raw=True) for r in records], indent=4)
     compressed = zlib.compress(json_str.encode())
     with open(file_path, 'wb') as f:
         f.write(compressed)
 
+def write_json(records, file_path):
+    json_str = json.dumps([r.to_kvpairs(raw=True) for r in records], indent=4)
+    with open(file_path, 'w') as f:
+        f.write(json_str)
+
 def add_fake_snapshot_if_needed(records):
     '''
     perf and record file format stores only snapshot end time.  For a record
     having only single snapshot, hence, the reader of the files cannot knwo the
     start time of the snapshot.  Add a fake snapshot for the case.
     '''
 
@@ -470,28 +488,31 @@
     if file_permission < 0o0 or file_permission > 0o777:
         return None, 'out of available permission range'
     return file_permission, None
 
 file_type_record = 'record'             # damo defined binary format
 file_type_perf_script = 'perf_script'   # perf script output
 file_type_perf_data = 'perf_data'       # perf record result file
+file_type_json = 'json'                 # list of DamonRecord objects in json
 file_type_json_compressed = 'json_compressed'
 
-file_types = [file_type_json_compressed, file_type_perf_script,
+file_types = [file_type_json_compressed, file_type_json, file_type_perf_script,
         file_type_perf_data, file_type_record]
-self_write_supported_file_types = [file_type_json_compressed,
+self_write_supported_file_types = [file_type_json_compressed, file_type_json,
         file_type_perf_script, file_type_record]
 
 def write_damon_records(records, file_path, file_type, file_permission=None):
     '''Returns None if success, an error string otherwise'''
     if not file_type in self_write_supported_file_types:
         return 'write unsupported file type: %s' % file_type
 
     if file_type == file_type_json_compressed:
         write_json_compressed(records, file_path)
+    elif file_type == file_type_json:
+        write_json(records, file_path)
     elif file_type == file_type_perf_script:
         write_perf_script(records, file_path)
     elif file_type == file_type_record:
         write_binary(records, file_path, 2)
 
     if file_permission != None:
         os.chmod(file_path, file_permission)
```

### Comparing `damo-1.8.6/src/damo/_damon_sysfs.py` & `damo-1.8.7/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo.py` & `damo-1.8.7/src/damo/damo.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import argparse
 
 import os
 os.sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 import sys
 
 import damo_adjust
+import damo_show
 import damo_convert_record_format
 import damo_features
 import damo_fmt_json
 import damo_lru_sort
 import damo_monitor
 import damo_reclaim
 import damo_record
 import damo_report
 import damo_schemes
-import damo_show
 import damo_start
 import damo_stat
+import damo_status
 import damo_stop
 import damo_translate_damos
 import damo_tune
 import damo_validate
 import damo_version
 
 import _damo_subcmds
@@ -65,17 +66,19 @@
             msg='print the version number'),
         _damo_subcmds.DamoSubCmd(name='translate_damos',
             module=damo_translate_damos,
             msg='translate old .damos to the new json format'),
         _damo_subcmds.DamoSubCmd(name='convert_record_format',
             module=damo_convert_record_format,
             msg='convert DAMON result record file\'s format'),
-        _damo_subcmds.DamoSubCmd(name='show',
-            module=damo_show,
-            msg='show status or results of damon operations'),
+        _damo_subcmds.DamoSubCmd(name='status',
+            module=damo_status,
+            msg='show DAMON status'),
+        _damo_subcmds.DamoSubCmd(name='show', module=damo_show,
+            msg='show monitored access pattern'),
         ]
 
 class SubCmdHelpFormatter(argparse.RawDescriptionHelpFormatter):
     def _format_action(self, action):
         parts = super(argparse.RawDescriptionHelpFormatter,
                 self)._format_action(action)
         # skip sub parsers help
```

### Comparing `damo-1.8.6/src/damo/damo_adjust.py` & `damo-1.8.7/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_convert_record_format.py` & `damo-1.8.7/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_features.py` & `damo-1.8.7/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_fmt_json.py` & `damo-1.8.7/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_heats.py` & `damo-1.8.7/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_lru_sort.py` & `damo-1.8.7/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_monitor.py` & `damo-1.8.7/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_nr_regions.py` & `damo-1.8.7/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_reclaim.py` & `damo-1.8.7/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_record.py` & `damo-1.8.7/src/damo/damo_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,18 @@
             print('could not turn DAMON on (%s)' % err)
             cleanup_exit(-2)
         data_for_cleanup.kdamonds_idxs = ['%d' % idx
                 for idx, k in enumerate(kdamonds)]
         # TODO: Support multiple kdamonds, multiple contexts
         monitoring_intervals = kdamonds[0].contexts[0].intervals
     else:
+        if not _damon.any_kdamond_running():
+            print('DAMON is not turned on')
+            exit(1)
+
         # TODO: Support multiple kdamonds, multiple contexts
         monitoring_intervals = data_for_cleanup.orig_kdamonds[
                 0].contexts[0].intervals
 
     data_for_cleanup.perf_pipe = _damon_result.start_monitoring_record(
             args.out, args.output_type, args.output_permission,
             monitoring_intervals)
```

### Comparing `damo-1.8.6/src/damo/damo_record_info.py` & `damo-1.8.7/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_report.py` & `damo-1.8.7/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_report_raw.py` & `damo-1.8.7/src/damo/damo_report_raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,33 @@
 import json
 import os
 import sys
 
 import _damon_result
 import _damo_fmt_str
 
+def filter_snapshots(records, start_time_sec, end_time_sec):
+    for record in records:
+        if len(record.snapshots) == 0:
+            continue
+        base_time = record.snapshots[0].start_time
+        filtered_snapshots = []
+        for snapshot in record.snapshots:
+            offset_sec = (snapshot.start_time - base_time) / 1000000000
+            if offset_sec < start_time_sec:
+                continue
+            if offset_sec > end_time_sec:
+                break
+            filtered_snapshots.append(snapshot)
+        record.snapshots = filtered_snapshots
+
 def pr_records(args, records):
+    if args.duration:
+        filter_snapshots(records, args.duration[0], args.duration[1])
+
     if args.json:
         print(json.dumps([r.to_kvpairs(args.raw_number)
             for r in records], indent=4))
         exit(0)
 
     for record in records:
         snapshots = record.snapshots
@@ -20,20 +38,14 @@
             continue
 
         base_time = snapshots[0].start_time
         print('base_time_absolute: %s\n' %
                 _damo_fmt_str.format_time_ns(base_time, args.raw_number))
 
         for snapshot in snapshots:
-            if args.duration:
-                time_offset_sec = (snapshot.start_time - base_time) / 1000000000
-                if time_offset_sec < args.duration[0]:
-                    continue
-                if time_offset_sec > args.duration[1]:
-                    break
             print('monitoring_start:    %16s' %
                     _damo_fmt_str.format_time_ns(
                         snapshot.start_time - base_time, args.raw_number))
             print('monitoring_end:      %16s' %
                     _damo_fmt_str.format_time_ns(
                         snapshot.end_time - base_time, args.raw_number))
             print('monitoring_duration: %16s' %
```

### Comparing `damo-1.8.6/src/damo/damo_schemes.py` & `damo-1.8.7/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_show_accesses.py` & `damo-1.8.7/src/damo/damo_stat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,77 @@
 # SPDX-License-Identifier: GPL-2.0
 
-"""
-Retrieve DAMON-observed accesses from a given source and show those in a
-specific format.
-"""
-
-import argparse
-
-import damo_heats
-import damo_nr_regions
-import damo_record_info
-import damo_report_raw
-import damo_wss
+import signal
+import time
+
+import damo_stat_kdamonds
+import damo_stat_regions
+import damo_stat_schemes
 
 import _damo_subcmds
+import _damon
+import _damon_args
+
+def pr_damon_interface(args):
+    _damon.ensure_root_and_initialized(args)
+    print(_damon.damon_interface())
 
 subcmds = [
-        _damo_subcmds.DamoSubCmd(name='info', module=damo_record_info,
-            msg='basic information about the record'),
-        _damo_subcmds.DamoSubCmd(name='raw', module=damo_report_raw,
-            msg='human readable raw data'),
-        _damo_subcmds.DamoSubCmd(name='heats', module=damo_heats,
-            msg='heats of regions'),
-        _damo_subcmds.DamoSubCmd(name='wss', module=damo_wss,
-            msg='working set size'),
-        _damo_subcmds.DamoSubCmd(name='nr_regions', module=damo_nr_regions,
-            msg='number of regions')]
+        _damo_subcmds.DamoSubCmd(name='kdamonds', module=damo_stat_kdamonds,
+            msg='detailed status of kdamonds'),
+        _damo_subcmds.DamoSubCmd(name='regions', module=damo_stat_regions,
+            msg='monitoring regions'),
+        _damo_subcmds.DamoSubCmd(name='schemes_stats',
+            module=damo_stat_schemes,
+            msg='schemes apply stats'),
+        _damo_subcmds.DamoSubCmd(name='schemes_tried_regions',
+            module=damo_stat_schemes,
+            msg='schemes tried regions in detail'),
+        _damo_subcmds.DamoSubCmd(name='damon_interface',
+            module=_damo_subcmds.DamoSubCmdModule(None, pr_damon_interface),
+            msg='default DAMON interface'),
+        ]
+
+def set_common_argparser(parser):
+    parser.add_argument('--delay', metavar='<secs>', default=3, type=float,
+            help='delay between repeated status prints')
+    parser.add_argument('--count', metavar='<count>', default=1, type=int,
+            help='number of repeated status prints.  zero means infinite')
+    parser.add_argument('--raw', action='store_true',
+            help='print numbers in machine friendly raw form')
 
 def set_argparser(parser):
-    parser.add_argument('accesses_source',
-            choices=['file'], # TODO: Add snapshot and scheme_tried_regions
-            default='file', nargs='?',
-            help='source of the accesses to show')
-    subparsers = parser.add_subparsers(title='format', dest='output_format',
-            metavar='<output format>',
-            help='the format of the output to show the record')
+    subparsers = parser.add_subparsers(title='stat type', dest='stat_type',
+            metavar='<stat type>', help='the type of the stat to show')
     subparsers.required = True
 
     for subcmd in subcmds:
         subcmd.add_parser(subparsers)
 
+    _damon_args.set_common_argparser(parser)
+    return parser
+
+def sighandler(signum, frame):
+    exit(0)
+
+def run_count_delay(func, args):
+    signal.signal(signal.SIGINT, sighandler)
+    signal.signal(signal.SIGTERM, sighandler)
+
+    i = 0
+    while args.count == 0 or i < args.count:
+        func(args)
+        if i != args.count - 1:
+            time.sleep(args.delay)
+        i += 1
+
 def main(args=None):
     if not args:
-        parser = argparse.ArgumentParser()
-        set_argparser(parser)
+        parser = set_argparser(None)
         args = parser.parse_args()
 
     for subcmd in subcmds:
-        if subcmd.name == args.output_format:
+        if subcmd.name == args.stat_type:
             subcmd.execute(args)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.6/src/damo/damo_show_status.py` & `damo-1.8.7/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_start.py` & `damo-1.8.7/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_stat_kdamonds.py` & `damo-1.8.7/src/damo/damo_stat_kdamonds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import json
 
 import damo_stat
-import damo_show_status
+import damo_status
 
 import _damo_deprecation_notice
 import _damo_fmt_str
 import _damon
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
     parser.add_argument('--detail', action='store_true',
             help='print detailed stat of kdamonds')
     parser.add_argument('--json', action='store_true',
             help='print kdamond in json format')
 
 def __main(args):
     if not args.detail:
-        damo_show_status.update_pr_kdamonds_summary(args.json, args.raw)
+        damo_status.update_pr_kdamonds_summary(args.json, args.raw)
     else:
-        damo_show_status.update_pr_kdamonds(args.json, args.raw)
+        damo_status.update_pr_kdamonds(args.json, args.raw)
 
 def main(args=None):
     _damo_deprecation_notice.will_be_deprecated('\'damo stat kdamonds\'',
             'near future', 'Use \'damo show status kdamonds\' instead')
 
     if not args:
         parser = argparse.ArgumentParser()
```

### Comparing `damo-1.8.6/src/damo/damo_stat_regions.py` & `damo-1.8.7/src/damo/damo_stat_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_stat_schemes.py` & `damo-1.8.7/src/damo/damo_stat_schemes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
-import damo_show_status
+import damo_status
 import damo_stat
 
 import _damo_deprecation_notice
 import _damo_fmt_str
 import _damo_subcmds
 import _damon
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
 
 def __main(args):
     if args.stat_type == 'schemes_stats':
-        damo_show_status.update_pr_schemes_stats(args.raw)
+        damo_status.update_pr_schemes_stats(args.raw)
     elif args.stat_type == 'schemes_tried_regions':
-        damo_show_status.update_pr_schemes_tried_regions(args.raw)
+        damo_status.update_pr_schemes_tried_regions(args.raw)
 
 def main(args=None):
     _damo_deprecation_notice.will_be_deprecated('\'damo stat schemes*\'',
             'near future', 'Use \'damo show status schemes*\' instead')
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
```

### Comparing `damo-1.8.6/src/damo/damo_stop.py` & `damo-1.8.7/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_translate_damos.py` & `damo-1.8.7/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_tune.py` & `damo-1.8.7/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_validate.py` & `damo-1.8.7/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo/damo_wss.py` & `damo-1.8.7/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.6/src/damo.egg-info/PKG-INFO` & `damo-1.8.7/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.6
+Version: 1.8.7
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.6/src/damo.egg-info/SOURCES.txt` & `damo-1.8.7/src/damo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,20 @@
 src/damo/damo_reclaim.py
 src/damo/damo_record.py
 src/damo/damo_record_info.py
 src/damo/damo_report.py
 src/damo/damo_report_raw.py
 src/damo/damo_schemes.py
 src/damo/damo_show.py
-src/damo/damo_show_accesses.py
-src/damo/damo_show_snapshot.py
-src/damo/damo_show_status.py
 src/damo/damo_start.py
 src/damo/damo_stat.py
 src/damo/damo_stat_kdamonds.py
 src/damo/damo_stat_regions.py
 src/damo/damo_stat_schemes.py
+src/damo/damo_status.py
 src/damo/damo_stop.py
 src/damo/damo_translate_damos.py
 src/damo/damo_tune.py
 src/damo/damo_validate.py
 src/damo/damo_version.py
 src/damo/damo_wss.py
 src/damo.egg-info/PKG-INFO
```

