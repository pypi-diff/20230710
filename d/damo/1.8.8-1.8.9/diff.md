# Comparing `tmp/damo-1.8.8.tar.gz` & `tmp/damo-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.8.tar", last modified: Mon Jul  3 17:22:48 2023, max compression
+gzip compressed data, was "damo-1.8.9.tar", last modified: Mon Jul 10 18:38:44 2023, max compression
```

## Comparing `damo-1.8.8.tar` & `damo-1.8.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.400680 damo-1.8.8/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8360 2023-07-03 17:22:48.396680 damo-1.8.8/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7839 2023-07-03 17:22:44.000000 damo-1.8.8/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.8/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-03 17:22:48.400680 damo-1.8.8/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.8/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.380680 damo-1.8.8/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.396680 damo-1.8.8/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:44.000000 damo-1.8.8/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.8/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.8/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35325 2023-07-02 19:16:32.000000 damo-1.8.8/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11832 2023-07-02 17:35:49.000000 damo-1.8.8/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.8.8/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    26299 2023-07-02 19:16:32.000000 damo-1.8.8/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19598 2023-07-02 18:42:47.000000 damo-1.8.8/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3992 2023-06-25 17:52:33.000000 damo-1.8.8/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.8/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.8/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13386 2023-06-18 17:39:30.000000 damo-1.8.8/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.8/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5725 2023-06-25 17:13:05.000000 damo-1.8.8/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-06-18 17:31:57.000000 damo-1.8.8/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.8/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3766 2023-06-24 18:02:53.000000 damo-1.8.8/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.8/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7610 2023-07-02 19:16:32.000000 damo-1.8.8/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.8/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1044 2023-07-02 19:29:16.000000 damo-1.8.8/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3150 2023-07-02 19:28:36.000000 damo-1.8.8/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      987 2023-07-02 19:29:03.000000 damo-1.8.8/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-25 17:28:02.000000 damo-1.8.8/src/damo/damo_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.8/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3930 2023-06-18 17:35:51.000000 damo-1.8.8/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-03 17:21:47.000000 damo-1.8.8/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-06-18 17:22:23.000000 damo-1.8.8/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.396680 damo-1.8.8/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8360 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.584291 damo-1.8.9/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-10 18:38:44.584291 damo-1.8.9/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-07-10 18:38:40.000000 damo-1.8.9/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.9/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-10 18:38:44.584291 damo-1.8.9/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.9/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.568291 damo-1.8.9/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.580291 damo-1.8.9/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:40.000000 damo-1.8.9/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.9/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9841 2023-07-09 19:46:58.000000 damo-1.8.9/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35332 2023-07-09 19:39:19.000000 damo-1.8.9/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11838 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.8.9/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    27404 2023-07-09 19:29:35.000000 damo-1.8.9/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19598 2023-07-02 18:42:47.000000 damo-1.8.9/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3991 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.9/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.9/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.9/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.8.9/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3766 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.9/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    12170 2023-07-09 19:59:30.000000 damo-1.8.9/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.8.9/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2382 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1043 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3149 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      986 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-25 17:28:02.000000 damo-1.8.9/src/damo/damo_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.8.9/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.9/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-10 18:37:33.000000 damo-1.8.9/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.584291 damo-1.8.9/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.8/PKG-INFO` & `damo-1.8.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.8
+Version: 1.8.9
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -137,17 +137,17 @@
 - ``wss_dist.png`` will show the distribution of the working set size.
 - ``wss_chron_change.png`` will show how the working set size has
   chronologically changed.
 
 You can show the images on a web page [1].  Those made with other realistic
 workloads are also available [2,3,4].
 
-[1] https://damonitor.github.io/doc/html/latest/admin-guide/mm/damon/start.html#visualizing-recorded-patterns  
-[2] https://damonitor.github.io/test/result/visual/latest/rec.heatmap.1.png.html  
-[3] https://damonitor.github.io/test/result/visual/latest/rec.wss_sz.png.html  
+[1] https://damonitor.github.io/doc/html/latest/admin-guide/mm/damon/start.html#visualizing-recorded-patterns<br>
+[2] https://damonitor.github.io/test/result/visual/latest/rec.heatmap.1.png.html<br>
+[3] https://damonitor.github.io/test/result/visual/latest/rec.wss_sz.png.html<br>
 [4] https://damonitor.github.io/test/result/visual/latest/rec.wss_time.png.html
 
 
 Data Access Pattern Aware Memory Management
 ===========================================
 
 Below three commands make every memory region of size >=4K that hasn't accessed
```

### Comparing `damo-1.8.8/README.md` & `damo-1.8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,19 +75,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -122,17 +122,17 @@
 - ``wss_dist.png`` will show the distribution of the working set size.
 - ``wss_chron_change.png`` will show how the working set size has
   chronologically changed.
 
 You can show the images on a web page [1].  Those made with other realistic
 workloads are also available [2,3,4].
 
-[1] https://damonitor.github.io/doc/html/latest/admin-guide/mm/damon/start.html#visualizing-recorded-patterns  
-[2] https://damonitor.github.io/test/result/visual/latest/rec.heatmap.1.png.html  
-[3] https://damonitor.github.io/test/result/visual/latest/rec.wss_sz.png.html  
+[1] https://damonitor.github.io/doc/html/latest/admin-guide/mm/damon/start.html#visualizing-recorded-patterns<br>
+[2] https://damonitor.github.io/test/result/visual/latest/rec.heatmap.1.png.html<br>
+[3] https://damonitor.github.io/test/result/visual/latest/rec.wss_sz.png.html<br>
 [4] https://damonitor.github.io/test/result/visual/latest/rec.wss_time.png.html
 
 
 Data Access Pattern Aware Memory Management
 ===========================================
 
 Below three commands make every memory region of size >=4K that hasn't accessed
```

### Comparing `damo-1.8.8/setup.py` & `damo-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/_damo_deprecated.py` & `damo-1.8.9/src/damo/_damo_deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 '''
 
 import json
 import os
 import subprocess
 import sys
 
-import _damon
-
 import _damo_deprecation_notice
 import _damo_fmt_str
+import _damon
 
 '''
 Python2 support
 '''
 
 if sys.version.startswith('2.'):
     _damo_deprecation_notice.deprecated(feature='Python2 support of damo',
```

### Comparing `damo-1.8.8/src/damo/_damo_deprecation_notice.py` & `damo-1.8.9/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/_damo_dist.py` & `damo-1.8.9/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/_damo_fmt_str.py` & `damo-1.8.9/src/damo/_damo_fmt_str.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,20 @@
     # cut '0.' prefix
     under_percent_str = under_percent_str[2:]
 
     if under_percent_str == '':
         return '%s %%' % over_percent_str
     return '%s.%s %%' % (over_percent_str, under_percent_str)
 
+def format_percent(percent, machine_friendly):
+    if machine_friendly:
+        return '%f' % percent
+
+    return format_ratio(float(percent) / 100, machine_friendly)
+
 def format_permil(permil, machine_friendly):
     if machine_friendly:
         return '%f' % permil
 
     return format_ratio(float(permil) / 1000, machine_friendly)
 
 def indent_lines(string, indent_width):
```

### Comparing `damo-1.8.8/src/damo/_damo_fs.py` & `damo-1.8.9/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/_damo_paddr_layout.py` & `damo-1.8.9/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/_damo_subcmds.py` & `damo-1.8.9/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/_damon.py` & `damo-1.8.9/src/damo/_damon.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,15 +901,15 @@
 # DAMON control
 
 def stage_kdamonds(kdamonds):
     return _damon_fs.stage_kdamonds(kdamonds)
 
 def commit_staged(kdamond_idxs):
     if _damon_fs == _damon_dbgfs:
-        return 'debugfs interface unsupport commit_staged()'
+        return 'debugfs interface does not support commit_staged()'
     return _damon_fs.commit_staged(kdamond_idxs)
 
 def commit(kdamonds):
     err = stage_kdamonds(kdamonds)
     if err:
         return 'staging updates failed (%s)' % err
     err = commit_staged(['%s' % idx for idx, k in enumerate(kdamonds)])
```

### Comparing `damo-1.8.8/src/damo/_damon_args.py` & `damo-1.8.9/src/damo/_damon_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return [damos], None
 
     if not 'schemes' in args or args.schemes == None:
         return [], None
 
     schemes, err = schemes_option_to_damos(args.schemes)
     if err:
-        return None, 'failed damo schemes arguents parsing (%s)' % err
+        return None, 'failed damo schemes arguments parsing (%s)' % err
     return schemes, None
 
 def damon_ctx_for(args):
     try:
         intervals = damon_intervals_for(args)
     except Exception as e:
         return None, 'invalid intervals arguments (%s)' % e
@@ -139,43 +139,43 @@
         else:
             kdamonds_str = arg
         kdamonds_kvpairs = json.loads(kdamonds_str)['kdamonds']
         return [kdamond.from_kvpairs(kvp) for kvp in kdamonds_kvpairs], None
     except Exception as e:
         return None, e
 
-target_type_explict = 'explict'
+target_type_explicit = 'explicit'
 target_type_cmd = 'cmd'
 target_type_pid = 'pid'
 target_type_unknown = None
 
 def deduced_target_type(target):
     if target in ['vaddr', 'paddr', 'fvaddr']:
-        return target_type_explict
+        return target_type_explicit
     try:
         subprocess.check_output(['which', target.split()[0]])
         return target_type_cmd
     except:
         pass
     try:
         pid = int(target)
         return target_type_pid
     except:
         pass
     return target_type_unknown
 
 def warn_option_override(option_name):
-    print('warning: %s is overriden by <deducible target>' % option_name)
+    print('warning: %s is overridden by <deducible target>' % option_name)
 
 def deduce_target_update_args(args):
     args.self_started_target = False
     target_type = deduced_target_type(args.deducible_target)
     if target_type == target_type_unknown:
         return 'target \'%s\' is not supported' % args.deducible_target
-    if target_type == target_type_explict and args.deducible_target == 'paddr':
+    if target_type == target_type_explicit and args.deducible_target == 'paddr':
         if not args.ops in ['paddr', None]:
             warn_option_override('--ops')
         args.ops = 'paddr'
         if args.target_pid != None:
             warn_option_override('--target_pid')
         args.target_pid = None
         return None
```

### Comparing `damo-1.8.8/src/damo/_damon_dbgfs.py` & `damo-1.8.9/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/_damon_result.py` & `damo-1.8.9/src/damo/_damon_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -409,15 +409,15 @@
     json_str = json.dumps([r.to_kvpairs(raw=True) for r in records], indent=4)
     with open(file_path, 'w') as f:
         f.write(json_str)
 
 def add_fake_snapshot_if_needed(records):
     '''
     perf and record file format stores only snapshot end time.  For a record
-    having only single snapshot, hence, the reader of the files cannot knwo the
+    having only single snapshot, hence, the reader of the files cannot know the
     start time of the snapshot.  Add a fake snapshot for the case.
     '''
 
     for record in records:
         snapshots = record.snapshots
         if len(snapshots) != 1:
             continue
@@ -562,66 +562,70 @@
             monitoring_intervals)
     if err != None:
         print('converting format from perf_data to %s failed (%s)' %
                 (file_format, err))
 
 # for snapshot
 
-def install_scheme(scheme_to_install):
+def find_install_scheme(scheme_to_find):
     '''Install given scheme to all contexts if effectively same scheme is not
     installed.
-    Returns whether it found a context doesn't having the scheme, and an error
-    if something wrong.
+    Returns whether it found a context doesn't having the scheme, indices list
+    for the effectively same schemes, and an error if something wrong.
     '''
     installed = False
+    indices = []
     kdamonds = _damon.current_kdamonds()
-    for kdamond in kdamonds:
-        for ctx in kdamond.contexts:
+    for kidx, kdamond in enumerate(kdamonds):
+        for cidx, ctx in enumerate(kdamond.contexts):
             ctx_has_the_scheme = False
-            for scheme in ctx.schemes:
-                if scheme.effectively_equal(scheme_to_install, ctx.intervals):
+            for sidx, scheme in enumerate(ctx.schemes):
+                if scheme.effectively_equal(scheme_to_find, ctx.intervals):
                     ctx_has_the_scheme = True
+                    indices.append([kidx, cidx, sidx])
                     break
             if ctx_has_the_scheme:
                 continue
-            ctx.schemes.append(scheme_to_install)
+            ctx.schemes.append(scheme_to_find)
             installed = True
+            indices.append([kidx, cidx, len(ctx.schemes) - 1])
     if installed:
         err = _damon.commit(kdamonds)
         if err != None:
-            return (False,
+            return (False, [],
                     'committing scheme installed kdamonds failed: %s' % err)
-    return installed, None
+    return installed, indices, None
 
 def tried_regions_to_snapshot(tried_regions, intervals):
     snapshot_end_time_ns = time.time() * 1000000000
     snapshot_start_time_ns = snapshot_end_time_ns - intervals.aggr * 1000
     snapshot = DamonSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
 
     for tried_region in tried_regions:
         snapshot.regions.append(tried_region)
     return snapshot
 
-def tried_regions_to_records(monitor_scheme):
+def tried_regions_to_records_of(idxs):
+    '''idxs: list of kdamond/context/scheme indices to get records for.  If it
+    is None, return records for all schemes'''
     records = []
     for kdamond_idx, kdamond in enumerate(_damon.current_kdamonds()):
         if kdamond.state != 'on':
             continue
-        # TODO: Make a cleaner way for passing the index
         for ctx_idx, ctx in enumerate(kdamond.contexts):
-            for scheme in ctx.schemes:
-                if not scheme.effectively_equal(monitor_scheme, ctx.intervals):
+            for scheme_idx, scheme in enumerate(ctx.schemes):
+                if not [kdamond_idx, ctx_idx, scheme_idx] in idxs:
                     continue
 
                 snapshot = tried_regions_to_snapshot(scheme.tried_regions,
                         ctx.intervals)
                 snapshot.total_bytes = scheme.tried_bytes
 
                 records.append(DamonRecord(kdamond_idx, ctx_idx, ctx.intervals,
-                    None, None))
+                    scheme_idx, None))
                 records[-1].snapshots.append(snapshot)
                 break
     return records
 
 def three_regions_of(pid):
     '''
     Return three big mapped virtual address ranges of a given process, which
@@ -691,22 +695,22 @@
     orig_kdamonds = _damon.current_kdamonds()
 
     err = install_target_regions_if_needed(orig_kdamonds)
     if err != None:
         return None, 'vaddr region install failed (%s)' % err
 
     monitor_scheme = _damon.Damos(access_pattern=access_pattern)
-    installed, err = install_scheme(monitor_scheme)
+    installed, idxs, err = find_install_scheme(monitor_scheme)
     if err:
         return None, 'monitoring scheme install failed: %s' % err
 
     if total_sz_only:
         err = _damon.update_schemes_tried_bytes(running_kdamond_idxs)
         if err == None:
-            records = tried_regions_to_records(monitor_scheme)
+            records = tried_regions_to_records_of(idxs)
 
             if installed:
                 err = _damon.commit(orig_kdamonds)
                 if err:
                     return records, 'monitoring scheme uninstall failed: %s' % err
             return records, None
 
@@ -714,14 +718,34 @@
     if err != None:
         if installed:
             err = _damon.commit(orig_kdamonds)
             if err:
                 return None, 'monitoring scheme uninstall failed: %s' % err
         return None, 'updating schemes tried regions fail: %s' % err
 
-    records = tried_regions_to_records(monitor_scheme)
+    records = tried_regions_to_records_of(idxs)
 
     if installed:
         err = _damon.commit(orig_kdamonds)
         if err:
             return records, 'monitoring scheme uninstall failed: %s' % err
     return records, None
+
+def get_snapshot_records_for_schemes(idxs, total_sz_only):
+    '''idxs: list of kdamond/context/scheme indices to get records for.
+    Return DamonRecord objects each having single DamonSnapshot and an error'''
+    running_kdamond_idxs = _damon.running_kdamond_idxs()
+    if len(running_kdamond_idxs) == 0:
+        return None, 'no kdamond running'
+
+    if total_sz_only:
+        err = _damon.update_schemes_tried_bytes(running_kdamond_idxs)
+        if err == None:
+            records = tried_regions_to_records_of(idxs)
+            return records, None
+
+    err = _damon.update_schemes_tried_regions(running_kdamond_idxs)
+    if err != None:
+        return None, 'updating schemes tried regions fail: %s' % err
+
+    records = tried_regions_to_records_of(idxs)
+    return records, None
```

### Comparing `damo-1.8.8/src/damo/_damon_sysfs.py` & `damo-1.8.9/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo.py` & `damo-1.8.9/src/damo/damo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
-
 import os
+
 os.sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 import sys
 
+import _damo_subcmds
 import damo_adjust
-import damo_show
 import damo_convert_record_format
 import damo_features
 import damo_fmt_json
 import damo_lru_sort
 import damo_monitor
 import damo_reclaim
 import damo_record
 import damo_report
 import damo_schemes
+import damo_show
 import damo_start
 import damo_stat
 import damo_status
 import damo_stop
 import damo_translate_damos
 import damo_tune
 import damo_validate
 import damo_version
 
-import _damo_subcmds
-
 def pr_damo_version(args_not_use):
     print(damo_version.__version__)
 
 subcmds = [
         _damo_subcmds.DamoSubCmd(name='record', module=damo_record,
             msg='record data accesses'),
         _damo_subcmds.DamoSubCmd(name='schemes', module=damo_schemes,
```

### Comparing `damo-1.8.8/src/damo/damo_adjust.py` & `damo-1.8.9/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_convert_record_format.py` & `damo-1.8.9/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_features.py` & `damo-1.8.9/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_fmt_json.py` & `damo-1.8.9/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_heats.py` & `damo-1.8.9/src/damo/damo_heats.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 import argparse
 import os
 import subprocess
 import sys
 import tempfile
 
-import _damon_result
 import _damo_fmt_str
+import _damon_result
 
 class HeatPixel:
     time = None
     addr = None
     heat = None
 
     def __init__(self, time, addr, heat):
@@ -337,15 +337,15 @@
     parser.add_argument('--input', '-i', type=str, metavar='<file>',
             default='damon.data', help='input file name')
 
     parser.add_argument('--tid', metavar='<id>', type=int,
             help='target id')
     parser.add_argument('--resol', metavar='<resolution>', type=int, nargs=2,
             default=[500, 500],
-            help='resolutions for time and address axises')
+            help='resolutions for time and address axes')
     parser.add_argument('--time_range', metavar='<time>', type=int, nargs=2,
             help='start and end time of the output')
     parser.add_argument('--address_range', metavar='<address>', type=int,
             nargs=2, help='start and end address of the output')
     parser.add_argument('--abs_time', action='store_true', default=False,
             help='display absolute time in output')
     parser.add_argument('--abs_addr', action='store_true', default=False,
```

### Comparing `damo-1.8.8/src/damo/damo_lru_sort.py` & `damo-1.8.9/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_monitor.py` & `damo-1.8.9/src/damo/damo_monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     target = args.target
     target_fields = target.split()
     target_type = _damon_args.deduced_target_type(target)
     if target_type == None:
         print('invalid target \'%s\'' % target)
         exit(1)
-    if target_type == _damon_args.target_type_explict and target == 'paddr':
+    if target_type == _damon_args.target_type_explicit and target == 'paddr':
         pass
     elif target_type == _damon_args.target_type_cmd:
         cmd_pipe = subprocess.Popen(target, shell=True, executable='/bin/bash',
                 stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         target = cmd_pipe.pid
     else:
         pid = int(target)
```

### Comparing `damo-1.8.8/src/damo/damo_nr_regions.py` & `damo-1.8.9/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_reclaim.py` & `damo-1.8.9/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_record.py` & `damo-1.8.9/src/damo/damo_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
             help='output file\'s type')
     parser.add_argument('--output_permission', type=str, default='600',
             help='permission of the output file')
     parser.add_argument('--perf_path', type=str, default='perf',
             help='path of perf tool ')
     parser.add_argument('--include_child_tasks', action='store_true',
             help='record accesses of child processes')
+    parser.description='Record monitoring results'
     return parser
 
 def main(args=None):
     global data_for_cleanup
 
     if not args:
         parser = set_argparser(None)
```

### Comparing `damo-1.8.8/src/damo/damo_record_info.py` & `damo-1.8.9/src/damo/damo_record_info.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 """
 Print basic information of the access monitoring results record file.
 """
 
 import argparse
 
-import _damon_result
 import _damo_fmt_str
+import _damon_result
 
 class GuideInfo:
     tid = None
     start_time = None
     end_time = None
     lowest_addr = None
     highest_addr = None
```

### Comparing `damo-1.8.8/src/damo/damo_report.py` & `damo-1.8.9/src/damo/damo_report.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
+import _damo_subcmds
 import damo_heats
 import damo_nr_regions
 import damo_report_raw
 import damo_wss
 
-import _damo_subcmds
-
 subcmds = [
         _damo_subcmds.DamoSubCmd(name='raw', module=damo_report_raw,
             msg='human readable raw data'),
         _damo_subcmds.DamoSubCmd(name='heats', module=damo_heats,
             msg='heats of regions'),
         _damo_subcmds.DamoSubCmd(name='wss', module=damo_wss,
             msg='working set size'),
```

### Comparing `damo-1.8.8/src/damo/damo_report_raw.py` & `damo-1.8.9/src/damo/damo_report_raw.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import json
 import os
 import sys
 
-import _damon_result
 import _damo_fmt_str
+import _damon_result
 
 def filter_snapshots(records, start_time_sec, end_time_sec):
     for record in records:
         if len(record.snapshots) == 0:
             continue
         base_time = record.snapshots[0].start_time
         filtered_snapshots = []
```

### Comparing `damo-1.8.8/src/damo/damo_schemes.py` & `damo-1.8.9/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_start.py` & `damo-1.8.9/src/damo/damo_tune.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # SPDX-License-Identifier: GPL-2.0
 
 """
-Start DAMON with given parameters.
+Update DAMON input parameters.
 """
 
 import _damon
 import _damon_args
 
 def set_argparser(parser):
     return _damon_args.set_argparser(parser, add_record_options=False)
 
 def main(args=None):
     if not args:
-        parser = set_pargparser(None)
+        parser = set_argparser(None)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    err, kdamonds = _damon_args.turn_damon_on(args)
+    if not _damon.any_kdamond_running():
+        print('DAMON is not turned on')
+        exit(1)
+
+    kdamonds, err = _damon_args.commit_kdamonds(args)
     if err:
-        print('could not turn on damon (%s)' % err)
+        print('tuning failed (%s)' % err)
         exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.8/src/damo/damo_stat.py` & `damo-1.8.9/src/damo/damo_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import signal
 import time
 
-import damo_stat_kdamonds
-import damo_stat_regions
-import damo_stat_schemes
-
 import _damo_subcmds
 import _damon
 import _damon_args
+import damo_stat_kdamonds
+import damo_stat_regions
+import damo_stat_schemes
 
 def pr_damon_interface(args):
     _damon.ensure_root_and_initialized(args)
     print(_damon.damon_interface())
 
 subcmds = [
         _damo_subcmds.DamoSubCmd(name='kdamonds', module=damo_stat_kdamonds,
```

### Comparing `damo-1.8.8/src/damo/damo_stat_kdamonds.py` & `damo-1.8.9/src/damo/damo_stat_kdamonds.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import json
 
-import damo_stat
-import damo_status
-
 import _damo_deprecation_notice
 import _damo_fmt_str
 import _damon
+import damo_stat
+import damo_status
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
     parser.add_argument('--detail', action='store_true',
             help='print detailed stat of kdamonds')
     parser.add_argument('--json', action='store_true',
             help='print kdamond in json format')
```

### Comparing `damo-1.8.8/src/damo/damo_stat_regions.py` & `damo-1.8.9/src/damo/damo_stat_regions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
-import damo_stat
-
 import _damo_deprecation_notice
 import _damo_fmt_str
 import _damo_subcmds
 import _damon
 import _damon_result
+import damo_stat
 
 def priority(region, weights):
     if region.nr_accesses.samples > 0:
         return (region.nr_accesses.samples * weights[0] +
                 region.age * weights[1])
     return region.age * weights[1] * -1
```

### Comparing `damo-1.8.8/src/damo/damo_stat_schemes.py` & `damo-1.8.9/src/damo/damo_stat_schemes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
-import damo_status
-import damo_stat
-
 import _damo_deprecation_notice
 import _damo_fmt_str
 import _damo_subcmds
 import _damon
+import damo_stat
+import damo_status
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
 
 def __main(args):
     if args.stat_type == 'schemes_stats':
         damo_status.update_pr_schemes_stats(args.raw)
```

### Comparing `damo-1.8.8/src/damo/damo_status.py` & `damo-1.8.9/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_stop.py` & `damo-1.8.9/src/damo/damo_stop.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 Stop DAMON.
 """
 
 import _damon
 import _damon_args
 
 def set_argparser(parser):
-    return _damon_args.set_common_argparser(parser)
+    _damon_args.set_common_argparser(parser)
+    parser.description='Stop DAMON'
+    return parser
 
 def main(args=None):
     if not args:
         parser = set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
```

### Comparing `damo-1.8.8/src/damo/damo_translate_damos.py` & `damo-1.8.9/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.8/src/damo/damo_tune.py` & `damo-1.8.9/src/damo/damo_start.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # SPDX-License-Identifier: GPL-2.0
 
 """
-Update DAMON input parameters.
+Start DAMON with given parameters.
 """
 
 import _damon
 import _damon_args
 
 def set_argparser(parser):
-    return _damon_args.set_argparser(parser, add_record_options=False)
+    parser = _damon_args.set_argparser(parser, add_record_options=False)
+    parser.description='Start DAMON'
+    return parser
 
 def main(args=None):
     if not args:
-        parser = set_argparser(None)
+        parser = set_pargparser(None)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    if not _damon.any_kdamond_running():
-        print('DAMON is not turned on')
-        exit(1)
-
-    kdamonds, err = _damon_args.commit_kdamonds(args)
+    err, kdamonds = _damon_args.turn_damon_on(args)
     if err:
-        print('tuning failed (%s)' % err)
+        print('could not turn on damon (%s)' % err)
         exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.8/src/damo/damo_validate.py` & `damo-1.8.9/src/damo/damo_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     but error allowed, exit with non-zero else'''
     if not min_max:
         return 0
     if min_max[0] <= value and value <= min_max[1]:
         return 0
     if error_allowed:
         return 1
-    print('invalid: expecte %d<=%s<=%d but %d' %
+    print('invalid: expect %d<=%s<=%d but %d' %
             (min_max[0], name, min_max[1], value))
     exit(1)
 
 def check_boundary(region, regions_boundary):
     in_boundary = False
     for boundary in regions_boundary:
         if (region.start >= boundary[0] and
```

### Comparing `damo-1.8.8/src/damo/damo_wss.py` & `damo-1.8.9/src/damo/damo_wss.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 "Print out the distribution of the working set sizes of the given trace"
 
 import argparse
 import sys
 import tempfile
 
 import _damo_dist
-import _damon_result
 import _damo_fmt_str
+import _damon_result
 
 def get_wss_dists(records, acc_thres, sz_thres, do_sort):
     wss_dists = {}
     for record in records:
         wss_dist = []
         for snapshot in record.snapshots:
             wss = 0
```

### Comparing `damo-1.8.8/src/damo.egg-info/PKG-INFO` & `damo-1.8.9/src/damo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.8
+Version: 1.8.9
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -137,17 +137,17 @@
 - ``wss_dist.png`` will show the distribution of the working set size.
 - ``wss_chron_change.png`` will show how the working set size has
   chronologically changed.
 
 You can show the images on a web page [1].  Those made with other realistic
 workloads are also available [2,3,4].
 
-[1] https://damonitor.github.io/doc/html/latest/admin-guide/mm/damon/start.html#visualizing-recorded-patterns  
-[2] https://damonitor.github.io/test/result/visual/latest/rec.heatmap.1.png.html  
-[3] https://damonitor.github.io/test/result/visual/latest/rec.wss_sz.png.html  
+[1] https://damonitor.github.io/doc/html/latest/admin-guide/mm/damon/start.html#visualizing-recorded-patterns<br>
+[2] https://damonitor.github.io/test/result/visual/latest/rec.heatmap.1.png.html<br>
+[3] https://damonitor.github.io/test/result/visual/latest/rec.wss_sz.png.html<br>
 [4] https://damonitor.github.io/test/result/visual/latest/rec.wss_time.png.html
 
 
 Data Access Pattern Aware Memory Management
 ===========================================
 
 Below three commands make every memory region of size >=4K that hasn't accessed
```

### Comparing `damo-1.8.8/src/damo.egg-info/SOURCES.txt` & `damo-1.8.9/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

