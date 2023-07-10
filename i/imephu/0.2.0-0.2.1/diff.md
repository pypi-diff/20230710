# Comparing `tmp/imephu-0.2.0.tar.gz` & `tmp/imephu-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imephu-0.2.0.tar", last modified: Wed May  3 19:02:23 2023, max compression
+gzip compressed data, was "imephu-0.2.1.tar", max compression
```

## Comparing `imephu-0.2.0.tar` & `imephu-0.2.1.tar`

### file list

```diff
@@ -1,116 +1,31 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.477321 imephu-0.2.0/
--rw-r--r--   0 christian   (501) staff       (20)     1102 2022-01-15 12:25:41.000000 imephu-0.2.0/LICENSE
--rw-r--r--   0 christian   (501) staff       (20)       50 2022-01-15 12:25:41.000000 imephu-0.2.0/MANIFEST.in
--rw-r--r--   0 christian   (501) staff       (20)     1426 2023-05-03 19:02:23.477481 imephu-0.2.0/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1015 2023-05-03 18:55:18.000000 imephu-0.2.0/README.md
--rw-r--r--   0 christian   (501) staff       (20)      179 2022-02-11 15:02:42.000000 imephu-0.2.0/pyproject.toml
--rw-r--r--   0 christian   (501) staff       (20)     2631 2023-05-03 19:02:23.479383 imephu-0.2.0/setup.cfg
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.347705 imephu-0.2.0/src/
--rw-r--r--   0 christian   (501) staff       (20)     6148 2022-03-15 07:56:29.000000 imephu-0.2.0/src/.DS_Store
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.354756 imephu-0.2.0/src/imephu/
--rw-r--r--   0 christian   (501) staff       (20)     6148 2022-01-19 10:57:49.000000 imephu-0.2.0/src/imephu/.DS_Store
--rw-r--r--   0 christian   (501) staff       (20)      185 2023-05-03 18:55:18.000000 imephu-0.2.0/src/imephu/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.372200 imephu-0.2.0/src/imephu/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      345 2023-05-03 18:57:09.000000 imephu-0.2.0/src/imephu/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)      343 2022-07-06 16:37:45.000000 imephu-0.2.0/src/imephu/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     9704 2022-06-14 07:19:18.000000 imephu-0.2.0/src/imephu/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     9693 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/cli.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)    12059 2023-05-03 18:57:09.000000 imephu-0.2.0/src/imephu/__pycache__/finder_chart.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)    13432 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/finder_chart.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     7848 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/__pycache__/geometry.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     7870 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/geometry.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3528 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3522 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/utils.cpython-38.pyc
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.374858 imephu-0.2.0/src/imephu/annotation/
--rw-r--r--   0 christian   (501) staff       (20)     1550 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.380954 imephu-0.2.0/src/imephu/annotation/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)     2093 2022-02-16 12:01:09.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     2105 2022-07-06 16:37:45.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4075 2022-01-20 07:33:05.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/general.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     6146 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/motion.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     6137 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/motion.cpython-38.pyc
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.388639 imephu-0.2.0/src/imephu/annotation/general/
--rw-r--r--   0 christian   (501) staff       (20)      746 2022-04-10 10:07:01.000000 imephu-0.2.0/src/imephu/annotation/general/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.410065 imephu-0.2.0/src/imephu/annotation/general/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      825 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)      849 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3797 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/arrow.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3775 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/arrow.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4219 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/circle.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4197 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/circle.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     2703 2022-03-16 19:12:35.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/crosshairs.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     2660 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/crosshairs.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     2205 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/empty.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     2215 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/empty.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3881 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/group.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3890 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/group.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4998 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/line_path.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4966 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/line_path.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4715 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/rectangle.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4699 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/rectangle.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     5280 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/text.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     5242 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/text.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4480 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/general/arrow.py
--rw-r--r--   0 christian   (501) staff       (20)     3879 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/circle.py
--rw-r--r--   0 christian   (501) staff       (20)     2581 2022-03-16 15:48:57.000000 imephu-0.2.0/src/imephu/annotation/general/crosshairs.py
--rw-r--r--   0 christian   (501) staff       (20)     1646 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/empty.py
--rw-r--r--   0 christian   (501) staff       (20)     3021 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/general/group.py
--rw-r--r--   0 christian   (501) staff       (20)     4428 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/line_path.py
--rw-r--r--   0 christian   (501) staff       (20)     4425 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/general/rectangle.py
--rw-r--r--   0 christian   (501) staff       (20)     5316 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/text.py
--rw-r--r--   0 christian   (501) staff       (20)     9170 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/motion.py
--rw-r--r--   0 christian   (501) staff       (20)    11976 2022-04-10 10:02:05.000000 imephu-0.2.0/src/imephu/cli.py
--rw-r--r--   0 christian   (501) staff       (20)    12939 2023-05-03 18:55:18.000000 imephu-0.2.0/src/imephu/finder_chart.py
--rw-r--r--   0 christian   (501) staff       (20)     9710 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/geometry.py
--rw-r--r--   0 christian   (501) staff       (20)        0 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/py.typed
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.421076 imephu-0.2.0/src/imephu/salt/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.436061 imephu-0.2.0/src/imephu/salt/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      168 2022-01-26 13:02:56.000000 imephu-0.2.0/src/imephu/salt/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)    12811 2022-04-10 10:22:44.000000 imephu-0.2.0/src/imephu/salt/__pycache__/finder_chart.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)    12855 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/salt/__pycache__/finder_chart.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     6895 2022-01-26 15:41:26.000000 imephu-0.2.0/src/imephu/salt/__pycache__/general.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     1389 2022-01-26 19:29:20.000000 imephu-0.2.0/src/imephu/salt/__pycache__/rss.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4839 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4792 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/__pycache__/utils.cpython-38.pyc
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.442757 imephu-0.2.0/src/imephu/salt/annotation/
--rw-r--r--   0 christian   (501) staff       (20)        0 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/salt/annotation/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.464242 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      168 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)      166 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8892 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/nir.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8889 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/nir.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)      171 2022-02-01 19:33:00.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/observation.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3687 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/rss.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3697 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/rss.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     1375 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/salticam.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     1376 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/salticam.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8241 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/telescope.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8245 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/telescope.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)    12154 2022-04-10 10:06:48.000000 imephu-0.2.0/src/imephu/salt/annotation/nir.py
--rw-r--r--   0 christian   (501) staff       (20)     3860 2022-04-10 10:06:44.000000 imephu-0.2.0/src/imephu/salt/annotation/rss.py
--rw-r--r--   0 christian   (501) staff       (20)     1196 2022-04-10 10:06:38.000000 imephu-0.2.0/src/imephu/salt/annotation/salticam.py
--rw-r--r--   0 christian   (501) staff       (20)     9025 2022-04-10 10:06:34.000000 imephu-0.2.0/src/imephu/salt/annotation/telescope.py
--rw-r--r--   0 christian   (501) staff       (20)    14796 2022-04-10 10:06:27.000000 imephu-0.2.0/src/imephu/salt/finder_chart.py
--rw-r--r--   0 christian   (501) staff       (20)     4859 2022-04-10 10:06:20.000000 imephu-0.2.0/src/imephu/salt/utils.py
--rw-r--r--   0 christian   (501) staff       (20)    10458 2022-04-10 10:02:05.000000 imephu-0.2.0/src/imephu/schema.json
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.467019 imephu-0.2.0/src/imephu/service/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.471611 imephu-0.2.0/src/imephu/service/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)     7558 2022-06-14 07:19:19.000000 imephu-0.2.0/src/imephu/service/__pycache__/horizons.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     7550 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/service/__pycache__/horizons.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)    14053 2023-05-03 18:57:10.000000 imephu-0.2.0/src/imephu/service/__pycache__/survey.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8529 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/service/__pycache__/survey.cpython-38.pyc
--rw-r--r--   0 christian   (501) staff       (20)     9473 2022-04-10 10:06:12.000000 imephu-0.2.0/src/imephu/service/horizons.py
--rw-r--r--   0 christian   (501) staff       (20)    14909 2023-05-03 18:55:18.000000 imephu-0.2.0/src/imephu/service/survey.py
--rw-r--r--   0 christian   (501) staff       (20)     3680 2022-04-10 10:06:07.000000 imephu-0.2.0/src/imephu/utils.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.360043 imephu-0.2.0/src/imephu.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)     1426 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     4470 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       42 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/entry_points.txt
--rw-r--r--   0 christian   (501) staff       (20)      161 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)        7 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/top_level.txt
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.476383 imephu-0.2.0/tests/
--rw-r--r--   0 christian   (501) staff       (20)    13797 2023-05-03 18:55:18.000000 imephu-0.2.0/tests/test_cli.py
--rw-r--r--   0 christian   (501) staff       (20)    11263 2023-05-03 18:55:19.000000 imephu-0.2.0/tests/test_finder_chart.py
--rw-r--r--   0 christian   (501) staff       (20)     2224 2022-02-11 15:02:42.000000 imephu-0.2.0/tests/test_geometry.py
--rw-r--r--   0 christian   (501) staff       (20)     4282 2022-04-10 10:02:27.000000 imephu-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.2.1/README.md
+-rw-r--r--   0        0        0      991 2023-07-10 14:47:42.724245 imephu-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      185 2023-07-10 14:47:42.735179 imephu-0.2.1/src/imephu/__init__.py
+-rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.2.1/src/imephu/annotation/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.2.1/src/imephu/annotation/general/__init__.py
+-rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.2.1/src/imephu/annotation/general/arrow.py
+-rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.2.1/src/imephu/annotation/general/circle.py
+-rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.2.1/src/imephu/annotation/general/crosshairs.py
+-rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.2.1/src/imephu/annotation/general/empty.py
+-rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.2.1/src/imephu/annotation/general/group.py
+-rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.2.1/src/imephu/annotation/general/line_path.py
+-rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.2.1/src/imephu/annotation/general/rectangle.py
+-rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.2.1/src/imephu/annotation/general/text.py
+-rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.2.1/src/imephu/annotation/motion.py
+-rw-r--r--   0        0        0    12039 2023-07-10 14:47:42.739506 imephu-0.2.1/src/imephu/cli.py
+-rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.2.1/src/imephu/finder_chart.py
+-rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.2.1/src/imephu/geometry.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.2.1/src/imephu/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.2.1/src/imephu/salt/annotation/__init__.py
+-rw-r--r--   0        0        0    12257 2023-07-10 14:47:42.740967 imephu-0.2.1/src/imephu/salt/annotation/nir.py
+-rw-r--r--   0        0        0     3859 2023-07-10 14:47:42.741179 imephu-0.2.1/src/imephu/salt/annotation/rss.py
+-rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.2.1/src/imephu/salt/annotation/salticam.py
+-rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.2.1/src/imephu/salt/annotation/telescope.py
+-rw-r--r--   0        0        0    14802 2023-07-10 14:47:42.741868 imephu-0.2.1/src/imephu/salt/finder_chart.py
+-rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.2.1/src/imephu/salt/utils.py
+-rw-r--r--   0        0        0    10458 2023-07-10 14:47:42.742329 imephu-0.2.1/src/imephu/schema.json
+-rw-r--r--   0        0        0     9472 2023-07-10 14:47:42.742725 imephu-0.2.1/src/imephu/service/horizons.py
+-rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.2.1/src/imephu/service/survey.py
+-rw-r--r--   0        0        0     3680 2023-07-10 14:47:42.743218 imephu-0.2.1/src/imephu/utils.py
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.2.1/PKG-INFO
```

### Comparing `imephu-0.2.0/LICENSE` & `imephu-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/README.md` & `imephu-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/__pycache__/finder_chart.cpython-310.pyc` & `imephu-0.2.1/src/imephu/finder_chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,754 +1,807 @@
-00000000: 6f0d 0d0a 0000 0000 16ae 5264 8b32 0000  o.........Rd.2..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0173 1401 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 5a04 6400 6403 6c05 6d05 5a05 0100 6400  Z.d.d.l.m.Z...d.
-00000060: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
-00000070: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
-00000080: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
-00000090: 6d11 5a11 0100 6400 6402 6c12 6d13 5a14  m.Z...d.d.l.m.Z.
-000000a0: 0100 6400 6406 6c15 6d16 5a17 0100 6400  ..d.d.l.m.Z...d.
-000000b0: 6407 6c18 6d19 5a19 6d1a 5a1a 0100 6400  d.l.m.Z.m.Z...d.
-000000c0: 6408 6c1b 6d1c 5a1c 0100 6400 6409 6c1d  d.l.m.Z...d.d.l.
-000000d0: 6d1e 5a1e 0100 6400 640a 6c1f 6d20 5a20  m.Z...d.d.l.m Z 
-000000e0: 0100 6400 640b 6c21 6d22 5a22 0100 6400  ..d.d.l!m"Z"..d.
-000000f0: 640c 6c23 6d24 5a24 6d25 5a25 0100 6400  d.l#m$Z$m%Z%..d.
-00000100: 640d 6c26 6d27 5a27 0100 6400 640e 6c28  d.l&m'Z'..d.d.l(
-00000110: 6d29 5a29 0100 6400 640f 6c2a 6d2b 5a2b  m)Z)..d.d.l*m+Z+
-00000120: 0100 6400 6410 6c2c 6d2d 5a2d 0100 0900  ..d.d.l,m-Z-....
-00000130: 4700 6411 6412 8400 6412 8302 5a2e 6402  G.d.d...d...Z.d.
-00000140: 5300 2913 e900 0000 0029 01da 0b61 6e6e  S.)......)...ann
-00000150: 6f74 6174 696f 6e73 4e29 01da 0864 6174  otationsN)...dat
-00000160: 6574 696d 6529 01da 0742 7974 6573 494f  etime)...BytesIO
-00000170: 2909 da03 416e 79da 0842 696e 6172 7949  )...Any..BinaryI
-00000180: 4fda 0843 616c 6c61 626c 65da 0444 6963  O..Callable..Dic
-00000190: 74da 0947 656e 6572 6174 6f72 da04 4c69  t..Generator..Li
-000001a0: 7374 da08 4f70 7469 6f6e 616c da05 5475  st..Optional..Tu
-000001b0: 706c 65da 0555 6e69 6f6e 2901 da05 756e  ple..Union)...un
-000001c0: 6974 7329 02da 0541 6e67 6c65 da08 536b  its)...Angle..Sk
-000001d0: 7943 6f6f 7264 2901 da04 6669 7473 2901  yCoord)...fits).
-000001e0: da1c 4173 796d 6d65 7472 6963 5065 7263  ..AsymmetricPerc
-000001f0: 656e 7469 6c65 496e 7465 7276 616c 2901  entileInterval).
-00000200: da0b 7369 6d70 6c65 5f6e 6f72 6d29 01da  ..simple_norm)..
-00000210: 0e57 4353 4178 6573 5375 6270 6c6f 7429  .WCSAxesSubplot)
-00000220: 02da 0357 4353 da10 4649 5453 4669 7865  ...WCS..FITSFixe
-00000230: 6457 6172 6e69 6e67 2901 da06 4669 6775  dWarning)...Figu
-00000240: 7265 2901 da0a 416e 6e6f 7461 7469 6f6e  re)...Annotation
-00000250: 2901 da09 6c6f 6164 5f66 6974 7329 01da  )...load_fits)..
-00000260: 0945 7068 656d 6572 6973 6300 0000 0000  .Ephemerisc.....
-00000270: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00000280: 0000 0173 9c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000290: 6401 5a03 643c 6404 6405 8404 5a04 6505  d.Z.d<d.d...Z.e.
-000002a0: 643d 640e 640f 8404 8301 5a06 6505 643e  d=d.d.....Z.e.d>
-000002b0: 6419 641a 8404 8301 5a07 6508 643f 641c  d.d.....Z.e.d?d.
-000002c0: 641d 8404 8301 5a09 6440 6421 6422 8404  d.....Z.d@d!d"..
-000002d0: 5a0a 6508 6441 6424 6425 8404 8301 5a0b  Z.e.dAd$d%....Z.
-000002e0: 6442 6429 642a 8404 5a0c 6443 642b 642c  dBd)d*..Z.dCd+d,
-000002f0: 8404 5a0d 092d 6444 6445 6431 6432 8405  ..Z..-dDdEd1d2..
-00000300: 5a0e 6446 6434 6435 8404 5a0f 6447 6438  Z.dFd4d5..Z.dGd8
-00000310: 6439 8404 5a10 6447 643a 643b 8404 5a11  d9..Z.dGd:d;..Z.
-00000320: 642d 5300 2948 da0b 4669 6e64 6572 4368  d-S.)H..FinderCh
-00000330: 6172 7461 ad02 0000 4120 6669 6e64 6572  arta....A finder
-00000340: 2063 6861 7274 2066 6f72 2061 6e20 6173   chart for an as
-00000350: 7472 6f6e 6f6d 6963 616c 206f 6273 6572  tronomical obser
-00000360: 7661 7469 6f6e 2e0a 0a20 2020 2054 6865  vation...    The
-00000370: 2066 696e 6465 7220 6368 6172 7420 6973   finder chart is
-00000380: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
-00000390: 6120 4649 5453 2066 696c 652e 2042 7920  a FITS file. By 
-000003a0: 6465 6661 756c 7420 7468 6520 6669 6e64  default the find
-000003b0: 6572 2063 6861 7274 206a 7573 740a 2020  er chart just.  
-000003c0: 2020 7368 6f77 7320 7468 6520 7265 6769    shows the regi
-000003d0: 6f6e 2077 6974 6820 616e 206f 7665 726c  on with an overl
-000003e0: 6169 6420 636f 6f72 6469 6e61 7465 2067  aid coordinate g
-000003f0: 7269 642e 2054 6865 2061 7865 7320 7368  rid. The axes sh
-00000400: 6f77 2057 4353 2063 6f6f 7264 696e 6174  ow WCS coordinat
-00000410: 6573 2e0a 2020 2020 5573 6520 7468 6520  es..    Use the 
-00000420: 6061 6464 5f61 6e6e 6f74 6174 696f 6e60  `add_annotation`
-00000430: 206d 6574 686f 6420 746f 2061 6464 206d   method to add m
-00000440: 6f72 6520 636f 6e74 656e 7420 746f 2074  ore content to t
-00000450: 6865 2066 696e 6465 7220 6368 6172 742e  he finder chart.
-00000460: 0a0a 2020 2020 596f 7520 6361 6e20 6469  ..    You can di
-00000470: 7370 6c61 7920 7468 6520 6669 6e64 6572  splay the finder
-00000480: 2063 6861 7274 206f 6e20 7468 6520 7363   chart on the sc
-00000490: 7265 656e 206f 7220 7361 7665 2069 7420  reen or save it 
-000004a0: 6173 2061 2066 696c 652e 0a0a 2020 2020  as a file...    
-000004b0: 5468 6973 2063 6c61 7373 2075 7365 7320  This class uses 
-000004c0: 4d61 7470 6c6f 746c 6962 2066 6f72 2067  Matplotlib for g
-000004d0: 656e 6572 6174 696e 6720 7468 6520 6669  enerating the fi
-000004e0: 6e64 6572 2063 6861 7274 2e0a 0a20 2020  nder chart...   
-000004f0: 202e 2e20 7761 726e 696e 673a 3a20 4265   .. warning:: Be
-00000500: 2063 6172 6566 756c 2077 6865 6e20 776f   careful when wo
-00000510: 726b 696e 6720 7769 7468 2073 6576 6572  rking with sever
-00000520: 616c 2066 696e 6465 7220 6368 6172 7473  al finder charts
-00000530: 2061 7320 616c 6c20 7468 6520 6669 6e64   as all the find
-00000540: 6572 0a20 2020 2020 2020 6368 6172 7473  er.       charts
-00000550: 2075 7365 2074 6865 2073 616d 6520 4d61   use the same Ma
-00000560: 7470 6c6f 746c 6962 2066 6967 7572 652e  tplotlib figure.
-00000570: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000580: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00000590: 2020 2020 6e61 6d65 3a20 6073 7472 602c      name: `str`,
-000005a0: 2060 7061 7468 2d6c 696b 6560 206f 7220   `path-like` or 
-000005b0: 6062 696e 6172 7920 6669 6c65 2d6c 696b  `binary file-lik
-000005c0: 6560 0a20 2020 2020 2020 2046 4954 5320  e`.        FITS 
-000005d0: 6669 6c65 2074 6f20 6469 7370 6c61 792e  file to display.
-000005e0: 0a20 2020 20da 046e 616d 65fa 2655 6e69  .    ..name.&Uni
-000005f0: 6f6e 5b73 7472 2c20 4269 6e61 7279 494f  on[str, BinaryIO
-00000600: 2c20 6f73 2e50 6174 684c 696b 655b 416e  , os.PathLike[An
-00000610: 795d 5d63 0200 0000 0000 0000 0000 0000  y]]c............
-00000620: 0200 0000 0800 0000 4300 0001 736e 0000  ........C...sn..
-00000630: 0074 00a0 017c 01a1 0164 0119 007c 005f  .t...|...d...|._
-00000640: 027c 006a 026a 037c 005f 0474 0583 007c  .|.j.j.|._.t...|
-00000650: 005f 0674 07a0 08a1 008f 1501 0074 076a  ._.t.........t.j
-00000660: 0964 0274 0a64 038d 0201 0074 0b7c 006a  .d.t.d.....t.|.j
-00000670: 0283 017c 005f 0c57 0064 0004 0004 0083  ...|._.W.d......
-00000680: 0301 006e 0831 0073 2d77 0101 0001 0001  ...n.1.s-w......
-00000690: 0059 0001 0067 007c 005f 0d64 0053 0029  .Y...g.|._.d.S.)
-000006a0: 044e 7201 0000 00da 0669 676e 6f72 6529  .Nr......ignore)
-000006b0: 01da 0863 6174 6567 6f72 7929 0e72 1100  ...category).r..
-000006c0: 0000 da04 6f70 656e da04 5f68 6475 da04  ....open.._hdu..
-000006d0: 6461 7461 da05 5f64 6174 61da 0464 6963  data.._data..dic
-000006e0: 74da 095f 6d65 7461 6461 7461 da08 7761  t.._metadata..wa
-000006f0: 726e 696e 6773 da0e 6361 7463 685f 7761  rnings..catch_wa
-00000700: 726e 696e 6773 da0c 7369 6d70 6c65 6669  rnings..simplefi
-00000710: 6c74 6572 7216 0000 0072 1500 0000 da04  lterr....r......
-00000720: 5f77 6373 da0c 5f61 6e6e 6f74 6174 696f  _wcs.._annotatio
-00000730: 6e73 2902 da04 7365 6c66 721c 0000 00a9  ns)...selfr.....
-00000740: 0072 2c00 0000 fa3f 2f55 7365 7273 2f63  .r,....?/Users/c
-00000750: 6872 6973 7469 616e 2f49 6465 6150 726f  hristian/IdeaPro
-00000760: 6a65 6374 732f 696d 6570 6875 2f73 7263  jects/imephu/src
-00000770: 2f69 6d65 7068 752f 6669 6e64 6572 5f63  /imephu/finder_c
-00000780: 6861 7274 2e70 79da 085f 5f69 6e69 745f  hart.py..__init_
-00000790: 5f39 0000 0073 1000 0000 1001 0a03 0801  _9...s..........
-000007a0: 0a01 0e01 0e01 1cfe 0a03 7a14 4669 6e64  ..........z.Find
-000007b0: 6572 4368 6172 742e 5f5f 696e 6974 5f5f  erChart.__init__
-000007c0: da06 7375 7276 6579 da03 7374 72da 0b66  ..survey..str..f
-000007d0: 6974 735f 6365 6e74 6572 7210 0000 00da  its_centerr.....
-000007e0: 0473 697a 6572 0f00 0000 da06 7265 7475  .sizer......retu
-000007f0: 726e fa0d 2746 696e 6465 7243 6861 7274  rn..'FinderChart
-00000800: 2763 0300 0000 0000 0000 0000 0000 0400  'c..............
-00000810: 0000 0400 0000 4300 0001 7314 0000 0074  ......C...s....t
-00000820: 007c 007c 017c 0283 037d 0374 017c 0383  .|.|.|...}.t.|..
-00000830: 0153 0029 0161 a201 0000 4372 6561 7465  .S.).a....Create
-00000840: 2061 2066 696e 6465 7220 6368 6172 7420   a finder chart 
-00000850: 6672 6f6d 2061 2073 6b79 2073 7572 7665  from a sky surve
-00000860: 7920 4649 5453 2069 6d61 6765 2e0a 0a20  y FITS image... 
-00000870: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00000880: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00000890: 2d2d 2d2d 0a20 2020 2020 2020 2073 7572  ----.        sur
-000008a0: 7665 793a 2060 7374 7260 0a20 2020 2020  vey: `str`.     
-000008b0: 2020 2020 2020 2054 6865 206e 616d 6520         The name 
-000008c0: 6f66 2074 6865 2073 7572 7665 7920 746f  of the survey to
-000008d0: 2071 7565 7279 2066 6f72 2074 6865 2046   query for the F
-000008e0: 4954 5320 6669 6c65 2e0a 2020 2020 2020  ITS file..      
-000008f0: 2020 6669 7473 5f63 656e 7465 723a 2060    fits_center: `
-00000900: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
-00000910: 6174 6573 2e53 6b79 436f 6f72 6460 0a20  ates.SkyCoord`. 
-00000920: 2020 2020 2020 2020 2020 2054 6865 2063             The c
-00000930: 656e 7465 7220 706f 7369 7469 6f6e 206f  enter position o
-00000940: 6620 7468 6520 6c6f 6164 6564 2046 4954  f the loaded FIT
-00000950: 5320 6669 6c65 2e0a 2020 2020 2020 2020  S file..        
-00000960: 7369 7a65 3a20 607e 6173 7472 6f70 792e  size: `~astropy.
-00000970: 636f 6f72 6469 6e61 7465 732e 416e 676c  coordinates.Angl
-00000980: 6560 0a20 2020 2020 2020 2020 2020 2054  e`.            T
-00000990: 6865 2077 6964 7468 2061 6e64 2068 6569  he width and hei
-000009a0: 6768 7420 6f66 2074 6865 2046 4954 5320  ght of the FITS 
-000009b0: 6669 6c65 2069 6d61 6765 2c20 6173 2061  file image, as a
-000009c0: 6e20 616e 676c 6520 6f6e 2074 6865 2073  n angle on the s
-000009d0: 6b79 2e0a 2020 2020 2020 2020 2902 7219  ky..        ).r.
-000009e0: 0000 0072 1b00 0000 2904 722f 0000 0072  ...r....).r/...r
-000009f0: 3100 0000 7232 0000 005a 0a66 6974 735f  1...r2...Z.fits_
-00000a00: 696d 6167 6572 2c00 0000 722c 0000 0072  imager,...r,...r
-00000a10: 2d00 0000 da0b 6672 6f6d 5f73 7572 7665  -.....from_surve
-00000a20: 7944 0000 0073 0400 0000 0c0d 0801 7a17  yD...s........z.
-00000a30: 4669 6e64 6572 4368 6172 742e 6672 6f6d  FinderChart.from
-00000a40: 5f73 7572 7665 79da 0573 7461 7274 7203  _survey..startr.
-00000a50: 0000 00da 0365 6e64 da0b 6570 6865 6d65  .....end..epheme
-00000a60: 7269 6465 73fa 0f4c 6973 745b 4570 6865  rides..List[Ephe
-00000a70: 6d65 7269 735d da10 6d61 785f 7472 6163  meris]..max_trac
-00000a80: 6b5f 6c65 6e67 7468 da13 6372 6561 7465  k_length..create
-00000a90: 5f66 696e 6465 725f 6368 6172 74fa 2a43  _finder_chart.*C
-00000aa0: 616c 6c61 626c 655b 5b4c 6973 745b 4570  allable[[List[Ep
-00000ab0: 6865 6d65 7269 735d 5d2c 2027 4669 6e64  hemeris]], 'Find
-00000ac0: 6572 4368 6172 7427 5dfa 4647 656e 6572  erChart'].FGener
-00000ad0: 6174 6f72 5b54 7570 6c65 5b27 4669 6e64  ator[Tuple['Find
-00000ae0: 6572 4368 6172 7427 2c20 5475 706c 655b  erChart', Tuple[
-00000af0: 6461 7465 7469 6d65 2c20 6461 7465 7469  datetime, dateti
-00000b00: 6d65 5d5d 2c20 4e6f 6e65 2c20 4e6f 6e65  me]], None, None
-00000b10: 5d63 0500 0000 0000 0000 0000 0000 1000  ]c..............
-00000b20: 0000 0500 0000 6300 0001 73be 0100 0081  ......c...s.....
-00000b30: 007c 006a 0064 0175 0073 0e7c 006a 00a0  .|.j.d.u.s.|.j..
-00000b40: 0164 01a1 0164 0175 0072 1274 0264 0283  .d...d.u.r.t.d..
-00000b50: 0182 017c 016a 0064 0175 0073 1f7c 016a  ...|.j.d.u.s.|.j
-00000b60: 00a0 0164 01a1 0164 0175 0072 2374 0264  ...d...d.u.r#t.d
-00000b70: 0383 0182 017c 007c 016b 0572 2b74 0264  .....|.|.k.r+t.d
-00000b80: 0483 0182 017c 007c 0264 0519 006a 036b  .....|.|.d...j.k
-00000b90: 0072 3674 0264 0683 0182 017c 017c 0264  .r6t.d.....|.|.d
-00000ba0: 0719 006a 036b 0472 4174 0264 0883 0182  ...j.k.rAt.d....
-00000bb0: 017c 03a0 0474 056a 06a1 0164 056b 0172  .|...t.j...d.k.r
-00000bc0: 4d74 0264 0983 0182 0164 0a64 0b84 007c  Mt.d.....d.d...|
-00000bd0: 0244 0083 017d 0574 07a0 087c 057c 00a1  .D...}.t...|.|..
-00000be0: 0264 0c18 007d 0674 07a0 077c 057c 01a1  .d...}.t...|.|..
-00000bf0: 027d 077c 0764 056b 0472 727c 057c 0764  .}.|.d.k.rr|.|.d
-00000c00: 0c18 0019 007c 016b 0272 727c 0764 0c38  .....|.k.rr|.d.8
-00000c10: 007d 077c 067c 076b 0272 7a74 0264 0d83  .}.|.|.k.rzt.d..
-00000c20: 0182 017c 027c 0619 0067 017d 087c 0867  ...|.|...g.}.|.g
-00000c30: 017d 0974 097c 0664 0c17 007c 0764 0c17  .}.t.|.d...|.d..
-00000c40: 0083 0244 005d 337d 0a7c 027c 0a19 007d  ...D.]3}.|.|...}
-00000c50: 0b7c 0864 0719 006a 0aa0 0b7c 0b6a 0aa1  .|.d...j...|.j..
-00000c60: 017c 036b 0472 a074 0264 0e83 0182 017c  .|.k.r.t.d.....|
-00000c70: 0864 0519 006a 0aa0 0b7c 0b6a 0aa1 017d  .d...j...|.j...}
-00000c80: 0c7c 0c7c 036b 0172 b37c 08a0 0c7c 0ba1  .|.|.k.r.|...|..
-00000c90: 0101 0071 8b7c 0864 0719 007c 0b67 027d  ...q.|.d...|.g.}
-00000ca0: 087c 09a0 0c7c 08a1 0101 0071 8b7c 0944  .|...|.....q.|.D
-00000cb0: 005d 1b7d 0d7c 0d64 0519 006a 037c 0d64  .].}.|.d...j.|.d
-00000cc0: 0719 006a 0366 027d 0e7c 047c 0d83 017d  ...j.f.}.|.|...}
-00000cd0: 0f7c 0fa0 0d64 0f7c 0ea1 0201 007c 0f7c  .|...d.|.....|.|
-00000ce0: 0e66 0256 0001 0071 c164 0153 0029 1061  .f.V...q.d.S.).a
-00000cf0: 8008 0000 4372 6561 7465 2066 696e 6465  ....Create finde
-00000d00: 7220 6368 6172 7473 2066 6f72 2061 2074  r charts for a t
-00000d10: 696d 6520 696e 7465 7276 616c 2e0a 0a20  ime interval... 
-00000d20: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-00000d30: 6f64 2069 7320 696e 7465 6e64 6564 2066  od is intended f
-00000d40: 6f72 206e 6f6e 2d73 6964 6572 6561 6c20  or non-sidereal 
-00000d50: 7461 7267 6574 732c 2077 6869 6368 206d  targets, which m
-00000d60: 6179 2072 6571 7569 7265 206d 756c 7469  ay require multi
-00000d70: 706c 650a 2020 2020 2020 2020 6669 6e64  ple.        find
-00000d80: 6572 2063 6861 7274 7320 746f 2063 6f76  er charts to cov
-00000d90: 6572 2074 6865 6972 2074 7261 636b 206f  er their track o
-00000da0: 7665 7220 6120 7469 6d65 2069 6e74 6572  ver a time inter
-00000db0: 7661 6c2e 2049 7420 6372 6561 7465 7320  val. It creates 
-00000dc0: 6669 6e64 6572 0a20 2020 2020 2020 2063  finder.        c
-00000dd0: 6861 7274 7320 6163 636f 7264 696e 6720  harts according 
-00000de0: 746f 2074 6865 2066 6f6c 6c6f 7769 6e67  to the following
-00000df0: 2072 756c 6573 3a0a 0a20 2020 2020 2020   rules:..       
-00000e00: 202a 2054 616b 656e 2074 6f67 6574 6865   * Taken togethe
-00000e10: 722c 2074 6865 2066 696e 6465 7220 6368  r, the finder ch
-00000e20: 6172 7473 2063 6f76 6572 2074 6865 2077  arts cover the w
-00000e30: 686f 6c65 2074 696d 6520 696e 7465 7276  hole time interv
-00000e40: 616c 2e0a 2020 2020 2020 2020 2a20 5468  al..        * Th
-00000e50: 6520 7472 6163 6b20 6c65 6e67 7468 206f  e track length o
-00000e60: 6e20 6561 6368 2066 696e 6465 7220 6368  n each finder ch
-00000e70: 6172 7420 646f 6573 206e 6f74 2065 7863  art does not exc
-00000e80: 6565 6420 606d 6178 5f74 7261 636b 5f6c  eed `max_track_l
-00000e90: 656e 6774 6860 2e0a 2020 2020 2020 2020  ength`..        
-00000ea0: 2a20 4561 6368 2066 696e 6465 7220 6368  * Each finder ch
-00000eb0: 6172 7420 6973 2063 7265 6174 6564 2075  art is created u
-00000ec0: 7369 6e67 2060 6063 7265 6174 655f 6669  sing ``create_fi
-00000ed0: 6e64 6572 5f63 6861 7274 6060 2e0a 0a20  nder_chart``... 
-00000ee0: 2020 2020 2020 2054 6865 206d 6574 686f         The metho
-00000ef0: 6420 6973 2063 6f6d 706c 6574 656c 7920  d is completely 
-00000f00: 6167 6e6f 7374 6963 2061 7320 746f 2077  agnostic as to w
-00000f10: 6861 7420 6120 6669 6e64 6572 2063 6861  hat a finder cha
-00000f20: 7274 2073 686f 756c 6420 6c6f 6f6b 206c  rt should look l
-00000f30: 696b 653b 0a20 2020 2020 2020 2074 6869  ike;.        thi
-00000f40: 7320 6465 6369 7369 6f6e 2069 7320 6c65  s decision is le
-00000f50: 6674 2063 6f6d 706c 6574 656c 7920 746f  ft completely to
-00000f60: 2060 6063 7265 6174 655f 6669 6e64 6572   ``create_finder
-00000f70: 5f63 6861 7274 6060 2e20 496e 2070 6172  _chart``. In par
-00000f80: 7469 6375 6c61 722c 2069 660a 2020 2020  ticular, if.    
-00000f90: 2020 2020 796f 7520 6e65 6564 2061 6e79      you need any
-00000fa0: 2061 6e6e 6f74 6174 696f 6e73 2066 6f72   annotations for
-00000fb0: 2074 6865 206e 6f6e 2d73 6964 6572 6561   the non-siderea
-00000fc0: 6c20 6e61 7475 7265 2c20 6974 2069 7320  l nature, it is 
-00000fd0: 7570 2074 6f0a 2020 2020 2020 2020 6060  up to.        ``
-00000fe0: 6372 6561 7465 5f66 696e 6465 725f 6368  create_finder_ch
-00000ff0: 6172 7460 6020 746f 2070 726f 7669 6465  art`` to provide
-00001000: 2074 6865 6d2e 0a0a 2020 2020 2020 2020   them...        
-00001010: 5468 6520 6060 6372 6561 7465 5f66 696e  The ``create_fin
-00001020: 6465 725f 6368 6172 7460 6020 6675 6e63  der_chart`` func
-00001030: 7469 6f6e 2068 6173 2074 6f20 6163 6365  tion has to acce
-00001040: 7074 2061 7320 6974 7320 7369 6e67 6c65  pt as its single
-00001050: 2061 7267 756d 656e 7420 7468 650a 2020   argument the.  
-00001060: 2020 2020 2020 6c69 7374 206f 6620 6570        list of ep
-00001070: 6865 6d65 7269 6465 7320 746f 2069 6e63  hemerides to inc
-00001080: 6c75 6465 206f 6e20 7468 6520 6669 6e64  lude on the find
-00001090: 6572 2063 6861 7274 2e0a 0a20 2020 2020  er chart...     
-000010a0: 2020 2054 6865 2066 696e 6465 7220 6368     The finder ch
-000010b0: 6172 7473 2061 7265 2072 6574 7572 6e65  arts are returne
-000010c0: 6420 616c 6f6e 6720 7769 7468 2074 6865  d along with the
-000010d0: 2074 696d 6520 696e 7465 7276 616c 2074   time interval t
-000010e0: 6865 7920 636f 7665 722e 2054 6865 2074  hey cover. The t
-000010f0: 696d 650a 2020 2020 2020 2020 696e 7465  ime.        inte
-00001100: 7276 616c 2069 7320 616c 736f 2061 6464  rval is also add
-00001110: 6564 2061 7320 6120 7475 706c 6520 6f66  ed as a tuple of
-00001120: 2060 7e64 6174 6574 696d 652e 6461 7465   `~datetime.date
-00001130: 7469 6d65 6020 7661 6c75 6573 2077 6974  time` values wit
-00001140: 6820 7468 6520 6b65 790a 2020 2020 2020  h the key.      
-00001150: 2020 6060 7661 6c69 645f 666f 7260 6020    ``valid_for`` 
-00001160: 746f 2074 6865 2066 696e 6465 7220 6368  to the finder ch
-00001170: 6172 7427 7320 6d65 7461 6461 7461 2e0a  art's metadata..
-00001180: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00001190: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-000011a0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2073  ------.        s
-000011b0: 7461 7274 3a20 607e 6461 7465 7469 6d65  tart: `~datetime
-000011c0: 2e64 6174 6574 696d 6560 0a20 2020 2020  .datetime`.     
-000011d0: 2020 2020 2020 2054 6865 2073 7461 7274         The start
-000011e0: 2074 696d 6520 6f66 2074 6865 2069 6e74   time of the int
-000011f0: 6572 7661 6c20 746f 2062 6520 636f 7665  erval to be cove
-00001200: 7265 6420 6279 2074 6865 2066 696e 6465  red by the finde
-00001210: 7220 6368 6172 7473 2e20 5468 6973 206d  r charts. This m
-00001220: 7573 740a 2020 2020 2020 2020 2020 2020  ust.            
-00001230: 6265 2061 2074 696d 657a 6f6e 652d 6177  be a timezone-aw
-00001240: 6172 6520 6461 7465 7469 6d65 2e0a 2020  are datetime..  
-00001250: 2020 2020 2020 656e 643a 2060 7e64 6174        end: `~dat
-00001260: 6574 696d 652e 6461 7465 7469 6d65 600a  etime.datetime`.
-00001270: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001280: 656e 6420 7469 6d65 206f 6620 7468 6520  end time of the 
-00001290: 696e 7465 7276 616c 2074 6f20 6265 2063  interval to be c
-000012a0: 6f76 6572 6564 2062 7920 7468 6520 6669  overed by the fi
-000012b0: 6e64 6572 2063 6861 7274 732e 2054 6869  nder charts. Thi
-000012c0: 7320 6d75 7374 0a20 2020 2020 2020 2020  s must.         
-000012d0: 2020 2062 6520 6120 7469 6d65 7a6f 6e65     be a timezone
-000012e0: 2d61 7761 7265 2064 6174 6574 696d 652e  -aware datetime.
-000012f0: 0a20 2020 2020 2020 2065 7068 656d 6572  .        ephemer
-00001300: 6964 6573 3a20 6c69 7374 206f 6620 607e  ides: list of `~
-00001310: 696d 6570 6875 2e75 7469 6c73 2e45 7068  imephu.utils.Eph
-00001320: 656d 6572 6973 600a 2020 2020 2020 2020  emeris`.        
-00001330: 2020 2020 5468 6520 6c69 7374 206f 6620      The list of 
-00001340: 6570 6865 6d65 7269 6465 732e 2054 6865  ephemerides. The
-00001350: 2074 696d 6520 696e 7465 7276 616c 2066   time interval f
-00001360: 726f 6d20 6060 7374 6172 7460 6020 746f  rom ``start`` to
-00001370: 2060 6065 6e64 6060 206d 7573 7420 6265   ``end`` must be
-00001380: 0a20 2020 2020 2020 2020 2020 2066 756c  .            ful
-00001390: 6c79 2063 6f76 6572 6564 2062 7920 7468  ly covered by th
-000013a0: 6520 6570 6865 6d65 7269 6465 732e 0a20  e ephemerides.. 
-000013b0: 2020 2020 2020 206d 6178 5f74 7261 636b         max_track
-000013c0: 5f6c 656e 6774 683a 2066 6c6f 6174 0a20  _length: float. 
-000013d0: 2020 2020 2020 2020 2020 2054 6865 206d             The m
-000013e0: 6178 696d 756d 206c 656e 6774 6820 6120  aximum length a 
-000013f0: 7472 6163 6b20 6d61 7920 6861 7665 206f  track may have o
-00001400: 6e20 6120 6669 6e64 6572 2063 6861 7274  n a finder chart
-00001410: 2c20 6173 2061 6e20 616e 676c 6520 6f6e  , as an angle on
-00001420: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00001430: 2073 6b79 2e0a 2020 2020 2020 2020 6372   sky..        cr
-00001440: 6561 7465 5f66 696e 6465 725f 6368 6172  eate_finder_char
-00001450: 743a 2066 756e 6374 696f 6e0a 2020 2020  t: function.    
-00001460: 2020 2020 2020 2020 5468 6520 6675 6e63          The func
-00001470: 7469 6f6e 2066 6f72 2063 7265 6174 696e  tion for creatin
-00001480: 6720 6120 6669 6e64 6572 2063 6861 7274  g a finder chart
-00001490: 2066 726f 6d20 6120 6c69 7374 206f 6620   from a list of 
-000014a0: 6570 6865 6d65 7269 6465 732e 0a0a 2020  ephemerides...  
-000014b0: 2020 2020 2020 5969 656c 6473 0a20 2020        Yields.   
-000014c0: 2020 2020 202d 2d2d 2d2d 2d0a 2020 2020       ------.    
-000014d0: 2020 2020 7475 706c 6520 6f66 2061 2060      tuple of a `
-000014e0: 7e69 6d65 7068 752e 6669 6e64 6572 5f63  ~imephu.finder_c
-000014f0: 6861 7274 2e46 696e 6465 7243 6861 7274  hart.FinderChart
-00001500: 6020 616e 6420 6120 6461 7465 7469 6d65  ` and a datetime
-00001510: 2069 6e74 6572 7661 6c0a 2020 2020 2020   interval.      
-00001520: 2020 2020 2020 5468 6520 6765 6e65 7261        The genera
-00001530: 7465 6420 6669 6e64 6572 2063 6861 7274  ted finder chart
-00001540: 7320 616c 6f6e 6720 7769 7468 2074 6865  s along with the
-00001550: 2074 696d 6520 696e 7465 7276 616c 7320   time intervals 
-00001560: 7468 6579 2063 6f76 6572 2e0a 2020 2020  they cover..    
-00001570: 2020 2020 4e7a 2654 6865 2073 7461 7274      Nz&The start
-00001580: 2074 696d 6520 6d75 7374 2062 6520 7469   time must be ti
-00001590: 6d65 7a6f 6e65 2d61 7761 7265 2e7a 2454  mezone-aware.z$T
-000015a0: 6865 2065 6e64 2074 696d 6520 6d75 7374  he end time must
-000015b0: 2062 6520 7469 6d65 7a6f 6e65 2d61 7761   be timezone-awa
-000015c0: 7265 2e7a 3154 6865 2073 7461 7274 2074  re.z1The start t
-000015d0: 696d 6520 6d75 7374 2062 6520 6561 726c  ime must be earl
-000015e0: 6965 7220 7468 616e 2074 6865 2065 6e64  ier than the end
-000015f0: 2074 696d 652e 7201 0000 007a 3854 6865   time.r....z8The
-00001600: 2073 7461 7274 2074 696d 6520 6d75 7374   start time must
-00001610: 206e 6f74 2062 6520 6561 726c 6965 7220   not be earlier 
-00001620: 7468 616e 2074 6865 2066 6972 7374 2065  than the first e
-00001630: 706f 6368 2ee9 ffff ffff 7a33 5468 6520  poch......z3The 
-00001640: 656e 6420 7469 6d65 206d 7573 7420 6e6f  end time must no
-00001650: 7420 6265 206c 6174 6572 2074 6861 6e20  t be later than 
-00001660: 7468 6520 6c61 7374 2065 706f 6368 2e7a  the last epoch.z
-00001670: 2a54 6865 206d 6178 696d 756d 2074 7261  *The maximum tra
-00001680: 636b 206c 656e 6774 6820 6d75 7374 2062  ck length must b
-00001690: 6520 706f 7369 7469 7665 2e63 0100 0000  e positive.c....
-000016a0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000016b0: 5300 0001 7312 0000 0067 007c 005d 057d  S...s....g.|.].}
-000016c0: 017c 016a 0091 0271 0253 0072 2c00 0000  .|.j...q.S.r,...
-000016d0: 2901 da05 6570 6f63 6829 02da 022e 30da  )...epoch)....0.
-000016e0: 0165 722c 0000 0072 2c00 0000 722d 0000  .er,...r,...r-..
-000016f0: 00da 0a3c 6c69 7374 636f 6d70 3e9a 0000  ...<listcomp>...
-00001700: 0073 0200 0000 1200 7a31 4669 6e64 6572  .s......z1Finder
-00001710: 4368 6172 742e 666f 725f 7469 6d65 5f69  Chart.for_time_i
-00001720: 6e74 6572 7661 6c2e 3c6c 6f63 616c 733e  nterval.<locals>
-00001730: 2e3c 6c69 7374 636f 6d70 3ee9 0100 0000  .<listcomp>.....
-00001740: 7a28 5468 6520 696e 7465 7276 616c 206d  z(The interval m
-00001750: 7573 7420 6861 7665 2061 2070 6f73 6974  ust have a posit
-00001760: 6976 6520 6c65 6e67 7468 7a37 5468 6520  ive lengthz7The 
-00001770: 6d61 7869 6d75 6d20 7472 6163 6b20 6c65  maximum track le
-00001780: 6e67 7468 206f 6e20 6120 6669 6e64 6572  ngth on a finder
-00001790: 2063 6861 7274 2069 7320 6578 6365 6564   chart is exceed
-000017a0: 6564 2eda 0976 616c 6964 5f66 6f72 290e  ed...valid_for).
-000017b0: da06 747a 696e 666f da09 7574 636f 6666  ..tzinfo..utcoff
-000017c0: 7365 74da 0a56 616c 7565 4572 726f 7272  set..ValueErrorr
-000017d0: 3f00 0000 da08 746f 5f76 616c 7565 da01  ?.....to_value..
-000017e0: 75da 0661 7263 6d69 6eda 0662 6973 6563  u..arcmin..bisec
-000017f0: 74da 0c62 6973 6563 745f 7269 6768 74da  t..bisect_right.
-00001800: 0572 616e 6765 da08 706f 7369 7469 6f6e  .range..position
-00001810: da0a 7365 7061 7261 7469 6f6e da06 6170  ..separation..ap
-00001820: 7065 6e64 da0c 6164 645f 6d65 7461 6461  pend..add_metada
-00001830: 7461 2910 7236 0000 0072 3700 0000 7238  ta).r6...r7...r8
-00001840: 0000 0072 3a00 0000 723b 0000 005a 0961  ...r:...r;...Z.a
-00001850: 6c6c 5f74 696d 6573 5a0b 7374 6172 745f  ll_timesZ.start_
-00001860: 696e 6465 78da 0965 6e64 5f69 6e64 6578  index..end_index
-00001870: 5a0d 6375 7272 656e 745f 6772 6f75 70da  Z.current_group.
-00001880: 0667 726f 7570 73da 0169 5a0e 6e65 7874  .groups..iZ.next
-00001890: 5f65 7068 656d 6572 6973 5a0c 7472 6163  _ephemerisZ.trac
-000018a0: 6b5f 6c65 6e67 7468 da05 6772 6f75 7072  k_length..groupr
-000018b0: 4400 0000 da0c 6669 6e64 6572 5f63 6861  D.....finder_cha
-000018c0: 7274 722c 0000 0072 2c00 0000 722d 0000  rtr,...r,...r-..
-000018d0: 00da 1166 6f72 5f74 696d 655f 696e 7465  ...for_time_inte
-000018e0: 7276 616c 5400 0000 7352 0000 0002 801a  rvalT...sR......
-000018f0: 3508 011a 0108 0108 0208 010e 0208 010e  5...............
-00001900: 0108 0110 0208 010e 0310 010c 0118 0108  ................
-00001910: 0108 0308 010a 0506 0116 0108 0110 0302  ................
-00001920: 0104 ff02 0302 0104 ff12 0308 010c 010c  ................
-00001930: 020c 0108 0314 0108 010c 010c 0104 fc7a  ...............z
-00001940: 1d46 696e 6465 7243 6861 7274 2e66 6f72  .FinderChart.for
-00001950: 5f74 696d 655f 696e 7465 7276 616c 7215  _time_intervalr.
-00001960: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001970: 0100 0000 0200 0000 4300 0001 f30a 0000  ........C.......
-00001980: 007c 006a 00a0 01a1 0053 0029 017a a952  .|.j.....S.).z.R
-00001990: 6574 7572 6e20 6120 6465 6570 2063 6f70  eturn a deep cop
-000019a0: 7920 6f66 2074 6865 2057 4353 206f 626a  y of the WCS obj
-000019b0: 6563 7420 6f66 2074 6865 2066 696e 6465  ect of the finde
-000019c0: 7220 6368 6172 742e 0a0a 2020 2020 2020  r chart...      
-000019d0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-000019e0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-000019f0: 2020 607e 6173 7472 6f70 792e 7763 732e    `~astropy.wcs.
-00001a00: 5743 5360 0a20 2020 2020 2020 2020 2020  WCS`.           
-00001a10: 2041 2064 6565 7020 636f 7079 206f 6620   A deep copy of 
-00001a20: 7468 6520 5743 5320 6f62 6a65 6374 2e0a  the WCS object..
-00001a30: 2020 2020 2020 2020 2902 7229 0000 00da          ).r)....
-00001a40: 0864 6565 7063 6f70 79a9 0172 2b00 0000  .deepcopy..r+...
-00001a50: 722c 0000 0072 2c00 0000 722d 0000 00da  r,...r,...r-....
-00001a60: 0377 6373 c100 0000 7302 0000 000a 097a  .wcs....s......z
-00001a70: 0f46 696e 6465 7243 6861 7274 2e77 6373  .FinderChart.wcs
-00001a80: da0a 616e 6e6f 7461 7469 6f6e 7218 0000  ..annotationr...
-00001a90: 00da 044e 6f6e 6563 0200 0000 0000 0000  ...Nonec........
-00001aa0: 0000 0000 0200 0000 0300 0000 4300 0001  ............C...
-00001ab0: 7310 0000 007c 006a 00a0 017c 01a1 0101  s....|.j...|....
-00001ac0: 0064 0153 0029 027a fc41 6464 2061 6e20  .d.S.).z.Add an 
-00001ad0: 616e 6e6f 7461 7469 6f6e 2074 6f20 7468  annotation to th
-00001ae0: 6520 6669 6e64 6572 2063 6861 7274 2e0a  e finder chart..
-00001af0: 0a20 2020 2020 2020 2041 6e6e 6f74 6174  .        Annotat
-00001b00: 696f 6e73 2077 696c 6c20 6265 2070 6c6f  ions will be plo
-00001b10: 7474 6564 206f 6e74 6f20 7468 6520 6669  tted onto the fi
-00001b20: 6e64 6572 2063 6861 7274 2069 6e20 7468  nder chart in th
-00001b30: 6520 6f72 6465 7220 7468 6579 2068 6176  e order they hav
-00001b40: 6520 6265 656e 0a20 2020 2020 2020 2061  e been.        a
-00001b50: 6464 6564 2e20 536f 2c20 666f 7220 6578  dded. So, for ex
-00001b60: 616d 706c 652c 2074 6865 2061 6e6e 6f74  ample, the annot
-00001b70: 6174 696f 6e20 6164 6465 6420 6c61 7374  ation added last
-00001b80: 2077 696c 6c20 6265 206f 7574 7075 7420   will be output 
-00001b90: 6f6e 2074 6f70 206f 6620 616c 6c0a 2020  on top of all.  
-00001ba0: 2020 2020 2020 7468 6520 6f74 6865 7220        the other 
-00001bb0: 616e 6e6f 7461 7469 6f6e 732e 0a20 2020  annotations..   
-00001bc0: 2020 2020 204e 2902 722a 0000 0072 5000       N).r*...rP.
-00001bd0: 0000 2902 722b 0000 0072 5c00 0000 722c  ..).r+...r\...r,
-00001be0: 0000 0072 2c00 0000 722d 0000 00da 0e61  ...r,...r-.....a
-00001bf0: 6464 5f61 6e6e 6f74 6174 696f 6ecc 0000  dd_annotation...
-00001c00: 0073 0200 0000 1007 7a1a 4669 6e64 6572  .s......z.Finder
-00001c10: 4368 6172 742e 6164 645f 616e 6e6f 7461  Chart.add_annota
-00001c20: 7469 6f6e fa0e 4469 6374 5b73 7472 2c20  tion..Dict[str, 
-00001c30: 416e 795d 6301 0000 0000 0000 0000 0000  Any]c...........
-00001c40: 0001 0000 0002 0000 0043 0000 0172 5800  .........C...rX.
-00001c50: 0000 2901 610b 0100 000a 2020 2020 2020  ..).a.....      
-00001c60: 2020 5265 7475 726e 2074 6865 206d 6574    Return the met
-00001c70: 6164 6174 6120 666f 7220 7468 6520 6669  adata for the fi
-00001c80: 6e64 6572 2063 6861 7274 2e0a 0a20 2020  nder chart...   
-00001c90: 2020 2020 204d 6574 6164 6174 6120 6361       Metadata ca
-00001ca0: 6e20 2062 6520 6164 6465 6420 7769 7468  n  be added with
-00001cb0: 2074 6865 2060 6164 645f 6d65 7461 6461   the `add_metada
-00001cc0: 7461 6020 6d65 7468 6f64 2e20 4120 7368  ta` method. A sh
-00001cd0: 616c 6c6f 7720 636f 7079 206f 6620 7468  allow copy of th
-00001ce0: 650a 2020 2020 2020 2020 6d65 7461 6461  e.        metada
-00001cf0: 7461 2069 7320 7265 7475 726e 6564 2e0a  ta is returned..
-00001d00: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00001d10: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00001d20: 0a20 2020 2020 2020 2064 6963 740a 2020  .        dict.  
-00001d30: 2020 2020 2020 2020 2020 5468 6520 6d65            The me
-00001d40: 7461 6461 7461 206f 6620 7468 6520 6669  tadata of the fi
-00001d50: 6e64 6572 2063 6861 7274 2e0a 2020 2020  nder chart..    
-00001d60: 2020 2020 2902 7225 0000 00da 0463 6f70      ).r%.....cop
-00001d70: 7972 5a00 0000 722c 0000 0072 2c00 0000  yrZ...r,...r,...
-00001d80: 722d 0000 00da 086d 6574 6164 6174 61d5  r-.....metadata.
-00001d90: 0000 0073 0200 0000 0a0d 7a14 4669 6e64  ...s......z.Find
-00001da0: 6572 4368 6172 742e 6d65 7461 6461 7461  erChart.metadata
-00001db0: da03 6b65 79da 0576 616c 7565 7205 0000  ..key..valuer...
-00001dc0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
-00001dd0: 0000 0300 0000 4300 0001 730e 0000 007c  ......C...s....|
-00001de0: 027c 006a 007c 013c 0064 0153 0029 0261  .|.j.|.<.d.S.).a
-00001df0: 2501 0000 0a20 2020 2020 2020 2041 6464  %....        Add
-00001e00: 2061 206b 6579 2d76 616c 7565 2074 6f20   a key-value to 
-00001e10: 7468 6520 6669 6e64 6572 2063 6861 7274  the finder chart
-00001e20: 2773 206d 6574 6164 6174 612e 0a0a 2020  's metadata...  
-00001e30: 2020 2020 2020 4966 2074 6865 206b 6579        If the key
-00001e40: 2065 7869 7374 7273 2069 6e20 7468 6520   existrs in the 
-00001e50: 6d65 7461 6461 7461 2061 6c72 6561 6479  metadata already
-00001e60: 2c20 7468 6520 6578 6973 7469 6e67 2076  , the existing v
-00001e70: 616c 7565 2066 6f72 2074 6865 206b 6579  alue for the key
-00001e80: 2069 730a 2020 2020 2020 2020 7265 706c   is.        repl
-00001e90: 6163 6564 2e0a 0a20 2020 2020 2020 2050  aced...        P
-00001ea0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00001eb0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00001ec0: 2020 2020 206b 6579 3a20 6073 7472 600a       key: `str`.
-00001ed0: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
-00001ee0: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
-00001ef0: 607e 7479 7069 6e67 2e41 6e79 600a 2020  `~typing.Any`.  
-00001f00: 2020 2020 2020 2020 2020 5661 6c75 652e            Value.
-00001f10: 0a20 2020 2020 2020 204e 2901 7225 0000  .        N).r%..
-00001f20: 0029 0372 2b00 0000 7262 0000 0072 6300  .).r+...rb...rc.
-00001f30: 0000 722c 0000 0072 2c00 0000 722d 0000  ..r,...r,...r-..
-00001f40: 0072 5100 0000 e400 0000 7302 0000 000e  .rQ.......s.....
-00001f50: 0e7a 1846 696e 6465 7243 6861 7274 2e61  .z.FinderChart.a
-00001f60: 6464 5f6d 6574 6164 6174 6163 0100 0000  dd_metadatac....
-00001f70: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001f80: 4300 0001 731e 0000 007c 00a0 00a1 007d  C...s....|.....}
-00001f90: 0174 01a0 02a1 0001 0074 01a0 037c 01a1  .t.......t...|..
-00001fa0: 0101 0064 0153 0029 027a 2744 6973 706c  ...d.S.).z'Displ
-00001fb0: 6179 2074 6865 2066 696e 6465 7220 6368  ay the finder ch
-00001fc0: 6172 7420 6f6e 2074 6865 2073 6372 6565  art on the scree
-00001fd0: 6e2e 4e29 04da 0c5f 6372 6561 7465 5f70  n.N)..._create_p
-00001fe0: 6c6f 74da 0370 6c74 da04 7368 6f77 da05  lot..plt..show..
-00001ff0: 636c 6f73 6529 0272 2b00 0000 da06 6669  close).r+.....fi
-00002000: 6775 7265 722c 0000 0072 2c00 0000 722d  gurer,...r,...r-
-00002010: 0000 0072 6600 0000 f400 0000 7306 0000  ...rf.......s...
-00002020: 0008 0208 010e 017a 1046 696e 6465 7243  .......z.FinderC
-00002030: 6861 7274 2e73 686f 774e fa3a 556e 696f  hart.showN.:Unio
-00002040: 6e5b 7374 722c 2042 696e 6172 7949 4f2c  n[str, BinaryIO,
-00002050: 206f 732e 5061 7468 4c69 6b65 5b73 7472   os.PathLike[str
-00002060: 5d2c 206f 732e 5061 7468 4c69 6b65 5b62  ], os.PathLike[b
-00002070: 7974 6573 5d5d da06 666f 726d 6174 fa0d  ytes]]..format..
-00002080: 4f70 7469 6f6e 616c 5b73 7472 5d63 0300  Optional[str]c..
-00002090: 0000 0000 0000 0000 0000 0600 0000 0800  ................
-000020a0: 0000 4300 0001 73a0 0000 007c 00a0 00a1  ..C...s....|....
-000020b0: 007d 037c 0272 417c 02a0 01a1 0064 016b  .}.|.rA|.....d.k
-000020c0: 0272 4174 0283 007d 0474 036a 047c 047c  .rAt...}.t.j.|.|
-000020d0: 0264 0264 038d 0301 0074 057c 0164 0483  .d.d.....t.|.d..
-000020e0: 0272 247c 01a0 067c 04a0 07a1 00a1 0101  .r$|...|........
-000020f0: 006e 2574 087c 0164 0583 028f 0f7d 057c  .n%t.|.d.....}.|
-00002100: 05a0 067c 04a0 07a1 00a1 0101 0057 0064  ...|.........W.d
-00002110: 0604 0004 0083 0301 006e 0831 0073 3b77  .........n.1.s;w
-00002120: 0101 0001 0001 0059 0001 006e 0874 036a  .......Y...n.t.j
-00002130: 047c 017c 0264 0264 038d 0301 0074 03a0  .|.|.d.d.....t..
-00002140: 097c 03a1 0101 0064 0653 0029 0761 4702  .|.....d.S.).aG.
-00002150: 0000 5361 7665 2074 6865 2066 696e 6465  ..Save the finde
-00002160: 7220 6368 6172 7420 696e 2061 2066 696c  r chart in a fil
-00002170: 652e 0a0a 2020 2020 2020 2020 4966 2060  e...        If `
-00002180: 666f 726d 6174 6020 6973 206e 6f74 2073  format` is not s
-00002190: 6574 2c20 7468 6520 6669 6c65 2065 7874  et, the file ext
-000021a0: 656e 7369 6f6e 206f 6620 606e 616d 6560  ension of `name`
-000021b0: 2069 7320 7573 6564 2074 6f20 6669 6775   is used to figu
-000021c0: 7265 206f 7574 2074 6865 0a20 2020 2020  re out the.     
-000021d0: 2020 2066 696c 6520 6f72 2c20 6966 2074     file or, if t
-000021e0: 6865 7265 2069 7320 6e6f 2065 7874 656e  here is no exten
-000021f0: 7369 6f6e 2c20 4d61 7470 6c6f 746c 6962  sion, Matplotlib
-00002200: 2773 2064 6566 6175 6c74 2069 7320 7573  's default is us
-00002210: 6564 2e20 5365 650a 2020 2020 2020 2020  ed. See.        
-00002220: 4d61 7470 6c6f 746c 6962 2773 2060 6d61  Matplotlib's `ma
-00002230: 7470 6c6f 746c 6962 2e70 7970 6c6f 742e  tplotlib.pyplot.
-00002240: 7361 7665 6669 6760 2066 756e 6374 696f  savefig` functio
-00002250: 6e20 666f 7220 6d6f 7265 2064 6574 6169  n for more detai
-00002260: 6c73 2072 6567 6172 6469 6e67 0a20 2020  ls regarding.   
-00002270: 2020 2020 2074 6865 2066 6f72 6d61 742e       the format.
-00002280: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00002290: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-000022a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000022b0: 6e61 6d65 3a20 6073 7472 602c 2060 7061  name: `str`, `pa
-000022c0: 7468 2d6c 696b 6560 206f 7220 6062 696e  th-like` or `bin
-000022d0: 6172 7920 6669 6c65 2d6c 696b 6560 0a20  ary file-like`. 
-000022e0: 2020 2020 2020 2020 2020 2054 6865 2066             The f
-000022f0: 696c 6520 746f 2077 6869 6368 2074 6865  ile to which the
-00002300: 2066 696e 6465 7220 6368 6172 7420 6973   finder chart is
-00002310: 2073 6176 6564 2e20 416e 2065 7869 7374   saved. An exist
-00002320: 696e 6720 6669 6c65 2069 7320 7265 706c  ing file is repl
-00002330: 6163 6564 2e0a 2020 2020 2020 2020 666f  aced..        fo
-00002340: 726d 6174 3a20 6073 7472 602c 206f 7074  rmat: `str`, opt
-00002350: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-00002360: 2020 5468 6520 666f 726d 6174 2069 6e20    The format in 
-00002370: 7768 6963 6820 746f 2073 746f 7265 2074  which to store t
-00002380: 6865 2066 696e 6465 7220 6368 6172 742e  he finder chart.
-00002390: 0a20 2020 2020 2020 20da 0370 6466 da05  .        ..pdf..
-000023a0: 7469 6768 7429 0272 6a00 0000 5a0b 6262  tight).rj...Z.bb
-000023b0: 6f78 5f69 6e63 6865 73da 0577 7269 7465  ox_inches..write
-000023c0: da02 7762 4e29 0a72 6400 0000 da05 6c6f  ..wbN).rd.....lo
-000023d0: 7765 7272 0400 0000 7265 0000 005a 0773  werr....re...Z.s
-000023e0: 6176 6566 6967 da07 6861 7361 7474 7272  avefig..hasattrr
-000023f0: 6e00 0000 da08 6765 7476 616c 7565 7220  n.....getvaluer 
-00002400: 0000 0072 6700 0000 2906 722b 0000 0072  ...rg...).r+...r
-00002410: 1c00 0000 726a 0000 0072 6800 0000 726c  ....rj...rh...rl
-00002420: 0000 00da 0166 722c 0000 0072 2c00 0000  .....fr,...r,...
-00002430: 722d 0000 00da 0473 6176 65fa 0000 0073  r-.....save....s
-00002440: 1800 0000 0813 1001 0601 1001 0a01 1001  ................
-00002450: 0c02 1001 1cff 0280 1003 0e01 7a10 4669  ............z.Fi
-00002460: 6e64 6572 4368 6172 742e 7361 7665 7217  nderChart.saver.
-00002470: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00002480: 0400 0000 0500 0000 4300 0001 7358 0000  ........C...sX..
-00002490: 0074 006a 0164 0164 028d 017d 0174 006a  .t.j.d.d...}.t.j
-000024a0: 027c 006a 0364 038d 017d 027c 00a0 047c  .|.j.d...}.|...|
-000024b0: 02a1 0101 007c 00a0 057c 02a1 0101 007c  .....|...|.....|
-000024c0: 026a 0664 0464 0564 0664 078d 0301 007c  .j.d.d.d.d.....|
-000024d0: 006a 0744 005d 077d 037c 03a0 087c 02a1  .j.D.].}.|...|..
-000024e0: 0101 0071 227c 0153 0029 084e 2902 e90a  ...q"|.S.).N)...
-000024f0: 0000 00e9 0900 0000 2901 da07 6669 6773  ........)...figs
-00002500: 697a 6529 015a 0a70 726f 6a65 6374 696f  ize).Z.projectio
-00002510: 6e54 da04 626c 7565 679a 9999 9999 99c9  nT..blueg.......
-00002520: 3f29 02da 0563 6f6c 6f72 da05 616c 7068  ?)...color..alph
-00002530: 6129 0972 6500 0000 7268 0000 005a 0773  a).re...rh...Z.s
-00002540: 7562 706c 6f74 7229 0000 00da 115f 6164  ubplotr)....._ad
-00002550: 645f 6669 7473 5f63 6f6e 7465 6e74 da0c  d_fits_content..
-00002560: 5f75 7064 6174 655f 6178 6573 da04 6772  _update_axes..gr
-00002570: 6964 722a 0000 005a 0661 6464 5f74 6f29  idr*...Z.add_to)
-00002580: 0472 2b00 0000 7268 0000 00da 0261 7872  .r+...rh.....axr
-00002590: 5c00 0000 722c 0000 0072 2c00 0000 722d  \...r,...r,...r-
-000025a0: 0000 0072 6400 0000 1a01 0000 7310 0000  ...rd.......s...
-000025b0: 000c 010e 010a 020a 0110 020a 020c 0104  ................
-000025c0: 027a 1846 696e 6465 7243 6861 7274 2e5f  .z.FinderChart._
-000025d0: 6372 6561 7465 5f70 6c6f 7472 7e00 0000  create_plotr~...
-000025e0: 7214 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000025f0: 0000 0900 0000 0800 0000 4300 0001 7384  ..........C...s.
-00002600: 0000 0074 006a 01a0 0264 01a1 017d 0264  ...t.j...d...}.d
-00002610: 027d 0364 037d 0474 037c 037c 0464 0464  .}.d.}.t.|.|.d.d
-00002620: 058d 037d 057c 05a0 047c 006a 056a 06a1  ...}.|...|.j.j..
-00002630: 015c 027d 067d 0764 067c 077c 0618 0014  .\.}.}.d.|.|....
-00002640: 007c 0617 007d 0664 077c 077c 0618 0014  .|...}.d.|.|....
-00002650: 007c 0717 007d 0774 077c 006a 0864 087c  .|...}.t.|.j.d.|
-00002660: 067c 0764 098d 047d 087c 016a 097c 006a  .|.d...}.|.j.|.j
-00002670: 056a 067c 0264 0a64 0b7c 0864 0c64 0d8d  .j.|.d.d.|.d.d..
-00002680: 0601 0064 0e53 0029 0f7a 6b0a 2020 2020  ...d.S.).zk.    
-00002690: 2020 2020 2041 6464 2063 6f6e 7465 6e74       Add content
-000026a0: 206f 6620 7468 6520 4649 5453 2066 696c   of the FITS fil
-000026b0: 6520 746f 2074 6865 2070 6c6f 742e 0a0a  e to the plot...
-000026c0: 2020 2020 2020 2020 5468 6520 636f 6465          The code
-000026d0: 2068 6173 2062 6565 6e20 6164 6170 7465   has been adapte
-000026e0: 6420 6672 6f6d 2041 504c 7079 2e0a 2020  d from APLpy..  
-000026f0: 2020 2020 2020 da09 6769 7374 5f79 6172        ..gist_yar
-00002700: 6767 0000 0000 0000 d03f 6700 0000 0000  gg.......?g.....
-00002710: f058 4069 1027 0000 2901 5a09 6e5f 7361  .X@i.'..).Z.n_sa
-00002720: 6d70 6c65 7367 9a99 9999 9999 b9bf 679a  mplesg........g.
-00002730: 9999 9999 99b9 3fe9 0200 0000 2903 da05  ......?.....)...
-00002740: 706f 7765 725a 076d 696e 5f63 7574 5a07  powerZ.min_cutZ.
-00002750: 6d61 785f 6375 74da 076e 6561 7265 7374  max_cut..nearest
-00002760: 7270 0000 00da 0565 7175 616c 2905 da04  rp.....equal)...
-00002770: 636d 6170 da0d 696e 7465 7270 6f6c 6174  cmap..interpolat
-00002780: 696f 6eda 066f 7269 6769 6eda 046e 6f72  ion..origin..nor
-00002790: 6dda 0661 7370 6563 744e 290a 7265 0000  m..aspectN).re..
-000027a0: 00da 0263 6dda 0867 6574 5f63 6d61 7072  ...cm..get_cmapr
-000027b0: 1200 0000 5a0a 6765 745f 6c69 6d69 7473  ....Z.get_limits
-000027c0: 7221 0000 0072 2200 0000 7213 0000 0072  r!...r"...r....r
-000027d0: 2300 0000 5a06 696d 7368 6f77 2909 722b  #...Z.imshow).r+
-000027e0: 0000 0072 7e00 0000 7284 0000 005a 0470  ...r~...r....Z.p
-000027f0: 6d69 6e5a 0470 6d61 78da 0869 6e74 6572  minZ.pmax..inter
-00002800: 7661 6cda 0476 6d69 6eda 0476 6d61 785a  val..vmin..vmaxZ
-00002810: 0a6e 6f72 6d61 6c69 7a65 7272 2c00 0000  .normalizerr,...
-00002820: 722c 0000 0072 2d00 0000 727b 0000 0028  r,...r-...r{...(
-00002830: 0100 0073 2000 0000 0c06 0403 0401 0e01  ...s ...........
-00002840: 1201 1001 1001 1202 0402 0601 0201 0201  ................
-00002850: 0201 0201 0201 0afa 7a1d 4669 6e64 6572  ........z.Finder
-00002860: 4368 6172 742e 5f61 6464 5f66 6974 735f  Chart._add_fits_
-00002870: 636f 6e74 656e 7463 0200 0000 0000 0000  contentc........
-00002880: 0000 0000 0800 0000 0400 0000 4300 0001  ............C...
-00002890: 73a2 0000 0064 0164 0264 039c 027d 027c  s....d.d.d...}.|
-000028a0: 006a 006a 017d 037c 0364 0419 007d 047c  .j.j.}.|.d...}.|
-000028b0: 0364 0519 007d 057c 0464 066b 0372 1974  .d...}.|.d.k.r.t
-000028c0: 0264 0783 0182 017c 0564 086b 0372 2174  .d.....|.d.k.r!t
-000028d0: 0264 0983 0182 017c 016a 0364 0419 007d  .d.....|.j.d...}
-000028e0: 067c 016a 0364 0519 007d 077c 06a0 047c  .|.j.d...}.|...|
-000028f0: 027c 0419 00a1 0101 007c 07a0 047c 027c  .|.......|...|.|
-00002900: 0519 00a1 0101 007c 06a0 0564 0aa1 0101  .......|...d....
-00002910: 007c 07a0 0564 0aa1 0101 007c 066a 0664  .|...d.....|.j.d
-00002920: 0b64 0c8d 0101 007c 076a 0664 0b64 0c8d  .d.....|.j.d.d..
-00002930: 0101 0064 0053 0029 0d4e 7a0a 4465 6320  ...d.S.).Nz.Dec 
-00002940: 2849 4352 5329 7a09 5241 2028 4943 5253  (ICRS)z.RA (ICRS
-00002950: 2929 02fa 0a70 6f73 2e65 712e 6465 63fa  ))...pos.eq.dec.
-00002960: 0970 6f73 2e65 712e 7261 7201 0000 0072  .pos.eq.rar....r
-00002970: 4300 0000 728f 0000 007a 494f 6e6c 7920  C...r....zIOnly 
-00002980: 706f 732e 6571 2e72 6120 6973 2073 7570  pos.eq.ra is sup
-00002990: 706f 7274 6564 2066 6f72 2074 6865 2070  ported for the p
-000029a0: 6879 7369 6361 6c20 7479 7065 206f 6620  hysical type of 
-000029b0: 7468 6520 6669 7273 7420 776f 726c 6420  the first world 
-000029c0: 6178 6973 728e 0000 007a 4b4f 6e6c 7920  axisr....zKOnly 
-000029d0: 706f 732e 6571 2e64 6563 2069 7320 7375  pos.eq.dec is su
-000029e0: 7070 6f72 7465 6420 666f 7220 7468 6520  pported for the 
-000029f0: 7068 7973 6963 616c 2074 7970 6520 6f66  physical type of
-00002a00: 2074 6865 2073 6563 6f6e 6420 776f 726c   the second worl
-00002a10: 6420 6178 6973 54e9 0700 0000 2901 7232  d axisT.....).r2
-00002a20: 0000 0029 0772 2900 0000 5a19 776f 726c  ...).r)...Z.worl
-00002a30: 645f 6178 6973 5f70 6879 7369 6361 6c5f  d_axis_physical_
-00002a40: 7479 7065 7372 4700 0000 da06 636f 6f72  typesrG.....coor
-00002a50: 6473 5a0d 7365 745f 6178 6973 6c61 6265  dsZ.set_axislabe
-00002a60: 6c5a 1364 6973 706c 6179 5f6d 696e 6f72  lZ.display_minor
-00002a70: 5f74 6963 6b73 5a09 7365 745f 7469 636b  _ticksZ.set_tick
-00002a80: 7329 0872 2b00 0000 727e 0000 005a 0f61  s).r+...r~...Z.a
-00002a90: 7869 735f 7479 7065 5f6e 616d 6573 5a0a  xis_type_namesZ.
-00002aa0: 6178 6973 5f74 7970 6573 5a0b 785f 6178  axis_typesZ.x_ax
-00002ab0: 6973 5f74 7970 655a 0b79 5f61 7869 735f  is_typeZ.y_axis_
-00002ac0: 7479 7065 da01 78da 0179 722c 0000 0072  type..x..yr,...r
-00002ad0: 2c00 0000 722d 0000 0072 7c00 0000 4301  ,...r-...r|...C.
-00002ae0: 0000 732c 0000 0002 0202 0106 fe08 0408  ..s,............
-00002af0: 0108 0108 0102 0102 0104 ff08 0402 0102  ................
-00002b00: 0104 ff0a 050a 010e 010e 010a 020a 010c  ................
-00002b10: 0210 017a 1846 696e 6465 7243 6861 7274  ...z.FinderChart
-00002b20: 2e5f 7570 6461 7465 5f61 7865 7329 0272  ._update_axes).r
-00002b30: 1c00 0000 721d 0000 0029 0872 2f00 0000  ....r....).r/...
-00002b40: 7230 0000 0072 3100 0000 7210 0000 0072  r0...r1...r....r
-00002b50: 3200 0000 720f 0000 0072 3300 0000 7234  2...r....r3...r4
-00002b60: 0000 0029 0c72 3600 0000 7203 0000 0072  ...).r6...r....r
-00002b70: 3700 0000 7203 0000 0072 3800 0000 7239  7...r....r8...r9
-00002b80: 0000 0072 3a00 0000 720f 0000 0072 3b00  ...r:...r....r;.
-00002b90: 0000 723c 0000 0072 3300 0000 723d 0000  ..r<...r3...r=..
-00002ba0: 0029 0272 3300 0000 7215 0000 0029 0472  .).r3...r....).r
-00002bb0: 5c00 0000 7218 0000 0072 3300 0000 725d  \...r....r3...r]
-00002bc0: 0000 0029 0272 3300 0000 725f 0000 0029  ...).r3...r_...)
-00002bd0: 0672 6200 0000 7230 0000 0072 6300 0000  .rb...r0...rc...
-00002be0: 7205 0000 0072 3300 0000 725d 0000 0029  r....r3...r]...)
-00002bf0: 0272 3300 0000 725d 0000 0029 014e 2906  .r3...r]...).N).
-00002c00: 721c 0000 0072 6900 0000 726a 0000 0072  r....ri...rj...r
-00002c10: 6b00 0000 7233 0000 0072 5d00 0000 2902  k...r3...r]...).
-00002c20: 7233 0000 0072 1700 0000 2904 727e 0000  r3...r....).r~..
-00002c30: 0072 1400 0000 7233 0000 0072 5d00 0000  .r....r3...r]...
-00002c40: 2912 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00002c50: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00002c60: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-00002c70: 2e00 0000 da0c 7374 6174 6963 6d65 7468  ......staticmeth
-00002c80: 6f64 7235 0000 0072 5700 0000 da08 7072  odr5...rW.....pr
-00002c90: 6f70 6572 7479 725b 0000 0072 5e00 0000  opertyr[...r^...
-00002ca0: 7261 0000 0072 5100 0000 7266 0000 0072  ra...rQ...rf...r
-00002cb0: 7400 0000 7264 0000 0072 7b00 0000 727c  t...rd...r{...r|
-00002cc0: 0000 0072 2c00 0000 722c 0000 0072 2c00  ...r,...r,...r,.
-00002cd0: 0000 722d 0000 0072 1b00 0000 2500 0000  ..r-...r....%...
-00002ce0: 7326 0000 0008 0004 010a 1302 0b0c 0102  s&..............
-00002cf0: 0f0c 0102 6c0c 010a 0a02 090c 010a 0e0a  ....l...........
-00002d00: 1002 090c fd0a 200a 0e0e 1b72 1b00 0000  ...... ....r....
-00002d10: 292f da0a 5f5f 6675 7475 7265 5f5f 7202  )/..__future__r.
-00002d20: 0000 0072 4b00 0000 da02 6f73 7226 0000  ...rK.....osr&..
-00002d30: 0072 0300 0000 da02 696f 7204 0000 00da  .r......ior.....
-00002d40: 0674 7970 696e 6772 0500 0000 7206 0000  .typingr....r...
-00002d50: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00002d60: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00002d70: 0d00 0000 da11 6d61 7470 6c6f 746c 6962  ......matplotlib
-00002d80: 2e70 7970 6c6f 74da 0670 7970 6c6f 7472  .pyplot..pyplotr
-00002d90: 6500 0000 da07 6173 7472 6f70 7972 0e00  e.....astropyr..
-00002da0: 0000 7249 0000 00da 1361 7374 726f 7079  ..rI.....astropy
-00002db0: 2e63 6f6f 7264 696e 6174 6573 720f 0000  .coordinatesr...
-00002dc0: 0072 1000 0000 da0a 6173 7472 6f70 792e  .r......astropy.
-00002dd0: 696f 7211 0000 005a 1e61 7374 726f 7079  ior....Z.astropy
-00002de0: 2e76 6973 7561 6c69 7a61 7469 6f6e 2e69  .visualization.i
-00002df0: 6e74 6572 7661 6c72 1200 0000 5a23 6173  ntervalr....Z#as
-00002e00: 7472 6f70 792e 7669 7375 616c 697a 6174  tropy.visualizat
-00002e10: 696f 6e2e 6d70 6c5f 6e6f 726d 616c 697a  ion.mpl_normaliz
-00002e20: 6572 1300 0000 5a22 6173 7472 6f70 792e  er....Z"astropy.
-00002e30: 7669 7375 616c 697a 6174 696f 6e2e 7763  visualization.wc
-00002e40: 7361 7865 732e 636f 7265 7214 0000 005a  saxes.corer....Z
-00002e50: 0b61 7374 726f 7079 2e77 6373 7215 0000  .astropy.wcsr...
-00002e60: 0072 1600 0000 5a11 6d61 7470 6c6f 746c  .r....Z.matplotl
-00002e70: 6962 2e66 6967 7572 6572 1700 0000 5a11  ib.figurer....Z.
-00002e80: 696d 6570 6875 2e61 6e6e 6f74 6174 696f  imephu.annotatio
-00002e90: 6e72 1800 0000 da15 696d 6570 6875 2e73  nr......imephu.s
-00002ea0: 6572 7669 6365 2e73 7572 7665 7972 1900  ervice.surveyr..
-00002eb0: 0000 da0c 696d 6570 6875 2e75 7469 6c73  ....imephu.utils
-00002ec0: 721a 0000 0072 1b00 0000 722c 0000 0072  r....r....r,...r
-00002ed0: 2c00 0000 722c 0000 0072 2d00 0000 da08  ,...r,...r-.....
-00002ee0: 3c6d 6f64 756c 653e 0100 0000 732a 0000  <module>....s*..
-00002ef0: 000c 0008 0208 0108 010c 010c 012c 010c  .............,..
-00002f00: 0c0c 0110 010c 010c 010c 010c 0110 010c  ................
-00002f10: 010c 020c 010c 0102 0212 03              ...........
+00000000: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
+00000010: 696d 706f 7274 2061 6e6e 6f74 6174 696f  import annotatio
+00000020: 6e73 0a0a 696d 706f 7274 2062 6973 6563  ns..import bisec
+00000030: 740a 696d 706f 7274 206f 730a 696d 706f  t.import os.impo
+00000040: 7274 2077 6172 6e69 6e67 730a 6672 6f6d  rt warnings.from
+00000050: 2064 6174 6574 696d 6520 696d 706f 7274   datetime import
+00000060: 2064 6174 6574 696d 650a 6672 6f6d 2069   datetime.from i
+00000070: 6f20 696d 706f 7274 2042 7974 6573 494f  o import BytesIO
+00000080: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000090: 6f72 7420 280a 2020 2020 416e 792c 0a20  ort (.    Any,. 
+000000a0: 2020 2042 696e 6172 7949 4f2c 0a20 2020     BinaryIO,.   
+000000b0: 2043 616c 6c61 626c 652c 0a20 2020 2044   Callable,.    D
+000000c0: 6963 742c 0a20 2020 2047 656e 6572 6174  ict,.    Generat
+000000d0: 6f72 2c0a 2020 2020 4c69 7374 2c0a 2020  or,.    List,.  
+000000e0: 2020 4f70 7469 6f6e 616c 2c0a 2020 2020    Optional,.    
+000000f0: 5475 706c 652c 0a20 2020 2055 6e69 6f6e  Tuple,.    Union
+00000100: 2c0a 290a 0a69 6d70 6f72 7420 6d61 7470  ,.)..import matp
+00000110: 6c6f 746c 6962 2e70 7970 6c6f 7420 6173  lotlib.pyplot as
+00000120: 2070 6c74 0a66 726f 6d20 6173 7472 6f70   plt.from astrop
+00000130: 7920 696d 706f 7274 2075 6e69 7473 2061  y import units a
+00000140: 7320 750a 6672 6f6d 2061 7374 726f 7079  s u.from astropy
+00000150: 2e63 6f6f 7264 696e 6174 6573 2069 6d70  .coordinates imp
+00000160: 6f72 7420 416e 676c 652c 2053 6b79 436f  ort Angle, SkyCo
+00000170: 6f72 640a 6672 6f6d 2061 7374 726f 7079  ord.from astropy
+00000180: 2e69 6f20 696d 706f 7274 2066 6974 730a  .io import fits.
+00000190: 6672 6f6d 2061 7374 726f 7079 2e76 6973  from astropy.vis
+000001a0: 7561 6c69 7a61 7469 6f6e 2e69 6e74 6572  ualization.inter
+000001b0: 7661 6c20 696d 706f 7274 2041 7379 6d6d  val import Asymm
+000001c0: 6574 7269 6350 6572 6365 6e74 696c 6549  etricPercentileI
+000001d0: 6e74 6572 7661 6c0a 6672 6f6d 2061 7374  nterval.from ast
+000001e0: 726f 7079 2e76 6973 7561 6c69 7a61 7469  ropy.visualizati
+000001f0: 6f6e 2e6d 706c 5f6e 6f72 6d61 6c69 7a65  on.mpl_normalize
+00000200: 2069 6d70 6f72 7420 7369 6d70 6c65 5f6e   import simple_n
+00000210: 6f72 6d0a 6672 6f6d 2061 7374 726f 7079  orm.from astropy
+00000220: 2e76 6973 7561 6c69 7a61 7469 6f6e 2e77  .visualization.w
+00000230: 6373 6178 6573 2e63 6f72 6520 696d 706f  csaxes.core impo
+00000240: 7274 2057 4353 4178 6573 5375 6270 6c6f  rt WCSAxesSubplo
+00000250: 740a 6672 6f6d 2061 7374 726f 7079 2e77  t.from astropy.w
+00000260: 6373 2069 6d70 6f72 7420 5743 532c 2046  cs import WCS, F
+00000270: 4954 5346 6978 6564 5761 726e 696e 670a  ITSFixedWarning.
+00000280: 6672 6f6d 206d 6174 706c 6f74 6c69 622e  from matplotlib.
+00000290: 6669 6775 7265 2069 6d70 6f72 7420 4669  figure import Fi
+000002a0: 6775 7265 0a0a 6672 6f6d 2069 6d65 7068  gure..from imeph
+000002b0: 752e 616e 6e6f 7461 7469 6f6e 2069 6d70  u.annotation imp
+000002c0: 6f72 7420 416e 6e6f 7461 7469 6f6e 0a66  ort Annotation.f
+000002d0: 726f 6d20 696d 6570 6875 2e73 6572 7669  rom imephu.servi
+000002e0: 6365 2e73 7572 7665 7920 696d 706f 7274  ce.survey import
+000002f0: 206c 6f61 645f 6669 7473 0a66 726f 6d20   load_fits.from 
+00000300: 696d 6570 6875 2e75 7469 6c73 2069 6d70  imephu.utils imp
+00000310: 6f72 7420 4570 6865 6d65 7269 730a 0a22  ort Ephemeris.."
+00000320: 2222 4120 6669 6e64 6572 2063 6861 7274  ""A finder chart
+00000330: 2e22 2222 0a0a 0a63 6c61 7373 2046 696e  ."""...class Fin
+00000340: 6465 7243 6861 7274 3a0a 2020 2020 2222  derChart:.    ""
+00000350: 2241 2066 696e 6465 7220 6368 6172 7420  "A finder chart 
+00000360: 666f 7220 616e 2061 7374 726f 6e6f 6d69  for an astronomi
+00000370: 6361 6c20 6f62 7365 7276 6174 696f 6e2e  cal observation.
+00000380: 0a0a 2020 2020 5468 6520 6669 6e64 6572  ..    The finder
+00000390: 2063 6861 7274 2069 7320 6765 6e65 7261   chart is genera
+000003a0: 7465 6420 6672 6f6d 2061 2046 4954 5320  ted from a FITS 
+000003b0: 6669 6c65 2e20 4279 2064 6566 6175 6c74  file. By default
+000003c0: 2074 6865 2066 696e 6465 7220 6368 6172   the finder char
+000003d0: 7420 6a75 7374 0a20 2020 2073 686f 7773  t just.    shows
+000003e0: 2074 6865 2072 6567 696f 6e20 7769 7468   the region with
+000003f0: 2061 6e20 6f76 6572 6c61 6964 2063 6f6f   an overlaid coo
+00000400: 7264 696e 6174 6520 6772 6964 2e20 5468  rdinate grid. Th
+00000410: 6520 6178 6573 2073 686f 7720 5743 5320  e axes show WCS 
+00000420: 636f 6f72 6469 6e61 7465 732e 0a20 2020  coordinates..   
+00000430: 2055 7365 2074 6865 2060 6164 645f 616e   Use the `add_an
+00000440: 6e6f 7461 7469 6f6e 6020 6d65 7468 6f64  notation` method
+00000450: 2074 6f20 6164 6420 6d6f 7265 2063 6f6e   to add more con
+00000460: 7465 6e74 2074 6f20 7468 6520 6669 6e64  tent to the find
+00000470: 6572 2063 6861 7274 2e0a 0a20 2020 2059  er chart...    Y
+00000480: 6f75 2063 616e 2064 6973 706c 6179 2074  ou can display t
+00000490: 6865 2066 696e 6465 7220 6368 6172 7420  he finder chart 
+000004a0: 6f6e 2074 6865 2073 6372 6565 6e20 6f72  on the screen or
+000004b0: 2073 6176 6520 6974 2061 7320 6120 6669   save it as a fi
+000004c0: 6c65 2e0a 0a20 2020 2054 6869 7320 636c  le...    This cl
+000004d0: 6173 7320 7573 6573 204d 6174 706c 6f74  ass uses Matplot
+000004e0: 6c69 6220 666f 7220 6765 6e65 7261 7469  lib for generati
+000004f0: 6e67 2074 6865 2066 696e 6465 7220 6368  ng the finder ch
+00000500: 6172 742e 0a0a 2020 2020 2e2e 2077 6172  art...    .. war
+00000510: 6e69 6e67 3a3a 2042 6520 6361 7265 6675  ning:: Be carefu
+00000520: 6c20 7768 656e 2077 6f72 6b69 6e67 2077  l when working w
+00000530: 6974 6820 7365 7665 7261 6c20 6669 6e64  ith several find
+00000540: 6572 2063 6861 7274 7320 6173 2061 6c6c  er charts as all
+00000550: 2074 6865 2066 696e 6465 720a 2020 2020   the finder.    
+00000560: 2020 2063 6861 7274 7320 7573 6520 7468     charts use th
+00000570: 6520 7361 6d65 204d 6174 706c 6f74 6c69  e same Matplotli
+00000580: 6220 6669 6775 7265 2e0a 0a20 2020 2050  b figure...    P
+00000590: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+000005a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 616d  --------.    nam
+000005b0: 653a 2060 7374 7260 2c20 6070 6174 682d  e: `str`, `path-
+000005c0: 6c69 6b65 6020 6f72 2060 6269 6e61 7279  like` or `binary
+000005d0: 2066 696c 652d 6c69 6b65 600a 2020 2020   file-like`.    
+000005e0: 2020 2020 4649 5453 2066 696c 6520 746f      FITS file to
+000005f0: 2064 6973 706c 6179 2e0a 2020 2020 2222   display..    ""
+00000600: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00000610: 745f 5f28 7365 6c66 2c20 6e61 6d65 3a20  t__(self, name: 
+00000620: 556e 696f 6e5b 7374 722c 2042 696e 6172  Union[str, Binar
+00000630: 7949 4f2c 206f 732e 5061 7468 4c69 6b65  yIO, os.PathLike
+00000640: 5b41 6e79 5d5d 293a 0a20 2020 2020 2020  [Any]]):.       
+00000650: 2073 656c 662e 5f68 6475 203d 2066 6974   self._hdu = fit
+00000660: 732e 6f70 656e 286e 616d 6529 5b30 5d0a  s.open(name)[0].
+00000670: 2020 2020 2020 2020 2320 5468 6520 4649          # The FI
+00000680: 5453 2064 6174 6120 6973 2072 6561 6420  TS data is read 
+00000690: 696e 206f 6e6c 7920 7768 656e 2069 7420  in only when it 
+000006a0: 6973 206e 6565 6465 642e 2054 6f20 6176  is needed. To av
+000006b0: 6f69 6420 7472 7969 6e67 2074 6f20 7265  oid trying to re
+000006c0: 6164 2066 726f 6d0a 2020 2020 2020 2020  ad from.        
+000006d0: 2320 6120 636c 6f73 6564 2073 7472 6561  # a closed strea
+000006e0: 6d20 6c61 7465 7220 6f6e 2c20 7765 2074  m later on, we t
+000006f0: 6875 7320 666f 7263 6520 7468 6520 6461  hus force the da
+00000700: 7461 2074 6f20 6265 2072 6561 6420 696e  ta to be read in
+00000710: 2069 6d6d 6564 6961 7465 6c79 2e0a 2020   immediately..  
+00000720: 2020 2020 2020 7365 6c66 2e5f 6461 7461        self._data
+00000730: 203d 2073 656c 662e 5f68 6475 2e64 6174   = self._hdu.dat
+00000740: 610a 2020 2020 2020 2020 7365 6c66 2e5f  a.        self._
+00000750: 6d65 7461 6461 7461 3a20 4469 6374 5b73  metadata: Dict[s
+00000760: 7472 2c20 416e 795d 203d 2064 6963 7428  tr, Any] = dict(
+00000770: 290a 2020 2020 2020 2020 7769 7468 2077  ).        with w
+00000780: 6172 6e69 6e67 732e 6361 7463 685f 7761  arnings.catch_wa
+00000790: 726e 696e 6773 2829 3a0a 2020 2020 2020  rnings():.      
+000007a0: 2020 2020 2020 7761 726e 696e 6773 2e73        warnings.s
+000007b0: 696d 706c 6566 696c 7465 7228 2269 676e  implefilter("ign
+000007c0: 6f72 6522 2c20 6361 7465 676f 7279 3d46  ore", category=F
+000007d0: 4954 5346 6978 6564 5761 726e 696e 6729  ITSFixedWarning)
+000007e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000007f0: 662e 5f77 6373 203d 2057 4353 2873 656c  f._wcs = WCS(sel
+00000800: 662e 5f68 6475 290a 2020 2020 2020 2020  f._hdu).        
+00000810: 7365 6c66 2e5f 616e 6e6f 7461 7469 6f6e  self._annotation
+00000820: 733a 204c 6973 745b 416e 6e6f 7461 7469  s: List[Annotati
+00000830: 6f6e 5d20 3d20 5b5d 0a0a 2020 2020 4073  on] = []..    @s
+00000840: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00000850: 6465 6620 6672 6f6d 5f73 7572 7665 7928  def from_survey(
+00000860: 7375 7276 6579 3a20 7374 722c 2066 6974  survey: str, fit
+00000870: 735f 6365 6e74 6572 3a20 536b 7943 6f6f  s_center: SkyCoo
+00000880: 7264 2c20 7369 7a65 3a20 416e 676c 6529  rd, size: Angle)
+00000890: 202d 3e20 2246 696e 6465 7243 6861 7274   -> "FinderChart
+000008a0: 223a 0a20 2020 2020 2020 2022 2222 4372  ":.        """Cr
+000008b0: 6561 7465 2061 2066 696e 6465 7220 6368  eate a finder ch
+000008c0: 6172 7420 6672 6f6d 2061 2073 6b79 2073  art from a sky s
+000008d0: 7572 7665 7920 4649 5453 2069 6d61 6765  urvey FITS image
+000008e0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+000008f0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00000900: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00000910: 2073 7572 7665 793a 2060 7374 7260 0a20   survey: `str`. 
+00000920: 2020 2020 2020 2020 2020 2054 6865 206e             The n
+00000930: 616d 6520 6f66 2074 6865 2073 7572 7665  ame of the surve
+00000940: 7920 746f 2071 7565 7279 2066 6f72 2074  y to query for t
+00000950: 6865 2046 4954 5320 6669 6c65 2e0a 2020  he FITS file..  
+00000960: 2020 2020 2020 6669 7473 5f63 656e 7465        fits_cente
+00000970: 723a 2060 7e61 7374 726f 7079 2e63 6f6f  r: `~astropy.coo
+00000980: 7264 696e 6174 6573 2e53 6b79 436f 6f72  rdinates.SkyCoor
+00000990: 6460 0a20 2020 2020 2020 2020 2020 2054  d`.            T
+000009a0: 6865 2063 656e 7465 7220 706f 7369 7469  he center positi
+000009b0: 6f6e 206f 6620 7468 6520 6c6f 6164 6564  on of the loaded
+000009c0: 2046 4954 5320 6669 6c65 2e0a 2020 2020   FITS file..    
+000009d0: 2020 2020 7369 7a65 3a20 607e 6173 7472      size: `~astr
+000009e0: 6f70 792e 636f 6f72 6469 6e61 7465 732e  opy.coordinates.
+000009f0: 416e 676c 6560 0a20 2020 2020 2020 2020  Angle`.         
+00000a00: 2020 2054 6865 2077 6964 7468 2061 6e64     The width and
+00000a10: 2068 6569 6768 7420 6f66 2074 6865 2046   height of the F
+00000a20: 4954 5320 6669 6c65 2069 6d61 6765 2c20  ITS file image, 
+00000a30: 6173 2061 6e20 616e 676c 6520 6f6e 2074  as an angle on t
+00000a40: 6865 2073 6b79 2e0a 2020 2020 2020 2020  he sky..        
+00000a50: 2222 220a 2020 2020 2020 2020 6669 7473  """.        fits
+00000a60: 5f69 6d61 6765 203d 206c 6f61 645f 6669  _image = load_fi
+00000a70: 7473 2873 7572 7665 792c 2066 6974 735f  ts(survey, fits_
+00000a80: 6365 6e74 6572 2c20 7369 7a65 290a 2020  center, size).  
+00000a90: 2020 2020 2020 7265 7475 726e 2046 696e        return Fin
+00000aa0: 6465 7243 6861 7274 2866 6974 735f 696d  derChart(fits_im
+00000ab0: 6167 6529 0a0a 2020 2020 4073 7461 7469  age)..    @stati
+00000ac0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00000ad0: 666f 725f 7469 6d65 5f69 6e74 6572 7661  for_time_interva
+00000ae0: 6c28 0a20 2020 2020 2020 2073 7461 7274  l(.        start
+00000af0: 3a20 6461 7465 7469 6d65 2c0a 2020 2020  : datetime,.    
+00000b00: 2020 2020 656e 643a 2064 6174 6574 696d      end: datetim
+00000b10: 652c 0a20 2020 2020 2020 2065 7068 656d  e,.        ephem
+00000b20: 6572 6964 6573 3a20 4c69 7374 5b45 7068  erides: List[Eph
+00000b30: 656d 6572 6973 5d2c 0a20 2020 2020 2020  emeris],.       
+00000b40: 206d 6178 5f74 7261 636b 5f6c 656e 6774   max_track_lengt
+00000b50: 683a 2041 6e67 6c65 2c0a 2020 2020 2020  h: Angle,.      
+00000b60: 2020 6372 6561 7465 5f66 696e 6465 725f    create_finder_
+00000b70: 6368 6172 743a 2043 616c 6c61 626c 655b  chart: Callable[
+00000b80: 5b4c 6973 745b 4570 6865 6d65 7269 735d  [List[Ephemeris]
+00000b90: 5d2c 2022 4669 6e64 6572 4368 6172 7422  ], "FinderChart"
+00000ba0: 5d2c 0a20 2020 2029 202d 3e20 4765 6e65  ],.    ) -> Gene
+00000bb0: 7261 746f 725b 5475 706c 655b 2246 696e  rator[Tuple["Fin
+00000bc0: 6465 7243 6861 7274 222c 2054 7570 6c65  derChart", Tuple
+00000bd0: 5b64 6174 6574 696d 652c 2064 6174 6574  [datetime, datet
+00000be0: 696d 655d 5d2c 204e 6f6e 652c 204e 6f6e  ime]], None, Non
+00000bf0: 655d 3a0a 2020 2020 2020 2020 2222 2243  e]:.        """C
+00000c00: 7265 6174 6520 6669 6e64 6572 2063 6861  reate finder cha
+00000c10: 7274 7320 666f 7220 6120 7469 6d65 2069  rts for a time i
+00000c20: 6e74 6572 7661 6c2e 0a0a 2020 2020 2020  nterval...      
+00000c30: 2020 5468 6973 206d 6574 686f 6420 6973    This method is
+00000c40: 2069 6e74 656e 6465 6420 666f 7220 6e6f   intended for no
+00000c50: 6e2d 7369 6465 7265 616c 2074 6172 6765  n-sidereal targe
+00000c60: 7473 2c20 7768 6963 6820 6d61 7920 7265  ts, which may re
+00000c70: 7175 6972 6520 6d75 6c74 6970 6c65 0a20  quire multiple. 
+00000c80: 2020 2020 2020 2066 696e 6465 7220 6368         finder ch
+00000c90: 6172 7473 2074 6f20 636f 7665 7220 7468  arts to cover th
+00000ca0: 6569 7220 7472 6163 6b20 6f76 6572 2061  eir track over a
+00000cb0: 2074 696d 6520 696e 7465 7276 616c 2e20   time interval. 
+00000cc0: 4974 2063 7265 6174 6573 2066 696e 6465  It creates finde
+00000cd0: 720a 2020 2020 2020 2020 6368 6172 7473  r.        charts
+00000ce0: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
+00000cf0: 6520 666f 6c6c 6f77 696e 6720 7275 6c65  e following rule
+00000d00: 733a 0a0a 2020 2020 2020 2020 2a20 5461  s:..        * Ta
+00000d10: 6b65 6e20 746f 6765 7468 6572 2c20 7468  ken together, th
+00000d20: 6520 6669 6e64 6572 2063 6861 7274 7320  e finder charts 
+00000d30: 636f 7665 7220 7468 6520 7768 6f6c 6520  cover the whole 
+00000d40: 7469 6d65 2069 6e74 6572 7661 6c2e 0a20  time interval.. 
+00000d50: 2020 2020 2020 202a 2054 6865 2074 7261         * The tra
+00000d60: 636b 206c 656e 6774 6820 6f6e 2065 6163  ck length on eac
+00000d70: 6820 6669 6e64 6572 2063 6861 7274 2064  h finder chart d
+00000d80: 6f65 7320 6e6f 7420 6578 6365 6564 2060  oes not exceed `
+00000d90: 6d61 785f 7472 6163 6b5f 6c65 6e67 7468  max_track_length
+00000da0: 602e 0a20 2020 2020 2020 202a 2045 6163  `..        * Eac
+00000db0: 6820 6669 6e64 6572 2063 6861 7274 2069  h finder chart i
+00000dc0: 7320 6372 6561 7465 6420 7573 696e 6720  s created using 
+00000dd0: 6060 6372 6561 7465 5f66 696e 6465 725f  ``create_finder_
+00000de0: 6368 6172 7460 602e 0a0a 2020 2020 2020  chart``...      
+00000df0: 2020 5468 6520 6d65 7468 6f64 2069 7320    The method is 
+00000e00: 636f 6d70 6c65 7465 6c79 2061 676e 6f73  completely agnos
+00000e10: 7469 6320 6173 2074 6f20 7768 6174 2061  tic as to what a
+00000e20: 2066 696e 6465 7220 6368 6172 7420 7368   finder chart sh
+00000e30: 6f75 6c64 206c 6f6f 6b20 6c69 6b65 3b0a  ould look like;.
+00000e40: 2020 2020 2020 2020 7468 6973 2064 6563          this dec
+00000e50: 6973 696f 6e20 6973 206c 6566 7420 636f  ision is left co
+00000e60: 6d70 6c65 7465 6c79 2074 6f20 6060 6372  mpletely to ``cr
+00000e70: 6561 7465 5f66 696e 6465 725f 6368 6172  eate_finder_char
+00000e80: 7460 602e 2049 6e20 7061 7274 6963 756c  t``. In particul
+00000e90: 6172 2c20 6966 0a20 2020 2020 2020 2079  ar, if.        y
+00000ea0: 6f75 206e 6565 6420 616e 7920 616e 6e6f  ou need any anno
+00000eb0: 7461 7469 6f6e 7320 666f 7220 7468 6520  tations for the 
+00000ec0: 6e6f 6e2d 7369 6465 7265 616c 206e 6174  non-sidereal nat
+00000ed0: 7572 652c 2069 7420 6973 2075 7020 746f  ure, it is up to
+00000ee0: 0a20 2020 2020 2020 2060 6063 7265 6174  .        ``creat
+00000ef0: 655f 6669 6e64 6572 5f63 6861 7274 6060  e_finder_chart``
+00000f00: 2074 6f20 7072 6f76 6964 6520 7468 656d   to provide them
+00000f10: 2e0a 0a20 2020 2020 2020 2054 6865 2060  ...        The `
+00000f20: 6063 7265 6174 655f 6669 6e64 6572 5f63  `create_finder_c
+00000f30: 6861 7274 6060 2066 756e 6374 696f 6e20  hart`` function 
+00000f40: 6861 7320 746f 2061 6363 6570 7420 6173  has to accept as
+00000f50: 2069 7473 2073 696e 676c 6520 6172 6775   its single argu
+00000f60: 6d65 6e74 2074 6865 0a20 2020 2020 2020  ment the.       
+00000f70: 206c 6973 7420 6f66 2065 7068 656d 6572   list of ephemer
+00000f80: 6964 6573 2074 6f20 696e 636c 7564 6520  ides to include 
+00000f90: 6f6e 2074 6865 2066 696e 6465 7220 6368  on the finder ch
+00000fa0: 6172 742e 0a0a 2020 2020 2020 2020 5468  art...        Th
+00000fb0: 6520 6669 6e64 6572 2063 6861 7274 7320  e finder charts 
+00000fc0: 6172 6520 7265 7475 726e 6564 2061 6c6f  are returned alo
+00000fd0: 6e67 2077 6974 6820 7468 6520 7469 6d65  ng with the time
+00000fe0: 2069 6e74 6572 7661 6c20 7468 6579 2063   interval they c
+00000ff0: 6f76 6572 2e20 5468 6520 7469 6d65 0a20  over. The time. 
+00001000: 2020 2020 2020 2069 6e74 6572 7661 6c20         interval 
+00001010: 6973 2061 6c73 6f20 6164 6465 6420 6173  is also added as
+00001020: 2061 2074 7570 6c65 206f 6620 607e 6461   a tuple of `~da
+00001030: 7465 7469 6d65 2e64 6174 6574 696d 6560  tetime.datetime`
+00001040: 2076 616c 7565 7320 7769 7468 2074 6865   values with the
+00001050: 206b 6579 0a20 2020 2020 2020 2060 6076   key.        ``v
+00001060: 616c 6964 5f66 6f72 6060 2074 6f20 7468  alid_for`` to th
+00001070: 6520 6669 6e64 6572 2063 6861 7274 2773  e finder chart's
+00001080: 206d 6574 6164 6174 612e 0a0a 2020 2020   metadata...    
+00001090: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000010a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000010b0: 2d0a 2020 2020 2020 2020 7374 6172 743a  -.        start:
+000010c0: 2060 7e64 6174 6574 696d 652e 6461 7465   `~datetime.date
+000010d0: 7469 6d65 600a 2020 2020 2020 2020 2020  time`.          
+000010e0: 2020 5468 6520 7374 6172 7420 7469 6d65    The start time
+000010f0: 206f 6620 7468 6520 696e 7465 7276 616c   of the interval
+00001100: 2074 6f20 6265 2063 6f76 6572 6564 2062   to be covered b
+00001110: 7920 7468 6520 6669 6e64 6572 2063 6861  y the finder cha
+00001120: 7274 732e 2054 6869 7320 6d75 7374 0a20  rts. This must. 
+00001130: 2020 2020 2020 2020 2020 2062 6520 6120             be a 
+00001140: 7469 6d65 7a6f 6e65 2d61 7761 7265 2064  timezone-aware d
+00001150: 6174 6574 696d 652e 0a20 2020 2020 2020  atetime..       
+00001160: 2065 6e64 3a20 607e 6461 7465 7469 6d65   end: `~datetime
+00001170: 2e64 6174 6574 696d 6560 0a20 2020 2020  .datetime`.     
+00001180: 2020 2020 2020 2054 6865 2065 6e64 2074         The end t
+00001190: 696d 6520 6f66 2074 6865 2069 6e74 6572  ime of the inter
+000011a0: 7661 6c20 746f 2062 6520 636f 7665 7265  val to be covere
+000011b0: 6420 6279 2074 6865 2066 696e 6465 7220  d by the finder 
+000011c0: 6368 6172 7473 2e20 5468 6973 206d 7573  charts. This mus
+000011d0: 740a 2020 2020 2020 2020 2020 2020 6265  t.            be
+000011e0: 2061 2074 696d 657a 6f6e 652d 6177 6172   a timezone-awar
+000011f0: 6520 6461 7465 7469 6d65 2e0a 2020 2020  e datetime..    
+00001200: 2020 2020 6570 6865 6d65 7269 6465 733a      ephemerides:
+00001210: 206c 6973 7420 6f66 2060 7e69 6d65 7068   list of `~imeph
+00001220: 752e 7574 696c 732e 4570 6865 6d65 7269  u.utils.Ephemeri
+00001230: 7360 0a20 2020 2020 2020 2020 2020 2054  s`.            T
+00001240: 6865 206c 6973 7420 6f66 2065 7068 656d  he list of ephem
+00001250: 6572 6964 6573 2e20 5468 6520 7469 6d65  erides. The time
+00001260: 2069 6e74 6572 7661 6c20 6672 6f6d 2060   interval from `
+00001270: 6073 7461 7274 6060 2074 6f20 6060 656e  `start`` to ``en
+00001280: 6460 6020 6d75 7374 2062 650a 2020 2020  d`` must be.    
+00001290: 2020 2020 2020 2020 6675 6c6c 7920 636f          fully co
+000012a0: 7665 7265 6420 6279 2074 6865 2065 7068  vered by the eph
+000012b0: 656d 6572 6964 6573 2e0a 2020 2020 2020  emerides..      
+000012c0: 2020 6d61 785f 7472 6163 6b5f 6c65 6e67    max_track_leng
+000012d0: 7468 3a20 666c 6f61 740a 2020 2020 2020  th: float.      
+000012e0: 2020 2020 2020 5468 6520 6d61 7869 6d75        The maximu
+000012f0: 6d20 6c65 6e67 7468 2061 2074 7261 636b  m length a track
+00001300: 206d 6179 2068 6176 6520 6f6e 2061 2066   may have on a f
+00001310: 696e 6465 7220 6368 6172 742c 2061 7320  inder chart, as 
+00001320: 616e 2061 6e67 6c65 206f 6e20 7468 650a  an angle on the.
+00001330: 2020 2020 2020 2020 2020 2020 736b 792e              sky.
+00001340: 0a20 2020 2020 2020 2063 7265 6174 655f  .        create_
+00001350: 6669 6e64 6572 5f63 6861 7274 3a20 6675  finder_chart: fu
+00001360: 6e63 7469 6f6e 0a20 2020 2020 2020 2020  nction.         
+00001370: 2020 2054 6865 2066 756e 6374 696f 6e20     The function 
+00001380: 666f 7220 6372 6561 7469 6e67 2061 2066  for creating a f
+00001390: 696e 6465 7220 6368 6172 7420 6672 6f6d  inder chart from
+000013a0: 2061 206c 6973 7420 6f66 2065 7068 656d   a list of ephem
+000013b0: 6572 6964 6573 2e0a 0a20 2020 2020 2020  erides...       
+000013c0: 2059 6965 6c64 730a 2020 2020 2020 2020   Yields.        
+000013d0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2074  ------.        t
+000013e0: 7570 6c65 206f 6620 6120 607e 696d 6570  uple of a `~imep
+000013f0: 6875 2e66 696e 6465 725f 6368 6172 742e  hu.finder_chart.
+00001400: 4669 6e64 6572 4368 6172 7460 2061 6e64  FinderChart` and
+00001410: 2061 2064 6174 6574 696d 6520 696e 7465   a datetime inte
+00001420: 7276 616c 0a20 2020 2020 2020 2020 2020  rval.           
+00001430: 2054 6865 2067 656e 6572 6174 6564 2066   The generated f
+00001440: 696e 6465 7220 6368 6172 7473 2061 6c6f  inder charts alo
+00001450: 6e67 2077 6974 6820 7468 6520 7469 6d65  ng with the time
+00001460: 2069 6e74 6572 7661 6c73 2074 6865 7920   intervals they 
+00001470: 636f 7665 722e 0a20 2020 2020 2020 2022  cover..        "
+00001480: 2222 0a20 2020 2020 2020 2023 2054 6865  "".        # The
+00001490: 2073 7461 7274 2061 6e64 2065 6e64 2074   start and end t
+000014a0: 696d 6520 6d75 7374 2062 6520 7469 6d65  ime must be time
+000014b0: 7a6f 6e65 2d61 7761 7265 0a20 2020 2020  zone-aware.     
+000014c0: 2020 2069 6620 7374 6172 742e 747a 696e     if start.tzin
+000014d0: 666f 2069 7320 4e6f 6e65 206f 7220 7374  fo is None or st
+000014e0: 6172 742e 747a 696e 666f 2e75 7463 6f66  art.tzinfo.utcof
+000014f0: 6673 6574 284e 6f6e 6529 2069 7320 4e6f  fset(None) is No
+00001500: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00001510: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00001520: 2822 5468 6520 7374 6172 7420 7469 6d65  ("The start time
+00001530: 206d 7573 7420 6265 2074 696d 657a 6f6e   must be timezon
+00001540: 652d 6177 6172 652e 2229 0a20 2020 2020  e-aware.").     
+00001550: 2020 2069 6620 656e 642e 747a 696e 666f     if end.tzinfo
+00001560: 2069 7320 4e6f 6e65 206f 7220 656e 642e   is None or end.
+00001570: 747a 696e 666f 2e75 7463 6f66 6673 6574  tzinfo.utcoffset
+00001580: 284e 6f6e 6529 2069 7320 4e6f 6e65 3a0a  (None) is None:.
+00001590: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000015a0: 6520 5661 6c75 6545 7272 6f72 2822 5468  e ValueError("Th
+000015b0: 6520 656e 6420 7469 6d65 206d 7573 7420  e end time must 
+000015c0: 6265 2074 696d 657a 6f6e 652d 6177 6172  be timezone-awar
+000015d0: 652e 2229 0a0a 2020 2020 2020 2020 6966  e.")..        if
+000015e0: 2073 7461 7274 203e 3d20 656e 643a 0a20   start >= end:. 
+000015f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00001600: 2056 616c 7565 4572 726f 7228 2254 6865   ValueError("The
+00001610: 2073 7461 7274 2074 696d 6520 6d75 7374   start time must
+00001620: 2062 6520 6561 726c 6965 7220 7468 616e   be earlier than
+00001630: 2074 6865 2065 6e64 2074 696d 652e 2229   the end time.")
+00001640: 0a0a 2020 2020 2020 2020 6966 2073 7461  ..        if sta
+00001650: 7274 203c 2065 7068 656d 6572 6964 6573  rt < ephemerides
+00001660: 5b30 5d2e 6570 6f63 683a 0a20 2020 2020  [0].epoch:.     
+00001670: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00001680: 7565 4572 726f 7228 2254 6865 2073 7461  ueError("The sta
+00001690: 7274 2074 696d 6520 6d75 7374 206e 6f74  rt time must not
+000016a0: 2062 6520 6561 726c 6965 7220 7468 616e   be earlier than
+000016b0: 2074 6865 2066 6972 7374 2065 706f 6368   the first epoch
+000016c0: 2e22 290a 2020 2020 2020 2020 6966 2065  .").        if e
+000016d0: 6e64 203e 2065 7068 656d 6572 6964 6573  nd > ephemerides
+000016e0: 5b2d 315d 2e65 706f 6368 3a0a 2020 2020  [-1].epoch:.    
+000016f0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00001700: 6c75 6545 7272 6f72 2822 5468 6520 656e  lueError("The en
+00001710: 6420 7469 6d65 206d 7573 7420 6e6f 7420  d time must not 
+00001720: 6265 206c 6174 6572 2074 6861 6e20 7468  be later than th
+00001730: 6520 6c61 7374 2065 706f 6368 2e22 290a  e last epoch.").
+00001740: 0a20 2020 2020 2020 2069 6620 6d61 785f  .        if max_
+00001750: 7472 6163 6b5f 6c65 6e67 7468 2e74 6f5f  track_length.to_
+00001760: 7661 6c75 6528 752e 6172 636d 696e 2920  value(u.arcmin) 
+00001770: 3c3d 2030 3a0a 2020 2020 2020 2020 2020  <= 0:.          
+00001780: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00001790: 6f72 2822 5468 6520 6d61 7869 6d75 6d20  or("The maximum 
+000017a0: 7472 6163 6b20 6c65 6e67 7468 206d 7573  track length mus
+000017b0: 7420 6265 2070 6f73 6974 6976 652e 2229  t be positive.")
+000017c0: 0a0a 2020 2020 2020 2020 2320 4669 6e64  ..        # Find
+000017d0: 2074 6865 2073 6d61 6c6c 6573 7420 696e   the smallest in
+000017e0: 7465 7276 616c 2063 6f76 6572 696e 6720  terval covering 
+000017f0: 7468 6520 7469 6d65 2069 6e74 6572 7661  the time interva
+00001800: 6c0a 2020 2020 2020 2020 616c 6c5f 7469  l.        all_ti
+00001810: 6d65 7320 3d20 5b65 2e65 706f 6368 2066  mes = [e.epoch f
+00001820: 6f72 2065 2069 6e20 6570 6865 6d65 7269  or e in ephemeri
+00001830: 6465 735d 0a20 2020 2020 2020 2073 7461  des].        sta
+00001840: 7274 5f69 6e64 6578 203d 2062 6973 6563  rt_index = bisec
+00001850: 742e 6269 7365 6374 5f72 6967 6874 2861  t.bisect_right(a
+00001860: 6c6c 5f74 696d 6573 2c20 7374 6172 7429  ll_times, start)
+00001870: 202d 2031 0a20 2020 2020 2020 2065 6e64   - 1.        end
+00001880: 5f69 6e64 6578 203d 2062 6973 6563 742e  _index = bisect.
+00001890: 6269 7365 6374 2861 6c6c 5f74 696d 6573  bisect(all_times
+000018a0: 2c20 656e 6429 0a20 2020 2020 2020 2069  , end).        i
+000018b0: 6620 656e 645f 696e 6465 7820 3e20 3020  f end_index > 0 
+000018c0: 616e 6420 616c 6c5f 7469 6d65 735b 656e  and all_times[en
+000018d0: 645f 696e 6465 7820 2d20 315d 203d 3d20  d_index - 1] == 
+000018e0: 656e 643a 0a20 2020 2020 2020 2020 2020  end:.           
+000018f0: 2065 6e64 5f69 6e64 6578 202d 3d20 310a   end_index -= 1.
+00001900: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+00001910: 7368 6f75 6c64 206e 6576 6572 2068 6170  should never hap
+00001920: 7065 6e2c 2062 7574 206c 6574 2773 2072  pen, but let's r
+00001930: 756c 6520 6f75 7420 696e 7465 7276 616c  ule out interval
+00001940: 7320 7769 7468 207a 6572 6f20 6c65 6e67  s with zero leng
+00001950: 7468 0a20 2020 2020 2020 2069 6620 7374  th.        if st
+00001960: 6172 745f 696e 6465 7820 3d3d 2065 6e64  art_index == end
+00001970: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
+00001980: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00001990: 7272 6f72 2822 5468 6520 696e 7465 7276  rror("The interv
+000019a0: 616c 206d 7573 7420 6861 7665 2061 2070  al must have a p
+000019b0: 6f73 6974 6976 6520 6c65 6e67 7468 2229  ositive length")
+000019c0: 0a0a 2020 2020 2020 2020 2320 5370 6c69  ..        # Spli
+000019d0: 7420 7468 6520 6570 6865 6d65 7269 6465  t the ephemeride
+000019e0: 7320 736f 2074 6861 7420 7468 6520 6d61  s so that the ma
+000019f0: 7869 6d75 6d20 7472 6163 6b20 6c65 6e67  ximum track leng
+00001a00: 7468 2069 736e 2774 2065 7863 6565 6465  th isn't exceede
+00001a10: 6420 666f 7220 6561 6368 0a20 2020 2020  d for each.     
+00001a20: 2020 2023 2067 726f 7570 2e20 5765 2061     # group. We a
+00001a30: 7373 756d 6520 6120 6c69 6e65 6172 2070  ssume a linear p
+00001a40: 6174 682c 2073 6f20 7468 6174 2074 6865  ath, so that the
+00001a50: 2074 7261 636b 206c 656e 6774 6820 6973   track length is
+00001a60: 2065 7175 616c 2074 6f20 7468 6520 616e   equal to the an
+00001a70: 676c 650a 2020 2020 2020 2020 2320 6265  gle.        # be
+00001a80: 7477 6565 6e20 7468 6520 6669 7273 7420  tween the first 
+00001a90: 616e 6420 6c61 7374 2070 6f73 6974 696f  and last positio
+00001aa0: 6e2e 0a20 2020 2020 2020 2063 7572 7265  n..        curre
+00001ab0: 6e74 5f67 726f 7570 203d 205b 6570 6865  nt_group = [ephe
+00001ac0: 6d65 7269 6465 735b 7374 6172 745f 696e  merides[start_in
+00001ad0: 6465 785d 5d0a 2020 2020 2020 2020 6772  dex]].        gr
+00001ae0: 6f75 7073 203d 205b 6375 7272 656e 745f  oups = [current_
+00001af0: 6772 6f75 705d 0a20 2020 2020 2020 2066  group].        f
+00001b00: 6f72 2069 2069 6e20 7261 6e67 6528 7374  or i in range(st
+00001b10: 6172 745f 696e 6465 7820 2b20 312c 2065  art_index + 1, e
+00001b20: 6e64 5f69 6e64 6578 202b 2031 293a 0a20  nd_index + 1):. 
+00001b30: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00001b40: 6570 6865 6d65 7269 7320 3d20 6570 6865  ephemeris = ephe
+00001b50: 6d65 7269 6465 735b 695d 0a20 2020 2020  merides[i].     
+00001b60: 2020 2020 2020 2023 2053 7562 7365 7175         # Subsequ
+00001b70: 656e 7420 706f 7369 7469 6f6e 7320 6d75  ent positions mu
+00001b80: 7374 206e 6f74 2062 6520 6d6f 7265 2074  st not be more t
+00001b90: 6861 6e20 6d61 785f 7472 6163 6b5f 6c65  han max_track_le
+00001ba0: 6e67 7468 2061 7061 7274 0a20 2020 2020  ngth apart.     
+00001bb0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00001bc0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00001bd0: 656e 745f 6772 6f75 705b 2d31 5d2e 706f  ent_group[-1].po
+00001be0: 7369 7469 6f6e 2e73 6570 6172 6174 696f  sition.separatio
+00001bf0: 6e28 6e65 7874 5f65 7068 656d 6572 6973  n(next_ephemeris
+00001c00: 2e70 6f73 6974 696f 6e29 0a20 2020 2020  .position).     
+00001c10: 2020 2020 2020 2020 2020 203e 206d 6178             > max
+00001c20: 5f74 7261 636b 5f6c 656e 6774 680a 2020  _track_length.  
+00001c30: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00001c40: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00001c50: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2022 5468 6520 6d61 7869 6d75 6d20     "The maximum 
+00001c80: 7472 6163 6b20 6c65 6e67 7468 206f 6e20  track length on 
+00001c90: 6120 6669 6e64 6572 2063 6861 7274 2069  a finder chart i
+00001ca0: 7320 6578 6365 6564 6564 2e22 0a20 2020  s exceeded.".   
+00001cb0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00001cc0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00001cd0: 5f6c 656e 6774 6820 3d20 6375 7272 656e  _length = curren
+00001ce0: 745f 6772 6f75 705b 305d 2e70 6f73 6974  t_group[0].posit
+00001cf0: 696f 6e2e 7365 7061 7261 7469 6f6e 286e  ion.separation(n
+00001d00: 6578 745f 6570 6865 6d65 7269 732e 706f  ext_ephemeris.po
+00001d10: 7369 7469 6f6e 290a 2020 2020 2020 2020  sition).        
+00001d20: 2020 2020 6966 2074 7261 636b 5f6c 656e      if track_len
+00001d30: 6774 6820 3c3d 206d 6178 5f74 7261 636b  gth <= max_track
+00001d40: 5f6c 656e 6774 683a 0a20 2020 2020 2020  _length:.       
+00001d50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00001d60: 5f67 726f 7570 2e61 7070 656e 6428 6e65  _group.append(ne
+00001d70: 7874 5f65 7068 656d 6572 6973 290a 2020  xt_ephemeris).  
+00001d80: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 6375 7272 656e 745f 6772 6f75 7020 3d20  current_group = 
+00001db0: 5b63 7572 7265 6e74 5f67 726f 7570 5b2d  [current_group[-
+00001dc0: 315d 2c20 6e65 7874 5f65 7068 656d 6572  1], next_ephemer
+00001dd0: 6973 5d0a 2020 2020 2020 2020 2020 2020  is].            
+00001de0: 2020 2020 6772 6f75 7073 2e61 7070 656e      groups.appen
+00001df0: 6428 6375 7272 656e 745f 6772 6f75 7029  d(current_group)
+00001e00: 0a0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
+00001e10: 7465 2074 6865 2066 696e 6465 7220 6368  te the finder ch
+00001e20: 6172 7473 0a20 2020 2020 2020 2066 6f72  arts.        for
+00001e30: 2067 726f 7570 2069 6e20 6772 6f75 7073   group in groups
+00001e40: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
+00001e50: 6c69 645f 666f 7220 3d20 2867 726f 7570  lid_for = (group
+00001e60: 5b30 5d2e 6570 6f63 682c 2067 726f 7570  [0].epoch, group
+00001e70: 5b2d 315d 2e65 706f 6368 290a 2020 2020  [-1].epoch).    
+00001e80: 2020 2020 2020 2020 6669 6e64 6572 5f63          finder_c
+00001e90: 6861 7274 203d 2063 7265 6174 655f 6669  hart = create_fi
+00001ea0: 6e64 6572 5f63 6861 7274 2867 726f 7570  nder_chart(group
+00001eb0: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
+00001ec0: 6e64 6572 5f63 6861 7274 2e61 6464 5f6d  nder_chart.add_m
+00001ed0: 6574 6164 6174 6128 2276 616c 6964 5f66  etadata("valid_f
+00001ee0: 6f72 222c 2076 616c 6964 5f66 6f72 290a  or", valid_for).
+00001ef0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00001f00: 6420 6669 6e64 6572 5f63 6861 7274 2c20  d finder_chart, 
+00001f10: 7661 6c69 645f 666f 720a 0a20 2020 2040  valid_for..    @
+00001f20: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00001f30: 2077 6373 2873 656c 6629 202d 3e20 5743   wcs(self) -> WC
+00001f40: 533a 0a20 2020 2020 2020 2022 2222 5265  S:.        """Re
+00001f50: 7475 726e 2061 2064 6565 7020 636f 7079  turn a deep copy
+00001f60: 206f 6620 7468 6520 5743 5320 6f62 6a65   of the WCS obje
+00001f70: 6374 206f 6620 7468 6520 6669 6e64 6572  ct of the finder
+00001f80: 2063 6861 7274 2e0a 0a20 2020 2020 2020   chart...       
+00001f90: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00001fa0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00001fb0: 2060 7e61 7374 726f 7079 2e77 6373 2e57   `~astropy.wcs.W
+00001fc0: 4353 600a 2020 2020 2020 2020 2020 2020  CS`.            
+00001fd0: 4120 6465 6570 2063 6f70 7920 6f66 2074  A deep copy of t
+00001fe0: 6865 2057 4353 206f 626a 6563 742e 0a20  he WCS object.. 
+00001ff0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00002000: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00002010: 7763 732e 6465 6570 636f 7079 2829 0a0a  wcs.deepcopy()..
+00002020: 2020 2020 6465 6620 6164 645f 616e 6e6f      def add_anno
+00002030: 7461 7469 6f6e 2873 656c 662c 2061 6e6e  tation(self, ann
+00002040: 6f74 6174 696f 6e3a 2041 6e6e 6f74 6174  otation: Annotat
+00002050: 696f 6e29 202d 3e20 4e6f 6e65 3a0a 2020  ion) -> None:.  
+00002060: 2020 2020 2020 2222 2241 6464 2061 6e20        """Add an 
+00002070: 616e 6e6f 7461 7469 6f6e 2074 6f20 7468  annotation to th
+00002080: 6520 6669 6e64 6572 2063 6861 7274 2e0a  e finder chart..
+00002090: 0a20 2020 2020 2020 2041 6e6e 6f74 6174  .        Annotat
+000020a0: 696f 6e73 2077 696c 6c20 6265 2070 6c6f  ions will be plo
+000020b0: 7474 6564 206f 6e74 6f20 7468 6520 6669  tted onto the fi
+000020c0: 6e64 6572 2063 6861 7274 2069 6e20 7468  nder chart in th
+000020d0: 6520 6f72 6465 7220 7468 6579 2068 6176  e order they hav
+000020e0: 6520 6265 656e 0a20 2020 2020 2020 2061  e been.        a
+000020f0: 6464 6564 2e20 536f 2c20 666f 7220 6578  dded. So, for ex
+00002100: 616d 706c 652c 2074 6865 2061 6e6e 6f74  ample, the annot
+00002110: 6174 696f 6e20 6164 6465 6420 6c61 7374  ation added last
+00002120: 2077 696c 6c20 6265 206f 7574 7075 7420   will be output 
+00002130: 6f6e 2074 6f70 206f 6620 616c 6c0a 2020  on top of all.  
+00002140: 2020 2020 2020 7468 6520 6f74 6865 7220        the other 
+00002150: 616e 6e6f 7461 7469 6f6e 732e 0a20 2020  annotations..   
+00002160: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00002170: 2073 656c 662e 5f61 6e6e 6f74 6174 696f   self._annotatio
+00002180: 6e73 2e61 7070 656e 6428 616e 6e6f 7461  ns.append(annota
+00002190: 7469 6f6e 290a 0a20 2020 2040 7072 6f70  tion)..    @prop
+000021a0: 6572 7479 0a20 2020 2064 6566 206d 6574  erty.    def met
+000021b0: 6164 6174 6128 7365 6c66 2920 2d3e 2044  adata(self) -> D
+000021c0: 6963 745b 7374 722c 2041 6e79 5d3a 0a20  ict[str, Any]:. 
+000021d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000021e0: 2020 2052 6574 7572 6e20 7468 6520 6d65     Return the me
+000021f0: 7461 6461 7461 2066 6f72 2074 6865 2066  tadata for the f
+00002200: 696e 6465 7220 6368 6172 742e 0a0a 2020  inder chart...  
+00002210: 2020 2020 2020 4d65 7461 6461 7461 2063        Metadata c
+00002220: 616e 2020 6265 2061 6464 6564 2077 6974  an  be added wit
+00002230: 6820 7468 6520 6061 6464 5f6d 6574 6164  h the `add_metad
+00002240: 6174 6160 206d 6574 686f 642e 2041 2073  ata` method. A s
+00002250: 6861 6c6c 6f77 2063 6f70 7920 6f66 2074  hallow copy of t
+00002260: 6865 0a20 2020 2020 2020 206d 6574 6164  he.        metad
+00002270: 6174 6120 6973 2072 6574 7572 6e65 642e  ata is returned.
+00002280: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00002290: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000022a0: 2d0a 2020 2020 2020 2020 6469 6374 0a20  -.        dict. 
+000022b0: 2020 2020 2020 2020 2020 2054 6865 206d             The m
+000022c0: 6574 6164 6174 6120 6f66 2074 6865 2066  etadata of the f
+000022d0: 696e 6465 7220 6368 6172 742e 0a20 2020  inder chart..   
+000022e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000022f0: 2072 6574 7572 6e20 7365 6c66 2e5f 6d65   return self._me
+00002300: 7461 6461 7461 2e63 6f70 7928 290a 0a20  tadata.copy().. 
+00002310: 2020 2064 6566 2061 6464 5f6d 6574 6164     def add_metad
+00002320: 6174 6128 7365 6c66 2c20 6b65 793a 2073  ata(self, key: s
+00002330: 7472 2c20 7661 6c75 653a 2041 6e79 2920  tr, value: Any) 
+00002340: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00002350: 2022 2222 0a20 2020 2020 2020 2041 6464   """.        Add
+00002360: 2061 206b 6579 2d76 616c 7565 2074 6f20   a key-value to 
+00002370: 7468 6520 6669 6e64 6572 2063 6861 7274  the finder chart
+00002380: 2773 206d 6574 6164 6174 612e 0a0a 2020  's metadata...  
+00002390: 2020 2020 2020 4966 2074 6865 206b 6579        If the key
+000023a0: 2065 7869 7374 7273 2069 6e20 7468 6520   existrs in the 
+000023b0: 6d65 7461 6461 7461 2061 6c72 6561 6479  metadata already
+000023c0: 2c20 7468 6520 6578 6973 7469 6e67 2076  , the existing v
+000023d0: 616c 7565 2066 6f72 2074 6865 206b 6579  alue for the key
+000023e0: 2069 730a 2020 2020 2020 2020 7265 706c   is.        repl
+000023f0: 6163 6564 2e0a 0a20 2020 2020 2020 2050  aced...        P
+00002400: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00002410: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00002420: 2020 2020 206b 6579 3a20 6073 7472 600a       key: `str`.
+00002430: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
+00002440: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
+00002450: 607e 7479 7069 6e67 2e41 6e79 600a 2020  `~typing.Any`.  
+00002460: 2020 2020 2020 2020 2020 5661 6c75 652e            Value.
+00002470: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002480: 2020 2020 2073 656c 662e 5f6d 6574 6164       self._metad
+00002490: 6174 615b 6b65 795d 203d 2076 616c 7565  ata[key] = value
+000024a0: 0a0a 2020 2020 6465 6620 7368 6f77 2873  ..    def show(s
+000024b0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+000024c0: 2020 2020 2020 2222 2244 6973 706c 6179        """Display
+000024d0: 2074 6865 2066 696e 6465 7220 6368 6172   the finder char
+000024e0: 7420 6f6e 2074 6865 2073 6372 6565 6e2e  t on the screen.
+000024f0: 2222 220a 2020 2020 2020 2020 6669 6775  """.        figu
+00002500: 7265 203d 2073 656c 662e 5f63 7265 6174  re = self._creat
+00002510: 655f 706c 6f74 2829 0a20 2020 2020 2020  e_plot().       
+00002520: 2070 6c74 2e73 686f 7728 290a 2020 2020   plt.show().    
+00002530: 2020 2020 706c 742e 636c 6f73 6528 6669      plt.close(fi
+00002540: 6775 7265 290a 0a20 2020 2064 6566 2073  gure)..    def s
+00002550: 6176 6528 0a20 2020 2020 2020 2073 656c  ave(.        sel
+00002560: 662c 0a20 2020 2020 2020 206e 616d 653a  f,.        name:
+00002570: 2055 6e69 6f6e 5b73 7472 2c20 4269 6e61   Union[str, Bina
+00002580: 7279 494f 2c20 6f73 2e50 6174 684c 696b  ryIO, os.PathLik
+00002590: 655b 7374 725d 2c20 6f73 2e50 6174 684c  e[str], os.PathL
+000025a0: 696b 655b 6279 7465 735d 5d2c 0a20 2020  ike[bytes]],.   
+000025b0: 2020 2020 2066 6f72 6d61 743a 204f 7074       format: Opt
+000025c0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000025d0: 652c 0a20 2020 2029 202d 3e20 4e6f 6e65  e,.    ) -> None
+000025e0: 3a0a 2020 2020 2020 2020 2222 2253 6176  :.        """Sav
+000025f0: 6520 7468 6520 6669 6e64 6572 2063 6861  e the finder cha
+00002600: 7274 2069 6e20 6120 6669 6c65 2e0a 0a20  rt in a file... 
+00002610: 2020 2020 2020 2049 6620 6066 6f72 6d61         If `forma
+00002620: 7460 2069 7320 6e6f 7420 7365 742c 2074  t` is not set, t
+00002630: 6865 2066 696c 6520 6578 7465 6e73 696f  he file extensio
+00002640: 6e20 6f66 2060 6e61 6d65 6020 6973 2075  n of `name` is u
+00002650: 7365 6420 746f 2066 6967 7572 6520 6f75  sed to figure ou
+00002660: 7420 7468 650a 2020 2020 2020 2020 6669  t the.        fi
+00002670: 6c65 206f 722c 2069 6620 7468 6572 6520  le or, if there 
+00002680: 6973 206e 6f20 6578 7465 6e73 696f 6e2c  is no extension,
+00002690: 204d 6174 706c 6f74 6c69 6227 7320 6465   Matplotlib's de
+000026a0: 6661 756c 7420 6973 2075 7365 642e 2053  fault is used. S
+000026b0: 6565 0a20 2020 2020 2020 204d 6174 706c  ee.        Matpl
+000026c0: 6f74 6c69 6227 7320 606d 6174 706c 6f74  otlib's `matplot
+000026d0: 6c69 622e 7079 706c 6f74 2e73 6176 6566  lib.pyplot.savef
+000026e0: 6967 6020 6675 6e63 7469 6f6e 2066 6f72  ig` function for
+000026f0: 206d 6f72 6520 6465 7461 696c 7320 7265   more details re
+00002700: 6761 7264 696e 670a 2020 2020 2020 2020  garding.        
+00002710: 7468 6520 666f 726d 6174 2e0a 0a20 2020  the format...   
+00002720: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00002730: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00002740: 2d2d 0a20 2020 2020 2020 206e 616d 653a  --.        name:
+00002750: 2060 7374 7260 2c20 6070 6174 682d 6c69   `str`, `path-li
+00002760: 6b65 6020 6f72 2060 6269 6e61 7279 2066  ke` or `binary f
+00002770: 696c 652d 6c69 6b65 600a 2020 2020 2020  ile-like`.      
+00002780: 2020 2020 2020 5468 6520 6669 6c65 2074        The file t
+00002790: 6f20 7768 6963 6820 7468 6520 6669 6e64  o which the find
+000027a0: 6572 2063 6861 7274 2069 7320 7361 7665  er chart is save
+000027b0: 642e 2041 6e20 6578 6973 7469 6e67 2066  d. An existing f
+000027c0: 696c 6520 6973 2072 6570 6c61 6365 642e  ile is replaced.
+000027d0: 0a20 2020 2020 2020 2066 6f72 6d61 743a  .        format:
+000027e0: 2060 7374 7260 2c20 6f70 7469 6f6e 616c   `str`, optional
+000027f0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00002800: 2066 6f72 6d61 7420 696e 2077 6869 6368   format in which
+00002810: 2074 6f20 7374 6f72 6520 7468 6520 6669   to store the fi
+00002820: 6e64 6572 2063 6861 7274 2e0a 2020 2020  nder chart..    
+00002830: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00002840: 6669 6775 7265 203d 2073 656c 662e 5f63  figure = self._c
+00002850: 7265 6174 655f 706c 6f74 2829 0a20 2020  reate_plot().   
+00002860: 2020 2020 2069 6620 666f 726d 6174 2061       if format a
+00002870: 6e64 2066 6f72 6d61 742e 6c6f 7765 7228  nd format.lower(
+00002880: 2920 3d3d 2022 7064 6622 3a0a 2020 2020  ) == "pdf":.    
+00002890: 2020 2020 2020 2020 7064 6620 3d20 4279          pdf = By
+000028a0: 7465 7349 4f28 290a 2020 2020 2020 2020  tesIO().        
+000028b0: 2020 2020 706c 742e 7361 7665 6669 6728      plt.savefig(
+000028c0: 7064 662c 2066 6f72 6d61 743d 666f 726d  pdf, format=form
+000028d0: 6174 2c20 6262 6f78 5f69 6e63 6865 733d  at, bbox_inches=
+000028e0: 2274 6967 6874 2229 0a20 2020 2020 2020  "tight").       
+000028f0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00002900: 6e61 6d65 2c20 2277 7269 7465 2229 3a0a  name, "write"):.
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 6e61 6d65 2e77 7269 7465 2870 6466 2e67  name.write(pdf.g
+00002930: 6574 7661 6c75 6528 2929 0a20 2020 2020  etvalue()).     
+00002940: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00002950: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00002960: 6820 6f70 656e 286e 616d 652c 2022 7762  h open(name, "wb
+00002970: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+00002980: 2020 2020 2020 2020 2020 2020 2066 2e77               f.w
+00002990: 7269 7465 2870 6466 2e67 6574 7661 6c75  rite(pdf.getvalu
+000029a0: 6528 2929 0a20 2020 2020 2020 2065 6c73  e()).        els
+000029b0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+000029c0: 6c74 2e73 6176 6566 6967 286e 616d 652c  lt.savefig(name,
+000029d0: 2066 6f72 6d61 743d 666f 726d 6174 2c20   format=format, 
+000029e0: 6262 6f78 5f69 6e63 6865 733d 2274 6967  bbox_inches="tig
+000029f0: 6874 2229 0a20 2020 2020 2020 2070 6c74  ht").        plt
+00002a00: 2e63 6c6f 7365 2866 6967 7572 6529 0a0a  .close(figure)..
+00002a10: 2020 2020 6465 6620 5f63 7265 6174 655f      def _create_
+00002a20: 706c 6f74 2873 656c 6629 202d 3e20 4669  plot(self) -> Fi
+00002a30: 6775 7265 3a0a 2020 2020 2020 2020 6669  gure:.        fi
+00002a40: 6775 7265 203d 2070 6c74 2e66 6967 7572  gure = plt.figur
+00002a50: 6528 6669 6773 697a 653d 2831 302c 2039  e(figsize=(10, 9
+00002a60: 2929 0a20 2020 2020 2020 2061 7820 3d20  )).        ax = 
+00002a70: 706c 742e 7375 6270 6c6f 7428 7072 6f6a  plt.subplot(proj
+00002a80: 6563 7469 6f6e 3d73 656c 662e 5f77 6373  ection=self._wcs
+00002a90: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00002aa0: 5f61 6464 5f66 6974 735f 636f 6e74 656e  _add_fits_conten
+00002ab0: 7428 6178 290a 2020 2020 2020 2020 7365  t(ax).        se
+00002ac0: 6c66 2e5f 7570 6461 7465 5f61 7865 7328  lf._update_axes(
+00002ad0: 6178 290a 0a20 2020 2020 2020 2061 782e  ax)..        ax.
+00002ae0: 6772 6964 2854 7275 652c 2063 6f6c 6f72  grid(True, color
+00002af0: 3d22 626c 7565 222c 2061 6c70 6861 3d30  ="blue", alpha=0
+00002b00: 2e32 290a 0a20 2020 2020 2020 2066 6f72  .2)..        for
+00002b10: 2061 6e6e 6f74 6174 696f 6e20 696e 2073   annotation in s
+00002b20: 656c 662e 5f61 6e6e 6f74 6174 696f 6e73  elf._annotations
+00002b30: 3a0a 2020 2020 2020 2020 2020 2020 616e  :.            an
+00002b40: 6e6f 7461 7469 6f6e 2e61 6464 5f74 6f28  notation.add_to(
+00002b50: 6178 290a 0a20 2020 2020 2020 2072 6574  ax)..        ret
+00002b60: 7572 6e20 6669 6775 7265 0a0a 2020 2020  urn figure..    
+00002b70: 6465 6620 5f61 6464 5f66 6974 735f 636f  def _add_fits_co
+00002b80: 6e74 656e 7428 7365 6c66 2c20 6178 3a20  ntent(self, ax: 
+00002b90: 5743 5341 7865 7353 7562 706c 6f74 2920  WCSAxesSubplot) 
+00002ba0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00002bb0: 2022 2222 0a20 2020 2020 2020 2020 4164   """.         Ad
+00002bc0: 6420 636f 6e74 656e 7420 6f66 2074 6865  d content of the
+00002bd0: 2046 4954 5320 6669 6c65 2074 6f20 7468   FITS file to th
+00002be0: 6520 706c 6f74 2e0a 0a20 2020 2020 2020  e plot...       
+00002bf0: 2054 6865 2063 6f64 6520 6861 7320 6265   The code has be
+00002c00: 656e 2061 6461 7074 6564 2066 726f 6d20  en adapted from 
+00002c10: 4150 4c70 792e 0a20 2020 2020 2020 2022  APLpy..        "
+00002c20: 2222 0a20 2020 2020 2020 2063 6d61 7020  "".        cmap 
+00002c30: 3d20 706c 742e 636d 2e67 6574 5f63 6d61  = plt.cm.get_cma
+00002c40: 7028 2267 6973 745f 7961 7267 2229 0a0a  p("gist_yarg")..
+00002c50: 2020 2020 2020 2020 2320 7661 6c75 6520          # value 
+00002c60: 7261 6e67 6520 696e 2074 6865 2069 6d61  range in the ima
+00002c70: 6765 0a20 2020 2020 2020 2070 6d69 6e20  ge.        pmin 
+00002c80: 3d20 302e 3235 0a20 2020 2020 2020 2070  = 0.25.        p
+00002c90: 6d61 7820 3d20 3939 2e37 350a 2020 2020  max = 99.75.    
+00002ca0: 2020 2020 696e 7465 7276 616c 203d 2041      interval = A
+00002cb0: 7379 6d6d 6574 7269 6350 6572 6365 6e74  symmetricPercent
+00002cc0: 696c 6549 6e74 6572 7661 6c28 706d 696e  ileInterval(pmin
+00002cd0: 2c20 706d 6178 2c20 6e5f 7361 6d70 6c65  , pmax, n_sample
+00002ce0: 733d 3130 3030 3029 0a20 2020 2020 2020  s=10000).       
+00002cf0: 2076 6d69 6e2c 2076 6d61 7820 3d20 696e   vmin, vmax = in
+00002d00: 7465 7276 616c 2e67 6574 5f6c 696d 6974  terval.get_limit
+00002d10: 7328 7365 6c66 2e5f 6864 752e 6461 7461  s(self._hdu.data
+00002d20: 290a 2020 2020 2020 2020 766d 696e 203d  ).        vmin =
+00002d30: 202d 302e 3120 2a20 2876 6d61 7820 2d20   -0.1 * (vmax - 
+00002d40: 766d 696e 2920 2b20 766d 696e 0a20 2020  vmin) + vmin.   
+00002d50: 2020 2020 2076 6d61 7820 3d20 302e 3120       vmax = 0.1 
+00002d60: 2a20 2876 6d61 7820 2d20 766d 696e 2920  * (vmax - vmin) 
+00002d70: 2b20 766d 6178 0a0a 2020 2020 2020 2020  + vmax..        
+00002d80: 6e6f 726d 616c 697a 6572 203d 2073 696d  normalizer = sim
+00002d90: 706c 655f 6e6f 726d 2873 656c 662e 5f64  ple_norm(self._d
+00002da0: 6174 612c 2070 6f77 6572 3d32 2c20 6d69  ata, power=2, mi
+00002db0: 6e5f 6375 743d 766d 696e 2c20 6d61 785f  n_cut=vmin, max_
+00002dc0: 6375 743d 766d 6178 290a 0a20 2020 2020  cut=vmax)..     
+00002dd0: 2020 2061 782e 696d 7368 6f77 280a 2020     ax.imshow(.  
+00002de0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00002df0: 6864 752e 6461 7461 2c0a 2020 2020 2020  hdu.data,.      
+00002e00: 2020 2020 2020 636d 6170 3d63 6d61 702c        cmap=cmap,
+00002e10: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
+00002e20: 6572 706f 6c61 7469 6f6e 3d22 6e65 6172  erpolation="near
+00002e30: 6573 7422 2c0a 2020 2020 2020 2020 2020  est",.          
+00002e40: 2020 6f72 6967 696e 3d22 6c6f 7765 7222    origin="lower"
+00002e50: 2c0a 2020 2020 2020 2020 2020 2020 6e6f  ,.            no
+00002e60: 726d 3d6e 6f72 6d61 6c69 7a65 722c 0a20  rm=normalizer,. 
+00002e70: 2020 2020 2020 2020 2020 2061 7370 6563             aspec
+00002e80: 743d 2265 7175 616c 222c 0a20 2020 2020  t="equal",.     
+00002e90: 2020 2029 0a0a 2020 2020 6465 6620 5f75     )..    def _u
+00002ea0: 7064 6174 655f 6178 6573 2873 656c 662c  pdate_axes(self,
+00002eb0: 2061 783a 2057 4353 4178 6573 5375 6270   ax: WCSAxesSubp
+00002ec0: 6c6f 7429 202d 3e20 4e6f 6e65 3a0a 2020  lot) -> None:.  
+00002ed0: 2020 2020 2020 6178 6973 5f74 7970 655f        axis_type_
+00002ee0: 6e61 6d65 7320 3d20 7b0a 2020 2020 2020  names = {.      
+00002ef0: 2020 2020 2020 2270 6f73 2e65 712e 6465        "pos.eq.de
+00002f00: 6322 3a20 2244 6563 2028 4943 5253 2922  c": "Dec (ICRS)"
+00002f10: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
+00002f20: 6f73 2e65 712e 7261 223a 2022 5241 2028  os.eq.ra": "RA (
+00002f30: 4943 5253 2922 2c0a 2020 2020 2020 2020  ICRS)",.        
+00002f40: 7d0a 2020 2020 2020 2020 6178 6973 5f74  }.        axis_t
+00002f50: 7970 6573 203d 2073 656c 662e 5f77 6373  ypes = self._wcs
+00002f60: 2e77 6f72 6c64 5f61 7869 735f 7068 7973  .world_axis_phys
+00002f70: 6963 616c 5f74 7970 6573 0a20 2020 2020  ical_types.     
+00002f80: 2020 2078 5f61 7869 735f 7479 7065 203d     x_axis_type =
+00002f90: 2061 7869 735f 7479 7065 735b 305d 0a20   axis_types[0]. 
+00002fa0: 2020 2020 2020 2079 5f61 7869 735f 7479         y_axis_ty
+00002fb0: 7065 203d 2061 7869 735f 7479 7065 735b  pe = axis_types[
+00002fc0: 315d 0a20 2020 2020 2020 2069 6620 785f  1].        if x_
+00002fd0: 6178 6973 5f74 7970 6520 213d 2022 706f  axis_type != "po
+00002fe0: 732e 6571 2e72 6122 3a0a 2020 2020 2020  s.eq.ra":.      
+00002ff0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00003000: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00003010: 2020 2020 2020 2020 224f 6e6c 7920 706f          "Only po
+00003020: 732e 6571 2e72 6120 6973 2073 7570 706f  s.eq.ra is suppo
+00003030: 7274 6564 2066 6f72 2074 6865 2070 6879  rted for the phy
+00003040: 7369 6361 6c20 7479 7065 206f 6620 220a  sical type of ".
+00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003060: 2274 6865 2066 6972 7374 2077 6f72 6c64  "the first world
+00003070: 2061 7869 7322 0a20 2020 2020 2020 2020   axis".         
+00003080: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00003090: 795f 6178 6973 5f74 7970 6520 213d 2022  y_axis_type != "
+000030a0: 706f 732e 6571 2e64 6563 223a 0a20 2020  pos.eq.dec":.   
+000030b0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000030c0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+000030d0: 2020 2020 2020 2020 2020 2022 4f6e 6c79             "Only
+000030e0: 2070 6f73 2e65 712e 6465 6320 6973 2073   pos.eq.dec is s
+000030f0: 7570 706f 7274 6564 2066 6f72 2074 6865  upported for the
+00003100: 2070 6879 7369 6361 6c20 7479 7065 206f   physical type o
+00003110: 6620 220a 2020 2020 2020 2020 2020 2020  f ".            
+00003120: 2020 2020 2274 6865 2073 6563 6f6e 6420      "the second 
+00003130: 776f 726c 6420 6178 6973 220a 2020 2020  world axis".    
+00003140: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00003150: 2020 2078 203d 2061 782e 636f 6f72 6473     x = ax.coords
+00003160: 5b30 5d0a 2020 2020 2020 2020 7920 3d20  [0].        y = 
+00003170: 6178 2e63 6f6f 7264 735b 315d 0a20 2020  ax.coords[1].   
+00003180: 2020 2020 2078 2e73 6574 5f61 7869 736c       x.set_axisl
+00003190: 6162 656c 2861 7869 735f 7479 7065 5f6e  abel(axis_type_n
+000031a0: 616d 6573 5b78 5f61 7869 735f 7479 7065  ames[x_axis_type
+000031b0: 5d29 0a20 2020 2020 2020 2079 2e73 6574  ]).        y.set
+000031c0: 5f61 7869 736c 6162 656c 2861 7869 735f  _axislabel(axis_
+000031d0: 7479 7065 5f6e 616d 6573 5b79 5f61 7869  type_names[y_axi
+000031e0: 735f 7479 7065 5d29 0a0a 2020 2020 2020  s_type])..      
+000031f0: 2020 782e 6469 7370 6c61 795f 6d69 6e6f    x.display_mino
+00003200: 725f 7469 636b 7328 5472 7565 290a 2020  r_ticks(True).  
+00003210: 2020 2020 2020 792e 6469 7370 6c61 795f        y.display_
+00003220: 6d69 6e6f 725f 7469 636b 7328 5472 7565  minor_ticks(True
+00003230: 290a 0a20 2020 2020 2020 2078 2e73 6574  )..        x.set
+00003240: 5f74 6963 6b73 2873 697a 653d 3729 0a20  _ticks(size=7). 
+00003250: 2020 2020 2020 2079 2e73 6574 5f74 6963         y.set_tic
+00003260: 6b73 2873 697a 653d 3729 0a              ks(size=7).
```

### Comparing `imephu-0.2.0/src/imephu/__pycache__/geometry.cpython-310.pyc` & `imephu-0.2.1/src/imephu/geometry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,491 +1,607 @@
-00000000: 6f0d 0d0a 0000 0000 927a 0662 ee25 0000  o........z.b.%..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
-00000040: 6d02 5a02 6d03 5a03 0100 6400 6403 6c04  m.Z.m.Z...d.d.l.
-00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6400  m.Z.m.Z.m.Z...d.
-00000060: 6401 6c08 5a09 6400 6401 6c0a 6d04 5a0b  d.l.Z.d.d.l.m.Z.
-00000070: 0100 6400 6404 6c0c 6d0d 5a0e 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6405 6c0f 6d10 5a10 6d11 5a11 0100 6400  d.l.m.Z.m.Z...d.
-00000090: 6406 6c12 6d13 5a13 0100 6400 6407 6c14  d.l.m.Z...d.d.l.
-000000a0: 6d15 5a15 6d16 5a16 0100 6408 6511 6409  m.Z.m.Z...d.e.d.
-000000b0: 6511 640a 6510 640b 6513 640c 6511 660a  e.d.e.d.e.d.e.f.
-000000c0: 640d 640e 8404 5a17 6408 6511 640f 6510  d.d...Z.d.e.d.e.
-000000d0: 640c 6511 6606 6410 6411 8404 5a18 640b  d.e.f.d.d...Z.d.
-000000e0: 6513 640c 6506 6510 6510 6602 1900 6604  e.d.e.e.e.f...f.
-000000f0: 6412 6413 8404 5a19 6414 6511 640b 6513  d.d...Z.d.e.d.e.
-00000100: 640c 650b 6a1a 6509 6a1b 1900 6606 6415  d.e.j.e.j...f.d.
-00000110: 6416 8404 5a1c 6417 650b 6a1a 6509 6a1b  d...Z.d.e.j.e.j.
-00000120: 1900 640b 6513 640c 6511 6606 6418 6419  ..d.e.d.e.f.d.d.
-00000130: 8404 5a1d 640b 6513 640c 651e 6604 641a  ..Z.d.e.d.e.f.d.
-00000140: 641b 8404 5a1f 6401 5300 291c e900 0000  d...Z.d.S.).....
-00000150: 004e 2903 da05 6174 616e 32da 0363 6f73  .N)...atan2..cos
-00000160: da03 7369 6e29 03da 0341 6e79 da05 5475  ..sin)...Any..Tu
-00000170: 706c 65da 0463 6173 7429 01da 0575 6e69  ple..cast)...uni
-00000180: 7473 2902 da05 416e 676c 65da 0853 6b79  ts)...Angle..Sky
-00000190: 436f 6f72 6429 01da 0357 4353 2902 da11  Coord)...WCS)...
-000001a0: 7069 7865 6c5f 746f 5f73 6b79 636f 6f72  pixel_to_skycoor
-000001b0: 64da 1173 6b79 636f 6f72 645f 746f 5f70  d..skycoord_to_p
-000001c0: 6978 656c da01 76da 0570 6976 6f74 da05  ixel..v..pivot..
-000001d0: 616e 676c 65da 0377 6373 da06 7265 7475  angle..wcs..retu
-000001e0: 726e 6304 0000 0000 0000 0000 0000 0011  rnc.............
-000001f0: 0000 0006 0000 0043 0000 0073 c200 0000  .......C...s....
-00000200: 7400 7c00 7c03 8302 7d04 7400 7c01 7c03  t.|.|...}.t.|.|.
-00000210: 8302 7d05 7401 7c03 8301 5c02 7d06 7d07  ..}.t.|...\.}.}.
-00000220: 7c02 a002 7403 6a04 a101 7d08 7405 7c08  |...t.j...}.t.|.
-00000230: 8301 7d09 7406 7c08 8301 7d0a 7c09 7d0b  ..}.t.|...}.|.}.
-00000240: 7407 7c06 7c07 1b00 8301 7c0a 1400 7d0c  t.|.|.....|...}.
-00000250: 7408 7c0c 7c0b 8302 7d0d 7409 7c03 8301  t.|.|...}.t.|...
-00000260: 7335 7c0d 6401 3900 7d0d 740a a00b 7405  s5|.d.9.}.t...t.
-00000270: 7c0d 8301 7406 7c0d 8301 0b00 6702 7406  |...t.|.....g.t.
-00000280: 7c0d 8301 7405 7c0d 8301 6702 6702 a101  |...t.|...g.g...
-00000290: 7d0e 740a a00b 7c04 a101 740a a00b 7c05  }.t...|...t...|.
-000002a0: a101 1800 7d0f 740a a00b 7c05 a101 7c0e  ....}.t...|...|.
-000002b0: 7c0f 1000 1700 7d10 740c 7c10 7c03 8302  |.....}.t.|.|...
-000002c0: 5300 2903 61d5 0300 0052 6f74 6174 6520  S.).a....Rotate 
-000002d0: 6120 706f 696e 7420 6172 6f75 6e64 2061  a point around a
-000002e0: 2070 6976 6f74 2e0a 0a20 2020 2042 6f74   pivot...    Bot
-000002f0: 6820 7468 6520 7069 766f 7420 616e 6420  h the pivot and 
-00000300: 7468 6520 706f 696e 7420 746f 2072 6f74  the point to rot
-00000310: 6174 6520 6172 6520 6173 7375 6d65 6420  ate are assumed 
-00000320: 746f 2062 6520 6769 7665 6e20 6173 2072  to be given as r
-00000330: 6967 6874 2061 7363 656e 7369 6f6e 0a20  ight ascension. 
-00000340: 2020 2061 6e64 2064 6563 6c69 6e61 7469     and declinati
-00000350: 6f6e 2e20 5468 6520 726f 7461 7469 6f6e  on. The rotation
-00000360: 2061 6e67 6c65 2069 7320 7461 6b65 6e20   angle is taken 
-00000370: 746f 2062 6520 7468 6520 616e 676c 6520  to be the angle 
-00000380: 6f6e 2074 6865 2073 6b79 2e20 4966 2074  on the sky. If t
-00000390: 6865 0a20 2020 2070 6978 656c 2073 6361  he.    pixel sca
-000003a0: 6c65 7320 666f 7220 7269 6768 7420 6173  les for right as
-000003b0: 6365 6e73 696f 6e20 616e 6420 6465 636c  cension and decl
-000003c0: 696e 6174 696f 6e20 6469 6666 6572 2c20  ination differ, 
-000003d0: 7468 6520 616e 676c 6520 7365 656e 206f  the angle seen o
-000003e0: 6e20 7468 650a 2020 2020 6669 6e64 6572  n the.    finder
-000003f0: 2063 6861 7274 2077 696c 6c20 6469 6666   chart will diff
-00000400: 6572 2066 726f 6d20 7468 6973 2061 6e67  er from this ang
-00000410: 6c65 2e0a 0a20 2020 2054 6865 2061 6e67  le...    The ang
-00000420: 6c65 2069 7320 6d65 6173 7572 6564 2066  le is measured f
-00000430: 726f 6d20 6e6f 7274 6820 746f 2073 6f75  rom north to sou
-00000440: 7468 2e20 4865 6e63 6520 6974 2064 6570  th. Hence it dep
-00000450: 656e 6473 206f 6e20 7468 6520 6f72 6965  ends on the orie
-00000460: 6e74 6174 696f 6e20 6f66 0a20 2020 2074  ntation of.    t
-00000470: 6865 2063 6f6f 7264 696e 6174 6520 6178  he coordinate ax
-00000480: 6573 2077 6865 7468 6572 2061 2070 6f73  es whether a pos
-00000490: 6974 6976 6520 616e 676c 6520 636f 7272  itive angle corr
-000004a0: 6573 706f 6e64 7320 746f 2061 2063 6c6f  esponds to a clo
-000004b0: 636b 7769 7365 206f 720a 2020 2020 616e  ckwise or.    an
-000004c0: 7469 2d63 6c6f 636b 7769 7365 206f 7269  ti-clockwise ori
-000004d0: 656e 7461 7469 6f6e 2e0a 0a20 2020 2050  entation...    P
-000004e0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000004f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2076 3a20  --------.    v: 
-00000500: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
-00000510: 6e61 7465 732e 536b 7943 6f6f 7264 600a  nates.SkyCoord`.
-00000520: 2020 2020 2020 2020 5468 6520 706f 696e          The poin
-00000530: 7420 746f 2072 6f74 6174 652e 0a20 2020  t to rotate..   
-00000540: 2070 6976 6f74 3a20 607e 6173 7472 6f70   pivot: `~astrop
-00000550: 792e 636f 6f72 6469 6e61 7465 732e 536b  y.coordinates.Sk
-00000560: 7943 6f6f 7264 600a 2020 2020 2020 2020  yCoord`.        
-00000570: 5468 6520 706f 696e 7420 6172 6f75 6e64  The point around
-00000580: 2077 6869 6368 2074 6865 2070 6f69 6e74   which the point
-00000590: 2060 6076 6060 2069 7320 726f 7461 7465   ``v`` is rotate
-000005a0: 642e 0a20 2020 2061 6e67 6c65 3a20 607e  d..    angle: `~
-000005b0: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
-000005c0: 7465 732e 416e 676c 6560 0a20 2020 2020  tes.Angle`.     
-000005d0: 2020 2054 6865 2061 6e67 6c65 206f 6620     The angle of 
-000005e0: 726f 7461 7469 6f6e 2c20 6d65 6173 7572  rotation, measur
-000005f0: 6564 2066 726f 6d20 6e6f 7274 6820 746f  ed from north to
-00000600: 2065 6173 742e 0a20 2020 2077 6373 3a20   east..    wcs: 
-00000610: 607e 6173 7472 6f70 792e 7763 732e 5743  `~astropy.wcs.WC
-00000620: 5360 0a20 2020 2020 2020 2057 4353 206f  S`.        WCS o
-00000630: 626a 6563 742e 0a0a 2020 2020 5265 7475  bject...    Retu
-00000640: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00000650: 2020 2020 607e 6173 7472 6f70 792e 636f      `~astropy.co
-00000660: 6f72 6469 6e61 7465 732e 536b 7943 6f6f  ordinates.SkyCoo
-00000670: 7264 600a 2020 2020 2020 2020 5468 6520  rd`.        The 
-00000680: 706f 696e 7420 6166 7465 7220 7468 6520  point after the 
-00000690: 726f 7461 7469 6f6e 2e0a 2020 2020 e9ff  rotation..    ..
-000006a0: ffff ff4e 290d da15 736b 795f 706f 7369  ...N)...sky_posi
-000006b0: 7469 6f6e 5f74 6f5f 7069 7865 6cda 0c70  tion_to_pixel..p
-000006c0: 6978 656c 5f73 6361 6c65 73da 0874 6f5f  ixel_scales..to_
-000006d0: 7661 6c75 65da 0175 da03 7261 6472 0300  value..u..radr..
-000006e0: 0000 7204 0000 00da 0566 6c6f 6174 7202  ..r......floatr.
-000006f0: 0000 00da 215f 6973 5f70 6f73 6974 6976  ....!_is_positiv
-00000700: 655f 616e 676c 655f 616e 7469 5f63 6c6f  e_angle_anti_clo
-00000710: 636b 7769 7365 da02 6e70 da05 6172 7261  ckwise..np..arra
-00000720: 79da 1570 6978 656c 5f74 6f5f 736b 795f  y..pixel_to_sky_
-00000730: 706f 7369 7469 6f6e 2911 720e 0000 0072  position).r....r
-00000740: 0f00 0000 7210 0000 0072 1100 0000 5a04  ....r....r....Z.
-00000750: 765f 7078 5a08 7069 766f 745f 7078 da02  v_pxZ.pivot_px..
-00000760: 7378 da02 7379 5a09 616e 676c 655f 7261  sx..syZ.angle_ra
-00000770: 645a 0b78 5f61 6e67 6c65 5f73 6b79 5a0b  dZ.x_angle_skyZ.
-00000780: 795f 616e 676c 655f 736b 795a 0a78 5f61  y_angle_skyZ.x_a
-00000790: 6e67 6c65 5f70 785a 0a79 5f61 6e67 6c65  ngle_pxZ.y_angle
-000007a0: 5f70 785a 0861 6e67 6c65 5f70 78da 0872  _pxZ.angle_px..r
-000007b0: 6f74 6174 696f 6e5a 0e64 6966 665f 7665  otationZ.diff_ve
-000007c0: 6374 6f72 5f70 785a 0c72 6f74 6174 6564  ctor_pxZ.rotated
-000007d0: 5f76 5f70 78a9 0072 2100 0000 fa3b 2f55  _v_px..r!....;/U
-000007e0: 7365 7273 2f63 6872 6973 7469 616e 2f49  sers/christian/I
-000007f0: 6465 6150 726f 6a65 6374 732f 696d 6570  deaProjects/imep
-00000800: 6875 2f73 7263 2f69 6d65 7068 752f 6765  hu/src/imephu/ge
-00000810: 6f6d 6574 7279 2e70 79da 0672 6f74 6174  ometry.py..rotat
-00000820: 650d 0000 0073 2200 0000 0a1d 0a01 0c03  e....s".........
-00000830: 0c01 0801 0801 0401 1001 0a01 0804 0801  ................
-00000840: 0403 2001 04ff 1403 1201 0a03 7223 0000  .. .........r#..
-00000850: 00da 0c64 6973 706c 6163 656d 656e 7463  ...displacementc
-00000860: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00000870: 0500 0000 4300 0000 7342 0000 007c 0164  ....C...sB...|.d
-00000880: 0119 0074 007c 006a 01a0 0274 036a 04a1  ...t.|.j...t.j..
-00000890: 0183 011b 007d 027c 0164 0219 007d 037c  .....}.|.d...}.|
-000008a0: 006a 057c 0217 007d 047c 006a 017c 0317  .j.|...}.|.j.|..
-000008b0: 007d 0574 067c 047c 0564 038d 0253 0029  .}.t.|.|.d...S.)
-000008c0: 0561 1302 0000 4d6f 7665 2061 2070 6f69  .a....Move a poi
-000008d0: 6e74 2062 7920 6120 6469 7370 6c61 6365  nt by a displace
-000008e0: 6d65 6e74 2076 6563 746f 722e 0a0a 2020  ment vector...  
-000008f0: 2020 5468 6520 706f 696e 7420 746f 206d    The point to m
-00000900: 6f76 6520 6973 2061 7373 756d 6564 2074  ove is assumed t
-00000910: 6f20 6265 2067 6976 656e 2061 7320 7269  o be given as ri
-00000920: 6768 7420 6173 6365 6e73 696f 6e20 616e  ght ascension an
-00000930: 6420 6465 636c 696e 6174 696f 6e2e 2054  d declination. T
-00000940: 6865 0a20 2020 2064 6973 706c 6163 656d  he.    displacem
-00000950: 656e 7420 7665 6374 6f72 2069 7320 6173  ent vector is as
-00000960: 7375 6d65 6420 746f 2062 6520 6120 7665  sumed to be a ve
-00000970: 6374 6f72 206f 6e20 7468 6520 736b 792c  ctor on the sky,
-00000980: 2077 6974 6820 7265 616c 2061 6e67 6c65   with real angle
-00000990: 732c 2061 730a 2020 2020 6465 7363 7269  s, as.    descri
-000009a0: 6265 6420 666f 7220 7468 6520 607e 736b  bed for the `~sk
-000009b0: 795f 7665 6374 6f72 5f74 6f5f 7069 7865  y_vector_to_pixe
-000009c0: 6c60 206d 6574 686f 642e 0a0a 2020 2020  l` method...    
-000009d0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-000009e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 763a  ---------.    v:
-000009f0: 2060 7e61 7374 726f 7079 2e63 6f6f 7264   `~astropy.coord
-00000a00: 696e 6174 6573 2e53 6b79 436f 6f72 6460  inates.SkyCoord`
-00000a10: 0a20 2020 2020 2020 2050 6f69 6e74 2074  .        Point t
-00000a20: 6f20 6d6f 7665 2e0a 2020 2020 6469 7370  o move..    disp
-00000a30: 6c61 6365 6d65 6e74 3a20 3244 2061 7272  lacement: 2D arr
-00000a40: 6179 206f 6620 616e 676c 6573 0a20 2020  ay of angles.   
-00000a50: 2020 2020 2056 6563 746f 7220 6279 2077       Vector by w
-00000a60: 6869 6368 2074 6f20 6d6f 7665 2074 6865  hich to move the
-00000a70: 2070 6f69 6e74 2e0a 0a20 2020 2052 6574   point...    Ret
-00000a80: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00000a90: 0a20 2020 2060 7e61 7374 726f 7079 2e63  .    `~astropy.c
-00000aa0: 6f6f 7264 696e 6174 6573 2e53 6b79 436f  oordinates.SkyCo
-00000ab0: 6f72 6460 0a20 2020 2020 2020 2054 6865  ord`.        The
-00000ac0: 2070 6f69 6e74 2061 6674 6572 206d 6f76   point after mov
-00000ad0: 696e 672e 0a20 2020 2072 0100 0000 e901  ing..    r......
-00000ae0: 0000 00a9 02da 0272 61da 0364 6563 4e29  .......ra..decN)
-00000af0: 0772 0300 0000 7228 0000 0072 1600 0000  .r....r(...r....
-00000b00: 7217 0000 0072 1800 0000 7227 0000 0072  r....r....r'...r
-00000b10: 0a00 0000 2906 720e 0000 0072 2400 0000  ....).r....r$...
-00000b20: 5a15 6469 7370 6c61 6365 6d65 6e74 5f64  Z.displacement_d
-00000b30: 656c 7461 5f72 615a 1664 6973 706c 6163  elta_raZ.displac
-00000b40: 656d 656e 745f 6465 6c74 615f 6465 635a  ement_delta_decZ
-00000b50: 0f74 7261 6e73 6c61 7465 645f 765f 7261  .translated_v_ra
-00000b60: 5a10 7472 616e 736c 6174 6564 5f76 5f64  Z.translated_v_d
-00000b70: 6563 7221 0000 0072 2100 0000 7222 0000  ecr!...r!...r"..
-00000b80: 00da 0974 7261 6e73 6c61 7465 4600 0000  ...translateF...
-00000b90: 730a 0000 001a 1408 010a 030a 010c 0172  s..............r
-00000ba0: 2900 0000 6301 0000 0000 0000 0000 0000  )...c...........
-00000bb0: 0002 0000 0006 0000 0043 0000 0073 4200  .........C...sB.
-00000bc0: 0000 7400 a001 7c00 6a02 6401 1300 6a03  ..t...|.j.d...j.
-00000bd0: 6402 7404 6403 8d02 a101 7d01 7405 7c01  d.t.d.....}.t.|.
-00000be0: 6402 1900 7c00 6a06 6402 1900 8302 7405  d...|.j.d.....t.
-00000bf0: 7c01 6404 1900 7c00 6a06 6404 1900 8302  |.d...|.j.d.....
-00000c00: 6602 5300 2906 61aa 0600 000a 2020 2020  f.S.).a.....    
-00000c10: 4361 6c63 756c 6174 6520 7468 6520 7069  Calculate the pi
-00000c20: 7865 6c20 7363 616c 6573 206f 6620 6120  xel scales of a 
-00000c30: 5743 5320 6f62 6a65 6374 2e0a 0a20 2020  WCS object...   
-00000c40: 2046 6f72 2061 2057 4353 2072 6574 7572   For a WCS retur
-00000c50: 6e73 2070 6978 656c 2073 6361 6c65 7320  ns pixel scales 
-00000c60: 616c 6f6e 6720 6561 6368 2061 7869 7320  along each axis 
-00000c70: 6f66 2074 6865 2069 6d61 6765 2070 6978  of the image pix
-00000c80: 656c 2061 740a 2020 2020 7468 6520 6060  el at.    the ``
-00000c90: 4352 5049 5860 6020 6c6f 6361 7469 6f6e  CRPIX`` location
-00000ca0: 206f 6e63 6520 6974 2069 7320 7072 6f6a   once it is proj
-00000cb0: 6563 7465 6420 6f6e 746f 2074 6865 0a20  ected onto the. 
-00000cc0: 2020 2022 706c 616e 6520 6f66 2069 6e74     "plane of int
-00000cd0: 6572 6d65 6469 6174 6520 776f 726c 6420  ermediate world 
-00000ce0: 636f 6f72 6469 6e61 7465 7322 2061 7320  coordinates" as 
-00000cf0: 6465 6669 6e65 6420 696e 0a20 2020 2060  defined in.    `
-00000d00: 4772 6569 7365 6e20 2620 4361 6c61 6272  Greisen & Calabr
-00000d10: 6574 7461 2032 3030 322c 2041 2641 2c20  etta 2002, A&A, 
-00000d20: 3339 352c 2031 3036 310a 2020 2020 3c68  395, 1061.    <h
-00000d30: 7474 7073 3a2f 2f75 692e 6164 7361 6273  ttps://ui.adsabs
-00000d40: 2e68 6172 7661 7264 2e65 6475 2f61 6273  .harvard.edu/abs
-00000d50: 2f32 3030 3241 2532 3641 2e2e 2e33 3935  /2002A%26A...395
-00000d60: 2e31 3036 3147 3e60 5f2e 0a0a 2020 2020  .1061G>`_...    
-00000d70: 2e2e 206e 6f74 653a 3a0a 2020 2020 2020  .. note::.      
-00000d80: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00000d90: 6973 2063 6f6e 6365 726e 6564 202a 2a6f  is concerned **o
-00000da0: 6e6c 792a 2a20 6162 6f75 7420 7468 6520  nly** about the 
-00000db0: 7472 616e 7366 6f72 6d61 7469 6f6e 0a20  transformation. 
-00000dc0: 2020 2020 2020 2022 696d 6167 6520 706c         "image pl
-00000dd0: 616e 6522 2d3e 2270 726f 6a65 6374 696f  ane"->"projectio
-00000de0: 6e20 706c 616e 6522 2061 6e64 202a 2a6e  n plane" and **n
-00000df0: 6f74 2a2a 2061 626f 7574 2074 6865 0a20  ot** about the. 
-00000e00: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00000e10: 6174 696f 6e20 2263 656c 6573 7469 616c  ation "celestial
-00000e20: 2073 7068 6572 6522 2d3e 2270 726f 6a65   sphere"->"proje
-00000e30: 6374 696f 6e20 706c 616e 6522 2d3e 2269  ction plane"->"i
-00000e40: 6d61 6765 2070 6c61 6e65 222e 0a20 2020  mage plane"..   
-00000e50: 2020 2020 2054 6865 7265 666f 7265 2c20       Therefore, 
-00000e60: 7468 6973 2066 756e 6374 696f 6e20 6967  this function ig
-00000e70: 6e6f 7265 7320 6469 7374 6f72 7469 6f6e  nores distortion
-00000e80: 7320 6172 6973 696e 6720 6475 6520 746f  s arising due to
-00000e90: 0a20 2020 2020 2020 206e 6f6e 2d6c 696e  .        non-lin
-00000ea0: 6561 7220 6e61 7475 7265 206f 6620 6d6f  ear nature of mo
-00000eb0: 7374 2070 726f 6a65 6374 696f 6e73 2e0a  st projections..
-00000ec0: 0a20 2020 202e 2e20 6e6f 7465 3a3a 0a20  .    .. note::. 
-00000ed0: 2020 2020 2020 2049 6e20 6f72 6465 7220         In order 
-00000ee0: 746f 2063 6f6d 7075 7465 2074 6865 2073  to compute the s
-00000ef0: 6361 6c65 7320 636f 7272 6573 706f 6e64  cales correspond
-00000f00: 696e 6720 746f 2063 656c 6573 7469 616c  ing to celestial
-00000f10: 2061 7865 7320 6f6e 6c79 2c0a 2020 2020   axes only,.    
-00000f20: 2020 2020 6d61 6b65 2073 7572 6520 7468      make sure th
-00000f30: 6174 2074 6865 2069 6e70 7574 2060 7e61  at the input `~a
-00000f40: 7374 726f 7079 2e77 6373 2e57 4353 6020  stropy.wcs.WCS` 
-00000f50: 6f62 6a65 6374 2063 6f6e 7461 696e 730a  object contains.
-00000f60: 2020 2020 2020 2020 6365 6c65 7374 6961          celestia
-00000f70: 6c20 6178 6573 206f 6e6c 792c 2065 2e67  l axes only, e.g
-00000f80: 2e2c 2062 7920 7061 7373 696e 6720 696e  ., by passing in
-00000f90: 2074 6865 0a20 2020 2020 2020 2060 7e61   the.        `~a
-00000fa0: 7374 726f 7079 2e77 6373 2e57 4353 2e63  stropy.wcs.WCS.c
-00000fb0: 656c 6573 7469 616c 6020 5743 5320 6f62  elestial` WCS ob
-00000fc0: 6a65 6374 2e0a 0a20 2020 2054 6865 2063  ject...    The c
-00000fd0: 6f64 6520 6861 7320 6265 656e 2061 6461  ode has been ada
-00000fe0: 7074 6564 2066 726f 6d20 4150 4c70 792e  pted from APLpy.
-00000ff0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00001000: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00001010: 2020 2020 7763 7320 3a20 607e 6173 7472      wcs : `~astr
-00001020: 6f70 792e 7763 732e 5743 5360 0a20 2020  opy.wcs.WCS`.   
-00001030: 2020 2020 2041 2077 6f72 6c64 2063 6f6f       A world coo
-00001040: 7264 696e 6174 6520 7379 7374 656d 206f  rdinate system o
-00001050: 626a 6563 742e 0a0a 2020 2020 5265 7475  bject...    Retu
-00001060: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00001070: 2020 2020 7363 616c 6520 3a20 7475 706c      scale : tupl
-00001080: 6520 6f66 2060 7e61 7374 726f 7079 2e63  e of `~astropy.c
-00001090: 6f6f 7264 696e 6174 6573 2e41 6e67 6c65  oordinates.Angle
-000010a0: 600a 2020 2020 2020 2020 4120 7665 6374  `.        A vect
-000010b0: 6f72 2028 607e 6e75 6d70 792e 6e64 6172  or (`~numpy.ndar
-000010c0: 7261 7960 2920 6f66 2070 726f 6a65 6374  ray`) of project
-000010d0: 696f 6e20 706c 616e 6520 696e 6372 656d  ion plane increm
-000010e0: 656e 7473 0a20 2020 2020 2020 2063 6f72  ents.        cor
-000010f0: 7265 7370 6f6e 6469 6e67 2074 6f20 6561  responding to ea
-00001100: 6368 2070 6978 656c 2073 6964 6520 2861  ch pixel side (a
-00001110: 7869 7329 2e20 5468 6520 756e 6974 7320  xis). The units 
-00001120: 6f66 2074 6865 2072 6574 7572 6e65 640a  of the returned.
-00001130: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-00001140: 6172 6520 7468 6520 7361 6d65 2061 7320  are the same as 
-00001150: 7468 6520 756e 6974 7320 6f66 2060 7e61  the units of `~a
-00001160: 7374 726f 7079 2e77 6373 2e57 6373 7072  stropy.wcs.Wcspr
-00001170: 6d2e 6364 656c 7460 2c0a 2020 2020 2020  m.cdelt`,.      
-00001180: 2020 607e 6173 7472 6f70 792e 7763 732e    `~astropy.wcs.
-00001190: 5763 7370 726d 2e63 7276 616c 602c 2061  Wcsprm.crval`, a
-000011a0: 6e64 2060 7e61 7374 726f 7079 2e77 6373  nd `~astropy.wcs
-000011b0: 2e57 6373 7072 6d2e 6364 6020 666f 720a  .Wcsprm.cd` for.
-000011c0: 2020 2020 2020 2020 7468 6520 6365 6c65          the cele
-000011d0: 7374 6961 6c20 5743 5320 616e 6420 6361  stial WCS and ca
-000011e0: 6e20 6265 206f 6274 6169 6e65 6420 6279  n be obtained by
-000011f0: 2069 6e71 7569 7269 6e67 2074 6865 2076   inquiring the v
-00001200: 616c 7565 0a20 2020 2020 2020 206f 6620  alue.        of 
-00001210: 607e 6173 7472 6f70 792e 7763 732e 5763  `~astropy.wcs.Wc
-00001220: 7370 726d 2e63 756e 6974 6020 7072 6f70  sprm.cunit` prop
-00001230: 6572 7479 206f 6620 7468 6520 696e 7075  erty of the inpu
-00001240: 740a 2020 2020 2020 2020 607e 6173 7472  t.        `~astr
-00001250: 6f70 792e 7763 732e 5743 5360 2057 4353  opy.wcs.WCS` WCS
-00001260: 206f 626a 6563 742e 0a0a 2020 2020 5365   object...    Se
-00001270: 6520 416c 736f 0a20 2020 202d 2d2d 2d2d  e Also.    -----
-00001280: 2d2d 2d0a 2020 2020 6173 7472 6f70 792e  ---.    astropy.
-00001290: 7763 732e 7574 696c 732e 7072 6f6a 5f70  wcs.utils.proj_p
-000012a0: 6c61 6e65 5f70 6978 656c 5f61 7265 610a  lane_pixel_area.
-000012b0: 0a20 2020 20e9 0200 0000 7201 0000 0029  .    .....r....)
-000012c0: 02da 0461 7869 73da 0564 7479 7065 7225  ...axis..dtyper%
-000012d0: 0000 004e 2907 721b 0000 00da 0473 7172  ...N).r......sqr
-000012e0: 74da 1270 6978 656c 5f73 6361 6c65 5f6d  t..pixel_scale_m
-000012f0: 6174 7269 78da 0373 756d 7219 0000 0072  atrix..sumr....r
-00001300: 0900 0000 da10 776f 726c 645f 6178 6973  ......world_axis
-00001310: 5f75 6e69 7473 2902 7211 0000 00da 0d73  _units).r......s
-00001320: 6361 6c65 5f66 6163 746f 7273 7221 0000  cale_factorsr!..
-00001330: 0072 2100 0000 7222 0000 0072 1500 0000  .r!...r"...r....
-00001340: 6300 0000 7308 0000 001a 2e12 0212 0104  c...s...........
-00001350: fe72 1500 0000 da08 706f 7369 7469 6f6e  .r......position
-00001360: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00001370: 0006 0000 0043 0000 0073 3200 0000 7400  .....C...s2...t.
-00001380: 7c00 7c01 6401 8d02 7d02 7401 a002 7403  |.|.d...}.t...t.
-00001390: 7c02 6402 1900 a004 a100 8301 7403 7c02  |.d.........t.|.
-000013a0: 6403 1900 a004 a100 8301 6702 a101 5300  d.........g...S.
-000013b0: 2905 6151 0100 0043 6f6e 7665 7274 2061  ).aQ...Convert a
-000013c0: 2073 6b79 2070 6f73 6974 696f 6e20 746f   sky position to
-000013d0: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
-000013e0: 6e67 2070 6978 656c 2063 6f6f 7264 696e  ng pixel coordin
-000013f0: 6174 6573 2e0a 0a20 2020 2050 6172 616d  ates...    Param
-00001400: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00001410: 2d2d 2d2d 0a20 2020 2070 6f73 6974 696f  ----.    positio
-00001420: 6e3a 2060 7e61 7374 726f 7079 2e63 6f6f  n: `~astropy.coo
-00001430: 7264 696e 6174 6573 2e53 6b79 436f 6f72  rdinates.SkyCoor
-00001440: 6460 0a20 2020 2020 2020 2053 6b79 2070  d`.        Sky p
-00001450: 6f73 6974 696f 6e20 6173 2072 6967 6874  osition as right
-00001460: 2061 7363 656e 7369 6f6e 2061 6e64 2064   ascension and d
-00001470: 6563 6c69 6e61 7469 6f6e 2e0a 2020 2020  eclination..    
-00001480: 7763 733a 2060 7e61 7374 726f 7079 2e77  wcs: `~astropy.w
-00001490: 6373 2e57 4353 600a 2020 2020 2020 2020  cs.WCS`.        
-000014a0: 5743 5320 6f62 6a65 6374 2e0a 0a20 2020  WCS object...   
-000014b0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-000014c0: 2d2d 2d2d 0a20 2020 2060 7e6e 756d 7079  ----.    `~numpy
-000014d0: 2e6e 6461 7272 6179 6020 6f66 2060 666c  .ndarray` of `fl
-000014e0: 6f61 7460 0a20 2020 2020 2020 2054 6865  oat`.        The
-000014f0: 2070 6978 656c 2063 6f6f 7264 696e 6174   pixel coordinat
-00001500: 6573 2e0a 2020 2020 2902 da06 636f 6f72  es..    )...coor
-00001510: 6473 7211 0000 0072 0100 0000 7225 0000  dsr....r....r%..
-00001520: 004e 2905 720d 0000 0072 1b00 0000 721c  .N).r....r....r.
-00001530: 0000 0072 1900 0000 da04 6974 656d 2903  ...r......item).
-00001540: 7232 0000 0072 1100 0000 5a0c 7069 7865  r2...r....Z.pixe
-00001550: 6c5f 636f 6f72 6473 7221 0000 0072 2100  l_coordsr!...r!.
-00001560: 0000 7222 0000 0072 1400 0000 9800 0000  ..r"...r........
-00001570: 7304 0000 000c 0f26 0172 1400 0000 da0b  s......&.r......
-00001580: 706f 7369 7469 6f6e 5f70 7863 0200 0000  position_pxc....
-00001590: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000015a0: 4300 0000 7316 0000 0074 007c 0064 0119  C...s....t.|.d..
-000015b0: 007c 0064 0219 007c 0164 038d 0353 0029  .|.d...|.d...S.)
-000015c0: 0561 3201 0000 436f 6e76 6572 7420 7069  .a2...Convert pi
-000015d0: 7865 6c20 636f 6f72 6469 6e61 7465 7320  xel coordinates 
-000015e0: 746f 2074 6865 2063 6f72 7265 7370 6f6e  to the correspon
-000015f0: 6469 6e67 2073 6b79 2070 6f73 6974 696f  ding sky positio
-00001600: 6e2e 0a0a 2020 2020 5061 7261 6d65 7465  n...    Paramete
-00001610: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00001620: 2d0a 2020 2020 706f 7369 7469 6f6e 5f70  -.    position_p
-00001630: 783a 2060 7e6e 756d 7079 2e6e 6461 7272  x: `~numpy.ndarr
-00001640: 6179 6020 6f66 2060 666c 6f61 7460 0a20  ay` of `float`. 
-00001650: 2020 2020 2020 2050 6978 656c 2063 6f6f         Pixel coo
-00001660: 7264 696e 6174 6573 2e0a 2020 2020 7763  rdinates..    wc
-00001670: 733a 2060 7e61 7374 726f 7079 2e77 6373  s: `~astropy.wcs
-00001680: 2e57 4353 600a 2020 2020 2020 2020 5743  .WCS`.        WC
-00001690: 5320 6f62 6a65 6374 2e0a 0a20 2020 2052  S object...    R
-000016a0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-000016b0: 2d2d 0a20 2020 2060 7e61 7374 726f 7079  --.    `~astropy
-000016c0: 2e63 6f6f 7264 696e 6174 6573 2e53 6b79  .coordinates.Sky
-000016d0: 436f 6f72 6460 0a20 2020 2020 2020 2054  Coord`.        T
-000016e0: 6865 2073 6b79 2063 6f6f 7264 696e 6174  he sky coordinat
-000016f0: 6573 2e0a 2020 2020 7201 0000 0072 2500  es..    r....r%.
-00001700: 0000 2901 7211 0000 004e 2901 720c 0000  ..).r....N).r...
-00001710: 0029 0272 3500 0000 7211 0000 0072 2100  .).r5...r....r!.
-00001720: 0000 7221 0000 0072 2200 0000 721d 0000  ..r!...r"...r...
-00001730: 00ab 0000 0073 0200 0000 160f 721d 0000  .....s......r...
-00001740: 0063 0100 0000 0000 0000 0000 0000 1800  .c..............
-00001750: 0000 0700 0000 4300 0000 7338 0100 0074  ......C...s8...t
-00001760: 00a0 0164 01a1 017d 0174 027c 017c 0083  ...d...}.t.|.|..
-00001770: 027d 027c 026a 037d 037c 026a 047d 047c  .}.|.j.}.|.j.}.|
-00001780: 037d 057c 0464 0274 056a 0614 0017 007d  .}.|.d.t.j.....}
-00001790: 0674 077c 057c 0664 038d 027d 0774 087c  .t.|.|.d...}.t.|
-000017a0: 077c 0083 027d 087c 0364 0274 056a 0614  .|...}.|.d.t.j..
-000017b0: 0017 007d 097c 0464 0274 056a 0614 0017  ...}.|.d.t.j....
-000017c0: 007d 0a74 077c 097c 0a64 038d 027d 0b74  .}.t.|.|.d...}.t
-000017d0: 087c 0b7c 0083 027d 0c7c 0364 0274 056a  .|.|...}.|.d.t.j
-000017e0: 0614 0018 007d 0d7c 0464 0274 056a 0614  .....}.|.d.t.j..
-000017f0: 0017 007d 0e74 077c 0d7c 0e64 038d 027d  ...}.t.|.|.d...}
-00001800: 0f74 087c 0f7c 0083 027d 107c 087d 117c  .t.|.|...}.|.}.|
-00001810: 0c7d 127c 107d 1374 00a0 097c 117c 12a1  .}.|.}.t...|.|..
-00001820: 0274 006a 0aa0 0b7c 11a1 0174 006a 0aa0  .t.j...|...t.j..
-00001830: 0b7c 12a1 0114 001b 007d 1474 0ca0 0d7c  .|.......}.t...|
-00001840: 14a1 017d 1574 00a0 0174 0e7c 1583 0174  ...}.t...t.|...t
-00001850: 0f7c 1583 010b 0067 0274 0f7c 1583 0174  .|.....g.t.|...t
-00001860: 0e7c 1583 0167 0267 02a1 017d 1674 00a0  .|...g.g...}.t..
-00001870: 097c 167c 11a1 027d 1774 1074 1174 00a0  .|.|...}.t.t.t..
-00001880: 097c 177c 12a1 0274 00a0 097c 177c 13a1  .|.|...t...|.|..
-00001890: 026b 0483 0253 0029 0561 4e02 0000 0a20  .k...S.).aN.... 
-000018a0: 2020 2052 6574 7572 6e20 7768 6574 6865     Return whethe
-000018b0: 7220 666f 7220 6120 6769 7665 6e20 5743  r for a given WC
-000018c0: 5320 706f 7369 7469 7665 2061 6e67 6c65  S positive angle
-000018d0: 7320 6172 6520 616e 7469 2d63 6c6f 636b  s are anti-clock
-000018e0: 7769 7365 2077 6865 6e20 706c 6f74 7465  wise when plotte
-000018f0: 642e 0a0a 2020 2020 416e 676c 6573 206f  d...    Angles o
-00001900: 6e20 7468 6520 736b 7920 6172 6520 6d65  n the sky are me
-00001910: 6173 7572 6564 2066 726f 6d20 6e6f 7274  asured from nort
-00001920: 6820 746f 2065 6173 742c 2061 6e64 2064  h to east, and d
-00001930: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
-00001940: 6f72 6965 6e74 6174 696f 6e0a 2020 2020  orientation.    
-00001950: 6f66 2074 6865 2061 7865 7320 6f6e 2074  of the axes on t
-00001960: 6865 2066 696e 6465 7220 6368 6172 7420  he finder chart 
-00001970: 7468 6973 206d 6179 2063 6f72 7265 7370  this may corresp
-00001980: 6f6e 6420 746f 2061 206d 6174 6865 6d61  ond to a mathema
-00001990: 7469 6361 6c6c 7920 706f 7369 7469 7665  tically positive
-000019a0: 0a20 2020 2028 2261 6e74 692d 636c 6f63  .    ("anti-cloc
-000019b0: 6b77 6973 6522 2920 6f72 206e 6567 6174  kwise") or negat
-000019c0: 6976 6520 2822 636c 6f63 6b77 6973 6522  ive ("clockwise"
-000019d0: 2920 616e 676c 652e 0a0a 2020 2020 5061  ) angle...    Pa
-000019e0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-000019f0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7763 733a  -------.    wcs:
-00001a00: 2060 7e61 7374 726f 7079 2e77 6373 2e57   `~astropy.wcs.W
-00001a10: 4353 600a 2020 2020 2020 2020 5743 5320  CS`.        WCS 
-00001a20: 6f62 6a65 6374 2e0a 0a20 2020 2052 6574  object...    Ret
-00001a30: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00001a40: 0a20 2020 2062 6f6f 6c0a 2020 2020 2020  .    bool.      
-00001a50: 2020 6060 5472 7565 6060 2069 6620 616e    ``True`` if an
-00001a60: 676c 6573 2066 726f 6d20 6e6f 7274 6820  gles from north 
-00001a70: 746f 2065 6173 7420 636f 7272 6573 706f  to east correspo
-00001a80: 6e64 2074 6f20 6d61 7468 656d 6174 6963  nd to mathematic
-00001a90: 616c 6c79 2070 6f73 6974 6976 650a 2020  ally positive.  
-00001aa0: 2020 2020 2020 2822 616e 7469 2d63 6c6f        ("anti-clo
-00001ab0: 636b 7769 7365 2229 2061 6e67 6c65 7320  ckwise") angles 
-00001ac0: 6f6e 2061 2066 696e 6465 7220 6368 6172  on a finder char
-00001ad0: 742c 2060 6046 616c 7365 6060 206f 7468  t, ``False`` oth
-00001ae0: 6572 7769 7365 2e0a 2020 2020 2902 e700  erwise..    )...
-00001af0: 0000 0000 0000 0072 3600 0000 7225 0000  .......r6...r%..
-00001b00: 0072 2600 0000 4e29 1272 1b00 0000 721c  .r&...N).r....r.
-00001b10: 0000 0072 1d00 0000 7227 0000 0072 2800  ...r....r'...r(.
-00001b20: 0000 7217 0000 00da 0661 7263 6d69 6e72  ..r......arcminr
-00001b30: 0a00 0000 7214 0000 00da 0364 6f74 da06  ....r......dot..
-00001b40: 6c69 6e61 6c67 da04 6e6f 726d da04 6d61  linalg..norm..ma
-00001b50: 7468 da04 6163 6f73 7203 0000 0072 0400  th..acosr....r..
-00001b60: 0000 7207 0000 00da 0462 6f6f 6c29 1872  ..r......bool).r
-00001b70: 1100 0000 5a09 6f72 6967 696e 5f70 785a  ....Z.origin_pxZ
-00001b80: 0d6f 7269 6769 6e5f 6f6e 5f73 6b79 5a09  .origin_on_skyZ.
-00001b90: 6f72 6967 696e 5f72 615a 0a6f 7269 6769  origin_raZ.origi
-00001ba0: 6e5f 6465 635a 1170 6f69 6e74 5f74 6f5f  n_decZ.point_to_
-00001bb0: 6e6f 7274 685f 7261 5a12 706f 696e 745f  north_raZ.point_
-00001bc0: 746f 5f6e 6f72 7468 5f64 6563 5a0e 706f  to_north_decZ.po
-00001bd0: 696e 745f 746f 5f6e 6f72 7468 5a11 706f  int_to_northZ.po
-00001be0: 696e 745f 746f 5f6e 6f72 7468 5f70 785a  int_to_north_pxZ
-00001bf0: 1670 6f69 6e74 5f74 6f5f 6e6f 7274 685f  .point_to_north_
-00001c00: 6561 7374 5f72 615a 1770 6f69 6e74 5f74  east_raZ.point_t
-00001c10: 6f5f 6e6f 7274 685f 6561 7374 5f64 6563  o_north_east_dec
-00001c20: 5a13 706f 696e 745f 746f 5f6e 6f72 7468  Z.point_to_north
-00001c30: 5f65 6173 745a 1670 6f69 6e74 5f74 6f5f  _eastZ.point_to_
-00001c40: 6e6f 7274 685f 6561 7374 5f70 785a 1670  north_east_pxZ.p
-00001c50: 6f69 6e74 5f74 6f5f 6e6f 7274 685f 7765  oint_to_north_we
-00001c60: 7374 5f72 615a 1770 6f69 6e74 5f74 6f5f  st_raZ.point_to_
-00001c70: 6e6f 7274 685f 7765 7374 5f64 6563 5a13  north_west_decZ.
-00001c80: 706f 696e 745f 746f 5f6e 6f72 7468 5f77  point_to_north_w
-00001c90: 6573 745a 1670 6f69 6e74 5f74 6f5f 6e6f  estZ.point_to_no
-00001ca0: 7274 685f 7765 7374 5f70 785a 0f6e 6f72  rth_west_pxZ.nor
-00001cb0: 7468 5f76 6563 746f 725f 7078 5a14 6e6f  th_vector_pxZ.no
-00001cc0: 7274 685f 6561 7374 5f76 6563 746f 725f  rth_east_vector_
-00001cd0: 7078 5a14 6e6f 7274 685f 7765 7374 5f76  pxZ.north_west_v
-00001ce0: 6563 746f 725f 7078 da09 636f 735f 616e  ector_px..cos_an
-00001cf0: 676c 6572 1000 0000 7220 0000 005a 1772  gler....r ...Z.r
-00001d00: 6f74 6174 6564 5f6e 6f72 7468 5f76 6563  otated_north_vec
-00001d10: 746f 725f 7078 7221 0000 0072 2100 0000  tor_pxr!...r!...
-00001d20: 7222 0000 0072 1a00 0000 bd00 0000 734a  r"...r........sJ
-00001d30: 0000 000a 130a 0106 0106 0104 030e 010c  ................
-00001d40: 010a 010e 030e 0102 0104 0106 ff0a 030e  ................
-00001d50: 030e 0102 0104 0106 ff0a 0304 0504 0104  ................
-00001d60: 010a 0516 0104 ff0a 0304 0320 0104 ff0c  ........... ....
-00001d70: 0302 0602 010a 010a 0102 ff04 fe72 1a00  .............r..
-00001d80: 0000 2920 723b 0000 0072 0200 0000 7203  ..) r;...r....r.
-00001d90: 0000 0072 0400 0000 da06 7479 7069 6e67  ...r......typing
-00001da0: 7205 0000 0072 0600 0000 7207 0000 00da  r....r....r.....
-00001db0: 056e 756d 7079 721b 0000 005a 0c6e 756d  .numpyr....Z.num
-00001dc0: 7079 2e74 7970 696e 67da 036e 7074 da07  py.typing..npt..
-00001dd0: 6173 7472 6f70 7972 0800 0000 7217 0000  astropyr....r...
-00001de0: 00da 1361 7374 726f 7079 2e63 6f6f 7264  ...astropy.coord
-00001df0: 696e 6174 6573 7209 0000 0072 0a00 0000  inatesr....r....
-00001e00: da0b 6173 7472 6f70 792e 7763 7372 0b00  ..astropy.wcsr..
-00001e10: 0000 da11 6173 7472 6f70 792e 7763 732e  ....astropy.wcs.
-00001e20: 7574 696c 7372 0c00 0000 720d 0000 0072  utilsr....r....r
-00001e30: 2300 0000 7229 0000 0072 1500 0000 5a07  #...r)...r....Z.
-00001e40: 4e44 4172 7261 79da 0666 6c6f 6174 5f72  NDArray..float_r
-00001e50: 1400 0000 721d 0000 0072 3d00 0000 721a  ....r....r=...r.
-00001e60: 0000 0072 2100 0000 7221 0000 0072 2100  ...r!...r!...r!.
-00001e70: 0000 7222 0000 00da 083c 6d6f 6475 6c65  ..r".....<module
-00001e80: 3e01 0000 0073 1e00 0000 0800 1401 1401  >....s..........
-00001e90: 0802 0c01 0c01 1001 0c01 1001 1e03 1639  ...............9
-00001ea0: 1a1d 1e35 1e13 1612                      ...5....
+00000000: 696d 706f 7274 206d 6174 680a 6672 6f6d  import math.from
+00000010: 206d 6174 6820 696d 706f 7274 2061 7461   math import ata
+00000020: 6e32 2c20 636f 732c 2073 696e 0a66 726f  n2, cos, sin.fro
+00000030: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000040: 416e 792c 2054 7570 6c65 2c20 6361 7374  Any, Tuple, cast
+00000050: 0a0a 696d 706f 7274 206e 756d 7079 2061  ..import numpy a
+00000060: 7320 6e70 0a69 6d70 6f72 7420 6e75 6d70  s np.import nump
+00000070: 792e 7479 7069 6e67 2061 7320 6e70 740a  y.typing as npt.
+00000080: 6672 6f6d 2061 7374 726f 7079 2069 6d70  from astropy imp
+00000090: 6f72 7420 756e 6974 7320 6173 2075 0a66  ort units as u.f
+000000a0: 726f 6d20 6173 7472 6f70 792e 636f 6f72  rom astropy.coor
+000000b0: 6469 6e61 7465 7320 696d 706f 7274 2041  dinates import A
+000000c0: 6e67 6c65 2c20 536b 7943 6f6f 7264 0a66  ngle, SkyCoord.f
+000000d0: 726f 6d20 6173 7472 6f70 792e 7763 7320  rom astropy.wcs 
+000000e0: 696d 706f 7274 2057 4353 0a66 726f 6d20  import WCS.from 
+000000f0: 6173 7472 6f70 792e 7763 732e 7574 696c  astropy.wcs.util
+00000100: 7320 696d 706f 7274 2070 6978 656c 5f74  s import pixel_t
+00000110: 6f5f 736b 7963 6f6f 7264 2c20 736b 7963  o_skycoord, skyc
+00000120: 6f6f 7264 5f74 6f5f 7069 7865 6c0a 0a0a  oord_to_pixel...
+00000130: 6465 6620 726f 7461 7465 2876 3a20 536b  def rotate(v: Sk
+00000140: 7943 6f6f 7264 2c20 7069 766f 743a 2053  yCoord, pivot: S
+00000150: 6b79 436f 6f72 642c 2061 6e67 6c65 3a20  kyCoord, angle: 
+00000160: 416e 676c 652c 2077 6373 3a20 5743 5329  Angle, wcs: WCS)
+00000170: 202d 3e20 536b 7943 6f6f 7264 3a0a 2020   -> SkyCoord:.  
+00000180: 2020 2222 2252 6f74 6174 6520 6120 706f    """Rotate a po
+00000190: 696e 7420 6172 6f75 6e64 2061 2070 6976  int around a piv
+000001a0: 6f74 2e0a 0a20 2020 2042 6f74 6820 7468  ot...    Both th
+000001b0: 6520 7069 766f 7420 616e 6420 7468 6520  e pivot and the 
+000001c0: 706f 696e 7420 746f 2072 6f74 6174 6520  point to rotate 
+000001d0: 6172 6520 6173 7375 6d65 6420 746f 2062  are assumed to b
+000001e0: 6520 6769 7665 6e20 6173 2072 6967 6874  e given as right
+000001f0: 2061 7363 656e 7369 6f6e 0a20 2020 2061   ascension.    a
+00000200: 6e64 2064 6563 6c69 6e61 7469 6f6e 2e20  nd declination. 
+00000210: 5468 6520 726f 7461 7469 6f6e 2061 6e67  The rotation ang
+00000220: 6c65 2069 7320 7461 6b65 6e20 746f 2062  le is taken to b
+00000230: 6520 7468 6520 616e 676c 6520 6f6e 2074  e the angle on t
+00000240: 6865 2073 6b79 2e20 4966 2074 6865 0a20  he sky. If the. 
+00000250: 2020 2070 6978 656c 2073 6361 6c65 7320     pixel scales 
+00000260: 666f 7220 7269 6768 7420 6173 6365 6e73  for right ascens
+00000270: 696f 6e20 616e 6420 6465 636c 696e 6174  ion and declinat
+00000280: 696f 6e20 6469 6666 6572 2c20 7468 6520  ion differ, the 
+00000290: 616e 676c 6520 7365 656e 206f 6e20 7468  angle seen on th
+000002a0: 650a 2020 2020 6669 6e64 6572 2063 6861  e.    finder cha
+000002b0: 7274 2077 696c 6c20 6469 6666 6572 2066  rt will differ f
+000002c0: 726f 6d20 7468 6973 2061 6e67 6c65 2e0a  rom this angle..
+000002d0: 0a20 2020 2054 6865 2061 6e67 6c65 2069  .    The angle i
+000002e0: 7320 6d65 6173 7572 6564 2066 726f 6d20  s measured from 
+000002f0: 6e6f 7274 6820 746f 2073 6f75 7468 2e20  north to south. 
+00000300: 4865 6e63 6520 6974 2064 6570 656e 6473  Hence it depends
+00000310: 206f 6e20 7468 6520 6f72 6965 6e74 6174   on the orientat
+00000320: 696f 6e20 6f66 0a20 2020 2074 6865 2063  ion of.    the c
+00000330: 6f6f 7264 696e 6174 6520 6178 6573 2077  oordinate axes w
+00000340: 6865 7468 6572 2061 2070 6f73 6974 6976  hether a positiv
+00000350: 6520 616e 676c 6520 636f 7272 6573 706f  e angle correspo
+00000360: 6e64 7320 746f 2061 2063 6c6f 636b 7769  nds to a clockwi
+00000370: 7365 206f 720a 2020 2020 616e 7469 2d63  se or.    anti-c
+00000380: 6c6f 636b 7769 7365 206f 7269 656e 7461  lockwise orienta
+00000390: 7469 6f6e 2e0a 0a20 2020 2050 6172 616d  tion...    Param
+000003a0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000003b0: 2d2d 2d2d 0a20 2020 2076 3a20 607e 6173  ----.    v: `~as
+000003c0: 7472 6f70 792e 636f 6f72 6469 6e61 7465  tropy.coordinate
+000003d0: 732e 536b 7943 6f6f 7264 600a 2020 2020  s.SkyCoord`.    
+000003e0: 2020 2020 5468 6520 706f 696e 7420 746f      The point to
+000003f0: 2072 6f74 6174 652e 0a20 2020 2070 6976   rotate..    piv
+00000400: 6f74 3a20 607e 6173 7472 6f70 792e 636f  ot: `~astropy.co
+00000410: 6f72 6469 6e61 7465 732e 536b 7943 6f6f  ordinates.SkyCoo
+00000420: 7264 600a 2020 2020 2020 2020 5468 6520  rd`.        The 
+00000430: 706f 696e 7420 6172 6f75 6e64 2077 6869  point around whi
+00000440: 6368 2074 6865 2070 6f69 6e74 2060 6076  ch the point ``v
+00000450: 6060 2069 7320 726f 7461 7465 642e 0a20  `` is rotated.. 
+00000460: 2020 2061 6e67 6c65 3a20 607e 6173 7472     angle: `~astr
+00000470: 6f70 792e 636f 6f72 6469 6e61 7465 732e  opy.coordinates.
+00000480: 416e 676c 6560 0a20 2020 2020 2020 2054  Angle`.        T
+00000490: 6865 2061 6e67 6c65 206f 6620 726f 7461  he angle of rota
+000004a0: 7469 6f6e 2c20 6d65 6173 7572 6564 2066  tion, measured f
+000004b0: 726f 6d20 6e6f 7274 6820 746f 2065 6173  rom north to eas
+000004c0: 742e 0a20 2020 2077 6373 3a20 607e 6173  t..    wcs: `~as
+000004d0: 7472 6f70 792e 7763 732e 5743 5360 0a20  tropy.wcs.WCS`. 
+000004e0: 2020 2020 2020 2057 4353 206f 626a 6563         WCS objec
+000004f0: 742e 0a0a 2020 2020 5265 7475 726e 730a  t...    Returns.
+00000500: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00000510: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
+00000520: 6e61 7465 732e 536b 7943 6f6f 7264 600a  nates.SkyCoord`.
+00000530: 2020 2020 2020 2020 5468 6520 706f 696e          The poin
+00000540: 7420 6166 7465 7220 7468 6520 726f 7461  t after the rota
+00000550: 7469 6f6e 2e0a 2020 2020 2222 220a 2020  tion..    """.  
+00000560: 2020 2320 436f 6e76 6572 7420 6672 6f6d    # Convert from
+00000570: 2077 6f72 6c64 2063 6f6f 7264 696e 6174   world coordinat
+00000580: 6573 2074 6f20 7069 7865 6c73 0a20 2020  es to pixels.   
+00000590: 2076 5f70 7820 3d20 736b 795f 706f 7369   v_px = sky_posi
+000005a0: 7469 6f6e 5f74 6f5f 7069 7865 6c28 762c  tion_to_pixel(v,
+000005b0: 2077 6373 290a 2020 2020 7069 766f 745f   wcs).    pivot_
+000005c0: 7078 203d 2073 6b79 5f70 6f73 6974 696f  px = sky_positio
+000005d0: 6e5f 746f 5f70 6978 656c 2870 6976 6f74  n_to_pixel(pivot
+000005e0: 2c20 7763 7329 0a0a 2020 2020 2320 436f  , wcs)..    # Co
+000005f0: 7272 6563 7420 7468 6520 616e 676c 6520  rrect the angle 
+00000600: 666f 7220 6469 6666 6572 656e 7420 7069  for different pi
+00000610: 7865 6c20 7363 616c 6573 0a20 2020 2073  xel scales.    s
+00000620: 782c 2073 7920 3d20 7069 7865 6c5f 7363  x, sy = pixel_sc
+00000630: 616c 6573 2877 6373 290a 2020 2020 616e  ales(wcs).    an
+00000640: 676c 655f 7261 6420 3d20 616e 676c 652e  gle_rad = angle.
+00000650: 746f 5f76 616c 7565 2875 2e72 6164 290a  to_value(u.rad).
+00000660: 2020 2020 785f 616e 676c 655f 736b 7920      x_angle_sky 
+00000670: 3d20 636f 7328 616e 676c 655f 7261 6429  = cos(angle_rad)
+00000680: 0a20 2020 2079 5f61 6e67 6c65 5f73 6b79  .    y_angle_sky
+00000690: 203d 2073 696e 2861 6e67 6c65 5f72 6164   = sin(angle_rad
+000006a0: 290a 2020 2020 785f 616e 676c 655f 7078  ).    x_angle_px
+000006b0: 203d 2078 5f61 6e67 6c65 5f73 6b79 0a20   = x_angle_sky. 
+000006c0: 2020 2079 5f61 6e67 6c65 5f70 7820 3d20     y_angle_px = 
+000006d0: 666c 6f61 7428 7378 202f 2073 7929 202a  float(sx / sy) *
+000006e0: 2079 5f61 6e67 6c65 5f73 6b79 0a20 2020   y_angle_sky.   
+000006f0: 2061 6e67 6c65 5f70 7820 3d20 6174 616e   angle_px = atan
+00000700: 3228 795f 616e 676c 655f 7078 2c20 785f  2(y_angle_px, x_
+00000710: 616e 676c 655f 7078 290a 0a20 2020 2023  angle_px)..    #
+00000720: 2049 6620 6e65 6365 7373 6172 792c 2063   If necessary, c
+00000730: 6861 6e67 6520 7468 6520 7369 676e 206f  hange the sign o
+00000740: 6620 7468 6520 616e 676c 6520 746f 2061  f the angle to a
+00000750: 6363 6f6d 6d6f 6461 7465 2074 6865 206f  ccommodate the o
+00000760: 7269 656e 7461 7469 6f6e 206f 6620 7468  rientation of th
+00000770: 650a 2020 2020 2320 6178 6573 206f 6e20  e.    # axes on 
+00000780: 7468 6520 6669 6e64 6572 2063 6861 7274  the finder chart
+00000790: 2e0a 2020 2020 6966 206e 6f74 205f 6973  ..    if not _is
+000007a0: 5f70 6f73 6974 6976 655f 616e 676c 655f  _positive_angle_
+000007b0: 616e 7469 5f63 6c6f 636b 7769 7365 2877  anti_clockwise(w
+000007c0: 6373 293a 0a20 2020 2020 2020 2061 6e67  cs):.        ang
+000007d0: 6c65 5f70 7820 2a3d 202d 310a 0a20 2020  le_px *= -1..   
+000007e0: 2023 2050 6572 666f 726d 2074 6865 2072   # Perform the r
+000007f0: 6f74 6174 696f 6e0a 2020 2020 726f 7461  otation.    rota
+00000800: 7469 6f6e 3a20 416e 7920 3d20 6e70 2e61  tion: Any = np.a
+00000810: 7272 6179 280a 2020 2020 2020 2020 5b5b  rray(.        [[
+00000820: 636f 7328 616e 676c 655f 7078 292c 202d  cos(angle_px), -
+00000830: 7369 6e28 616e 676c 655f 7078 295d 2c20  sin(angle_px)], 
+00000840: 5b73 696e 2861 6e67 6c65 5f70 7829 2c20  [sin(angle_px), 
+00000850: 636f 7328 616e 676c 655f 7078 295d 5d0a  cos(angle_px)]].
+00000860: 2020 2020 290a 2020 2020 6469 6666 5f76      ).    diff_v
+00000870: 6563 746f 725f 7078 3a20 416e 7920 3d20  ector_px: Any = 
+00000880: 6e70 2e61 7272 6179 2876 5f70 7829 202d  np.array(v_px) -
+00000890: 206e 702e 6172 7261 7928 7069 766f 745f   np.array(pivot_
+000008a0: 7078 290a 2020 2020 726f 7461 7465 645f  px).    rotated_
+000008b0: 765f 7078 203d 206e 702e 6172 7261 7928  v_px = np.array(
+000008c0: 7069 766f 745f 7078 2920 2b20 726f 7461  pivot_px) + rota
+000008d0: 7469 6f6e 2040 2064 6966 665f 7665 6374  tion @ diff_vect
+000008e0: 6f72 5f70 780a 0a20 2020 2023 2043 6f6e  or_px..    # Con
+000008f0: 7665 7274 2062 6163 6b20 6672 6f6d 2070  vert back from p
+00000900: 6978 656c 7320 746f 2077 6f72 6c64 2063  ixels to world c
+00000910: 6f6f 7264 696e 6174 6573 0a20 2020 2072  oordinates.    r
+00000920: 6574 7572 6e20 7069 7865 6c5f 746f 5f73  eturn pixel_to_s
+00000930: 6b79 5f70 6f73 6974 696f 6e28 726f 7461  ky_position(rota
+00000940: 7465 645f 765f 7078 2c20 7763 7329 0a0a  ted_v_px, wcs)..
+00000950: 0a64 6566 2074 7261 6e73 6c61 7465 2876  .def translate(v
+00000960: 3a20 536b 7943 6f6f 7264 2c20 6469 7370  : SkyCoord, disp
+00000970: 6c61 6365 6d65 6e74 3a20 416e 676c 6529  lacement: Angle)
+00000980: 202d 3e20 536b 7943 6f6f 7264 3a0a 2020   -> SkyCoord:.  
+00000990: 2020 2222 224d 6f76 6520 6120 706f 696e    """Move a poin
+000009a0: 7420 6279 2061 2064 6973 706c 6163 656d  t by a displacem
+000009b0: 656e 7420 7665 6374 6f72 2e0a 0a20 2020  ent vector...   
+000009c0: 2054 6865 2070 6f69 6e74 2074 6f20 6d6f   The point to mo
+000009d0: 7665 2069 7320 6173 7375 6d65 6420 746f  ve is assumed to
+000009e0: 2062 6520 6769 7665 6e20 6173 2072 6967   be given as rig
+000009f0: 6874 2061 7363 656e 7369 6f6e 2061 6e64  ht ascension and
+00000a00: 2064 6563 6c69 6e61 7469 6f6e 2e20 5468   declination. Th
+00000a10: 650a 2020 2020 6469 7370 6c61 6365 6d65  e.    displaceme
+00000a20: 6e74 2076 6563 746f 7220 6973 2061 7373  nt vector is ass
+00000a30: 756d 6564 2074 6f20 6265 2061 2076 6563  umed to be a vec
+00000a40: 746f 7220 6f6e 2074 6865 2073 6b79 2c20  tor on the sky, 
+00000a50: 7769 7468 2072 6561 6c20 616e 676c 6573  with real angles
+00000a60: 2c20 6173 0a20 2020 2064 6573 6372 6962  , as.    describ
+00000a70: 6564 2066 6f72 2074 6865 2060 7e73 6b79  ed for the `~sky
+00000a80: 5f76 6563 746f 725f 746f 5f70 6978 656c  _vector_to_pixel
+00000a90: 6020 6d65 7468 6f64 2e0a 0a20 2020 2050  ` method...    P
+00000aa0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00000ab0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2076 3a20  --------.    v: 
+00000ac0: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
+00000ad0: 6e61 7465 732e 536b 7943 6f6f 7264 600a  nates.SkyCoord`.
+00000ae0: 2020 2020 2020 2020 506f 696e 7420 746f          Point to
+00000af0: 206d 6f76 652e 0a20 2020 2064 6973 706c   move..    displ
+00000b00: 6163 656d 656e 743a 2032 4420 6172 7261  acement: 2D arra
+00000b10: 7920 6f66 2061 6e67 6c65 730a 2020 2020  y of angles.    
+00000b20: 2020 2020 5665 6374 6f72 2062 7920 7768      Vector by wh
+00000b30: 6963 6820 746f 206d 6f76 6520 7468 6520  ich to move the 
+00000b40: 706f 696e 742e 0a0a 2020 2020 5265 7475  point...    Retu
+00000b50: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00000b60: 2020 2020 607e 6173 7472 6f70 792e 636f      `~astropy.co
+00000b70: 6f72 6469 6e61 7465 732e 536b 7943 6f6f  ordinates.SkyCoo
+00000b80: 7264 600a 2020 2020 2020 2020 5468 6520  rd`.        The 
+00000b90: 706f 696e 7420 6166 7465 7220 6d6f 7669  point after movi
+00000ba0: 6e67 2e0a 2020 2020 2222 220a 2020 2020  ng..    """.    
+00000bb0: 2320 436f 6e76 6572 7420 6672 6f6d 2073  # Convert from s
+00000bc0: 6b79 2063 6f6f 7264 696e 6174 6573 2074  ky coordinates t
+00000bd0: 6f20 7265 616c 2061 6e67 6c65 730a 2020  o real angles.  
+00000be0: 2020 6469 7370 6c61 6365 6d65 6e74 5f64    displacement_d
+00000bf0: 656c 7461 5f72 6120 3d20 6469 7370 6c61  elta_ra = displa
+00000c00: 6365 6d65 6e74 5b30 5d20 2f20 636f 7328  cement[0] / cos(
+00000c10: 762e 6465 632e 746f 5f76 616c 7565 2875  v.dec.to_value(u
+00000c20: 2e72 6164 2929 0a20 2020 2064 6973 706c  .rad)).    displ
+00000c30: 6163 656d 656e 745f 6465 6c74 615f 6465  acement_delta_de
+00000c40: 6320 3d20 6469 7370 6c61 6365 6d65 6e74  c = displacement
+00000c50: 5b31 5d0a 0a20 2020 2023 2050 6572 666f  [1]..    # Perfo
+00000c60: 726d 2074 6865 2074 7261 6e73 6c61 7469  rm the translati
+00000c70: 6f6e 0a20 2020 2074 7261 6e73 6c61 7465  on.    translate
+00000c80: 645f 765f 7261 203d 2076 2e72 6120 2b20  d_v_ra = v.ra + 
+00000c90: 6469 7370 6c61 6365 6d65 6e74 5f64 656c  displacement_del
+00000ca0: 7461 5f72 610a 2020 2020 7472 616e 736c  ta_ra.    transl
+00000cb0: 6174 6564 5f76 5f64 6563 203d 2076 2e64  ated_v_dec = v.d
+00000cc0: 6563 202b 2064 6973 706c 6163 656d 656e  ec + displacemen
+00000cd0: 745f 6465 6c74 615f 6465 630a 2020 2020  t_delta_dec.    
+00000ce0: 7265 7475 726e 2053 6b79 436f 6f72 6428  return SkyCoord(
+00000cf0: 7261 3d74 7261 6e73 6c61 7465 645f 765f  ra=translated_v_
+00000d00: 7261 2c20 6465 633d 7472 616e 736c 6174  ra, dec=translat
+00000d10: 6564 5f76 5f64 6563 290a 0a0a 6465 6620  ed_v_dec)...def 
+00000d20: 7069 7865 6c5f 7363 616c 6573 2877 6373  pixel_scales(wcs
+00000d30: 3a20 5743 5329 202d 3e20 5475 706c 655b  : WCS) -> Tuple[
+00000d40: 416e 676c 652c 2041 6e67 6c65 5d3a 0a20  Angle, Angle]:. 
+00000d50: 2020 2022 2222 0a20 2020 2043 616c 6375     """.    Calcu
+00000d60: 6c61 7465 2074 6865 2070 6978 656c 2073  late the pixel s
+00000d70: 6361 6c65 7320 6f66 2061 2057 4353 206f  cales of a WCS o
+00000d80: 626a 6563 742e 0a0a 2020 2020 466f 7220  bject...    For 
+00000d90: 6120 5743 5320 7265 7475 726e 7320 7069  a WCS returns pi
+00000da0: 7865 6c20 7363 616c 6573 2061 6c6f 6e67  xel scales along
+00000db0: 2065 6163 6820 6178 6973 206f 6620 7468   each axis of th
+00000dc0: 6520 696d 6167 6520 7069 7865 6c20 6174  e image pixel at
+00000dd0: 0a20 2020 2074 6865 2060 6043 5250 4958  .    the ``CRPIX
+00000de0: 6060 206c 6f63 6174 696f 6e20 6f6e 6365  `` location once
+00000df0: 2069 7420 6973 2070 726f 6a65 6374 6564   it is projected
+00000e00: 206f 6e74 6f20 7468 650a 2020 2020 2270   onto the.    "p
+00000e10: 6c61 6e65 206f 6620 696e 7465 726d 6564  lane of intermed
+00000e20: 6961 7465 2077 6f72 6c64 2063 6f6f 7264  iate world coord
+00000e30: 696e 6174 6573 2220 6173 2064 6566 696e  inates" as defin
+00000e40: 6564 2069 6e0a 2020 2020 6047 7265 6973  ed in.    `Greis
+00000e50: 656e 2026 2043 616c 6162 7265 7474 6120  en & Calabretta 
+00000e60: 3230 3032 2c20 4126 412c 2033 3935 2c20  2002, A&A, 395, 
+00000e70: 3130 3631 0a20 2020 203c 6874 7470 733a  1061.    <https:
+00000e80: 2f2f 7569 2e61 6473 6162 732e 6861 7276  //ui.adsabs.harv
+00000e90: 6172 642e 6564 752f 6162 732f 3230 3032  ard.edu/abs/2002
+00000ea0: 4125 3236 412e 2e2e 3339 352e 3130 3631  A%26A...395.1061
+00000eb0: 473e 605f 2e0a 0a20 2020 202e 2e20 6e6f  G>`_...    .. no
+00000ec0: 7465 3a3a 0a20 2020 2020 2020 2054 6869  te::.        Thi
+00000ed0: 7320 6675 6e63 7469 6f6e 2069 7320 636f  s function is co
+00000ee0: 6e63 6572 6e65 6420 2a2a 6f6e 6c79 2a2a  ncerned **only**
+00000ef0: 2061 626f 7574 2074 6865 2074 7261 6e73   about the trans
+00000f00: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
+00000f10: 2020 2269 6d61 6765 2070 6c61 6e65 222d    "image plane"-
+00000f20: 3e22 7072 6f6a 6563 7469 6f6e 2070 6c61  >"projection pla
+00000f30: 6e65 2220 616e 6420 2a2a 6e6f 742a 2a20  ne" and **not** 
+00000f40: 6162 6f75 7420 7468 650a 2020 2020 2020  about the.      
+00000f50: 2020 7472 616e 7366 6f72 6d61 7469 6f6e    transformation
+00000f60: 2022 6365 6c65 7374 6961 6c20 7370 6865   "celestial sphe
+00000f70: 7265 222d 3e22 7072 6f6a 6563 7469 6f6e  re"->"projection
+00000f80: 2070 6c61 6e65 222d 3e22 696d 6167 6520   plane"->"image 
+00000f90: 706c 616e 6522 2e0a 2020 2020 2020 2020  plane"..        
+00000fa0: 5468 6572 6566 6f72 652c 2074 6869 7320  Therefore, this 
+00000fb0: 6675 6e63 7469 6f6e 2069 676e 6f72 6573  function ignores
+00000fc0: 2064 6973 746f 7274 696f 6e73 2061 7269   distortions ari
+00000fd0: 7369 6e67 2064 7565 2074 6f0a 2020 2020  sing due to.    
+00000fe0: 2020 2020 6e6f 6e2d 6c69 6e65 6172 206e      non-linear n
+00000ff0: 6174 7572 6520 6f66 206d 6f73 7420 7072  ature of most pr
+00001000: 6f6a 6563 7469 6f6e 732e 0a0a 2020 2020  ojections...    
+00001010: 2e2e 206e 6f74 653a 3a0a 2020 2020 2020  .. note::.      
+00001020: 2020 496e 206f 7264 6572 2074 6f20 636f    In order to co
+00001030: 6d70 7574 6520 7468 6520 7363 616c 6573  mpute the scales
+00001040: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00001050: 6f20 6365 6c65 7374 6961 6c20 6178 6573  o celestial axes
+00001060: 206f 6e6c 792c 0a20 2020 2020 2020 206d   only,.        m
+00001070: 616b 6520 7375 7265 2074 6861 7420 7468  ake sure that th
+00001080: 6520 696e 7075 7420 607e 6173 7472 6f70  e input `~astrop
+00001090: 792e 7763 732e 5743 5360 206f 626a 6563  y.wcs.WCS` objec
+000010a0: 7420 636f 6e74 6169 6e73 0a20 2020 2020  t contains.     
+000010b0: 2020 2063 656c 6573 7469 616c 2061 7865     celestial axe
+000010c0: 7320 6f6e 6c79 2c20 652e 672e 2c20 6279  s only, e.g., by
+000010d0: 2070 6173 7369 6e67 2069 6e20 7468 650a   passing in the.
+000010e0: 2020 2020 2020 2020 607e 6173 7472 6f70          `~astrop
+000010f0: 792e 7763 732e 5743 532e 6365 6c65 7374  y.wcs.WCS.celest
+00001100: 6961 6c60 2057 4353 206f 626a 6563 742e  ial` WCS object.
+00001110: 0a0a 2020 2020 5468 6520 636f 6465 2068  ..    The code h
+00001120: 6173 2062 6565 6e20 6164 6170 7465 6420  as been adapted 
+00001130: 6672 6f6d 2041 504c 7079 2e0a 0a20 2020  from APLpy...   
+00001140: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00001150: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2077  ----------.    w
+00001160: 6373 203a 2060 7e61 7374 726f 7079 2e77  cs : `~astropy.w
+00001170: 6373 2e57 4353 600a 2020 2020 2020 2020  cs.WCS`.        
+00001180: 4120 776f 726c 6420 636f 6f72 6469 6e61  A world coordina
+00001190: 7465 2073 7973 7465 6d20 6f62 6a65 6374  te system object
+000011a0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+000011b0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2073     -------.    s
+000011c0: 6361 6c65 203a 2074 7570 6c65 206f 6620  cale : tuple of 
+000011d0: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
+000011e0: 6e61 7465 732e 416e 676c 6560 0a20 2020  nates.Angle`.   
+000011f0: 2020 2020 2041 2076 6563 746f 7220 2860       A vector (`
+00001200: 7e6e 756d 7079 2e6e 6461 7272 6179 6029  ~numpy.ndarray`)
+00001210: 206f 6620 7072 6f6a 6563 7469 6f6e 2070   of projection p
+00001220: 6c61 6e65 2069 6e63 7265 6d65 6e74 730a  lane increments.
+00001230: 2020 2020 2020 2020 636f 7272 6573 706f          correspo
+00001240: 6e64 696e 6720 746f 2065 6163 6820 7069  nding to each pi
+00001250: 7865 6c20 7369 6465 2028 6178 6973 292e  xel side (axis).
+00001260: 2054 6865 2075 6e69 7473 206f 6620 7468   The units of th
+00001270: 6520 7265 7475 726e 6564 0a20 2020 2020  e returned.     
+00001280: 2020 2072 6573 756c 7473 2061 7265 2074     results are t
+00001290: 6865 2073 616d 6520 6173 2074 6865 2075  he same as the u
+000012a0: 6e69 7473 206f 6620 607e 6173 7472 6f70  nits of `~astrop
+000012b0: 792e 7763 732e 5763 7370 726d 2e63 6465  y.wcs.Wcsprm.cde
+000012c0: 6c74 602c 0a20 2020 2020 2020 2060 7e61  lt`,.        `~a
+000012d0: 7374 726f 7079 2e77 6373 2e57 6373 7072  stropy.wcs.Wcspr
+000012e0: 6d2e 6372 7661 6c60 2c20 616e 6420 607e  m.crval`, and `~
+000012f0: 6173 7472 6f70 792e 7763 732e 5763 7370  astropy.wcs.Wcsp
+00001300: 726d 2e63 6460 2066 6f72 0a20 2020 2020  rm.cd` for.     
+00001310: 2020 2074 6865 2063 656c 6573 7469 616c     the celestial
+00001320: 2057 4353 2061 6e64 2063 616e 2062 6520   WCS and can be 
+00001330: 6f62 7461 696e 6564 2062 7920 696e 7175  obtained by inqu
+00001340: 6972 696e 6720 7468 6520 7661 6c75 650a  iring the value.
+00001350: 2020 2020 2020 2020 6f66 2060 7e61 7374          of `~ast
+00001360: 726f 7079 2e77 6373 2e57 6373 7072 6d2e  ropy.wcs.Wcsprm.
+00001370: 6375 6e69 7460 2070 726f 7065 7274 7920  cunit` property 
+00001380: 6f66 2074 6865 2069 6e70 7574 0a20 2020  of the input.   
+00001390: 2020 2020 2060 7e61 7374 726f 7079 2e77       `~astropy.w
+000013a0: 6373 2e57 4353 6020 5743 5320 6f62 6a65  cs.WCS` WCS obje
+000013b0: 6374 2e0a 0a20 2020 2053 6565 2041 6c73  ct...    See Als
+000013c0: 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  o.    --------. 
+000013d0: 2020 2061 7374 726f 7079 2e77 6373 2e75     astropy.wcs.u
+000013e0: 7469 6c73 2e70 726f 6a5f 706c 616e 655f  tils.proj_plane_
+000013f0: 7069 7865 6c5f 6172 6561 0a0a 2020 2020  pixel_area..    
+00001400: 2222 220a 2020 2020 7363 616c 655f 6661  """.    scale_fa
+00001410: 6374 6f72 7320 3d20 6e70 2e73 7172 7428  ctors = np.sqrt(
+00001420: 2877 6373 2e70 6978 656c 5f73 6361 6c65  (wcs.pixel_scale
+00001430: 5f6d 6174 7269 782a 2a32 292e 7375 6d28  _matrix**2).sum(
+00001440: 6178 6973 3d30 2c20 6474 7970 653d 666c  axis=0, dtype=fl
+00001450: 6f61 7429 290a 2020 2020 7265 7475 726e  oat)).    return
+00001460: 2028 0a20 2020 2020 2020 2041 6e67 6c65   (.        Angle
+00001470: 2873 6361 6c65 5f66 6163 746f 7273 5b30  (scale_factors[0
+00001480: 5d2c 2077 6373 2e77 6f72 6c64 5f61 7869  ], wcs.world_axi
+00001490: 735f 756e 6974 735b 305d 292c 0a20 2020  s_units[0]),.   
+000014a0: 2020 2020 2041 6e67 6c65 2873 6361 6c65       Angle(scale
+000014b0: 5f66 6163 746f 7273 5b31 5d2c 2077 6373  _factors[1], wcs
+000014c0: 2e77 6f72 6c64 5f61 7869 735f 756e 6974  .world_axis_unit
+000014d0: 735b 315d 292c 0a20 2020 2029 0a0a 0a64  s[1]),.    )...d
+000014e0: 6566 2073 6b79 5f70 6f73 6974 696f 6e5f  ef sky_position_
+000014f0: 746f 5f70 6978 656c 2870 6f73 6974 696f  to_pixel(positio
+00001500: 6e3a 2053 6b79 436f 6f72 642c 2077 6373  n: SkyCoord, wcs
+00001510: 3a20 5743 5329 202d 3e20 6e70 742e 4e44  : WCS) -> npt.ND
+00001520: 4172 7261 795b 6e70 2e66 6c6f 6174 5f5d  Array[np.float_]
+00001530: 3a0a 2020 2020 2222 2243 6f6e 7665 7274  :.    """Convert
+00001540: 2061 2073 6b79 2070 6f73 6974 696f 6e20   a sky position 
+00001550: 746f 2074 6865 2063 6f72 7265 7370 6f6e  to the correspon
+00001560: 6469 6e67 2070 6978 656c 2063 6f6f 7264  ding pixel coord
+00001570: 696e 6174 6573 2e0a 0a20 2020 2050 6172  inates...    Par
+00001580: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00001590: 2d2d 2d2d 2d2d 0a20 2020 2070 6f73 6974  ------.    posit
+000015a0: 696f 6e3a 2060 7e61 7374 726f 7079 2e63  ion: `~astropy.c
+000015b0: 6f6f 7264 696e 6174 6573 2e53 6b79 436f  oordinates.SkyCo
+000015c0: 6f72 6460 0a20 2020 2020 2020 2053 6b79  ord`.        Sky
+000015d0: 2070 6f73 6974 696f 6e20 6173 2072 6967   position as rig
+000015e0: 6874 2061 7363 656e 7369 6f6e 2061 6e64  ht ascension and
+000015f0: 2064 6563 6c69 6e61 7469 6f6e 2e0a 2020   declination..  
+00001600: 2020 7763 733a 2060 7e61 7374 726f 7079    wcs: `~astropy
+00001610: 2e77 6373 2e57 4353 600a 2020 2020 2020  .wcs.WCS`.      
+00001620: 2020 5743 5320 6f62 6a65 6374 2e0a 0a20    WCS object... 
+00001630: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00001640: 2d2d 2d2d 2d2d 0a20 2020 2060 7e6e 756d  ------.    `~num
+00001650: 7079 2e6e 6461 7272 6179 6020 6f66 2060  py.ndarray` of `
+00001660: 666c 6f61 7460 0a20 2020 2020 2020 2054  float`.        T
+00001670: 6865 2070 6978 656c 2063 6f6f 7264 696e  he pixel coordin
+00001680: 6174 6573 2e0a 2020 2020 2222 220a 2020  ates..    """.  
+00001690: 2020 7069 7865 6c5f 636f 6f72 6473 203d    pixel_coords =
+000016a0: 2073 6b79 636f 6f72 645f 746f 5f70 6978   skycoord_to_pix
+000016b0: 656c 2863 6f6f 7264 733d 706f 7369 7469  el(coords=positi
+000016c0: 6f6e 2c20 7763 733d 7763 7329 0a20 2020  on, wcs=wcs).   
+000016d0: 2072 6574 7572 6e20 6e70 2e61 7272 6179   return np.array
+000016e0: 285b 666c 6f61 7428 7069 7865 6c5f 636f  ([float(pixel_co
+000016f0: 6f72 6473 5b30 5d2e 6974 656d 2829 292c  ords[0].item()),
+00001700: 2066 6c6f 6174 2870 6978 656c 5f63 6f6f   float(pixel_coo
+00001710: 7264 735b 315d 2e69 7465 6d28 2929 5d29  rds[1].item())])
+00001720: 0a0a 0a64 6566 2070 6978 656c 5f74 6f5f  ...def pixel_to_
+00001730: 736b 795f 706f 7369 7469 6f6e 2870 6f73  sky_position(pos
+00001740: 6974 696f 6e5f 7078 3a20 6e70 742e 4e44  ition_px: npt.ND
+00001750: 4172 7261 795b 6e70 2e66 6c6f 6174 5f5d  Array[np.float_]
+00001760: 2c20 7763 733a 2057 4353 2920 2d3e 2053  , wcs: WCS) -> S
+00001770: 6b79 436f 6f72 643a 0a20 2020 2022 2222  kyCoord:.    """
+00001780: 436f 6e76 6572 7420 7069 7865 6c20 636f  Convert pixel co
+00001790: 6f72 6469 6e61 7465 7320 746f 2074 6865  ordinates to the
+000017a0: 2063 6f72 7265 7370 6f6e 6469 6e67 2073   corresponding s
+000017b0: 6b79 2070 6f73 6974 696f 6e2e 0a0a 2020  ky position...  
+000017c0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000017d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000017e0: 706f 7369 7469 6f6e 5f70 783a 2060 7e6e  position_px: `~n
+000017f0: 756d 7079 2e6e 6461 7272 6179 6020 6f66  umpy.ndarray` of
+00001800: 2060 666c 6f61 7460 0a20 2020 2020 2020   `float`.       
+00001810: 2050 6978 656c 2063 6f6f 7264 696e 6174   Pixel coordinat
+00001820: 6573 2e0a 2020 2020 7763 733a 2060 7e61  es..    wcs: `~a
+00001830: 7374 726f 7079 2e77 6373 2e57 4353 600a  stropy.wcs.WCS`.
+00001840: 2020 2020 2020 2020 5743 5320 6f62 6a65          WCS obje
+00001850: 6374 2e0a 0a20 2020 2052 6574 7572 6e73  ct...    Returns
+00001860: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00001870: 2060 7e61 7374 726f 7079 2e63 6f6f 7264   `~astropy.coord
+00001880: 696e 6174 6573 2e53 6b79 436f 6f72 6460  inates.SkyCoord`
+00001890: 0a20 2020 2020 2020 2054 6865 2073 6b79  .        The sky
+000018a0: 2063 6f6f 7264 696e 6174 6573 2e0a 2020   coordinates..  
+000018b0: 2020 2222 220a 2020 2020 7265 7475 726e    """.    return
+000018c0: 2070 6978 656c 5f74 6f5f 736b 7963 6f6f   pixel_to_skycoo
+000018d0: 7264 2870 6f73 6974 696f 6e5f 7078 5b30  rd(position_px[0
+000018e0: 5d2c 2070 6f73 6974 696f 6e5f 7078 5b31  ], position_px[1
+000018f0: 5d2c 2077 6373 3d77 6373 2920 2023 206e  ], wcs=wcs)  # n
+00001900: 6f71 610a 0a0a 6465 6620 5f69 735f 706f  oqa...def _is_po
+00001910: 7369 7469 7665 5f61 6e67 6c65 5f61 6e74  sitive_angle_ant
+00001920: 695f 636c 6f63 6b77 6973 6528 7763 733a  i_clockwise(wcs:
+00001930: 2057 4353 2920 2d3e 2062 6f6f 6c3a 0a20   WCS) -> bool:. 
+00001940: 2020 2022 2222 0a20 2020 2052 6574 7572     """.    Retur
+00001950: 6e20 7768 6574 6865 7220 666f 7220 6120  n whether for a 
+00001960: 6769 7665 6e20 5743 5320 706f 7369 7469  given WCS positi
+00001970: 7665 2061 6e67 6c65 7320 6172 6520 616e  ve angles are an
+00001980: 7469 2d63 6c6f 636b 7769 7365 2077 6865  ti-clockwise whe
+00001990: 6e20 706c 6f74 7465 642e 0a0a 2020 2020  n plotted...    
+000019a0: 416e 676c 6573 206f 6e20 7468 6520 736b  Angles on the sk
+000019b0: 7920 6172 6520 6d65 6173 7572 6564 2066  y are measured f
+000019c0: 726f 6d20 6e6f 7274 6820 746f 2065 6173  rom north to eas
+000019d0: 742c 2061 6e64 2064 6570 656e 6469 6e67  t, and depending
+000019e0: 206f 6e20 7468 6520 6f72 6965 6e74 6174   on the orientat
+000019f0: 696f 6e0a 2020 2020 6f66 2074 6865 2061  ion.    of the a
+00001a00: 7865 7320 6f6e 2074 6865 2066 696e 6465  xes on the finde
+00001a10: 7220 6368 6172 7420 7468 6973 206d 6179  r chart this may
+00001a20: 2063 6f72 7265 7370 6f6e 6420 746f 2061   correspond to a
+00001a30: 206d 6174 6865 6d61 7469 6361 6c6c 7920   mathematically 
+00001a40: 706f 7369 7469 7665 0a20 2020 2028 2261  positive.    ("a
+00001a50: 6e74 692d 636c 6f63 6b77 6973 6522 2920  nti-clockwise") 
+00001a60: 6f72 206e 6567 6174 6976 6520 2822 636c  or negative ("cl
+00001a70: 6f63 6b77 6973 6522 2920 616e 676c 652e  ockwise") angle.
+00001a80: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00001a90: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00001aa0: 2020 2020 7763 733a 2060 7e61 7374 726f      wcs: `~astro
+00001ab0: 7079 2e77 6373 2e57 4353 600a 2020 2020  py.wcs.WCS`.    
+00001ac0: 2020 2020 5743 5320 6f62 6a65 6374 2e0a      WCS object..
+00001ad0: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00001ae0: 202d 2d2d 2d2d 2d2d 0a20 2020 2062 6f6f   -------.    boo
+00001af0: 6c0a 2020 2020 2020 2020 6060 5472 7565  l.        ``True
+00001b00: 6060 2069 6620 616e 676c 6573 2066 726f  `` if angles fro
+00001b10: 6d20 6e6f 7274 6820 746f 2065 6173 7420  m north to east 
+00001b20: 636f 7272 6573 706f 6e64 2074 6f20 6d61  correspond to ma
+00001b30: 7468 656d 6174 6963 616c 6c79 2070 6f73  thematically pos
+00001b40: 6974 6976 650a 2020 2020 2020 2020 2822  itive.        ("
+00001b50: 616e 7469 2d63 6c6f 636b 7769 7365 2229  anti-clockwise")
+00001b60: 2061 6e67 6c65 7320 6f6e 2061 2066 696e   angles on a fin
+00001b70: 6465 7220 6368 6172 742c 2060 6046 616c  der chart, ``Fal
+00001b80: 7365 6060 206f 7468 6572 7769 7365 2e0a  se`` otherwise..
+00001b90: 2020 2020 2222 220a 2020 2020 6f72 6967      """.    orig
+00001ba0: 696e 5f70 783a 206e 7074 2e4e 4441 7272  in_px: npt.NDArr
+00001bb0: 6179 5b6e 702e 666c 6f61 745f 5d20 3d20  ay[np.float_] = 
+00001bc0: 6e70 2e61 7272 6179 2828 302e 302c 2030  np.array((0.0, 0
+00001bd0: 2e30 2929 0a20 2020 206f 7269 6769 6e5f  .0)).    origin_
+00001be0: 6f6e 5f73 6b79 203d 2070 6978 656c 5f74  on_sky = pixel_t
+00001bf0: 6f5f 736b 795f 706f 7369 7469 6f6e 286f  o_sky_position(o
+00001c00: 7269 6769 6e5f 7078 2c20 7763 7329 0a20  rigin_px, wcs). 
+00001c10: 2020 206f 7269 6769 6e5f 7261 203d 206f     origin_ra = o
+00001c20: 7269 6769 6e5f 6f6e 5f73 6b79 2e72 610a  rigin_on_sky.ra.
+00001c30: 2020 2020 6f72 6967 696e 5f64 6563 203d      origin_dec =
+00001c40: 206f 7269 6769 6e5f 6f6e 5f73 6b79 2e64   origin_on_sky.d
+00001c50: 6563 0a0a 2020 2020 2320 4120 2270 6f69  ec..    # A "poi
+00001c60: 6e74 2074 6f20 7468 6520 6e6f 7274 6822  nt to the north"
+00001c70: 206f 6e20 6120 6669 6e64 6572 2063 6861   on a finder cha
+00001c80: 7274 0a20 2020 2070 6f69 6e74 5f74 6f5f  rt.    point_to_
+00001c90: 6e6f 7274 685f 7261 203d 206f 7269 6769  north_ra = origi
+00001ca0: 6e5f 7261 0a20 2020 2070 6f69 6e74 5f74  n_ra.    point_t
+00001cb0: 6f5f 6e6f 7274 685f 6465 6320 3d20 6f72  o_north_dec = or
+00001cc0: 6967 696e 5f64 6563 202b 2031 202a 2075  igin_dec + 1 * u
+00001cd0: 2e61 7263 6d69 6e0a 2020 2020 706f 696e  .arcmin.    poin
+00001ce0: 745f 746f 5f6e 6f72 7468 203d 2053 6b79  t_to_north = Sky
+00001cf0: 436f 6f72 6428 7261 3d70 6f69 6e74 5f74  Coord(ra=point_t
+00001d00: 6f5f 6e6f 7274 685f 7261 2c20 6465 633d  o_north_ra, dec=
+00001d10: 706f 696e 745f 746f 5f6e 6f72 7468 5f64  point_to_north_d
+00001d20: 6563 290a 2020 2020 706f 696e 745f 746f  ec).    point_to
+00001d30: 5f6e 6f72 7468 5f70 7820 3d20 736b 795f  _north_px = sky_
+00001d40: 706f 7369 7469 6f6e 5f74 6f5f 7069 7865  position_to_pixe
+00001d50: 6c28 706f 696e 745f 746f 5f6e 6f72 7468  l(point_to_north
+00001d60: 2c20 7763 7329 0a0a 2020 2020 2320 4120  , wcs)..    # A 
+00001d70: 2270 6f69 6e74 2074 6f20 7468 6520 6e6f  "point to the no
+00001d80: 7274 682d 6561 7374 2220 6f6e 2061 2066  rth-east" on a f
+00001d90: 696e 6465 7220 6368 6172 740a 2020 2020  inder chart.    
+00001da0: 706f 696e 745f 746f 5f6e 6f72 7468 5f65  point_to_north_e
+00001db0: 6173 745f 7261 203d 206f 7269 6769 6e5f  ast_ra = origin_
+00001dc0: 7261 202b 2031 202a 2075 2e61 7263 6d69  ra + 1 * u.arcmi
+00001dd0: 6e0a 2020 2020 706f 696e 745f 746f 5f6e  n.    point_to_n
+00001de0: 6f72 7468 5f65 6173 745f 6465 6320 3d20  orth_east_dec = 
+00001df0: 6f72 6967 696e 5f64 6563 202b 2031 202a  origin_dec + 1 *
+00001e00: 2075 2e61 7263 6d69 6e0a 2020 2020 706f   u.arcmin.    po
+00001e10: 696e 745f 746f 5f6e 6f72 7468 5f65 6173  int_to_north_eas
+00001e20: 7420 3d20 536b 7943 6f6f 7264 280a 2020  t = SkyCoord(.  
+00001e30: 2020 2020 2020 7261 3d70 6f69 6e74 5f74        ra=point_t
+00001e40: 6f5f 6e6f 7274 685f 6561 7374 5f72 612c  o_north_east_ra,
+00001e50: 2064 6563 3d70 6f69 6e74 5f74 6f5f 6e6f   dec=point_to_no
+00001e60: 7274 685f 6561 7374 5f64 6563 0a20 2020  rth_east_dec.   
+00001e70: 2029 0a20 2020 2070 6f69 6e74 5f74 6f5f   ).    point_to_
+00001e80: 6e6f 7274 685f 6561 7374 5f70 7820 3d20  north_east_px = 
+00001e90: 736b 795f 706f 7369 7469 6f6e 5f74 6f5f  sky_position_to_
+00001ea0: 7069 7865 6c28 706f 696e 745f 746f 5f6e  pixel(point_to_n
+00001eb0: 6f72 7468 5f65 6173 742c 2077 6373 290a  orth_east, wcs).
+00001ec0: 0a20 2020 2023 2041 2022 706f 696e 7420  .    # A "point 
+00001ed0: 746f 2074 6865 206e 6f72 7468 2d65 6173  to the north-eas
+00001ee0: 7422 206f 6e20 6120 6669 6e64 6572 2063  t" on a finder c
+00001ef0: 6861 7274 0a20 2020 2070 6f69 6e74 5f74  hart.    point_t
+00001f00: 6f5f 6e6f 7274 685f 7765 7374 5f72 6120  o_north_west_ra 
+00001f10: 3d20 6f72 6967 696e 5f72 6120 2d20 3120  = origin_ra - 1 
+00001f20: 2a20 752e 6172 636d 696e 0a20 2020 2070  * u.arcmin.    p
+00001f30: 6f69 6e74 5f74 6f5f 6e6f 7274 685f 7765  oint_to_north_we
+00001f40: 7374 5f64 6563 203d 206f 7269 6769 6e5f  st_dec = origin_
+00001f50: 6465 6320 2b20 3120 2a20 752e 6172 636d  dec + 1 * u.arcm
+00001f60: 696e 0a20 2020 2070 6f69 6e74 5f74 6f5f  in.    point_to_
+00001f70: 6e6f 7274 685f 7765 7374 203d 2053 6b79  north_west = Sky
+00001f80: 436f 6f72 6428 0a20 2020 2020 2020 2072  Coord(.        r
+00001f90: 613d 706f 696e 745f 746f 5f6e 6f72 7468  a=point_to_north
+00001fa0: 5f77 6573 745f 7261 2c20 6465 633d 706f  _west_ra, dec=po
+00001fb0: 696e 745f 746f 5f6e 6f72 7468 5f77 6573  int_to_north_wes
+00001fc0: 745f 6465 630a 2020 2020 290a 2020 2020  t_dec.    ).    
+00001fd0: 706f 696e 745f 746f 5f6e 6f72 7468 5f77  point_to_north_w
+00001fe0: 6573 745f 7078 203d 2073 6b79 5f70 6f73  est_px = sky_pos
+00001ff0: 6974 696f 6e5f 746f 5f70 6978 656c 2870  ition_to_pixel(p
+00002000: 6f69 6e74 5f74 6f5f 6e6f 7274 685f 7765  oint_to_north_we
+00002010: 7374 2c20 7763 7329 0a0a 2020 2020 2320  st, wcs)..    # 
+00002020: 5468 6520 6469 6666 6572 656e 6365 2062  The difference b
+00002030: 6574 7765 656e 2074 6865 2070 6f69 6e74  etween the point
+00002040: 2074 6f20 7468 6520 6e6f 7274 6820 616e   to the north an
+00002050: 6420 7468 6520 6f72 6967 696e 2067 6976  d the origin giv
+00002060: 6573 2061 2076 6563 746f 720a 2020 2020  es a vector.    
+00002070: 2320 706f 696e 7469 6e67 206e 6f72 7468  # pointing north
+00002080: 202d 2062 7574 2061 7320 7468 6520 6f72   - but as the or
+00002090: 6967 696e 2069 7320 2830 2c20 3029 2074  igin is (0, 0) t
+000020a0: 6869 7320 6973 206a 7573 7420 7468 6520  his is just the 
+000020b0: 706f 696e 7420 746f 2074 6865 206e 6f72  point to the nor
+000020c0: 7468 2e0a 2020 2020 2320 5468 6520 7361  th..    # The sa
+000020d0: 6d65 2061 7267 756d 656e 7420 6170 706c  me argument appl
+000020e0: 6965 7320 666f 7220 7468 6520 7665 6374  ies for the vect
+000020f0: 6f72 2070 6f69 6e74 696e 6720 6e6f 7274  or pointing nort
+00002100: 682d 6561 7374 2e0a 2020 2020 6e6f 7274  h-east..    nort
+00002110: 685f 7665 6374 6f72 5f70 7820 3d20 706f  h_vector_px = po
+00002120: 696e 745f 746f 5f6e 6f72 7468 5f70 780a  int_to_north_px.
+00002130: 2020 2020 6e6f 7274 685f 6561 7374 5f76      north_east_v
+00002140: 6563 746f 725f 7078 203d 2070 6f69 6e74  ector_px = point
+00002150: 5f74 6f5f 6e6f 7274 685f 6561 7374 5f70  _to_north_east_p
+00002160: 780a 2020 2020 6e6f 7274 685f 7765 7374  x.    north_west
+00002170: 5f76 6563 746f 725f 7078 203d 2070 6f69  _vector_px = poi
+00002180: 6e74 5f74 6f5f 6e6f 7274 685f 7765 7374  nt_to_north_west
+00002190: 5f70 780a 0a20 2020 2023 2047 6574 2074  _px..    # Get t
+000021a0: 6865 2061 6e67 6c65 2062 6574 7765 656e  he angle between
+000021b0: 2074 6865 2076 6563 746f 7273 2074 6f20   the vectors to 
+000021c0: 7468 6520 6e6f 7274 6820 616e 6420 746f  the north and to
+000021d0: 2074 6865 206e 6f72 7468 2d65 6173 742e   the north-east.
+000021e0: 2044 7565 2074 6f0a 2020 2020 2320 7379   Due to.    # sy
+000021f0: 6d6d 6574 7279 2c20 7468 6973 2069 7320  mmetry, this is 
+00002200: 7468 6520 7361 6d65 2061 7320 7468 6520  the same as the 
+00002210: 616e 676c 6520 6265 7477 6565 6e20 7468  angle between th
+00002220: 6520 7665 6374 6f72 7320 746f 2074 6865  e vectors to the
+00002230: 206e 6f72 7468 2061 6e64 2074 6f0a 2020   north and to.  
+00002240: 2020 2320 6e6f 7274 682d 7765 7374 0a20    # north-west. 
+00002250: 2020 2063 6f73 5f61 6e67 6c65 203d 206e     cos_angle = n
+00002260: 702e 646f 7428 6e6f 7274 685f 7665 6374  p.dot(north_vect
+00002270: 6f72 5f70 782c 206e 6f72 7468 5f65 6173  or_px, north_eas
+00002280: 745f 7665 6374 6f72 5f70 7829 202f 2028  t_vector_px) / (
+00002290: 0a20 2020 2020 2020 206e 702e 6c69 6e61  .        np.lina
+000022a0: 6c67 2e6e 6f72 6d28 6e6f 7274 685f 7665  lg.norm(north_ve
+000022b0: 6374 6f72 5f70 7829 202a 206e 702e 6c69  ctor_px) * np.li
+000022c0: 6e61 6c67 2e6e 6f72 6d28 6e6f 7274 685f  nalg.norm(north_
+000022d0: 6561 7374 5f76 6563 746f 725f 7078 290a  east_vector_px).
+000022e0: 2020 2020 290a 2020 2020 616e 676c 6520      ).    angle 
+000022f0: 3d20 6d61 7468 2e61 636f 7328 636f 735f  = math.acos(cos_
+00002300: 616e 676c 6529 0a0a 2020 2020 2320 526f  angle)..    # Ro
+00002310: 7461 7465 2074 6865 2076 6563 746f 7220  tate the vector 
+00002320: 746f 2074 6865 206e 6f72 7468 2028 696e  to the north (in
+00002330: 2061 6e74 692d 636c 6f63 6b77 6973 6520   anti-clockwise 
+00002340: 6469 7265 6374 696f 6e29 2062 7920 7468  direction) by th
+00002350: 6973 2061 6e67 6c65 0a20 2020 2072 6f74  is angle.    rot
+00002360: 6174 696f 6e3a 206e 7074 2e4e 4441 7272  ation: npt.NDArr
+00002370: 6179 5b6e 702e 666c 6f61 745f 5d20 3d20  ay[np.float_] = 
+00002380: 6e70 2e61 7272 6179 280a 2020 2020 2020  np.array(.      
+00002390: 2020 5b5b 636f 7328 616e 676c 6529 2c20    [[cos(angle), 
+000023a0: 2d73 696e 2861 6e67 6c65 295d 2c20 5b73  -sin(angle)], [s
+000023b0: 696e 2861 6e67 6c65 292c 2063 6f73 2861  in(angle), cos(a
+000023c0: 6e67 6c65 295d 5d0a 2020 2020 290a 2020  ngle)]].    ).  
+000023d0: 2020 726f 7461 7465 645f 6e6f 7274 685f    rotated_north_
+000023e0: 7665 6374 6f72 5f70 7820 3d20 6e70 2e64  vector_px = np.d
+000023f0: 6f74 2872 6f74 6174 696f 6e2c 206e 6f72  ot(rotation, nor
+00002400: 7468 5f76 6563 746f 725f 7078 290a 0a20  th_vector_px).. 
+00002410: 2020 2023 2049 6620 6120 726f 7461 7469     # If a rotati
+00002420: 6f6e 2066 726f 6d20 6e6f 7274 6820 746f  on from north to
+00002430: 2065 6173 7420 636f 7272 6573 706f 6e64   east correspond
+00002440: 7320 746f 2061 6e20 616e 7469 2d63 6c6f  s to an anti-clo
+00002450: 636b 7769 7365 2072 6f74 6174 696f 6e20  ckwise rotation 
+00002460: 6f6e 2061 0a20 2020 2023 2066 696e 6465  on a.    # finde
+00002470: 7220 6368 6172 742c 2074 6865 2072 6f74  r chart, the rot
+00002480: 6174 6564 2076 6563 746f 7220 6d75 7374  ated vector must
+00002490: 2061 6c69 676e 6564 2077 6974 6820 7468   aligned with th
+000024a0: 6520 7665 6374 6f72 2074 6f20 7468 6520  e vector to the 
+000024b0: 6e6f 7274 682d 6561 7374 2e0a 2020 2020  north-east..    
+000024c0: 2320 5468 6973 2069 6d70 6c69 6573 2074  # This implies t
+000024d0: 6861 7420 7468 6569 7220 7363 616c 6172  hat their scalar
+000024e0: 2070 726f 6475 6374 2074 6865 6e20 6d75   product then mu
+000024f0: 7374 2062 6520 6c61 7267 6572 2074 6861  st be larger tha
+00002500: 6e20 7468 6174 2062 6574 7765 656e 2074  n that between t
+00002510: 6865 0a20 2020 2023 2072 6f74 6174 6564  he.    # rotated
+00002520: 2076 6563 746f 7220 616e 6420 7468 6520   vector and the 
+00002530: 7665 6374 6f72 2074 6f20 7468 6520 6e6f  vector to the no
+00002540: 7274 682d 7765 7374 2e0a 2020 2020 7265  rth-west..    re
+00002550: 7475 726e 2063 6173 7428 0a20 2020 2020  turn cast(.     
+00002560: 2020 2062 6f6f 6c2c 0a20 2020 2020 2020     bool,.       
+00002570: 206e 702e 646f 7428 726f 7461 7465 645f   np.dot(rotated_
+00002580: 6e6f 7274 685f 7665 6374 6f72 5f70 782c  north_vector_px,
+00002590: 206e 6f72 7468 5f65 6173 745f 7665 6374   north_east_vect
+000025a0: 6f72 5f70 7829 0a20 2020 2020 2020 203e  or_px).        >
+000025b0: 206e 702e 646f 7428 726f 7461 7465 645f   np.dot(rotated_
+000025c0: 6e6f 7274 685f 7665 6374 6f72 5f70 782c  north_vector_px,
+000025d0: 206e 6f72 7468 5f77 6573 745f 7665 6374   north_west_vect
+000025e0: 6f72 5f70 7829 2c0a 2020 2020 290a       or_px),.    ).
```

### Comparing `imephu-0.2.0/src/imephu/annotation/__init__.py` & `imephu-0.2.1/src/imephu/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/annotation/__pycache__/__init__.cpython-310.pyc` & `imephu-0.2.1/src/imephu/annotation/general/group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,189 @@
-00000000: 6f0d 0d0a 0000 0000 927a 0662 0e06 0000  o........z.b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6404 6701 5a07 4700 6405  m.Z...d.g.Z.G.d.
-00000060: 6404 8400 6404 6501 8303 5a08 6406 5300  d...d.e...Z.d.S.
-00000070: 2907 e900 0000 0029 01da 0850 726f 746f  )......)...Proto
-00000080: 636f 6c29 02da 0541 6e67 6c65 da08 536b  col)...Angle..Sk
-00000090: 7943 6f6f 7264 2901 da07 5743 5341 7865  yCoord)...WCSAxe
-000000a0: 73da 0a41 6e6e 6f74 6174 696f 6e63 0000  s..Annotationc..
-000000b0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-000000c0: 0000 4000 0000 734a 0000 0065 005a 0164  ..@...sJ...e.Z.d
-000000d0: 005a 0264 015a 0364 0265 0464 0364 0466  .Z.d.Z.d.e.d.d.f
-000000e0: 0464 0564 0684 045a 0564 0765 0664 0865  .d.d...Z.d.e.d.e
-000000f0: 0764 0364 0066 0664 0964 0a84 045a 0864  .d.d.f.d.d...Z.d
-00000100: 0b65 0764 0364 0066 0464 0c64 0d84 045a  .e.d.d.f.d.d...Z
-00000110: 0964 0453 0029 0e72 0600 0000 7a27 416e  .d.S.).r....z'An
-00000120: 2061 6e6e 6f74 6174 696f 6e20 746f 2061   annotation to a
-00000130: 6464 2074 6f20 6120 6669 6e64 6572 2063  dd to a finder c
-00000140: 6861 7274 2eda 0261 78da 0672 6574 7572  hart...ax..retur
-00000150: 6e4e 6302 0000 0000 0000 0000 0000 0002  nNc.............
-00000160: 0000 0001 0000 0043 0000 00f3 0400 0000  .......C........
-00000170: 6401 5300 2902 7aa2 4164 6420 7468 6973  d.S.).z.Add this
-00000180: 2061 6e6e 6f74 6174 696f 6e20 746f 2061   annotation to a
-00000190: 2066 696e 6465 7220 6368 6172 742e 0a0a   finder chart...
-000001a0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000001b0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000001c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6178  -----.        ax
-000001d0: 3a20 607e 6173 7472 6f70 792e 7669 7375  : `~astropy.visu
-000001e0: 616c 697a 6174 696f 6e2e 7763 7361 7865  alization.wcsaxe
-000001f0: 732e 5743 5341 7865 7360 0a20 2020 2020  s.WCSAxes`.     
-00000200: 2020 2020 2020 2050 6c6f 7420 6178 6573         Plot axes
-00000210: 2e0a 2020 2020 2020 2020 4ea9 0029 02da  ..        N..)..
-00000220: 0473 656c 6672 0700 0000 720a 0000 0072  .selfr....r....r
-00000230: 0a00 0000 fa46 2f55 7365 7273 2f63 6872  .....F/Users/chr
-00000240: 6973 7469 616e 2f49 6465 6150 726f 6a65  istian/IdeaProje
-00000250: 6374 732f 696d 6570 6875 2f73 7263 2f69  cts/imephu/src/i
-00000260: 6d65 7068 752f 616e 6e6f 7461 7469 6f6e  mephu/annotation
-00000270: 2f5f 5f69 6e69 745f 5f2e 7079 da06 6164  /__init__.py..ad
-00000280: 645f 746f 0c00 0000 7302 0000 0004 087a  d_to....s......z
-00000290: 1141 6e6e 6f74 6174 696f 6e2e 6164 645f  .Annotation.add_
-000002a0: 746f da05 7069 766f 74da 0561 6e67 6c65  to..pivot..angle
-000002b0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000002c0: 0001 0000 0043 0000 0072 0900 0000 2902  .....C...r....).
-000002d0: 6117 0200 0052 6f74 6174 6520 7468 6973  a....Rotate this
-000002e0: 2061 6e6e 6f74 6174 696f 6e20 6172 6f75   annotation arou
-000002f0: 6e64 2061 2070 6976 6f74 2061 6e64 2072  nd a pivot and r
-00000300: 6574 7572 6e20 7468 6520 7265 7375 6c74  eturn the result
-00000310: 2e0a 0a20 2020 2020 2020 2054 6865 2072  ...        The r
-00000320: 6f74 6174 696f 6e20 616e 676c 6520 6973  otation angle is
-00000330: 2061 6e20 616e 676c 6520 6f6e 2074 6865   an angle on the
-00000340: 2073 6b79 2c20 6d65 6173 7572 6564 2066   sky, measured f
-00000350: 726f 6d20 6e6f 7274 6820 746f 2065 6173  rom north to eas
-00000360: 742e 0a0a 2020 2020 2020 2020 5061 7261  t...        Para
-00000370: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00000380: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00000390: 2020 7069 766f 743a 2060 7e61 7374 726f    pivot: `~astro
-000003a0: 7079 2e63 6f6f 7264 696e 6174 6573 2e53  py.coordinates.S
-000003b0: 6b79 436f 6f72 6460 0a20 2020 2020 2020  kyCoord`.       
-000003c0: 2020 2020 2050 6f69 6e74 2061 726f 756e       Point aroun
-000003d0: 6420 7768 6963 6820 746f 2072 6f74 6174  d which to rotat
-000003e0: 6520 7468 6520 616e 6e6f 7461 7469 6f6e  e the annotation
-000003f0: 2e0a 2020 2020 2020 2020 616e 676c 653a  ..        angle:
-00000400: 2060 7e61 7374 726f 7079 2e63 6f6f 7264   `~astropy.coord
-00000410: 696e 6174 6573 2e41 6e67 6c65 600a 2020  inates.Angle`.  
-00000420: 2020 2020 2020 2020 2020 416e 676c 6520            Angle 
-00000430: 6f66 2072 6f74 6174 696f 6e2c 206d 6561  of rotation, mea
-00000440: 7375 7265 6420 6672 6f6d 206e 6f72 7468  sured from north
-00000450: 2074 6f77 6172 6473 2074 6865 2065 6173   towards the eas
-00000460: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
-00000470: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00000480: 2d2d 2d0a 2020 2020 2020 2020 607e 696d  ---.        `~im
-00000490: 6570 6875 2e61 6e6e 6f74 6174 696f 6e2e  ephu.annotation.
-000004a0: 416e 6e6f 7461 7469 6f6e 600a 2020 2020  Annotation`.    
-000004b0: 2020 2020 2020 2020 5468 6520 616e 6e6f          The anno
-000004c0: 7461 7469 6f6e 2072 6573 756c 7469 6e67  tation resulting
-000004d0: 2066 726f 6d20 7468 6520 726f 7461 7469   from the rotati
-000004e0: 6f6e 2e0a 2020 2020 2020 2020 4e72 0a00  on..        Nr..
-000004f0: 0000 2903 720b 0000 0072 0e00 0000 720f  ..).r....r....r.
-00000500: 0000 0072 0a00 0000 720a 0000 0072 0c00  ...r....r....r..
-00000510: 0000 da06 726f 7461 7465 1600 0000 7302  ....rotate....s.
-00000520: 0000 0004 117a 1141 6e6e 6f74 6174 696f  .....z.Annotatio
-00000530: 6e2e 726f 7461 7465 da0c 6469 7370 6c61  n.rotate..displa
-00000540: 6365 6d65 6e74 6302 0000 0000 0000 0000  cementc.........
-00000550: 0000 0002 0000 0001 0000 0043 0000 0072  ...........C...r
-00000560: 0900 0000 2902 616b 0100 000a 2020 2020  ....).ak....    
-00000570: 2020 2020 4d6f 7665 2074 6869 7320 616e      Move this an
-00000580: 6e6f 7461 7469 6f6e 2061 6c6f 6e67 2061  notation along a
-00000590: 2064 6973 706c 6163 656d 656e 7420 7665   displacement ve
-000005a0: 6374 6f72 2061 6e64 2072 6574 7572 6e20  ctor and return 
-000005b0: 7468 6520 7265 7375 6c74 2e0a 0a20 2020  the result...   
-000005c0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000005d0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000005e0: 2d2d 0a20 2020 2020 2020 2064 6973 706c  --.        displ
-000005f0: 6163 656d 656e 743a 2032 4420 6172 7261  acement: 2D arra
-00000600: 7920 6f66 2061 6e67 6c65 730a 2020 2020  y of angles.    
-00000610: 2020 2020 2020 2020 5468 6520 6469 7370          The disp
-00000620: 6c61 6365 6d65 6e74 2062 7920 7768 6963  lacement by whic
-00000630: 6820 746f 206d 6f76 6520 7468 6520 616e  h to move the an
-00000640: 6e6f 7461 7469 6f6e 2e0a 0a20 2020 2020  notation...     
-00000650: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00000660: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00000670: 2020 2060 7e69 6d65 7068 752e 616e 6e6f     `~imephu.anno
-00000680: 7461 7469 6f6e 2e41 6e6e 6f74 6174 696f  tation.Annotatio
-00000690: 6e60 0a20 2020 2020 2020 2020 2020 2054  n`.            T
-000006a0: 6865 2061 6e6e 6f74 6174 696f 6e20 7265  he annotation re
-000006b0: 7375 6c74 696e 6720 6672 6f6d 2074 6865  sulting from the
-000006c0: 2074 7261 6e73 6c61 7469 6f6e 2e0a 2020   translation..  
-000006d0: 2020 2020 2020 4e72 0a00 0000 2902 720b        Nr....).r.
-000006e0: 0000 0072 1100 0000 720a 0000 0072 0a00  ...r....r....r..
-000006f0: 0000 720c 0000 00da 0974 7261 6e73 6c61  ..r......transla
-00000700: 7465 2900 0000 7302 0000 0004 0e7a 1441  te)...s......z.A
-00000710: 6e6e 6f74 6174 696f 6e2e 7472 616e 736c  nnotation.transl
-00000720: 6174 6529 0ada 085f 5f6e 616d 655f 5fda  ate)...__name__.
-00000730: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000740: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-00000750: 5f5f 7205 0000 0072 0d00 0000 7204 0000  __r....r....r...
-00000760: 0072 0300 0000 7210 0000 0072 1200 0000  .r....r....r....
-00000770: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000780: 0c00 0000 7206 0000 0009 0000 0073 0a00  ....r........s..
-00000790: 0000 0800 0401 1202 160a 1613 4e29 09da  ............N)..
-000007a0: 0674 7970 696e 6772 0200 0000 da13 6173  .typingr......as
-000007b0: 7472 6f70 792e 636f 6f72 6469 6e61 7465  tropy.coordinate
-000007c0: 7372 0300 0000 7204 0000 005a 1d61 7374  sr....r....Z.ast
-000007d0: 726f 7079 2e76 6973 7561 6c69 7a61 7469  ropy.visualizati
-000007e0: 6f6e 2e77 6373 6178 6573 7205 0000 005a  on.wcsaxesr....Z
-000007f0: 065f 616c 6c5f 5f72 0600 0000 720a 0000  ._all__r....r...
-00000800: 0072 0a00 0000 720a 0000 0072 0c00 0000  .r....r....r....
-00000810: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
-00000820: 0000 000c 0010 020c 0106 0214 03         .............
+00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000010: 7274 204c 6973 742c 2053 6571 7565 6e63  rt List, Sequenc
+00000020: 650a 0a66 726f 6d20 6173 7472 6f70 792e  e..from astropy.
+00000030: 636f 6f72 6469 6e61 7465 7320 696d 706f  coordinates impo
+00000040: 7274 2041 6e67 6c65 2c20 536b 7943 6f6f  rt Angle, SkyCoo
+00000050: 7264 0a66 726f 6d20 6173 7472 6f70 792e  rd.from astropy.
+00000060: 7669 7375 616c 697a 6174 696f 6e2e 7763  visualization.wc
+00000070: 7361 7865 7320 696d 706f 7274 2057 4353  saxes import WCS
+00000080: 4178 6573 0a0a 6672 6f6d 2069 6d65 7068  Axes..from imeph
+00000090: 752e 616e 6e6f 7461 7469 6f6e 2069 6d70  u.annotation imp
+000000a0: 6f72 7420 416e 6e6f 7461 7469 6f6e 0a0a  ort Annotation..
+000000b0: 0a63 6c61 7373 2047 726f 7570 416e 6e6f  .class GroupAnno
+000000c0: 7461 7469 6f6e 2841 6e6e 6f74 6174 696f  tation(Annotatio
+000000d0: 6e29 3a0a 2020 2020 2222 220a 2020 2020  n):.    """.    
+000000e0: 416e 2061 6e6e 6f74 6174 696f 6e20 6d61  An annotation ma
+000000f0: 6465 206f 6620 6120 6772 6f75 7020 6f66  de of a group of
+00000100: 2061 6e6e 6f74 6174 696f 6e73 2e0a 0a20   annotations... 
+00000110: 2020 2054 6865 2061 6e6e 6f74 6174 696f     The annotatio
+00000120: 6e20 636f 6d70 7269 7365 7320 6120 6c69  n comprises a li
+00000130: 7374 206f 6620 616e 6e6f 7461 7469 6f6e  st of annotation
+00000140: 2069 7465 6d73 2e20 416e 7920 6f66 2074   items. Any of t
+00000150: 6865 0a20 2020 2060 7e69 6d70 6568 752e  he.    `~impehu.
+00000160: 616e 6e6f 7461 7469 6f6e 2e41 6e6e 6f74  annotation.Annot
+00000170: 6174 696f 6e60 206d 6574 686f 6473 2061  ation` methods a
+00000180: 7265 2061 7070 6c69 6564 2074 6f20 616c  re applied to al
+00000190: 6c20 7468 6520 6974 656d 7320 696e 2074  l the items in t
+000001a0: 6865 206c 6973 742c 0a20 2020 2069 6e20  he list,.    in 
+000001b0: 7468 6520 6f72 6465 7220 7468 6520 6974  the order the it
+000001c0: 656d 7320 6170 7065 6172 2069 6e20 7468  ems appear in th
+000001d0: 6520 6c69 7374 2e20 536f 2c20 666f 7220  e list. So, for 
+000001e0: 6578 616d 706c 652c 2074 6865 2060 6061  example, the ``a
+000001f0: 7070 6c79 5f74 6f60 6020 6d65 7468 6f64  pply_to`` method
+00000200: 0a20 2020 2063 616c 6c73 2074 6865 2060  .    calls the `
+00000210: 6061 7070 6c79 5f74 6f60 6020 6d65 7468  `apply_to`` meth
+00000220: 6f64 2066 6f72 2061 6c6c 206c 6973 7420  od for all list 
+00000230: 6974 656d 732c 2073 7461 7274 696e 6720  items, starting 
+00000240: 6672 6f6d 2074 6865 2066 6972 7374 2069  from the first i
+00000250: 7465 6d20 696e 0a20 2020 2074 6865 206c  tem in.    the l
+00000260: 6973 7420 616e 6420 6669 6e69 7368 696e  ist and finishin
+00000270: 6720 7769 7468 2074 6865 206c 6173 7420  g with the last 
+00000280: 6974 656d 2e0a 0a20 2020 2041 6e6e 6f74  item...    Annot
+00000290: 6174 696f 6e73 2063 616e 2062 6520 6164  ations can be ad
+000002a0: 6465 6420 746f 2074 6865 2067 726f 7570  ded to the group
+000002b0: 2077 6865 6e20 6361 6c6c 696e 6720 7468   when calling th
+000002c0: 6520 636f 6e73 7472 7563 746f 7220 6f72  e constructor or
+000002d0: 2062 7920 7573 696e 6720 7468 650a 2020   by using the.  
+000002e0: 2020 6060 6164 645f 6974 656d 6060 206d    ``add_item`` m
+000002f0: 6574 686f 6420 6166 7465 7277 6172 6473  ethod afterwards
+00000300: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+00000310: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00000320: 0a20 2020 2069 7465 6d73 3a20 7365 7175  .    items: sequ
+00000330: 656e 6365 206f 6620 607e 696d 6570 6875  ence of `~imephu
+00000340: 2e61 6e6e 6f74 6174 696f 6e2e 416e 6e6f  .annotation.Anno
+00000350: 7461 7469 6f6e 600a 2020 2020 2020 2020  tation`.        
+00000360: 5468 6520 696e 6974 6961 6c20 6c69 7374  The initial list
+00000370: 206f 6620 6772 6f75 7020 6974 656d 732e   of group items.
+00000380: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
+00000390: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+000003a0: 2069 7465 6d73 3a20 5365 7175 656e 6365   items: Sequence
+000003b0: 5b41 6e6e 6f74 6174 696f 6e5d 293a 0a20  [Annotation]):. 
+000003c0: 2020 2020 2020 2073 656c 662e 5f69 7465         self._ite
+000003d0: 6d73 3a20 4c69 7374 5b41 6e6e 6f74 6174  ms: List[Annotat
+000003e0: 696f 6e5d 203d 206c 6973 7428 6974 656d  ion] = list(item
+000003f0: 7329 0a0a 2020 2020 6465 6620 6164 645f  s)..    def add_
+00000400: 6974 656d 2873 656c 662c 2069 7465 6d3a  item(self, item:
+00000410: 2041 6e6e 6f74 6174 696f 6e29 202d 3e20   Annotation) -> 
+00000420: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00000430: 2241 6464 2061 6e20 616e 6e6f 7461 7469  "Add an annotati
+00000440: 6f6e 2074 6f20 7468 6973 2067 726f 7570  on to this group
+00000450: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00000460: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00000470: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00000480: 2069 7465 6d3a 2060 7e69 6d65 7068 752e   item: `~imephu.
+00000490: 616e 6e6f 7461 7469 6f6e 2e41 6e6e 6f74  annotation.Annot
+000004a0: 6174 696f 6e60 0a20 2020 2020 2020 2020  ation`.         
+000004b0: 2020 2041 6e6e 6f74 6174 696f 6e20 746f     Annotation to
+000004c0: 2061 6464 2074 6f20 7468 6973 2067 726f   add to this gro
+000004d0: 7570 2e0a 2020 2020 2020 2020 2222 220a  up..        """.
+000004e0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
+000004f0: 656d 732e 6170 7065 6e64 2869 7465 6d29  ems.append(item)
+00000500: 0a0a 2020 2020 6465 6620 6164 645f 746f  ..    def add_to
+00000510: 2873 656c 662c 2061 783a 2057 4353 4178  (self, ax: WCSAx
+00000520: 6573 2920 2d3e 204e 6f6e 653a 0a20 2020  es) -> None:.   
+00000530: 2020 2020 2022 2222 4164 6420 7468 6973       """Add this
+00000540: 2061 6e6e 6f74 6174 696f 6e20 746f 2061   annotation to a
+00000550: 2066 696e 6465 7220 6368 6172 742e 0a0a   finder chart...
+00000560: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00000570: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00000580: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6178  -----.        ax
+00000590: 3a20 607e 6173 7472 6f70 792e 7669 7375  : `~astropy.visu
+000005a0: 616c 697a 6174 696f 6e2e 7763 7361 7865  alization.wcsaxe
+000005b0: 732e 5743 5341 7865 7360 0a20 2020 2020  s.WCSAxes`.     
+000005c0: 2020 2020 2020 2050 6c6f 7420 6178 6573         Plot axes
+000005d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000005e0: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
+000005f0: 6e20 7365 6c66 2e5f 6974 656d 733a 0a20  n self._items:. 
+00000600: 2020 2020 2020 2020 2020 2069 7465 6d2e             item.
+00000610: 6164 645f 746f 2861 7829 0a0a 2020 2020  add_to(ax)..    
+00000620: 6465 6620 726f 7461 7465 2873 656c 662c  def rotate(self,
+00000630: 2070 6976 6f74 3a20 536b 7943 6f6f 7264   pivot: SkyCoord
+00000640: 2c20 616e 676c 653a 2041 6e67 6c65 2920  , angle: Angle) 
+00000650: 2d3e 2022 4772 6f75 7041 6e6e 6f74 6174  -> "GroupAnnotat
+00000660: 696f 6e22 3a0a 2020 2020 2020 2020 2222  ion":.        ""
+00000670: 2252 6f74 6174 6520 7468 6973 2061 6e6e  "Rotate this ann
+00000680: 6f74 6174 696f 6e20 6172 6f75 6e64 2061  otation around a
+00000690: 2070 6976 6f74 2061 6e64 2072 6574 7572   pivot and retur
+000006a0: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
+000006b0: 2020 2020 2020 2054 6865 2072 6f74 6174         The rotat
+000006c0: 696f 6e20 616e 676c 6520 6973 2061 6e20  ion angle is an 
+000006d0: 616e 676c 6520 6f6e 2074 6865 2073 6b79  angle on the sky
+000006e0: 2c20 6d65 6173 7572 6564 2066 726f 6d20  , measured from 
+000006f0: 6e6f 7274 6820 746f 2065 6173 742e 0a0a  north to east...
+00000700: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00000710: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00000720: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7069  -----.        pi
+00000730: 766f 743a 2060 7e61 7374 726f 7079 2e63  vot: `~astropy.c
+00000740: 6f6f 7264 696e 6174 6573 2e53 6b79 436f  oordinates.SkyCo
+00000750: 6f72 6460 0a20 2020 2020 2020 2020 2020  ord`.           
+00000760: 2050 6f69 6e74 2061 726f 756e 6420 7768   Point around wh
+00000770: 6963 6820 746f 2072 6f74 6174 6520 7468  ich to rotate th
+00000780: 6520 616e 6e6f 7461 7469 6f6e 2e0a 2020  e annotation..  
+00000790: 2020 2020 2020 616e 676c 653a 2060 7e61        angle: `~a
+000007a0: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
+000007b0: 6573 2e41 6e67 6c65 600a 2020 2020 2020  es.Angle`.      
+000007c0: 2020 2020 2020 416e 676c 6520 6f66 2072        Angle of r
+000007d0: 6f74 6174 696f 6e2c 206d 6561 7375 7265  otation, measure
+000007e0: 6420 6672 6f6d 206e 6f72 7468 2074 6f77  d from north tow
+000007f0: 6172 6473 2074 6865 2065 6173 742e 0a0a  ards the east...
+00000800: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00000810: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00000820: 2020 2020 2020 2020 607e 696d 6570 6875          `~imephu
+00000830: 2e61 6e6e 6f74 6174 696f 6e2e 6765 6e65  .annotation.gene
+00000840: 7261 6c2e 4772 6f75 7041 6e6e 6f74 6174  ral.GroupAnnotat
+00000850: 696f 6e60 0a20 2020 2020 2020 2020 2020  ion`.           
+00000860: 2054 6865 2061 6e6e 6f74 6174 696f 6e20   The annotation 
+00000870: 7265 7375 6c74 696e 6720 6672 6f6d 2074  resulting from t
+00000880: 6865 2072 6f74 6174 696f 6e2e 0a20 2020  he rotation..   
+00000890: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000008a0: 2072 6f74 6174 6564 5f69 7465 6d73 203d   rotated_items =
+000008b0: 205b 6974 656d 2e72 6f74 6174 6528 7069   [item.rotate(pi
+000008c0: 766f 742c 2061 6e67 6c65 2920 666f 7220  vot, angle) for 
+000008d0: 6974 656d 2069 6e20 7365 6c66 2e5f 6974  item in self._it
+000008e0: 656d 735d 0a20 2020 2020 2020 2072 6f74  ems].        rot
+000008f0: 6174 6564 5f61 6e6e 6f74 6174 696f 6e20  ated_annotation 
+00000900: 3d20 4772 6f75 7041 6e6e 6f74 6174 696f  = GroupAnnotatio
+00000910: 6e28 6974 656d 733d 726f 7461 7465 645f  n(items=rotated_
+00000920: 6974 656d 7329 0a20 2020 2020 2020 2072  items).        r
+00000930: 6574 7572 6e20 726f 7461 7465 645f 616e  eturn rotated_an
+00000940: 6e6f 7461 7469 6f6e 0a0a 2020 2020 6465  notation..    de
+00000950: 6620 7472 616e 736c 6174 6528 7365 6c66  f translate(self
+00000960: 2c20 6469 7370 6c61 6365 6d65 6e74 3a20  , displacement: 
+00000970: 416e 676c 6529 202d 3e20 2247 726f 7570  Angle) -> "Group
+00000980: 416e 6e6f 7461 7469 6f6e 223a 0a20 2020  Annotation":.   
+00000990: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000009a0: 204d 6f76 6520 7468 6973 2061 6e6e 6f74   Move this annot
+000009b0: 6174 696f 6e20 616c 6f6e 6720 6120 6469  ation along a di
+000009c0: 7370 6c61 6365 6d65 6e74 2076 6563 746f  splacement vecto
+000009d0: 7220 616e 6420 7265 7475 726e 2074 6865  r and return the
+000009e0: 2072 6573 756c 742e 0a0a 2020 2020 2020   result...      
+000009f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000a00: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00000a10: 2020 2020 2020 2020 6469 7370 6c61 6365          displace
+00000a20: 6d65 6e74 3a20 3244 2061 7272 6179 206f  ment: 2D array o
+00000a30: 6620 616e 676c 6573 0a20 2020 2020 2020  f angles.       
+00000a40: 2020 2020 2054 6865 2064 6973 706c 6163       The displac
+00000a50: 656d 656e 7420 6279 2077 6869 6368 2074  ement by which t
+00000a60: 6f20 6d6f 7665 2074 6865 2061 6e6e 6f74  o move the annot
+00000a70: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+00000a80: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00000a90: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00000aa0: 607e 696d 6570 6875 2e61 6e6e 6f74 6174  `~imephu.annotat
+00000ab0: 696f 6e2e 6765 6e65 7261 6c2e 4772 6f75  ion.general.Grou
+00000ac0: 7041 6e6e 6f74 6174 696f 6e60 0a20 2020  pAnnotation`.   
+00000ad0: 2020 2020 2020 2020 2054 6865 2061 6e6e           The ann
+00000ae0: 6f74 6174 696f 6e20 7265 7375 6c74 696e  otation resultin
+00000af0: 6720 6672 6f6d 2074 6865 2074 7261 6e73  g from the trans
+00000b00: 6c61 7469 6f6e 2e0a 2020 2020 2020 2020  lation..        
+00000b10: 2222 220a 2020 2020 2020 2020 7472 616e  """.        tran
+00000b20: 736c 6174 6564 5f69 7465 6d73 203d 205b  slated_items = [
+00000b30: 6974 656d 2e74 7261 6e73 6c61 7465 2864  item.translate(d
+00000b40: 6973 706c 6163 656d 656e 7429 2066 6f72  isplacement) for
+00000b50: 2069 7465 6d20 696e 2073 656c 662e 5f69   item in self._i
+00000b60: 7465 6d73 5d0a 2020 2020 2020 2020 7472  tems].        tr
+00000b70: 616e 736c 6174 6564 5f61 6e6e 6f74 6174  anslated_annotat
+00000b80: 696f 6e20 3d20 4772 6f75 7041 6e6e 6f74  ion = GroupAnnot
+00000b90: 6174 696f 6e28 7472 616e 736c 6174 6564  ation(translated
+00000ba0: 5f69 7465 6d73 290a 2020 2020 2020 2020  _items).        
+00000bb0: 7265 7475 726e 2074 7261 6e73 6c61 7465  return translate
+00000bc0: 645f 616e 6e6f 7461 7469 6f6e 0a         d_annotation.
```

### Comparing `imephu-0.2.0/src/imephu/annotation/general/__init__.py` & `imephu-0.2.1/src/imephu/annotation/general/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/annotation/general/__pycache__/circle.cpython-310.pyc` & `imephu-0.2.1/src/imephu/annotation/general/circle.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,264 +1,243 @@
-00000000: 6f0d 0d0a 0000 0000 6573 c762 270f 0000  o.......es.b'...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
-00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 0100 6400 6407 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
-00000090: 0100 6400 6408 6c12 6d13 5a13 6d14 5a14  ..d.d.l.m.Z.m.Z.
-000000a0: 6d15 5a15 6d16 5a16 0100 4700 6409 640a  m.Z.m.Z...G.d.d.
-000000b0: 8400 640a 6511 8303 5a17 640b 5300 290c  ..d.e...Z.d.S.).
-000000c0: e900 0000 0029 01da 0864 6565 7063 6f70  .....)...deepcop
-000000d0: 7929 04da 0341 6e79 da05 5475 706c 65da  y)...Any..Tuple.
-000000e0: 0555 6e69 6f6e da04 6361 7374 2902 da05  .Union..cast)...
-000000f0: 416e 676c 65da 0853 6b79 436f 6f72 6429  Angle..SkyCoord)
-00000100: 01da 0757 4353 4178 6573 2901 da03 5743  ...WCSAxes)...WC
-00000110: 5329 01da 0643 6972 636c 6529 01da 0a41  S)...Circle)...A
-00000120: 6e6e 6f74 6174 696f 6e29 04da 0c70 6978  nnotation)...pix
-00000130: 656c 5f73 6361 6c65 73da 0672 6f74 6174  el_scales..rotat
-00000140: 65da 1573 6b79 5f70 6f73 6974 696f 6e5f  e..sky_position_
-00000150: 746f 5f70 6978 656c da09 7472 616e 736c  to_pixel..transl
-00000160: 6174 6563 0000 0000 0000 0000 0000 0000  atec............
-00000170: 0000 0000 1000 0000 4000 0000 7396 0000  ........@...s...
-00000180: 0065 005a 0164 005a 0264 015a 0309 0209  .e.Z.d.Z.d.Z....
-00000190: 0364 1864 0465 0464 0565 0564 0665 0664  .d.d.e.d.e.d.e.d
-000001a0: 0765 0765 0865 0965 0a65 0a65 0a66 0319  .e.e.e.e.e.e.f..
-000001b0: 0066 0219 0064 0865 0765 0865 0965 0a65  .f...d.e.e.e.e.e
-000001c0: 0a65 0a66 0319 0066 0219 0064 0965 0b66  .e.f...f...d.e.f
-000001d0: 0c64 0a64 0b84 055a 0c64 0c65 0d64 0d64  .d.d...Z.d.e.d.d
-000001e0: 0e66 0464 0f64 1084 045a 0e64 1165 0464  .f.d.d...Z.d.e.d
-000001f0: 1265 0564 0d64 0066 0664 1364 1484 045a  .e.d.d.f.d.d...Z
-00000200: 0f64 1565 0564 0d64 0066 0464 1664 1784  .d.e.d.d.f.d.d..
-00000210: 045a 1064 0e53 0029 19da 1043 6972 636c  .Z.d.S.)...Circl
-00000220: 6541 6e6e 6f74 6174 696f 6e61 cf03 0000  eAnnotationa....
-00000230: 416e 2061 6e6e 6f74 6174 696f 6e20 666f  An annotation fo
-00000240: 7220 6164 6469 6e67 2061 2063 6972 636c  r adding a circl
-00000250: 6520 746f 2061 2070 6c6f 742e 0a0a 2020  e to a plot...  
-00000260: 2020 5468 6520 7261 6469 7573 206f 6620    The radius of 
-00000270: 7468 6520 6369 7263 6c65 2069 7320 6769  the circle is gi
-00000280: 7665 6e20 6173 2061 6e20 616e 6775 6c61  ven as an angula
-00000290: 7220 6469 7374 616e 6365 206f 6e20 7468  r distance on th
-000002a0: 6520 736b 792c 2069 6e20 7468 650a 2020  e sky, in the.  
-000002b0: 2020 6469 7265 6374 696f 6e20 6f66 2074    direction of t
-000002c0: 6865 2072 6967 6874 2061 7363 656e 7369  he right ascensi
-000002d0: 6f6e 2e20 4120 6369 7263 6c65 2069 7320  on. A circle is 
-000002e0: 6472 6177 6e20 6972 7265 7370 6563 7469  drawn irrespecti
-000002f0: 7665 206f 6620 7468 6520 7069 7865 6c20  ve of the pixel 
-00000300: 7363 616c 6573 0a20 2020 2066 6f72 2072  scales.    for r
-00000310: 6967 6874 2061 7363 656e 7369 6f6e 2061  ight ascension a
-00000320: 6e64 2064 6563 6c69 6e61 7469 6f6e 2e20  nd declination. 
-00000330: 4865 6e63 6520 7468 6520 6369 7263 6c65  Hence the circle
-00000340: 2069 6e20 6765 6e65 7261 6c20 6973 206e   in general is n
-00000350: 6f74 2061 2063 6972 636c 6520 6f6e 0a20  ot a circle on. 
-00000360: 2020 2074 6865 2073 6b79 2062 7574 206a     the sky but j
-00000370: 7573 7420 6f6e 2074 6865 2066 696e 6465  ust on the finde
-00000380: 7220 6368 6172 742e 0a0a 2020 2020 5061  r chart...    Pa
-00000390: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-000003a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6365 6e74  -------.    cent
-000003b0: 6572 3a20 607e 6173 7472 6f70 792e 636f  er: `~astropy.co
-000003c0: 6f72 6469 6e61 7465 732e 536b 7943 6f6f  ordinates.SkyCoo
-000003d0: 7264 600a 2020 2020 2020 2020 5468 6520  rd`.        The 
-000003e0: 7269 6768 7420 6173 6365 6e73 696f 6e20  right ascension 
-000003f0: 616e 6420 6465 636c 696e 6174 696f 6e20  and declination 
-00000400: 6f66 2074 6865 2063 6972 636c 6527 7320  of the circle's 
-00000410: 6365 6e74 6572 2e0a 2020 2020 7261 6469  center..    radi
-00000420: 7573 3a20 607e 6173 7472 6f70 792e 636f  us: `~astropy.co
-00000430: 6f72 6469 6e61 7465 732e 416e 676c 6560  ordinates.Angle`
-00000440: 0a20 2020 2020 2020 2054 6865 2072 6164  .        The rad
-00000450: 6975 7320 6f66 2074 6865 2063 6972 636c  ius of the circl
-00000460: 652c 2061 7320 616e 2061 6e67 756c 6172  e, as an angular
-00000470: 2064 6973 7461 6e63 6520 6f6e 2074 6865   distance on the
-00000480: 2073 6b79 2069 6e20 7269 6768 7420 6173   sky in right as
-00000490: 6365 6e73 696f 6e0a 2020 2020 2020 2020  cension.        
-000004a0: 6469 7265 6374 696f 6e2e 0a20 2020 2077  direction..    w
-000004b0: 6373 3a20 607e 6173 7472 6f70 792e 7763  cs: `~astropy.wc
-000004c0: 732e 5743 5360 0a20 2020 2020 2020 2057  s.WCS`.        W
-000004d0: 4353 206f 626a 6563 742e 0a20 2020 2065  CS object..    e
-000004e0: 6467 6563 6f6c 6f72 3a20 636f 6c6f 722c  dgecolor: color,
-000004f0: 2064 6566 6175 6c74 3a20 2262 6c61 636b   default: "black
-00000500: 220a 2020 2020 2020 2020 5468 6520 6564  ".        The ed
-00000510: 6765 2063 6f6c 6f72 2e0a 2020 2020 6661  ge color..    fa
-00000520: 6365 636f 6c6f 723a 2063 6f6c 6f72 2c20  cecolor: color, 
-00000530: 6465 6661 756c 743a 2022 6e6f 6e65 220a  default: "none".
-00000540: 2020 2020 2020 2020 5468 6520 6669 6c6c          The fill
-00000550: 696e 6720 636f 6c6f 722e 0a20 2020 202a  ing color..    *
-00000560: 2a6b 7761 7267 733a 2064 6963 742c 206f  *kwargs: dict, o
-00000570: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00000580: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
-00000590: 7264 2061 7267 756d 656e 7473 2c20 7768  rd arguments, wh
-000005a0: 6963 6820 7769 6c6c 2062 6520 7061 7373  ich will be pass
-000005b0: 6564 2074 6f20 4d61 7470 6c6f 746c 6962  ed to Matplotlib
-000005c0: 2773 0a20 2020 2020 2020 2060 7e6d 6174  's.        `~mat
-000005d0: 706c 6f74 6c69 622e 7061 7463 6865 732e  plotlib.patches.
-000005e0: 4369 7263 6c65 6020 7061 7463 6820 636f  Circle` patch co
-000005f0: 6e73 7472 7563 746f 722e 0a20 2020 20da  nstructor..    .
-00000600: 0562 6c61 636b da04 6e6f 6e65 da06 6365  .black..none..ce
-00000610: 6e74 6572 da06 7261 6469 7573 da03 7763  nter..radius..wc
-00000620: 73da 0965 6467 6563 6f6c 6f72 da09 6661  s..edgecolor..fa
-00000630: 6365 636f 6c6f 72da 066b 7761 7267 7363  cecolor..kwargsc
-00000640: 0600 0000 0000 0000 0000 0000 0700 0000  ................
-00000650: 0300 0000 4b00 0000 7334 0000 007c 017c  ....K...s4...|.|
-00000660: 005f 007c 027c 005f 017c 037c 005f 0274  ._.|.|._.|.|._.t
-00000670: 037c 0683 017c 005f 047c 047c 006a 0464  .|...|._.|.|.j.d
-00000680: 013c 007c 057c 006a 0464 023c 0064 0053  .<.|.|.j.d.<.d.S
-00000690: 0029 034e 7217 0000 0072 1800 0000 2905  .).Nr....r....).
-000006a0: da07 5f63 656e 7465 72da 075f 7261 6469  .._center.._radi
-000006b0: 7573 da04 5f77 6373 7202 0000 00da 075f  us.._wcsr......_
-000006c0: 6b77 6172 6773 2907 da04 7365 6c66 7214  kwargs)...selfr.
-000006d0: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-000006e0: 0000 7218 0000 0072 1900 0000 a900 721f  ..r....r......r.
-000006f0: 0000 00fa 4c2f 5573 6572 732f 6368 7269  ....L/Users/chri
-00000700: 7374 6961 6e2f 4964 6561 5072 6f6a 6563  stian/IdeaProjec
-00000710: 7473 2f69 6d65 7068 752f 7372 632f 696d  ts/imephu/src/im
-00000720: 6570 6875 2f61 6e6e 6f74 6174 696f 6e2f  ephu/annotation/
-00000730: 6765 6e65 7261 6c2f 6369 7263 6c65 2e70  general/circle.p
-00000740: 79da 085f 5f69 6e69 745f 5f27 0000 0073  y..__init__'...s
-00000750: 0c00 0000 0609 0601 0601 0a01 0a01 0e01  ................
-00000760: 7a19 4369 7263 6c65 416e 6e6f 7461 7469  z.CircleAnnotati
-00000770: 6f6e 2e5f 5f69 6e69 745f 5fda 0261 78da  on.__init__..ax.
-00000780: 0672 6574 7572 6e4e 6302 0000 0000 0000  .returnNc.......
-00000790: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
-000007a0: 0073 5a00 0000 7400 7401 7402 7402 6602  .sZ...t.t.t.t.f.
-000007b0: 1900 7403 7c00 6a04 7c00 6a05 8302 8302  ..t.|.j.|.j.....
-000007c0: 7d02 7406 7c00 6a05 8301 5c02 7d03 7d04  }.t.|.j...\.}.}.
-000007d0: 7402 7c00 6a07 7c03 1b00 8301 7d05 7408  t.|.j.|.....}.t.
-000007e0: 7c02 7c05 6602 6900 7c00 6a09 a401 8e01  |.|.f.i.|.j.....
-000007f0: 7d06 7c01 a00a 7c06 a101 0100 6401 5300  }.|...|.....d.S.
-00000800: 2902 7a7d 4164 6420 7468 6520 6369 7263  ).z}Add the circ
-00000810: 6c65 2074 6f20 6120 6669 6e64 6572 2063  le to a finder c
-00000820: 6861 7274 2e0a 0a20 2020 2020 2020 2061  hart...        a
-00000830: 783a 2060 7e61 7374 726f 7079 2e76 6973  x: `~astropy.vis
-00000840: 7561 6c69 7a61 7469 6f6e 2e77 6373 6178  ualization.wcsax
-00000850: 6573 2e57 4353 4178 6573 600a 2020 2020  es.WCSAxes`.    
-00000860: 2020 2020 2020 2020 5743 5320 6178 6573          WCS axes
-00000870: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
-00000880: 204e 290b 7206 0000 0072 0400 0000 da05   N).r....r......
-00000890: 666c 6f61 7472 0f00 0000 721a 0000 0072  floatr....r....r
-000008a0: 1c00 0000 720d 0000 0072 1b00 0000 720b  ....r....r....r.
-000008b0: 0000 0072 1d00 0000 da09 6164 645f 7061  ...r......add_pa
-000008c0: 7463 6829 0772 1e00 0000 7222 0000 005a  tch).r....r"...Z
-000008d0: 0963 656e 7465 725f 7078 5a0e 7261 5f70  .center_pxZ.ra_p
-000008e0: 6978 656c 5f73 6361 6c65 da01 5f5a 0972  ixel_scale.._Z.r
-000008f0: 6164 6975 735f 7078 5a0c 6369 7263 6c65  adius_pxZ.circle
-00000900: 5f70 6174 6368 721f 0000 0072 1f00 0000  _patchr....r....
-00000910: 7220 0000 00da 0661 6464 5f74 6f37 0000  r .....add_to7..
-00000920: 0073 0e00 0000 0206 1601 04ff 0e03 0e01  .s..............
-00000930: 1401 0e01 7a17 4369 7263 6c65 416e 6e6f  ....z.CircleAnno
-00000940: 7461 7469 6f6e 2e61 6464 5f74 6fda 0570  tation.add_to..p
-00000950: 6976 6f74 da05 616e 676c 6563 0300 0000  ivot..anglec....
-00000960: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-00000970: 4300 0000 7324 0000 0074 007c 0083 017d  C...s$...t.|...}
-00000980: 0374 017c 006a 027c 017c 027c 006a 0383  .t.|.j.|.|.|.j..
-00000990: 047d 047c 047c 035f 027c 0353 0029 0261  .}.|.|._.|.S.).a
-000009a0: 1c02 0000 526f 7461 7465 2074 6869 7320  ....Rotate this 
-000009b0: 616e 6e6f 7461 7469 6f6e 2061 726f 756e  annotation aroun
-000009c0: 6420 6120 7069 766f 7420 616e 6420 7265  d a pivot and re
-000009d0: 7475 726e 2074 6865 2072 6573 756c 742e  turn the result.
-000009e0: 0a0a 2020 2020 2020 2020 5468 6520 726f  ..        The ro
-000009f0: 7461 7469 6f6e 2061 6e67 6c65 2069 7320  tation angle is 
-00000a00: 616e 2061 6e67 6c65 206f 6e20 7468 6520  an angle on the 
-00000a10: 736b 792c 206d 6561 7375 7265 6420 6672  sky, measured fr
-00000a20: 6f6d 206e 6f72 7468 2074 6f20 6561 7374  om north to east
-00000a30: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00000a40: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00000a50: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00000a60: 2070 6976 6f74 3a20 607e 6173 7472 6f70   pivot: `~astrop
-00000a70: 792e 636f 6f72 6469 6e61 7465 732e 536b  y.coordinates.Sk
-00000a80: 7943 6f6f 7264 600a 2020 2020 2020 2020  yCoord`.        
-00000a90: 2020 2020 506f 696e 7420 6172 6f75 6e64      Point around
-00000aa0: 2077 6869 6368 2074 6f20 726f 7461 7465   which to rotate
-00000ab0: 2074 6865 2061 6e6e 6f74 6174 696f 6e2e   the annotation.
-00000ac0: 0a20 2020 2020 2020 2061 6e67 6c65 3a20  .        angle: 
-00000ad0: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
-00000ae0: 6e61 7465 732e 416e 676c 6560 0a20 2020  nates.Angle`.   
-00000af0: 2020 2020 2020 2020 2041 6e67 6c65 206f           Angle o
-00000b00: 6620 726f 7461 7469 6f6e 2c20 6d65 6173  f rotation, meas
-00000b10: 7572 6564 2066 726f 6d20 6e6f 7274 6820  ured from north 
-00000b20: 746f 2065 6173 742e 0a0a 2020 2020 2020  to east...      
-00000b30: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00000b40: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00000b50: 2020 607e 696d 6570 6875 2e61 6e6e 6f74    `~imephu.annot
-00000b60: 6174 696f 6e2e 6765 6e65 7261 6c2e 4369  ation.general.Ci
-00000b70: 7263 6c65 416e 6e6f 7461 7469 6f6e 600a  rcleAnnotation`.
-00000b80: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00000b90: 616e 6e6f 7461 7469 6f6e 2072 6573 756c  annotation resul
-00000ba0: 7469 6e67 2066 726f 6d20 7468 6520 726f  ting from the ro
-00000bb0: 7461 7469 6f6e 2e0a 2020 2020 2020 2020  tation..        
-00000bc0: 4e29 0472 0200 0000 720e 0000 0072 1a00  N).r....r....r..
-00000bd0: 0000 721c 0000 0029 0572 1e00 0000 7228  ..r....).r....r(
-00000be0: 0000 0072 2900 0000 5a12 726f 7461 7465  ...r)...Z.rotate
-00000bf0: 645f 616e 6e6f 7461 7469 6f6e 5a0e 726f  d_annotationZ.ro
-00000c00: 7461 7465 645f 6365 6e74 6572 721f 0000  tated_centerr...
-00000c10: 0072 1f00 0000 7220 0000 0072 0e00 0000  .r....r ...r....
-00000c20: 4500 0000 7308 0000 0008 1112 0106 0104  E...s...........
-00000c30: 017a 1743 6972 636c 6541 6e6e 6f74 6174  .z.CircleAnnotat
-00000c40: 696f 6e2e 726f 7461 7465 da0c 6469 7370  ion.rotate..disp
-00000c50: 6c61 6365 6d65 6e74 6302 0000 0000 0000  lacementc.......
-00000c60: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-00000c70: 0073 1e00 0000 7400 7c00 8301 7d02 7401  .s....t.|...}.t.
-00000c80: 7c00 6a02 7c01 8302 7d03 7c03 7c02 5f02  |.j.|...}.|.|._.
-00000c90: 7c02 5300 2902 6179 0100 000a 2020 2020  |.S.).ay....    
-00000ca0: 2020 2020 4d6f 7665 2074 6869 7320 616e      Move this an
-00000cb0: 6e6f 7461 7469 6f6e 2061 6c6f 6e67 2061  notation along a
-00000cc0: 2064 6973 706c 6163 656d 656e 7420 7665   displacement ve
-00000cd0: 6374 6f72 2061 6e64 2072 6574 7572 6e20  ctor and return 
-00000ce0: 7468 6520 7265 7375 6c74 2e0a 0a20 2020  the result...   
-00000cf0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00000d00: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00000d10: 2d2d 0a20 2020 2020 2020 2064 6973 706c  --.        displ
-00000d20: 6163 656d 656e 743a 2032 4420 6172 7261  acement: 2D arra
-00000d30: 7920 6f66 2061 6e67 6c65 730a 2020 2020  y of angles.    
-00000d40: 2020 2020 2020 2020 5468 6520 6469 7370          The disp
-00000d50: 6c61 6365 6d65 6e74 2062 7920 7768 6963  lacement by whic
-00000d60: 6820 746f 206d 6f76 6520 7468 6520 616e  h to move the an
-00000d70: 6e6f 7461 7469 6f6e 2e0a 0a20 2020 2020  notation...     
-00000d80: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00000d90: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00000da0: 2020 2060 7e69 6d65 7068 752e 616e 6e6f     `~imephu.anno
-00000db0: 7461 7469 6f6e 2e67 656e 6572 616c 2e43  tation.general.C
-00000dc0: 6972 636c 6541 6e6e 6f74 6174 696f 6e60  ircleAnnotation`
-00000dd0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00000de0: 2061 6e6e 6f74 6174 696f 6e20 7265 7375   annotation resu
-00000df0: 6c74 696e 6720 6672 6f6d 2074 6865 2074  lting from the t
-00000e00: 7261 6e73 6c61 7469 6f6e 2e0a 2020 2020  ranslation..    
-00000e10: 2020 2020 4e29 0372 0200 0000 7210 0000      N).r....r...
-00000e20: 0072 1a00 0000 2904 721e 0000 0072 2a00  .r....).r....r*.
-00000e30: 0000 5a15 7472 616e 736c 6174 6564 5f61  ..Z.translated_a
-00000e40: 6e6e 6f74 6174 696f 6e5a 1174 7261 6e73  nnotationZ.trans
-00000e50: 6c61 7465 645f 6365 6e74 6572 721f 0000  lated_centerr...
-00000e60: 0072 1f00 0000 7220 0000 0072 1000 0000  .r....r ...r....
-00000e70: 5b00 0000 7308 0000 0008 0e0c 0106 0104  [...s...........
-00000e80: 017a 1a43 6972 636c 6541 6e6e 6f74 6174  .z.CircleAnnotat
-00000e90: 696f 6e2e 7472 616e 736c 6174 6529 0272  ion.translate).r
-00000ea0: 1200 0000 7213 0000 0029 11da 085f 5f6e  ....r....)...__n
-00000eb0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000ec0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000ed0: 075f 5f64 6f63 5f5f 7208 0000 0072 0700  .__doc__r....r..
-00000ee0: 0000 720a 0000 0072 0500 0000 da03 7374  ..r....r......st
-00000ef0: 7272 0400 0000 7224 0000 0072 0300 0000  rr....r$...r....
-00000f00: 7221 0000 0072 0900 0000 7227 0000 0072  r!...r....r'...r
-00000f10: 0e00 0000 7210 0000 0072 1f00 0000 721f  ....r....r....r.
-00000f20: 0000 0072 1f00 0000 7220 0000 0072 1100  ...r....r ...r..
-00000f30: 0000 0d00 0000 7328 0000 0008 0004 0102  ......s(........
-00000f40: 1e02 0104 fa02 0202 fe02 0302 fd02 0402  ................
-00000f50: fc14 0502 fb14 0602 fa02 070a f912 1016  ................
-00000f60: 0e16 1672 1100 0000 4e29 18da 0463 6f70  ...r....N)...cop
-00000f70: 7972 0200 0000 da06 7479 7069 6e67 7203  yr......typingr.
-00000f80: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
-00000f90: 0000 da13 6173 7472 6f70 792e 636f 6f72  ....astropy.coor
-00000fa0: 6469 6e61 7465 7372 0700 0000 7208 0000  dinatesr....r...
-00000fb0: 00da 1d61 7374 726f 7079 2e76 6973 7561  ...astropy.visua
-00000fc0: 6c69 7a61 7469 6f6e 2e77 6373 6178 6573  lization.wcsaxes
-00000fd0: 7209 0000 00da 0b61 7374 726f 7079 2e77  r......astropy.w
-00000fe0: 6373 720a 0000 00da 126d 6174 706c 6f74  csr......matplot
-00000ff0: 6c69 622e 7061 7463 6865 7372 0b00 0000  lib.patchesr....
-00001000: 5a11 696d 6570 6875 2e61 6e6e 6f74 6174  Z.imephu.annotat
-00001010: 696f 6e72 0c00 0000 5a0f 696d 6570 6875  ionr....Z.imephu
-00001020: 2e67 656f 6d65 7472 7972 0d00 0000 720e  .geometryr....r.
-00001030: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-00001040: 0000 721f 0000 0072 1f00 0000 721f 0000  ..r....r....r...
-00001050: 0072 2000 0000 da08 3c6d 6f64 756c 653e  .r .....<module>
-00001060: 0100 0000 7312 0000 000c 0018 0110 020c  ....s...........
-00001070: 010c 010c 010c 0218 0114 03              ...........
+00000000: 6672 6f6d 2063 6f70 7920 696d 706f 7274  from copy import
+00000010: 2064 6565 7063 6f70 790a 6672 6f6d 2074   deepcopy.from t
+00000020: 7970 696e 6720 696d 706f 7274 2041 6e79  yping import Any
+00000030: 2c20 5475 706c 652c 2055 6e69 6f6e 2c20  , Tuple, Union, 
+00000040: 6361 7374 0a0a 6672 6f6d 2061 7374 726f  cast..from astro
+00000050: 7079 2e63 6f6f 7264 696e 6174 6573 2069  py.coordinates i
+00000060: 6d70 6f72 7420 416e 676c 652c 2053 6b79  mport Angle, Sky
+00000070: 436f 6f72 640a 6672 6f6d 2061 7374 726f  Coord.from astro
+00000080: 7079 2e76 6973 7561 6c69 7a61 7469 6f6e  py.visualization
+00000090: 2e77 6373 6178 6573 2069 6d70 6f72 7420  .wcsaxes import 
+000000a0: 5743 5341 7865 730a 6672 6f6d 2061 7374  WCSAxes.from ast
+000000b0: 726f 7079 2e77 6373 2069 6d70 6f72 7420  ropy.wcs import 
+000000c0: 5743 530a 6672 6f6d 206d 6174 706c 6f74  WCS.from matplot
+000000d0: 6c69 622e 7061 7463 6865 7320 696d 706f  lib.patches impo
+000000e0: 7274 2043 6972 636c 650a 0a66 726f 6d20  rt Circle..from 
+000000f0: 696d 6570 6875 2e61 6e6e 6f74 6174 696f  imephu.annotatio
+00000100: 6e20 696d 706f 7274 2041 6e6e 6f74 6174  n import Annotat
+00000110: 696f 6e0a 6672 6f6d 2069 6d65 7068 752e  ion.from imephu.
+00000120: 6765 6f6d 6574 7279 2069 6d70 6f72 7420  geometry import 
+00000130: 7069 7865 6c5f 7363 616c 6573 2c20 726f  pixel_scales, ro
+00000140: 7461 7465 2c20 736b 795f 706f 7369 7469  tate, sky_positi
+00000150: 6f6e 5f74 6f5f 7069 7865 6c2c 2074 7261  on_to_pixel, tra
+00000160: 6e73 6c61 7465 0a0a 0a63 6c61 7373 2043  nslate...class C
+00000170: 6972 636c 6541 6e6e 6f74 6174 696f 6e28  ircleAnnotation(
+00000180: 416e 6e6f 7461 7469 6f6e 293a 0a20 2020  Annotation):.   
+00000190: 2022 2222 416e 2061 6e6e 6f74 6174 696f   """An annotatio
+000001a0: 6e20 666f 7220 6164 6469 6e67 2061 2063  n for adding a c
+000001b0: 6972 636c 6520 746f 2061 2070 6c6f 742e  ircle to a plot.
+000001c0: 0a0a 2020 2020 5468 6520 7261 6469 7573  ..    The radius
+000001d0: 206f 6620 7468 6520 6369 7263 6c65 2069   of the circle i
+000001e0: 7320 6769 7665 6e20 6173 2061 6e20 616e  s given as an an
+000001f0: 6775 6c61 7220 6469 7374 616e 6365 206f  gular distance o
+00000200: 6e20 7468 6520 736b 792c 2069 6e20 7468  n the sky, in th
+00000210: 650a 2020 2020 6469 7265 6374 696f 6e20  e.    direction 
+00000220: 6f66 2074 6865 2072 6967 6874 2061 7363  of the right asc
+00000230: 656e 7369 6f6e 2e20 4120 6369 7263 6c65  ension. A circle
+00000240: 2069 7320 6472 6177 6e20 6972 7265 7370   is drawn irresp
+00000250: 6563 7469 7665 206f 6620 7468 6520 7069  ective of the pi
+00000260: 7865 6c20 7363 616c 6573 0a20 2020 2066  xel scales.    f
+00000270: 6f72 2072 6967 6874 2061 7363 656e 7369  or right ascensi
+00000280: 6f6e 2061 6e64 2064 6563 6c69 6e61 7469  on and declinati
+00000290: 6f6e 2e20 4865 6e63 6520 7468 6520 6369  on. Hence the ci
+000002a0: 7263 6c65 2069 6e20 6765 6e65 7261 6c20  rcle in general 
+000002b0: 6973 206e 6f74 2061 2063 6972 636c 6520  is not a circle 
+000002c0: 6f6e 0a20 2020 2074 6865 2073 6b79 2062  on.    the sky b
+000002d0: 7574 206a 7573 7420 6f6e 2074 6865 2066  ut just on the f
+000002e0: 696e 6465 7220 6368 6172 742e 0a0a 2020  inder chart...  
+000002f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000300: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000310: 6365 6e74 6572 3a20 607e 6173 7472 6f70  center: `~astrop
+00000320: 792e 636f 6f72 6469 6e61 7465 732e 536b  y.coordinates.Sk
+00000330: 7943 6f6f 7264 600a 2020 2020 2020 2020  yCoord`.        
+00000340: 5468 6520 7269 6768 7420 6173 6365 6e73  The right ascens
+00000350: 696f 6e20 616e 6420 6465 636c 696e 6174  ion and declinat
+00000360: 696f 6e20 6f66 2074 6865 2063 6972 636c  ion of the circl
+00000370: 6527 7320 6365 6e74 6572 2e0a 2020 2020  e's center..    
+00000380: 7261 6469 7573 3a20 607e 6173 7472 6f70  radius: `~astrop
+00000390: 792e 636f 6f72 6469 6e61 7465 732e 416e  y.coordinates.An
+000003a0: 676c 6560 0a20 2020 2020 2020 2054 6865  gle`.        The
+000003b0: 2072 6164 6975 7320 6f66 2074 6865 2063   radius of the c
+000003c0: 6972 636c 652c 2061 7320 616e 2061 6e67  ircle, as an ang
+000003d0: 756c 6172 2064 6973 7461 6e63 6520 6f6e  ular distance on
+000003e0: 2074 6865 2073 6b79 2069 6e20 7269 6768   the sky in righ
+000003f0: 7420 6173 6365 6e73 696f 6e0a 2020 2020  t ascension.    
+00000400: 2020 2020 6469 7265 6374 696f 6e2e 0a20      direction.. 
+00000410: 2020 2077 6373 3a20 607e 6173 7472 6f70     wcs: `~astrop
+00000420: 792e 7763 732e 5743 5360 0a20 2020 2020  y.wcs.WCS`.     
+00000430: 2020 2057 4353 206f 626a 6563 742e 0a20     WCS object.. 
+00000440: 2020 2065 6467 6563 6f6c 6f72 3a20 636f     edgecolor: co
+00000450: 6c6f 722c 2064 6566 6175 6c74 3a20 2262  lor, default: "b
+00000460: 6c61 636b 220a 2020 2020 2020 2020 5468  lack".        Th
+00000470: 6520 6564 6765 2063 6f6c 6f72 2e0a 2020  e edge color..  
+00000480: 2020 6661 6365 636f 6c6f 723a 2063 6f6c    facecolor: col
+00000490: 6f72 2c20 6465 6661 756c 743a 2022 6e6f  or, default: "no
+000004a0: 6e65 220a 2020 2020 2020 2020 5468 6520  ne".        The 
+000004b0: 6669 6c6c 696e 6720 636f 6c6f 722e 0a20  filling color.. 
+000004c0: 2020 202a 2a6b 7761 7267 733a 2064 6963     **kwargs: dic
+000004d0: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+000004e0: 2020 2020 4164 6469 7469 6f6e 616c 206b      Additional k
+000004f0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+00000500: 2c20 7768 6963 6820 7769 6c6c 2062 6520  , which will be 
+00000510: 7061 7373 6564 2074 6f20 4d61 7470 6c6f  passed to Matplo
+00000520: 746c 6962 2773 0a20 2020 2020 2020 2060  tlib's.        `
+00000530: 7e6d 6174 706c 6f74 6c69 622e 7061 7463  ~matplotlib.patc
+00000540: 6865 732e 4369 7263 6c65 6020 7061 7463  hes.Circle` patc
+00000550: 6820 636f 6e73 7472 7563 746f 722e 0a20  h constructor.. 
+00000560: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+00000570: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00000580: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00000590: 6365 6e74 6572 3a20 536b 7943 6f6f 7264  center: SkyCoord
+000005a0: 2c0a 2020 2020 2020 2020 7261 6469 7573  ,.        radius
+000005b0: 3a20 416e 676c 652c 0a20 2020 2020 2020  : Angle,.       
+000005c0: 2077 6373 3a20 5743 532c 0a20 2020 2020   wcs: WCS,.     
+000005d0: 2020 2065 6467 6563 6f6c 6f72 3a20 556e     edgecolor: Un
+000005e0: 696f 6e5b 7374 722c 2054 7570 6c65 5b66  ion[str, Tuple[f
+000005f0: 6c6f 6174 2c20 666c 6f61 742c 2066 6c6f  loat, float, flo
+00000600: 6174 5d5d 203d 2022 626c 6163 6b22 2c0a  at]] = "black",.
+00000610: 2020 2020 2020 2020 6661 6365 636f 6c6f          facecolo
+00000620: 723a 2055 6e69 6f6e 5b73 7472 2c20 5475  r: Union[str, Tu
+00000630: 706c 655b 666c 6f61 742c 2066 6c6f 6174  ple[float, float
+00000640: 2c20 666c 6f61 745d 5d20 3d20 226e 6f6e  , float]] = "non
+00000650: 6522 2c0a 2020 2020 2020 2020 2a2a 6b77  e",.        **kw
+00000660: 6172 6773 3a20 416e 792c 0a20 2020 2029  args: Any,.    )
+00000670: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00000680: 6365 6e74 6572 203d 2063 656e 7465 720a  center = center.
+00000690: 2020 2020 2020 2020 7365 6c66 2e5f 7261          self._ra
+000006a0: 6469 7573 203d 2072 6164 6975 730a 2020  dius = radius.  
+000006b0: 2020 2020 2020 7365 6c66 2e5f 7763 7320        self._wcs 
+000006c0: 3d20 7763 730a 2020 2020 2020 2020 7365  = wcs.        se
+000006d0: 6c66 2e5f 6b77 6172 6773 203d 2064 6565  lf._kwargs = dee
+000006e0: 7063 6f70 7928 6b77 6172 6773 290a 2020  pcopy(kwargs).  
+000006f0: 2020 2020 2020 7365 6c66 2e5f 6b77 6172        self._kwar
+00000700: 6773 5b22 6564 6765 636f 6c6f 7222 5d20  gs["edgecolor"] 
+00000710: 3d20 6564 6765 636f 6c6f 720a 2020 2020  = edgecolor.    
+00000720: 2020 2020 7365 6c66 2e5f 6b77 6172 6773      self._kwargs
+00000730: 5b22 6661 6365 636f 6c6f 7222 5d20 3d20  ["facecolor"] = 
+00000740: 6661 6365 636f 6c6f 720a 0a20 2020 2064  facecolor..    d
+00000750: 6566 2061 6464 5f74 6f28 7365 6c66 2c20  ef add_to(self, 
+00000760: 6178 3a20 5743 5341 7865 7329 202d 3e20  ax: WCSAxes) -> 
+00000770: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00000780: 2241 6464 2074 6865 2063 6972 636c 6520  "Add the circle 
+00000790: 746f 2061 2066 696e 6465 7220 6368 6172  to a finder char
+000007a0: 742e 0a0a 2020 2020 2020 2020 6178 3a20  t...        ax: 
+000007b0: 607e 6173 7472 6f70 792e 7669 7375 616c  `~astropy.visual
+000007c0: 697a 6174 696f 6e2e 7763 7361 7865 732e  ization.wcsaxes.
+000007d0: 5743 5341 7865 7360 0a20 2020 2020 2020  WCSAxes`.       
+000007e0: 2020 2020 2057 4353 2061 7865 7320 6f62       WCS axes ob
+000007f0: 6a65 6374 2e0a 2020 2020 2020 2020 2222  ject..        ""
+00000800: 220a 2020 2020 2020 2020 6365 6e74 6572  ".        center
+00000810: 5f70 7820 3d20 6361 7374 280a 2020 2020  _px = cast(.    
+00000820: 2020 2020 2020 2020 5475 706c 655b 666c          Tuple[fl
+00000830: 6f61 742c 2066 6c6f 6174 5d2c 2073 6b79  oat, float], sky
+00000840: 5f70 6f73 6974 696f 6e5f 746f 5f70 6978  _position_to_pix
+00000850: 656c 2873 656c 662e 5f63 656e 7465 722c  el(self._center,
+00000860: 2073 656c 662e 5f77 6373 290a 2020 2020   self._wcs).    
+00000870: 2020 2020 290a 2020 2020 2020 2020 7261      ).        ra
+00000880: 5f70 6978 656c 5f73 6361 6c65 2c20 5f20  _pixel_scale, _ 
+00000890: 3d20 7069 7865 6c5f 7363 616c 6573 2873  = pixel_scales(s
+000008a0: 656c 662e 5f77 6373 290a 2020 2020 2020  elf._wcs).      
+000008b0: 2020 7261 6469 7573 5f70 7820 3d20 666c    radius_px = fl
+000008c0: 6f61 7428 7365 6c66 2e5f 7261 6469 7573  oat(self._radius
+000008d0: 202f 2072 615f 7069 7865 6c5f 7363 616c   / ra_pixel_scal
+000008e0: 6529 0a20 2020 2020 2020 2063 6972 636c  e).        circl
+000008f0: 655f 7061 7463 6820 3d20 4369 7263 6c65  e_patch = Circle
+00000900: 2863 656e 7465 725f 7078 2c20 7261 6469  (center_px, radi
+00000910: 7573 5f70 782c 202a 2a73 656c 662e 5f6b  us_px, **self._k
+00000920: 7761 7267 7329 0a20 2020 2020 2020 2061  wargs).        a
+00000930: 782e 6164 645f 7061 7463 6828 6369 7263  x.add_patch(circ
+00000940: 6c65 5f70 6174 6368 290a 0a20 2020 2064  le_patch)..    d
+00000950: 6566 2072 6f74 6174 6528 7365 6c66 2c20  ef rotate(self, 
+00000960: 7069 766f 743a 2053 6b79 436f 6f72 642c  pivot: SkyCoord,
+00000970: 2061 6e67 6c65 3a20 416e 676c 6529 202d   angle: Angle) -
+00000980: 3e20 2243 6972 636c 6541 6e6e 6f74 6174  > "CircleAnnotat
+00000990: 696f 6e22 3a0a 2020 2020 2020 2020 2222  ion":.        ""
+000009a0: 2252 6f74 6174 6520 7468 6973 2061 6e6e  "Rotate this ann
+000009b0: 6f74 6174 696f 6e20 6172 6f75 6e64 2061  otation around a
+000009c0: 2070 6976 6f74 2061 6e64 2072 6574 7572   pivot and retur
+000009d0: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
+000009e0: 2020 2020 2020 2054 6865 2072 6f74 6174         The rotat
+000009f0: 696f 6e20 616e 676c 6520 6973 2061 6e20  ion angle is an 
+00000a00: 616e 676c 6520 6f6e 2074 6865 2073 6b79  angle on the sky
+00000a10: 2c20 6d65 6173 7572 6564 2066 726f 6d20  , measured from 
+00000a20: 6e6f 7274 6820 746f 2065 6173 742e 0a0a  north to east...
+00000a30: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00000a40: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00000a50: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7069  -----.        pi
+00000a60: 766f 743a 2060 7e61 7374 726f 7079 2e63  vot: `~astropy.c
+00000a70: 6f6f 7264 696e 6174 6573 2e53 6b79 436f  oordinates.SkyCo
+00000a80: 6f72 6460 0a20 2020 2020 2020 2020 2020  ord`.           
+00000a90: 2050 6f69 6e74 2061 726f 756e 6420 7768   Point around wh
+00000aa0: 6963 6820 746f 2072 6f74 6174 6520 7468  ich to rotate th
+00000ab0: 6520 616e 6e6f 7461 7469 6f6e 2e0a 2020  e annotation..  
+00000ac0: 2020 2020 2020 616e 676c 653a 2060 7e61        angle: `~a
+00000ad0: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
+00000ae0: 6573 2e41 6e67 6c65 600a 2020 2020 2020  es.Angle`.      
+00000af0: 2020 2020 2020 416e 676c 6520 6f66 2072        Angle of r
+00000b00: 6f74 6174 696f 6e2c 206d 6561 7375 7265  otation, measure
+00000b10: 6420 6672 6f6d 206e 6f72 7468 2074 6f20  d from north to 
+00000b20: 6561 7374 2e0a 0a20 2020 2020 2020 2052  east...        R
+00000b30: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00000b40: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2060  ------.        `
+00000b50: 7e69 6d65 7068 752e 616e 6e6f 7461 7469  ~imephu.annotati
+00000b60: 6f6e 2e67 656e 6572 616c 2e43 6972 636c  on.general.Circl
+00000b70: 6541 6e6e 6f74 6174 696f 6e60 0a20 2020  eAnnotation`.   
+00000b80: 2020 2020 2020 2020 2054 6865 2061 6e6e           The ann
+00000b90: 6f74 6174 696f 6e20 7265 7375 6c74 696e  otation resultin
+00000ba0: 6720 6672 6f6d 2074 6865 2072 6f74 6174  g from the rotat
+00000bb0: 696f 6e2e 0a20 2020 2020 2020 2022 2222  ion..        """
+00000bc0: 0a20 2020 2020 2020 2072 6f74 6174 6564  .        rotated
+00000bd0: 5f61 6e6e 6f74 6174 696f 6e20 3d20 6465  _annotation = de
+00000be0: 6570 636f 7079 2873 656c 6629 0a20 2020  epcopy(self).   
+00000bf0: 2020 2020 2072 6f74 6174 6564 5f63 656e       rotated_cen
+00000c00: 7465 7220 3d20 726f 7461 7465 2873 656c  ter = rotate(sel
+00000c10: 662e 5f63 656e 7465 722c 2070 6976 6f74  f._center, pivot
+00000c20: 2c20 616e 676c 652c 2073 656c 662e 5f77  , angle, self._w
+00000c30: 6373 290a 2020 2020 2020 2020 726f 7461  cs).        rota
+00000c40: 7465 645f 616e 6e6f 7461 7469 6f6e 2e5f  ted_annotation._
+00000c50: 6365 6e74 6572 203d 2072 6f74 6174 6564  center = rotated
+00000c60: 5f63 656e 7465 720a 2020 2020 2020 2020  _center.        
+00000c70: 7265 7475 726e 2072 6f74 6174 6564 5f61  return rotated_a
+00000c80: 6e6e 6f74 6174 696f 6e0a 0a20 2020 2064  nnotation..    d
+00000c90: 6566 2074 7261 6e73 6c61 7465 2873 656c  ef translate(sel
+00000ca0: 662c 2064 6973 706c 6163 656d 656e 743a  f, displacement:
+00000cb0: 2041 6e67 6c65 2920 2d3e 2022 4369 7263   Angle) -> "Circ
+00000cc0: 6c65 416e 6e6f 7461 7469 6f6e 223a 0a20  leAnnotation":. 
+00000cd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000ce0: 2020 204d 6f76 6520 7468 6973 2061 6e6e     Move this ann
+00000cf0: 6f74 6174 696f 6e20 616c 6f6e 6720 6120  otation along a 
+00000d00: 6469 7370 6c61 6365 6d65 6e74 2076 6563  displacement vec
+00000d10: 746f 7220 616e 6420 7265 7475 726e 2074  tor and return t
+00000d20: 6865 2072 6573 756c 742e 0a0a 2020 2020  he result...    
+00000d30: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00000d40: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00000d50: 2d0a 2020 2020 2020 2020 6469 7370 6c61  -.        displa
+00000d60: 6365 6d65 6e74 3a20 3244 2061 7272 6179  cement: 2D array
+00000d70: 206f 6620 616e 676c 6573 0a20 2020 2020   of angles.     
+00000d80: 2020 2020 2020 2054 6865 2064 6973 706c         The displ
+00000d90: 6163 656d 656e 7420 6279 2077 6869 6368  acement by which
+00000da0: 2074 6f20 6d6f 7665 2074 6865 2061 6e6e   to move the ann
+00000db0: 6f74 6174 696f 6e2e 0a0a 2020 2020 2020  otation...      
+00000dc0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00000dd0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00000de0: 2020 607e 696d 6570 6875 2e61 6e6e 6f74    `~imephu.annot
+00000df0: 6174 696f 6e2e 6765 6e65 7261 6c2e 4369  ation.general.Ci
+00000e00: 7263 6c65 416e 6e6f 7461 7469 6f6e 600a  rcleAnnotation`.
+00000e10: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00000e20: 616e 6e6f 7461 7469 6f6e 2072 6573 756c  annotation resul
+00000e30: 7469 6e67 2066 726f 6d20 7468 6520 7472  ting from the tr
+00000e40: 616e 736c 6174 696f 6e2e 0a20 2020 2020  anslation..     
+00000e50: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+00000e60: 7261 6e73 6c61 7465 645f 616e 6e6f 7461  ranslated_annota
+00000e70: 7469 6f6e 203d 2064 6565 7063 6f70 7928  tion = deepcopy(
+00000e80: 7365 6c66 290a 2020 2020 2020 2020 7472  self).        tr
+00000e90: 616e 736c 6174 6564 5f63 656e 7465 7220  anslated_center 
+00000ea0: 3d20 7472 616e 736c 6174 6528 7365 6c66  = translate(self
+00000eb0: 2e5f 6365 6e74 6572 2c20 6469 7370 6c61  ._center, displa
+00000ec0: 6365 6d65 6e74 290a 2020 2020 2020 2020  cement).        
+00000ed0: 7472 616e 736c 6174 6564 5f61 6e6e 6f74  translated_annot
+00000ee0: 6174 696f 6e2e 5f63 656e 7465 7220 3d20  ation._center = 
+00000ef0: 7472 616e 736c 6174 6564 5f63 656e 7465  translated_cente
+00000f00: 720a 2020 2020 2020 2020 7265 7475 726e  r.        return
+00000f10: 2074 7261 6e73 6c61 7465 645f 616e 6e6f   translated_anno
+00000f20: 7461 7469 6f6e 0a                        tation.
```

### Comparing `imephu-0.2.0/src/imephu/annotation/general/__pycache__/group.cpython-310.pyc` & `imephu-0.2.1/src/imephu/salt/annotation/rss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,243 +1,242 @@
-00000000: 6f0d 0d0a 0000 0000 927a 0662 cd0b 0000  o........z.b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
-00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
-00000070: 6509 8303 5a0a 6407 5300 2908 e900 0000  e...Z.d.S.).....
-00000080: 0029 02da 044c 6973 74da 0853 6571 7565  .)...List..Seque
-00000090: 6e63 6529 02da 0541 6e67 6c65 da08 536b  nce)...Angle..Sk
-000000a0: 7943 6f6f 7264 2901 da07 5743 5341 7865  yCoord)...WCSAxe
-000000b0: 7329 01da 0a41 6e6e 6f74 6174 696f 6e63  s)...Annotationc
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000d0: 0600 0000 4000 0000 736e 0000 0065 005a  ....@...sn...e.Z
-000000e0: 0164 005a 0264 015a 0364 0265 0465 0519  .d.Z.d.Z.d.e.e..
-000000f0: 0066 0264 0364 0484 045a 0664 0565 0564  .f.d.d...Z.d.e.d
-00000100: 0664 0766 0464 0864 0984 045a 0764 0a65  .d.f.d.d...Z.d.e
-00000110: 0864 0664 0766 0464 0b64 0c84 045a 0964  .d.d.f.d.d...Z.d
-00000120: 0d65 0a64 0e65 0b64 0664 0066 0664 0f64  .e.d.e.d.d.f.d.d
-00000130: 1084 045a 0c64 1165 0b64 0664 0066 0464  ...Z.d.e.d.d.f.d
-00000140: 1264 1384 045a 0d64 0753 0029 14da 0f47  .d...Z.d.S.)...G
-00000150: 726f 7570 416e 6e6f 7461 7469 6f6e 61aa  roupAnnotationa.
-00000160: 0200 000a 2020 2020 416e 2061 6e6e 6f74  ....    An annot
-00000170: 6174 696f 6e20 6d61 6465 206f 6620 6120  ation made of a 
-00000180: 6772 6f75 7020 6f66 2061 6e6e 6f74 6174  group of annotat
-00000190: 696f 6e73 2e0a 0a20 2020 2054 6865 2061  ions...    The a
-000001a0: 6e6e 6f74 6174 696f 6e20 636f 6d70 7269  nnotation compri
-000001b0: 7365 7320 6120 6c69 7374 206f 6620 616e  ses a list of an
-000001c0: 6e6f 7461 7469 6f6e 2069 7465 6d73 2e20  notation items. 
-000001d0: 416e 7920 6f66 2074 6865 0a20 2020 2060  Any of the.    `
-000001e0: 7e69 6d70 6568 752e 616e 6e6f 7461 7469  ~impehu.annotati
-000001f0: 6f6e 2e41 6e6e 6f74 6174 696f 6e60 206d  on.Annotation` m
-00000200: 6574 686f 6473 2061 7265 2061 7070 6c69  ethods are appli
-00000210: 6564 2074 6f20 616c 6c20 7468 6520 6974  ed to all the it
-00000220: 656d 7320 696e 2074 6865 206c 6973 742c  ems in the list,
-00000230: 0a20 2020 2069 6e20 7468 6520 6f72 6465  .    in the orde
-00000240: 7220 7468 6520 6974 656d 7320 6170 7065  r the items appe
-00000250: 6172 2069 6e20 7468 6520 6c69 7374 2e20  ar in the list. 
-00000260: 536f 2c20 666f 7220 6578 616d 706c 652c  So, for example,
-00000270: 2074 6865 2060 6061 7070 6c79 5f74 6f60   the ``apply_to`
-00000280: 6020 6d65 7468 6f64 0a20 2020 2063 616c  ` method.    cal
-00000290: 6c73 2074 6865 2060 6061 7070 6c79 5f74  ls the ``apply_t
-000002a0: 6f60 6020 6d65 7468 6f64 2066 6f72 2061  o`` method for a
-000002b0: 6c6c 206c 6973 7420 6974 656d 732c 2073  ll list items, s
-000002c0: 7461 7274 696e 6720 6672 6f6d 2074 6865  tarting from the
-000002d0: 2066 6972 7374 2069 7465 6d20 696e 0a20   first item in. 
-000002e0: 2020 2074 6865 206c 6973 7420 616e 6420     the list and 
-000002f0: 6669 6e69 7368 696e 6720 7769 7468 2074  finishing with t
-00000300: 6865 206c 6173 7420 6974 656d 2e0a 0a20  he last item... 
-00000310: 2020 2041 6e6e 6f74 6174 696f 6e73 2063     Annotations c
-00000320: 616e 2062 6520 6164 6465 6420 746f 2074  an be added to t
-00000330: 6865 2067 726f 7570 2077 6865 6e20 6361  he group when ca
-00000340: 6c6c 696e 6720 7468 6520 636f 6e73 7472  lling the constr
-00000350: 7563 746f 7220 6f72 2062 7920 7573 696e  uctor or by usin
-00000360: 6720 7468 650a 2020 2020 6060 6164 645f  g the.    ``add_
-00000370: 6974 656d 6060 206d 6574 686f 6420 6166  item`` method af
-00000380: 7465 7277 6172 6473 2e0a 0a20 2020 2050  terwards...    P
-00000390: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000003a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 7465  --------.    ite
-000003b0: 6d73 3a20 7365 7175 656e 6365 206f 6620  ms: sequence of 
-000003c0: 607e 696d 6570 6875 2e61 6e6e 6f74 6174  `~imephu.annotat
-000003d0: 696f 6e2e 416e 6e6f 7461 7469 6f6e 600a  ion.Annotation`.
-000003e0: 2020 2020 2020 2020 5468 6520 696e 6974          The init
-000003f0: 6961 6c20 6c69 7374 206f 6620 6772 6f75  ial list of grou
-00000400: 7020 6974 656d 732e 0a20 2020 20da 0569  p items..    ..i
-00000410: 7465 6d73 6302 0000 0000 0000 0000 0000  temsc...........
-00000420: 0002 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-00000430: 0000 7400 7c01 8301 7c00 5f01 6400 5300  ..t.|...|._.d.S.
-00000440: 2901 4e29 02da 046c 6973 74da 065f 6974  ).N)...list.._it
-00000450: 656d 7329 02da 0473 656c 6672 0900 0000  ems)...selfr....
-00000460: a900 720d 0000 00fa 4b2f 5573 6572 732f  ..r.....K/Users/
-00000470: 6368 7269 7374 6961 6e2f 4964 6561 5072  christian/IdeaPr
-00000480: 6f6a 6563 7473 2f69 6d65 7068 752f 7372  ojects/imephu/sr
-00000490: 632f 696d 6570 6875 2f61 6e6e 6f74 6174  c/imephu/annotat
-000004a0: 696f 6e2f 6765 6e65 7261 6c2f 6772 6f75  ion/general/grou
-000004b0: 702e 7079 da08 5f5f 696e 6974 5f5f 1c00  p.py..__init__..
-000004c0: 0000 7302 0000 000e 017a 1847 726f 7570  ..s......z.Group
-000004d0: 416e 6e6f 7461 7469 6f6e 2e5f 5f69 6e69  Annotation.__ini
-000004e0: 745f 5fda 0469 7465 6dda 0672 6574 7572  t__..item..retur
-000004f0: 6e4e 6302 0000 0000 0000 0000 0000 0002  nNc.............
-00000500: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
-00000510: 7c00 6a00 a001 7c01 a101 0100 6401 5300  |.j...|.....d.S.
-00000520: 2902 7aab 4164 6420 616e 2061 6e6e 6f74  ).z.Add an annot
-00000530: 6174 696f 6e20 746f 2074 6869 7320 6772  ation to this gr
-00000540: 6f75 702e 0a0a 2020 2020 2020 2020 5061  oup...        Pa
-00000550: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00000560: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000570: 2020 2020 6974 656d 3a20 607e 696d 6570      item: `~imep
-00000580: 6875 2e61 6e6e 6f74 6174 696f 6e2e 416e  hu.annotation.An
-00000590: 6e6f 7461 7469 6f6e 600a 2020 2020 2020  notation`.      
-000005a0: 2020 2020 2020 416e 6e6f 7461 7469 6f6e        Annotation
-000005b0: 2074 6f20 6164 6420 746f 2074 6869 7320   to add to this 
-000005c0: 6772 6f75 702e 0a20 2020 2020 2020 204e  group..        N
-000005d0: 2902 720b 0000 00da 0661 7070 656e 6429  ).r......append)
-000005e0: 0272 0c00 0000 7210 0000 0072 0d00 0000  .r....r....r....
-000005f0: 720d 0000 0072 0e00 0000 da08 6164 645f  r....r......add_
-00000600: 6974 656d 1f00 0000 7302 0000 0010 087a  item....s......z
-00000610: 1847 726f 7570 416e 6e6f 7461 7469 6f6e  .GroupAnnotation
-00000620: 2e61 6464 5f69 7465 6dda 0261 7863 0200  .add_item..axc..
-00000630: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000640: 0000 4300 0000 731a 0000 007c 006a 0044  ..C...s....|.j.D
-00000650: 005d 077d 027c 02a0 017c 01a1 0101 0071  .].}.|...|.....q
-00000660: 0364 0153 0029 027a a241 6464 2074 6869  .d.S.).z.Add thi
-00000670: 7320 616e 6e6f 7461 7469 6f6e 2074 6f20  s annotation to 
-00000680: 6120 6669 6e64 6572 2063 6861 7274 2e0a  a finder chart..
-00000690: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000006a0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-000006b0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2061  ------.        a
-000006c0: 783a 2060 7e61 7374 726f 7079 2e76 6973  x: `~astropy.vis
-000006d0: 7561 6c69 7a61 7469 6f6e 2e77 6373 6178  ualization.wcsax
-000006e0: 6573 2e57 4353 4178 6573 600a 2020 2020  es.WCSAxes`.    
-000006f0: 2020 2020 2020 2020 506c 6f74 2061 7865          Plot axe
-00000700: 732e 0a20 2020 2020 2020 204e 2902 720b  s..        N).r.
-00000710: 0000 00da 0661 6464 5f74 6f29 0372 0c00  .....add_to).r..
-00000720: 0000 7214 0000 0072 1000 0000 720d 0000  ..r....r....r...
-00000730: 0072 0d00 0000 720e 0000 0072 1500 0000  .r....r....r....
-00000740: 2900 0000 7306 0000 000a 080c 0104 ff7a  )...s..........z
-00000750: 1647 726f 7570 416e 6e6f 7461 7469 6f6e  .GroupAnnotation
-00000760: 2e61 6464 5f74 6fda 0570 6976 6f74 da05  .add_to..pivot..
-00000770: 616e 676c 6563 0300 0000 0000 0000 0000  anglec..........
-00000780: 0000 0500 0000 0300 0000 0300 0000 7324  ..............s$
-00000790: 0000 0087 0087 0166 0264 0164 0284 087c  .......f.d.d...|
-000007a0: 006a 0044 0083 017d 0374 017c 0364 038d  .j.D...}.t.|.d..
-000007b0: 017d 047c 0453 0029 0561 2402 0000 526f  .}.|.S.).a$...Ro
-000007c0: 7461 7465 2074 6869 7320 616e 6e6f 7461  tate this annota
-000007d0: 7469 6f6e 2061 726f 756e 6420 6120 7069  tion around a pi
-000007e0: 766f 7420 616e 6420 7265 7475 726e 2074  vot and return t
-000007f0: 6865 2072 6573 756c 742e 0a0a 2020 2020  he result...    
-00000800: 2020 2020 5468 6520 726f 7461 7469 6f6e      The rotation
-00000810: 2061 6e67 6c65 2069 7320 616e 2061 6e67   angle is an ang
-00000820: 6c65 206f 6e20 7468 6520 736b 792c 206d  le on the sky, m
-00000830: 6561 7375 7265 6420 6672 6f6d 206e 6f72  easured from nor
-00000840: 7468 2074 6f20 6561 7374 2e0a 0a20 2020  th to east...   
-00000850: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00000860: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00000870: 2d2d 0a20 2020 2020 2020 2070 6976 6f74  --.        pivot
-00000880: 3a20 607e 6173 7472 6f70 792e 636f 6f72  : `~astropy.coor
-00000890: 6469 6e61 7465 732e 536b 7943 6f6f 7264  dinates.SkyCoord
-000008a0: 600a 2020 2020 2020 2020 2020 2020 506f  `.            Po
-000008b0: 696e 7420 6172 6f75 6e64 2077 6869 6368  int around which
-000008c0: 2074 6f20 726f 7461 7465 2074 6865 2061   to rotate the a
-000008d0: 6e6e 6f74 6174 696f 6e2e 0a20 2020 2020  nnotation..     
-000008e0: 2020 2061 6e67 6c65 3a20 607e 6173 7472     angle: `~astr
-000008f0: 6f70 792e 636f 6f72 6469 6e61 7465 732e  opy.coordinates.
-00000900: 416e 676c 6560 0a20 2020 2020 2020 2020  Angle`.         
-00000910: 2020 2041 6e67 6c65 206f 6620 726f 7461     Angle of rota
-00000920: 7469 6f6e 2c20 6d65 6173 7572 6564 2066  tion, measured f
-00000930: 726f 6d20 6e6f 7274 6820 746f 7761 7264  rom north toward
-00000940: 7320 7468 6520 6561 7374 2e0a 0a20 2020  s the east...   
-00000950: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00000960: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00000970: 2020 2020 2060 7e69 6d65 7068 752e 616e       `~imephu.an
-00000980: 6e6f 7461 7469 6f6e 2e67 656e 6572 616c  notation.general
-00000990: 2e47 726f 7570 416e 6e6f 7461 7469 6f6e  .GroupAnnotation
-000009a0: 600a 2020 2020 2020 2020 2020 2020 5468  `.            Th
-000009b0: 6520 616e 6e6f 7461 7469 6f6e 2072 6573  e annotation res
-000009c0: 756c 7469 6e67 2066 726f 6d20 7468 6520  ulting from the 
-000009d0: 726f 7461 7469 6f6e 2e0a 2020 2020 2020  rotation..      
-000009e0: 2020 6301 0000 0000 0000 0000 0000 0002    c.............
-000009f0: 0000 0006 0000 0013 0000 0073 1800 0000  ...........s....
-00000a00: 6700 7c00 5d08 7d01 7c01 a000 8801 8800  g.|.].}.|.......
-00000a10: a102 9102 7102 5300 720d 0000 0029 01da  ....q.S.r....)..
-00000a20: 0672 6f74 6174 65a9 02da 022e 3072 1000  .rotate.....0r..
-00000a30: 0000 a902 7217 0000 0072 1600 0000 720d  ....r....r....r.
-00000a40: 0000 0072 0e00 0000 da0a 3c6c 6973 7463  ...r......<listc
-00000a50: 6f6d 703e 4500 0000 7302 0000 0018 007a  omp>E...s......z
-00000a60: 2a47 726f 7570 416e 6e6f 7461 7469 6f6e  *GroupAnnotation
-00000a70: 2e72 6f74 6174 652e 3c6c 6f63 616c 733e  .rotate.<locals>
-00000a80: 2e3c 6c69 7374 636f 6d70 3e29 0172 0900  .<listcomp>).r..
-00000a90: 0000 4ea9 0272 0b00 0000 7208 0000 0029  ..N..r....r....)
-00000aa0: 0572 0c00 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000ab0: 5a0d 726f 7461 7465 645f 6974 656d 73da  Z.rotated_items.
-00000ac0: 1272 6f74 6174 6564 5f61 6e6e 6f74 6174  .rotated_annotat
-00000ad0: 696f 6e72 0d00 0000 721b 0000 0072 0e00  ionr....r....r..
-00000ae0: 0000 7218 0000 0034 0000 0073 0600 0000  ..r....4...s....
-00000af0: 1611 0a01 0401 7a16 4772 6f75 7041 6e6e  ......z.GroupAnn
-00000b00: 6f74 6174 696f 6e2e 726f 7461 7465 da0c  otation.rotate..
-00000b10: 6469 7370 6c61 6365 6d65 6e74 6302 0000  displacementc...
-00000b20: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-00000b30: 0003 0000 0073 2000 0000 8700 6601 6401  .....s .....f.d.
-00000b40: 6402 8408 7c00 6a00 4400 8301 7d02 7401  d...|.j.D...}.t.
-00000b50: 7c02 8301 7d03 7c03 5300 2904 6178 0100  |...}.|.S.).ax..
-00000b60: 000a 2020 2020 2020 2020 4d6f 7665 2074  ..        Move t
-00000b70: 6869 7320 616e 6e6f 7461 7469 6f6e 2061  his annotation a
-00000b80: 6c6f 6e67 2061 2064 6973 706c 6163 656d  long a displacem
-00000b90: 656e 7420 7665 6374 6f72 2061 6e64 2072  ent vector and r
-00000ba0: 6574 7572 6e20 7468 6520 7265 7375 6c74  eturn the result
-00000bb0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00000bc0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00000bd0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00000be0: 2064 6973 706c 6163 656d 656e 743a 2032   displacement: 2
-00000bf0: 4420 6172 7261 7920 6f66 2061 6e67 6c65  D array of angle
-00000c00: 730a 2020 2020 2020 2020 2020 2020 5468  s.            Th
-00000c10: 6520 6469 7370 6c61 6365 6d65 6e74 2062  e displacement b
-00000c20: 7920 7768 6963 6820 746f 206d 6f76 6520  y which to move 
-00000c30: 7468 6520 616e 6e6f 7461 7469 6f6e 2e0a  the annotation..
-00000c40: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00000c50: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00000c60: 0a20 2020 2020 2020 2060 7e69 6d65 7068  .        `~imeph
-00000c70: 752e 616e 6e6f 7461 7469 6f6e 2e67 656e  u.annotation.gen
-00000c80: 6572 616c 2e47 726f 7570 416e 6e6f 7461  eral.GroupAnnota
-00000c90: 7469 6f6e 600a 2020 2020 2020 2020 2020  tion`.          
-00000ca0: 2020 5468 6520 616e 6e6f 7461 7469 6f6e    The annotation
-00000cb0: 2072 6573 756c 7469 6e67 2066 726f 6d20   resulting from 
-00000cc0: 7468 6520 7472 616e 736c 6174 696f 6e2e  the translation.
-00000cd0: 0a20 2020 2020 2020 2063 0100 0000 0000  .        c......
-00000ce0: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-00000cf0: 0000 7316 0000 0067 007c 005d 077d 017c  ..s....g.|.].}.|
-00000d00: 01a0 0088 00a1 0191 0271 0253 0072 0d00  .........q.S.r..
-00000d10: 0000 2901 da09 7472 616e 736c 6174 6572  ..)...translater
-00000d20: 1900 0000 a901 721f 0000 0072 0d00 0000  ......r....r....
-00000d30: 720e 0000 0072 1c00 0000 5700 0000 7302  r....r....W...s.
-00000d40: 0000 0016 007a 2d47 726f 7570 416e 6e6f  .....z-GroupAnno
-00000d50: 7461 7469 6f6e 2e74 7261 6e73 6c61 7465  tation.translate
-00000d60: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000d70: 6f6d 703e 4e72 1d00 0000 2904 720c 0000  omp>Nr....).r...
-00000d80: 0072 1f00 0000 5a10 7472 616e 736c 6174  .r....Z.translat
-00000d90: 6564 5f69 7465 6d73 da15 7472 616e 736c  ed_items..transl
-00000da0: 6174 6564 5f61 6e6e 6f74 6174 696f 6e72  ated_annotationr
-00000db0: 0d00 0000 7221 0000 0072 0e00 0000 7220  ....r!...r....r 
-00000dc0: 0000 0049 0000 0073 0600 0000 140e 0801  ...I...s........
-00000dd0: 0401 7a19 4772 6f75 7041 6e6e 6f74 6174  ..z.GroupAnnotat
-00000de0: 696f 6e2e 7472 616e 736c 6174 6529 0eda  ion.translate)..
-00000df0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000e00: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000e10: 655f 5fda 075f 5f64 6f63 5f5f 7203 0000  e__..__doc__r...
-00000e20: 0072 0700 0000 720f 0000 0072 1300 0000  .r....r....r....
-00000e30: 7206 0000 0072 1500 0000 7205 0000 0072  r....r....r....r
-00000e40: 0400 0000 7218 0000 0072 2000 0000 720d  ....r....r ...r.
-00000e50: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000e60: 0000 7208 0000 0009 0000 0073 0e00 0000  ..r........s....
-00000e70: 0800 0401 1212 1203 120a 160b 1615 7208  ..............r.
-00000e80: 0000 004e 290b da06 7479 7069 6e67 7202  ...N)...typingr.
-00000e90: 0000 0072 0300 0000 da13 6173 7472 6f70  ...r......astrop
-00000ea0: 792e 636f 6f72 6469 6e61 7465 7372 0400  y.coordinatesr..
-00000eb0: 0000 7205 0000 00da 1d61 7374 726f 7079  ..r......astropy
-00000ec0: 2e76 6973 7561 6c69 7a61 7469 6f6e 2e77  .visualization.w
-00000ed0: 6373 6178 6573 7206 0000 005a 1169 6d65  csaxesr....Z.ime
-00000ee0: 7068 752e 616e 6e6f 7461 7469 6f6e 7207  phu.annotationr.
-00000ef0: 0000 0072 0800 0000 720d 0000 0072 0d00  ...r....r....r..
-00000f00: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
-00000f10: 6f64 756c 653e 0100 0000 730a 0000 0010  odule>....s.....
-00000f20: 0010 020c 010c 0214 03                   .........
+00000000: 6672 6f6d 2061 7374 726f 7079 2069 6d70  from astropy imp
+00000010: 6f72 7420 756e 6974 7320 6173 2075 0a66  ort units as u.f
+00000020: 726f 6d20 6173 7472 6f70 792e 636f 6f72  rom astropy.coor
+00000030: 6469 6e61 7465 7320 696d 706f 7274 2041  dinates import A
+00000040: 6e67 6c65 2c20 536b 7943 6f6f 7264 0a66  ngle, SkyCoord.f
+00000050: 726f 6d20 6173 7472 6f70 792e 7763 7320  rom astropy.wcs 
+00000060: 696d 706f 7274 2057 4353 0a66 726f 6d20  import WCS.from 
+00000070: 696d 6570 6875 2e61 6e6e 6f74 6174 696f  imephu.annotatio
+00000080: 6e2e 6765 6e65 7261 6c20 696d 706f 7274  n.general import
+00000090: 2028 0a20 2020 2043 6972 636c 6541 6e6e   (.    CircleAnn
+000000a0: 6f74 6174 696f 6e2c 0a20 2020 2047 726f  otation,.    Gro
+000000b0: 7570 416e 6e6f 7461 7469 6f6e 2c0a 2020  upAnnotation,.  
+000000c0: 2020 5265 6374 616e 676c 6541 6e6e 6f74    RectangleAnnot
+000000d0: 6174 696f 6e2c 0a20 2020 2054 6578 7441  ation,.    TextA
+000000e0: 6e6e 6f74 6174 696f 6e2c 0a29 0a66 726f  nnotation,.).fro
+000000f0: 6d20 696d 6570 6875 2e67 656f 6d65 7472  m imephu.geometr
+00000100: 7920 696d 706f 7274 2074 7261 6e73 6c61  y import transla
+00000110: 7465 0a66 726f 6d20 696d 6570 6875 2e73  te.from imephu.s
+00000120: 616c 742e 7574 696c 7320 696d 706f 7274  alt.utils import
+00000130: 204d 6f73 4d61 736b 0a0a 0a64 6566 2066   MosMask...def f
+00000140: 6965 6c64 5f6f 665f 7669 6577 5f61 6e6e  ield_of_view_ann
+00000150: 6f74 6174 696f 6e28 6669 7473 5f63 656e  otation(fits_cen
+00000160: 7465 723a 2053 6b79 436f 6f72 642c 2077  ter: SkyCoord, w
+00000170: 6373 3a20 5743 5329 202d 3e20 4772 6f75  cs: WCS) -> Grou
+00000180: 7041 6e6e 6f74 6174 696f 6e3a 0a20 2020  pAnnotation:.   
+00000190: 2022 2222 0a20 2020 2052 6574 7572 6e20   """.    Return 
+000001a0: 616e 2061 6e6e 6f74 6174 696f 6e20 7769  an annotation wi
+000001b0: 7468 2074 6865 2052 5353 2066 6965 6c64  th the RSS field
+000001c0: 206f 6620 7669 6577 2e0a 0a20 2020 2050   of view...    P
+000001d0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+000001e0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 6974  --------.    fit
+000001f0: 735f 6365 6e74 6572 3a20 607e 6173 7472  s_center: `~astr
+00000200: 6f70 792e 636f 6f72 6469 6e61 7465 732e  opy.coordinates.
+00000210: 536b 7943 6f6f 7264 600a 2020 2020 2020  SkyCoord`.      
+00000220: 2020 5468 6520 6365 6e74 6572 206f 6620    The center of 
+00000230: 7468 6520 6669 6e64 6572 2063 6861 7274  the finder chart
+00000240: 2c20 696e 2072 6967 6874 2061 7363 656e  , in right ascen
+00000250: 7369 6f6e 2061 6e64 2064 6563 6c69 6e61  sion and declina
+00000260: 7469 6f6e 2e0a 2020 2020 7763 733a 2060  tion..    wcs: `
+00000270: 7e61 7374 726f 7079 2e77 6373 2e57 4353  ~astropy.wcs.WCS
+00000280: 600a 2020 2020 2020 2020 5743 5320 6f62  `.        WCS ob
+00000290: 6a65 6374 2e0a 0a20 2020 2052 6574 7572  ject...    Retur
+000002a0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+000002b0: 2020 2060 7e69 6d65 7068 752e 616e 6e6f     `~imephu.anno
+000002c0: 7461 7469 6f6e 2e67 656e 6572 616c 2e47  tation.general.G
+000002d0: 726f 7570 416e 6e6f 7461 7469 6f6e 600a  roupAnnotation`.
+000002e0: 2020 2020 2020 2020 416e 2061 6e6e 6f74          An annot
+000002f0: 6174 696f 6e20 7769 7468 2074 6865 2052  ation with the R
+00000300: 5353 2066 6965 6c64 206f 6620 7669 6577  SS field of view
+00000310: 2e0a 2020 2020 2222 220a 2020 2020 666f  ..    """.    fo
+00000320: 765f 616e 6e6f 7461 7469 6f6e 203d 2043  v_annotation = C
+00000330: 6972 636c 6541 6e6e 6f74 6174 696f 6e28  ircleAnnotation(
+00000340: 0a20 2020 2020 2020 2066 6974 735f 6365  .        fits_ce
+00000350: 6e74 6572 2c20 3420 2a20 752e 6172 636d  nter, 4 * u.arcm
+00000360: 696e 2c20 7763 733d 7763 732c 2065 6467  in, wcs=wcs, edg
+00000370: 6563 6f6c 6f72 3d22 6772 6565 6e22 0a20  ecolor="green". 
+00000380: 2020 2029 0a20 2020 206c 6162 656c 5f70     ).    label_p
+00000390: 6f73 6974 696f 6e20 3d20 7472 616e 736c  osition = transl
+000003a0: 6174 6528 6669 7473 5f63 656e 7465 722c  ate(fits_center,
+000003b0: 2028 2d32 2e39 2c20 322e 3929 202a 2075   (-2.9, 2.9) * u
+000003c0: 2e61 7263 6d69 6e29 0a20 2020 206e 616d  .arcmin).    nam
+000003d0: 655f 616e 6e6f 7461 7469 6f6e 203d 2054  e_annotation = T
+000003e0: 6578 7441 6e6e 6f74 6174 696f 6e28 0a20  extAnnotation(. 
+000003f0: 2020 2020 2020 206c 6162 656c 5f70 6f73         label_pos
+00000400: 6974 696f 6e2c 0a20 2020 2020 2020 2022  ition,.        "
+00000410: 5253 5322 2c0a 2020 2020 2020 2020 7763  RSS",.        wc
+00000420: 733d 7763 732c 0a20 2020 2020 2020 2073  s=wcs,.        s
+00000430: 7479 6c65 3d22 6974 616c 6963 222c 0a20  tyle="italic",. 
+00000440: 2020 2020 2020 2077 6569 6768 743d 2262         weight="b
+00000450: 6f6c 6422 2c0a 2020 2020 2020 2020 7369  old",.        si
+00000460: 7a65 3d22 6c61 7267 6522 2c0a 2020 2020  ze="large",.    
+00000470: 2020 2020 686f 7269 7a6f 6e74 616c 616c      horizontalal
+00000480: 6967 6e6d 656e 743d 226c 6566 7422 2c0a  ignment="left",.
+00000490: 2020 2020 2020 2020 636f 6c6f 723d 2830          color=(0
+000004a0: 2c20 302c 2031 292c 0a20 2020 2029 0a20  , 0, 1),.    ). 
+000004b0: 2020 2072 6574 7572 6e20 4772 6f75 7041     return GroupA
+000004c0: 6e6e 6f74 6174 696f 6e28 5b66 6f76 5f61  nnotation([fov_a
+000004d0: 6e6e 6f74 6174 696f 6e2c 206e 616d 655f  nnotation, name_
+000004e0: 616e 6e6f 7461 7469 6f6e 5d29 0a0a 0a64  annotation])...d
+000004f0: 6566 206c 6f6e 6773 6c69 745f 616e 6e6f  ef longslit_anno
+00000500: 7461 7469 6f6e 280a 2020 2020 6669 7473  tation(.    fits
+00000510: 5f63 656e 7465 723a 2053 6b79 436f 6f72  _center: SkyCoor
+00000520: 642c 0a20 2020 2073 6c69 745f 7769 6474  d,.    slit_widt
+00000530: 683a 2041 6e67 6c65 2c0a 2020 2020 736c  h: Angle,.    sl
+00000540: 6974 5f68 6569 6768 743a 2041 6e67 6c65  it_height: Angle
+00000550: 2c0a 2020 2020 706f 7369 7469 6f6e 5f61  ,.    position_a
+00000560: 6e67 6c65 3a20 416e 676c 652c 0a20 2020  ngle: Angle,.   
+00000570: 2077 6373 3a20 5743 532c 0a29 202d 3e20   wcs: WCS,.) -> 
+00000580: 5265 6374 616e 676c 6541 6e6e 6f74 6174  RectangleAnnotat
+00000590: 696f 6e3a 0a20 2020 2022 2222 5265 7475  ion:.    """Retu
+000005a0: 726e 2061 6e20 616e 6e6f 7461 7469 6f6e  rn an annotation
+000005b0: 2073 686f 7769 6e67 2061 206c 6f6e 6773   showing a longs
+000005c0: 6c69 742e 0a0a 2020 2020 5061 7261 6d65  lit...    Parame
+000005d0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+000005e0: 2d2d 2d0a 2020 2020 6669 7473 5f63 656e  ---.    fits_cen
+000005f0: 7465 723a 2060 7e61 7374 726f 7079 2e63  ter: `~astropy.c
+00000600: 6f6f 7264 696e 6174 6573 2e53 6b79 436f  oordinates.SkyCo
+00000610: 6f72 6460 0a20 2020 2020 2020 2054 6865  ord`.        The
+00000620: 2063 656e 7472 616c 2070 6f73 6974 696f   central positio
+00000630: 6e20 6f66 2074 6865 2066 696e 6465 7220  n of the finder 
+00000640: 6368 6172 742c 2069 6e20 7269 6768 7420  chart, in right 
+00000650: 6173 6365 6e73 696f 6e20 616e 6420 6465  ascension and de
+00000660: 636c 696e 6174 696f 6e0a 2020 2020 736c  clination.    sl
+00000670: 6974 5f77 6964 7468 3a20 607e 6173 7472  it_width: `~astr
+00000680: 6f70 792e 636f 6f72 6469 6e61 7465 732e  opy.coordinates.
+00000690: 416e 676c 6560 0a20 2020 2020 2020 2054  Angle`.        T
+000006a0: 6865 2077 6964 7468 206f 6620 7468 6520  he width of the 
+000006b0: 736c 6974 2c20 6173 2061 6e20 616e 676c  slit, as an angl
+000006c0: 6520 6f6e 2074 6865 2073 6b79 2e0a 2020  e on the sky..  
+000006d0: 2020 736c 6974 5f68 6569 6768 743a 2060    slit_height: `
+000006e0: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
+000006f0: 6174 6573 2e41 6e67 6c65 600a 2020 2020  ates.Angle`.    
+00000700: 2020 2020 5468 6520 6865 6967 6874 206f      The height o
+00000710: 6620 7468 6520 736c 6974 2c20 6173 2061  f the slit, as a
+00000720: 6e20 616e 676c 6520 6f6e 2074 6865 2073  n angle on the s
+00000730: 6b79 2e0a 2020 2020 706f 7369 7469 6f6e  ky..    position
+00000740: 5f61 6e67 6c65 3a20 607e 6173 7472 6f70  _angle: `~astrop
+00000750: 792e 636f 6f72 6469 6e61 7465 732e 416e  y.coordinates.An
+00000760: 676c 6560 0a20 2020 2020 2020 2054 6865  gle`.        The
+00000770: 2070 6f73 6974 696f 6e20 616e 676c 652c   position angle,
+00000780: 2061 7320 616e 2061 6e67 6c65 206f 6e20   as an angle on 
+00000790: 7468 6520 736b 7920 6d65 6173 7572 6564  the sky measured
+000007a0: 2066 726f 6d20 6e6f 7274 6820 746f 2065   from north to e
+000007b0: 6173 742e 0a20 2020 2077 6373 3a20 607e  ast..    wcs: `~
+000007c0: 6173 7472 6f70 792e 7763 732e 5743 5360  astropy.wcs.WCS`
+000007d0: 0a20 2020 2020 2020 2057 4353 206f 626a  .        WCS obj
+000007e0: 6563 742e 0a0a 2020 2020 5265 7475 726e  ect...    Return
+000007f0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00000800: 2020 6069 6d65 7068 752e 616e 6e6f 7461    `imephu.annota
+00000810: 7469 6f6e 2e67 656e 6572 616c 2e52 6563  tion.general.Rec
+00000820: 7461 6e67 6c65 416e 6e6f 7461 7469 6f6e  tangleAnnotation
+00000830: 600a 2020 2020 2020 2020 5468 6520 616e  `.        The an
+00000840: 6e6f 7461 7469 6f6e 2073 686f 7769 6e67  notation showing
+00000850: 2074 6865 206c 6f6e 6773 6c69 742e 0a20   the longslit.. 
+00000860: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
+00000870: 6e20 5265 6374 616e 676c 6541 6e6e 6f74  n RectangleAnnot
+00000880: 6174 696f 6e28 0a20 2020 2020 2020 2066  ation(.        f
+00000890: 6974 735f 6365 6e74 6572 2c20 736c 6974  its_center, slit
+000008a0: 5f77 6964 7468 2c20 736c 6974 5f68 6569  _width, slit_hei
+000008b0: 6768 742c 2077 6373 3d77 6373 2c20 6564  ght, wcs=wcs, ed
+000008c0: 6765 636f 6c6f 723d 2272 6564 222c 2061  gecolor="red", a
+000008d0: 6c70 6861 3d30 2e35 0a20 2020 2029 2e72  lpha=0.5.    ).r
+000008e0: 6f74 6174 6528 6669 7473 5f63 656e 7465  otate(fits_cente
+000008f0: 722c 2070 6f73 6974 696f 6e5f 616e 676c  r, position_angl
+00000900: 6529 0a0a 0a64 6566 206d 6f73 5f6d 6173  e)...def mos_mas
+00000910: 6b5f 616e 6e6f 7461 7469 6f6e 280a 2020  k_annotation(.  
+00000920: 2020 6d6f 735f 6d61 736b 3a20 4d6f 734d    mos_mask: MosM
+00000930: 6173 6b2c 2077 6373 3a20 5743 532c 2072  ask, wcs: WCS, r
+00000940: 6566 6572 656e 6365 5f73 7461 725f 626f  eference_star_bo
+00000950: 785f 7769 6474 683a 2041 6e67 6c65 203d  x_width: Angle =
+00000960: 2035 202a 2075 2e61 7263 7365 630a 2920   5 * u.arcsec.) 
+00000970: 2d3e 2047 726f 7570 416e 6e6f 7461 7469  -> GroupAnnotati
+00000980: 6f6e 3a0a 2020 2020 2222 2252 6574 7572  on:.    """Retur
+00000990: 6e20 7468 6520 616e 6e6f 7461 7469 6f6e  n the annotation
+000009a0: 2066 6f72 2061 204d 4f53 206d 6173 6b2e   for a MOS mask.
+000009b0: 0a0a 2020 2020 5468 6520 736c 6974 7320  ..    The slits 
+000009c0: 616e 6420 626f 7865 7320 6172 6f75 6e64  and boxes around
+000009d0: 2074 6865 2072 6566 6572 656e 6365 2073   the reference s
+000009e0: 7461 7273 2061 7265 2069 6e63 6c75 6465  tars are include
+000009f0: 6420 696e 2074 6865 2061 6e6e 6f74 6174  d in the annotat
+00000a00: 696f 6e2e 0a0a 2020 2020 5061 7261 6d65  ion...    Parame
+00000a10: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00000a20: 2d2d 2d0a 2020 2020 6d6f 735f 6d61 736b  ---.    mos_mask
+00000a30: 3a20 607e 696d 6570 6875 2e73 616c 742e  : `~imephu.salt.
+00000a40: 7574 696c 2e4d 6f73 4d61 736b 600a 2020  util.MosMask`.  
+00000a50: 2020 2020 2020 5468 6520 4d4f 5320 6d61        The MOS ma
+00000a60: 736b 2e0a 2020 2020 7763 733a 2060 7e61  sk..    wcs: `~a
+00000a70: 7374 726f 7079 2e77 6373 2e57 4353 600a  stropy.wcs.WCS`.
+00000a80: 2020 2020 2020 2020 5743 5320 6f62 6a65          WCS obje
+00000a90: 6374 2e0a 2020 2020 7265 6665 7265 6e63  ct..    referenc
+00000aa0: 655f 7374 6172 5f62 6f78 5f77 6964 7468  e_star_box_width
+00000ab0: 3a20 607e 6173 7472 6f70 792e 636f 6f72  : `~astropy.coor
+00000ac0: 6469 6e61 7465 732e 416e 676c 6560 2c20  dinates.Angle`, 
+00000ad0: 6465 6661 756c 743a 2035 2061 7263 7365  default: 5 arcse
+00000ae0: 636f 6e64 730a 2020 2020 2020 2020 5468  conds.        Th
+00000af0: 6520 7769 6474 6820 2861 6e64 2068 6569  e width (and hei
+00000b00: 6768 7429 206f 6620 7468 6520 626f 7865  ght) of the boxe
+00000b10: 7320 6172 6f75 6e64 2072 6566 6572 656e  s around referen
+00000b20: 6365 2073 7461 7273 2c20 6173 2061 6e20  ce stars, as an 
+00000b30: 616e 676c 6520 6f6e 2074 6865 0a20 2020  angle on the.   
+00000b40: 2020 2020 2073 6b79 2e0a 0a20 2020 2052       sky...    R
+00000b50: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00000b60: 2d2d 0a20 2020 2060 7e69 6d65 7068 752e  --.    `~imephu.
+00000b70: 616e 6e6f 7461 7469 6f6e 2e67 656e 6572  annotation.gener
+00000b80: 616c 2e47 726f 7570 416e 6e6f 7461 7469  al.GroupAnnotati
+00000b90: 6f6e 600a 2020 2020 2020 2020 5468 6520  on`.        The 
+00000ba0: 616e 6e6f 7461 7469 6f6e 2064 6973 706c  annotation displ
+00000bb0: 6179 696e 6720 7468 6520 4d4f 5320 6d61  aying the MOS ma
+00000bc0: 736b 2e0a 2020 2020 2222 220a 2020 2020  sk..    """.    
+00000bd0: 6d61 736b 5f61 6e6e 6f74 6174 696f 6e20  mask_annotation 
+00000be0: 3d20 4772 6f75 7041 6e6e 6f74 6174 696f  = GroupAnnotatio
+00000bf0: 6e28 5b5d 290a 0a20 2020 2070 6f73 6974  n([])..    posit
+00000c00: 696f 6e5f 616e 676c 6520 3d20 6d6f 735f  ion_angle = mos_
+00000c10: 6d61 736b 2e70 6f73 6974 696f 6e5f 616e  mask.position_an
+00000c20: 676c 650a 2020 2020 666f 7220 7374 6172  gle.    for star
+00000c30: 2069 6e20 6d6f 735f 6d61 736b 2e72 6566   in mos_mask.ref
+00000c40: 6572 656e 6365 5f73 7461 7273 3a0a 2020  erence_stars:.  
+00000c50: 2020 2020 2020 7265 6665 7265 6e63 655f        reference_
+00000c60: 7374 6172 5f61 6e6e 6f74 6174 696f 6e20  star_annotation 
+00000c70: 3d20 5265 6374 616e 676c 6541 6e6e 6f74  = RectangleAnnot
+00000c80: 6174 696f 6e28 0a20 2020 2020 2020 2020  ation(.         
+00000c90: 2020 2063 656e 7465 723d 7374 6172 2c0a     center=star,.
+00000ca0: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+00000cb0: 683d 7265 6665 7265 6e63 655f 7374 6172  h=reference_star
+00000cc0: 5f62 6f78 5f77 6964 7468 2c0a 2020 2020  _box_width,.    
+00000cd0: 2020 2020 2020 2020 6865 6967 6874 3d72          height=r
+00000ce0: 6566 6572 656e 6365 5f73 7461 725f 626f  eference_star_bo
+00000cf0: 785f 7769 6474 682c 0a20 2020 2020 2020  x_width,.       
+00000d00: 2020 2020 2077 6373 3d77 6373 2c0a 2020       wcs=wcs,.  
+00000d10: 2020 2020 2020 2020 2020 6564 6765 636f            edgeco
+00000d20: 6c6f 723d 2831 2c20 312c 2030 292c 0a20  lor=(1, 1, 0),. 
+00000d30: 2020 2020 2020 2020 2020 206c 696e 6577             linew
+00000d40: 6964 7468 3d32 2c0a 2020 2020 2020 2020  idth=2,.        
+00000d50: 292e 726f 7461 7465 2873 7461 722c 2070  ).rotate(star, p
+00000d60: 6f73 6974 696f 6e5f 616e 676c 6529 0a20  osition_angle). 
+00000d70: 2020 2020 2020 206d 6173 6b5f 616e 6e6f         mask_anno
+00000d80: 7461 7469 6f6e 2e61 6464 5f69 7465 6d28  tation.add_item(
+00000d90: 7265 6665 7265 6e63 655f 7374 6172 5f61  reference_star_a
+00000da0: 6e6e 6f74 6174 696f 6e29 0a0a 2020 2020  nnotation)..    
+00000db0: 666f 7220 736c 6974 2069 6e20 6d6f 735f  for slit in mos_
+00000dc0: 6d61 736b 2e73 6c69 7473 3a0a 2020 2020  mask.slits:.    
+00000dd0: 2020 2020 736c 6974 5f61 6e6e 6f74 6174      slit_annotat
+00000de0: 696f 6e20 3d20 5265 6374 616e 676c 6541  ion = RectangleA
+00000df0: 6e6e 6f74 6174 696f 6e28 0a20 2020 2020  nnotation(.     
+00000e00: 2020 2020 2020 2063 656e 7465 723d 736c         center=sl
+00000e10: 6974 2e63 656e 7465 722c 0a20 2020 2020  it.center,.     
+00000e20: 2020 2020 2020 2077 6964 7468 3d73 6c69         width=sli
+00000e30: 742e 7769 6474 682c 0a20 2020 2020 2020  t.width,.       
+00000e40: 2020 2020 2068 6569 6768 743d 736c 6974       height=slit
+00000e50: 2e68 6569 6768 742c 0a20 2020 2020 2020  .height,.       
+00000e60: 2020 2020 2077 6373 3d77 6373 2c0a 2020       wcs=wcs,.  
+00000e70: 2020 2020 2020 2020 2020 6564 6765 636f            edgeco
+00000e80: 6c6f 723d 2272 6564 222c 0a20 2020 2020  lor="red",.     
+00000e90: 2020 2029 2e72 6f74 6174 6528 736c 6974     ).rotate(slit
+00000ea0: 2e63 656e 7465 722c 2070 6f73 6974 696f  .center, positio
+00000eb0: 6e5f 616e 676c 6520 2b20 736c 6974 2e74  n_angle + slit.t
+00000ec0: 696c 7429 0a20 2020 2020 2020 206d 6173  ilt).        mas
+00000ed0: 6b5f 616e 6e6f 7461 7469 6f6e 2e61 6464  k_annotation.add
+00000ee0: 5f69 7465 6d28 736c 6974 5f61 6e6e 6f74  _item(slit_annot
+00000ef0: 6174 696f 6e29 0a0a 2020 2020 7265 7475  ation)..    retu
+00000f00: 726e 206d 6173 6b5f 616e 6e6f 7461 7469  rn mask_annotati
+00000f10: 6f6e 0a                                  on.
```

### Comparing `imephu-0.2.0/src/imephu/annotation/general/__pycache__/line_path.cpython-310.pyc` & `imephu-0.2.1/src/imephu/annotation/general/rectangle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,313 +1,277 @@
-00000000: 6f0d 0d0a 0000 0000 6573 c762 4c11 0000  o.......es.bL...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
-00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 0100 6400 6407 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
-00000090: 0100 6400 6408 6c12 6d13 5a13 0100 6400  ..d.d.l.m.Z...d.
-000000a0: 6409 6c14 6d15 5a15 6d16 5a16 6d17 5a17  d.l.m.Z.m.Z.m.Z.
-000000b0: 0100 4700 640a 640b 8400 640b 6513 8303  ..G.d.d...d.e...
-000000c0: 5a18 640c 5300 290d e900 0000 0029 01da  Z.d.S.)......)..
-000000d0: 0864 6565 7063 6f70 7929 04da 0341 6e79  .deepcopy)...Any
-000000e0: da08 5365 7175 656e 6365 da05 5475 706c  ..Sequence..Tupl
-000000f0: 65da 0555 6e69 6f6e 2902 da05 416e 676c  e..Union)...Angl
-00000100: 65da 0853 6b79 436f 6f72 6429 01da 0757  e..SkyCoord)...W
-00000110: 4353 4178 6573 2901 da03 5743 5329 01da  CSAxes)...WCS)..
-00000120: 0950 6174 6850 6174 6368 2901 da04 5061  .PathPatch)...Pa
-00000130: 7468 2901 da0a 416e 6e6f 7461 7469 6f6e  th)...Annotation
-00000140: 2903 da06 726f 7461 7465 da15 736b 795f  )...rotate..sky_
-00000150: 706f 7369 7469 6f6e 5f74 6f5f 7069 7865  position_to_pixe
-00000160: 6cda 0974 7261 6e73 6c61 7465 6300 0000  l..translatec...
-00000170: 0000 0000 0000 0000 0000 0000 0010 0000  ................
-00000180: 0040 0000 0073 9c00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000190: 5a02 6401 5a03 0902 0903 0904 6419 6405  Z.d.Z.......d.d.
-000001a0: 6504 6505 1900 6406 6506 6407 6507 6408  e.e...d.e.d.e.d.
-000001b0: 6508 6509 650a 650b 650b 650b 6603 1900  e.e.e.e.e.e.f...
-000001c0: 6602 1900 6409 6508 6509 650a 650b 650b  f...d.e.e.e.e.e.
-000001d0: 650b 6603 1900 6602 1900 640a 650c 660c  e.f...f...d.e.f.
-000001e0: 640b 640c 8405 5a0d 640d 650e 640e 640f  d.d...Z.d.e.d.d.
-000001f0: 6604 6410 6411 8404 5a0f 6412 6505 6413  f.d.d...Z.d.e.d.
-00000200: 6510 640e 6400 6606 6414 6415 8404 5a11  e.d.d.f.d.d...Z.
-00000210: 6416 6510 640e 6400 6604 6417 6418 8404  d.e.d.d.f.d.d...
-00000220: 5a12 640f 5300 291a da12 4c69 6e65 5061  Z.d.S.)...LinePa
-00000230: 7468 416e 6e6f 7461 7469 6f6e 6179 0400  thAnnotationay..
-00000240: 0041 6e20 616e 6e6f 7461 7469 6f6e 2063  .An annotation c
-00000250: 6f6e 7369 7374 696e 6720 6f66 2073 7472  onsisting of str
-00000260: 6169 6768 7420 6c69 6e65 7320 6265 7477  aight lines betw
-00000270: 6565 6e20 7665 7274 6963 6573 2e0a 0a20  een vertices... 
-00000280: 2020 2054 6865 2070 6174 6820 6469 7370     The path disp
-00000290: 6c61 7965 6420 6279 2074 6869 7320 616e  layed by this an
-000002a0: 6e6f 7461 7469 6f6e 2069 7320 6465 6669  notation is defi
-000002b0: 6e65 6420 6279 2061 2073 6574 206f 6620  ned by a set of 
-000002c0: 7665 7274 6963 6573 2c20 7768 6963 6820  vertices, which 
-000002d0: 6172 650a 2020 2020 636f 6e6e 6563 7465  are.    connecte
-000002e0: 6420 6279 2073 7472 6169 6768 7420 6c69  d by straight li
-000002f0: 6e65 7320 6f6e 2074 6865 2066 696e 6465  nes on the finde
-00000300: 7220 6368 6172 742e 2028 5468 6520 636f  r chart. (The co
-00000310: 6e6e 6563 7469 6e67 206c 696e 6573 2069  nnecting lines i
-00000320: 6e20 6765 6e65 7261 6c0a 2020 2020 7769  n general.    wi
-00000330: 6c6c 2072 6566 6572 2074 6f20 6375 7276  ll refer to curv
-00000340: 6564 206c 696e 6573 206f 6e20 7468 6520  ed lines on the 
-00000350: 736b 792e 290a 0a20 2020 2042 7920 6465  sky.)..    By de
-00000360: 6661 756c 7420 7468 6520 7061 7468 2069  fault the path i
-00000370: 7320 6173 7375 6d65 6420 746f 2062 6520  s assumed to be 
-00000380: 636c 6f73 6564 2c20 692e 652e 2074 6865  closed, i.e. the
-00000390: 206c 6173 7420 7665 7274 6578 2069 7320   last vertex is 
-000003a0: 636f 6e6e 6563 7465 6420 746f 0a20 2020  connected to.   
-000003b0: 2074 6865 2066 6972 7374 2062 7920 6120   the first by a 
-000003c0: 6c69 6e65 2e20 5468 6973 2062 6568 6176  line. This behav
-000003d0: 696f 7220 6d61 7920 6265 2063 6861 6e67  ior may be chang
-000003e0: 6564 2077 6974 6820 7468 6520 6060 636c  ed with the ``cl
-000003f0: 6f73 6564 6060 2070 6172 616d 6574 6572  osed`` parameter
-00000400: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00000410: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00000420: 0a20 2020 2076 6572 7469 6365 733a 2073  .    vertices: s
-00000430: 6571 7565 6e63 6520 6f66 2060 7e61 7374  equence of `~ast
-00000440: 726f 7079 2e63 6f6f 7264 696e 6174 6573  ropy.coordinates
-00000450: 2e53 6b79 436f 6f72 6460 0a20 2020 2020  .SkyCoord`.     
-00000460: 2020 2054 6865 2070 6174 6820 7665 7274     The path vert
-00000470: 6963 6573 2c20 6173 2061 6e20 6172 7261  ices, as an arra
-00000480: 7920 6f72 2073 6571 7565 6e63 6520 6f66  y or sequence of
-00000490: 2073 6b79 2063 6f6f 7264 696e 6174 6573   sky coordinates
-000004a0: 2028 7769 7468 2072 6967 6874 0a20 2020   (with right.   
-000004b0: 2020 2020 2061 7363 656e 7369 6f6e 2061       ascension a
-000004c0: 6264 2064 6563 6c69 6e61 7469 6f6e 292e  bd declination).
-000004d0: 0a20 2020 2077 6373 3a20 607e 6173 7472  .    wcs: `~astr
-000004e0: 6f70 792e 7763 732e 5743 5360 0a20 2020  opy.wcs.WCS`.   
-000004f0: 2020 2020 2057 4353 206f 626a 6563 742e       WCS object.
-00000500: 0a20 2020 2063 6c6f 7365 643a 2062 6f6f  .    closed: boo
-00000510: 6c2c 2064 6566 6175 6c74 3a20 5472 7565  l, default: True
-00000520: 0a20 2020 2020 2020 2057 6865 7468 6572  .        Whether
-00000530: 2074 6865 2074 6865 2070 6174 6820 6973   the the path is
-00000540: 2063 6c6f 7365 642c 2069 2e65 2e20 7768   closed, i.e. wh
-00000550: 6574 6865 7220 7468 6520 6c61 7374 2076  ether the last v
-00000560: 6572 7465 7820 6973 2063 6f6e 6e65 6374  ertex is connect
-00000570: 6564 2074 6f20 7468 650a 2020 2020 2020  ed to the.      
-00000580: 2020 6669 7273 7420 6279 2061 206c 696e    first by a lin
-00000590: 652e 0a20 2020 2065 6467 6563 6f6c 6f72  e..    edgecolor
-000005a0: 3a20 636f 6c6f 722c 2064 6566 6175 6c74  : color, default
-000005b0: 3a20 2262 6c61 636b 220a 2020 2020 2020  : "black".      
-000005c0: 2020 5468 6520 6564 6765 2063 6f6c 6f72    The edge color
-000005d0: 2e0a 2020 2020 6661 6365 636f 6c6f 723a  ..    facecolor:
-000005e0: 2063 6f6c 6f72 2c20 6465 6661 756c 743a   color, default:
-000005f0: 2022 6e6f 6e65 220a 2020 2020 2020 2020   "none".        
-00000600: 5468 6520 6669 6c6c 696e 6720 636f 6c6f  The filling colo
-00000610: 722e 0a20 2020 202a 2a6b 7761 7267 733a  r..    **kwargs:
-00000620: 2064 6963 742c 206f 7074 696f 6e61 6c0a   dict, optional.
-00000630: 2020 2020 2020 2020 4164 6469 7469 6f6e          Addition
-00000640: 616c 206b 6579 776f 7264 2061 7267 756d  al keyword argum
-00000650: 656e 7473 2c20 7768 6963 6820 7769 6c6c  ents, which will
-00000660: 2062 6520 7061 7373 6564 2074 6f20 4d61   be passed to Ma
-00000670: 7470 6c6f 746c 6962 2773 0a20 2020 2020  tplotlib's.     
-00000680: 2020 2060 7e6d 6174 706c 6f74 6c69 622e     `~matplotlib.
-00000690: 7061 7463 6865 732e 5061 7468 5061 7463  patches.PathPatc
-000006a0: 6860 2070 6174 6368 2063 6f6e 7374 7275  h` patch constru
-000006b0: 6374 6f72 2e0a 2020 2020 54da 0562 6c61  ctor..    T..bla
-000006c0: 636b da04 6e6f 6e65 da08 7665 7274 6963  ck..none..vertic
-000006d0: 6573 da03 7763 73da 0663 6c6f 7365 64da  es..wcs..closed.
-000006e0: 0965 6467 6563 6f6c 6f72 da09 6661 6365  .edgecolor..face
-000006f0: 636f 6c6f 72da 066b 7761 7267 7363 0600  color..kwargsc..
-00000700: 0000 0000 0000 0000 0000 0700 0000 0300  ................
-00000710: 0000 4b00 0000 735a 0000 007c 0372 1174  ..K...sZ...|.r.t
-00000720: 007c 0183 0164 0064 0085 0219 007c 0164  .|...d.d.....|.d
-00000730: 0119 0067 0117 007c 005f 016e 0574 007c  ...g...|._.n.t.|
-00000740: 0183 017c 005f 017c 027c 005f 027c 037c  ...|._.|.|._.|.|
-00000750: 005f 0374 047c 0683 017c 005f 057c 047c  ._.t.|...|._.|.|
-00000760: 006a 0564 023c 007c 057c 006a 0564 033c  .j.d.<.|.|.j.d.<
-00000770: 0064 0053 0029 044e e9ff ffff ff72 1700  .d.S.).N.....r..
-00000780: 0000 7218 0000 0029 06da 046c 6973 74da  ..r....)...list.
-00000790: 095f 7665 7274 6963 6573 da04 5f77 6373  ._vertices.._wcs
-000007a0: da07 5f63 6c6f 7365 6472 0200 0000 da07  .._closedr......
-000007b0: 5f6b 7761 7267 7329 07da 0473 656c 6672  _kwargs)...selfr
-000007c0: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
-000007d0: 0000 0072 1800 0000 7219 0000 00a9 0072  ...r....r......r
-000007e0: 2100 0000 fa4f 2f55 7365 7273 2f63 6872  !....O/Users/chr
-000007f0: 6973 7469 616e 2f49 6465 6150 726f 6a65  istian/IdeaProje
-00000800: 6374 732f 696d 6570 6875 2f73 7263 2f69  cts/imephu/src/i
-00000810: 6d65 7068 752f 616e 6e6f 7461 7469 6f6e  mephu/annotation
-00000820: 2f67 656e 6572 616c 2f6c 696e 655f 7061  /general/line_pa
-00000830: 7468 2e70 79da 085f 5f69 6e69 745f 5f2b  th.py..__init__+
-00000840: 0000 0073 1000 0000 0409 1e03 0a02 0601  ...s............
-00000850: 0601 0a01 0a01 0e01 7a1b 4c69 6e65 5061  ........z.LinePa
-00000860: 7468 416e 6e6f 7461 7469 6f6e 2e5f 5f69  thAnnotation.__i
-00000870: 6e69 745f 5fda 0261 78da 0672 6574 7572  nit__..ax..retur
-00000880: 6e4e 6302 0000 0000 0000 0000 0000 0005  nNc.............
-00000890: 0000 0004 0000 0003 0000 0073 4200 0000  ...........sB...
-000008a0: 8700 6601 6401 6402 8408 8800 6a00 4400  ..f.d.d.....j.D.
-000008b0: 8301 7d02 7401 7c02 8800 6a02 6403 8d02  ..}.t.|...j.d...
-000008c0: 7d03 7403 7c03 6601 6900 8800 6a04 a401  }.t.|.f.i...j...
-000008d0: 8e01 7d04 7c01 a005 7c04 a101 0100 6404  ..}.|...|.....d.
-000008e0: 5300 2905 7aa0 4164 6420 7468 6520 6c69  S.).z.Add the li
-000008f0: 6e65 2070 6174 6820 746f 2061 2066 696e  ne path to a fin
-00000900: 6465 7220 6368 6172 742e 0a0a 2020 2020  der chart...    
-00000910: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000920: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00000930: 2d0a 2020 2020 2020 2020 6178 3a20 607e  -.        ax: `~
-00000940: 6173 7472 6f70 792e 7669 7375 616c 697a  astropy.visualiz
-00000950: 6174 696f 6e2e 7763 7361 7865 732e 5743  ation.wcsaxes.WC
-00000960: 5341 7865 7360 0a20 2020 2020 2020 2020  SAxes`.         
-00000970: 2020 2050 6c6f 7420 6178 6573 2e0a 2020     Plot axes..  
-00000980: 2020 2020 2020 6301 0000 0000 0000 0000        c.........
-00000990: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-000009a0: 1800 0000 6700 7c00 5d08 7d01 7400 7c01  ....g.|.].}.t.|.
-000009b0: 8800 6a01 8302 9102 7102 5300 7221 0000  ..j.....q.S.r!..
-000009c0: 0029 0272 0f00 0000 721d 0000 00a9 02da  .).r....r.......
-000009d0: 022e 30da 0676 6572 7465 78a9 0172 2000  ..0..vertex..r .
-000009e0: 0000 7221 0000 0072 2200 0000 da0a 3c6c  ..r!...r".....<l
-000009f0: 6973 7463 6f6d 703e 4800 0000 7306 0000  istcomp>H...s...
-00000a00: 0006 000c 0106 ff7a 2d4c 696e 6550 6174  .......z-LinePat
-00000a10: 6841 6e6e 6f74 6174 696f 6e2e 6164 645f  hAnnotation.add_
-00000a20: 746f 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  to.<locals>.<lis
-00000a30: 7463 6f6d 703e 2901 7216 0000 004e 2906  tcomp>).r....N).
-00000a40: 721c 0000 0072 0c00 0000 721e 0000 0072  r....r....r....r
-00000a50: 0b00 0000 721f 0000 00da 0961 6464 5f70  ....r......add_p
-00000a60: 6174 6368 2905 7220 0000 0072 2400 0000  atch).r ...r$...
-00000a70: 5a0b 7665 7274 6963 6573 5f70 78da 0470  Z.vertices_px..p
-00000a80: 6174 685a 0a70 6174 685f 7061 7463 6872  athZ.path_patchr
-00000a90: 2100 0000 7229 0000 0072 2200 0000 da06  !...r)...r".....
-00000aa0: 6164 645f 746f 4000 0000 730c 0000 000a  add_to@...s.....
-00000ab0: 0804 0106 ff0e 0312 010e 017a 194c 696e  ...........z.Lin
-00000ac0: 6550 6174 6841 6e6e 6f74 6174 696f 6e2e  ePathAnnotation.
-00000ad0: 6164 645f 746f da05 7069 766f 74da 0561  add_to..pivot..a
-00000ae0: 6e67 6c65 6303 0000 0000 0000 0000 0000  nglec...........
-00000af0: 0005 0000 0003 0000 0003 0000 0073 2a00  .............s*.
-00000b00: 0000 7400 8802 8301 7d03 8700 8701 8702  ..t.....}.......
-00000b10: 6603 6401 6402 8408 8802 6a01 4400 8301  f.d.d.....j.D...
-00000b20: 7d04 7c04 7c03 5f01 7c03 5300 2904 6127  }.|.|._.|.S.).a'
-00000b30: 0200 0052 6f74 6174 6520 7468 6973 2061  ...Rotate this a
-00000b40: 6e6e 6f74 6174 696f 6e20 6172 6f75 6e64  nnotation around
-00000b50: 2061 2070 6976 6f74 2061 6e64 2072 6574   a pivot and ret
-00000b60: 7572 6e20 7468 6520 7265 7375 6c74 2e0a  urn the result..
-00000b70: 0a20 2020 2020 2020 2054 6865 2072 6f74  .        The rot
-00000b80: 6174 696f 6e20 616e 676c 6520 6973 2061  ation angle is a
-00000b90: 6e20 616e 676c 6520 6f6e 2074 6865 2073  n angle on the s
-00000ba0: 6b79 2c20 6d65 6173 7572 6564 2066 726f  ky, measured fro
-00000bb0: 6d20 6e6f 7274 6820 746f 2065 6173 742e  m north to east.
-00000bc0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00000bd0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00000be0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00000bf0: 7069 766f 743a 2060 7e61 7374 726f 7079  pivot: `~astropy
-00000c00: 2e63 6f6f 7264 696e 6174 6573 2e53 6b79  .coordinates.Sky
-00000c10: 436f 6f72 6460 0a20 2020 2020 2020 2020  Coord`.         
-00000c20: 2020 2050 6f69 6e74 2061 726f 756e 6420     Point around 
-00000c30: 7768 6963 6820 746f 2072 6f74 6174 6520  which to rotate 
-00000c40: 7468 6520 616e 6e6f 7461 7469 6f6e 2e0a  the annotation..
-00000c50: 2020 2020 2020 2020 616e 676c 653a 2060          angle: `
-00000c60: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
-00000c70: 6174 6573 2e41 6e67 6c65 600a 2020 2020  ates.Angle`.    
-00000c80: 2020 2020 2020 2020 416e 676c 6520 6f66          Angle of
-00000c90: 2072 6f74 6174 696f 6e2c 206d 6561 7375   rotation, measu
-00000ca0: 7265 6420 6672 6f6d 206e 6f72 7468 2074  red from north t
-00000cb0: 6f77 6172 6473 2074 6865 2065 6173 742e  owards the east.
-00000cc0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00000cd0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00000ce0: 2d0a 2020 2020 2020 2020 607e 696d 6570  -.        `~imep
-00000cf0: 6875 2e61 6e6e 6f74 6174 696f 6e2e 6765  hu.annotation.ge
-00000d00: 6e65 7261 6c2e 4c69 6e65 5061 7468 416e  neral.LinePathAn
-00000d10: 6e6f 7461 7469 6f6e 600a 2020 2020 2020  notation`.      
-00000d20: 2020 2020 2020 5468 6520 616e 6e6f 7461        The annota
-00000d30: 7469 6f6e 2072 6573 756c 7469 6e67 2066  tion resulting f
-00000d40: 726f 6d20 7468 6520 726f 7461 7469 6f6e  rom the rotation
-00000d50: 2e0a 2020 2020 2020 2020 6301 0000 0000  ..        c.....
-00000d60: 0000 0000 0000 0002 0000 0007 0000 0013  ................
-00000d70: 0000 0073 1c00 0000 6700 7c00 5d0a 7d01  ...s....g.|.].}.
-00000d80: 7400 7c01 8801 8800 8802 6a01 8304 9102  t.|.......j.....
-00000d90: 7102 5300 7221 0000 0029 0272 0e00 0000  q.S.r!...).r....
-00000da0: 721d 0000 0072 2600 0000 a903 722f 0000  r....r&.....r/..
-00000db0: 0072 2e00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00000dc0: 7222 0000 0072 2a00 0000 6100 0000 7306  r"...r*...a...s.
-00000dd0: 0000 0006 0010 0106 ff7a 2d4c 696e 6550  .........z-LineP
-00000de0: 6174 6841 6e6e 6f74 6174 696f 6e2e 726f  athAnnotation.ro
-00000df0: 7461 7465 2e3c 6c6f 6361 6c73 3e2e 3c6c  tate.<locals>.<l
-00000e00: 6973 7463 6f6d 703e 4ea9 0272 0200 0000  istcomp>N..r....
-00000e10: 721c 0000 0029 0572 2000 0000 722e 0000  r....).r ...r...
-00000e20: 0072 2f00 0000 da12 726f 7461 7465 645f  .r/.....rotated_
-00000e30: 616e 6e6f 7461 7469 6f6e 5a10 726f 7461  annotationZ.rota
-00000e40: 7465 645f 7665 7274 6963 6573 7221 0000  ted_verticesr!..
-00000e50: 0072 3000 0000 7222 0000 0072 0e00 0000  .r0...r"...r....
-00000e60: 4f00 0000 730c 0000 0008 110e 0104 0106  O...s...........
-00000e70: ff06 0304 017a 194c 696e 6550 6174 6841  .....z.LinePathA
-00000e80: 6e6e 6f74 6174 696f 6e2e 726f 7461 7465  nnotation.rotate
-00000e90: da0c 6469 7370 6c61 6365 6d65 6e74 6302  ..displacementc.
-00000ea0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00000eb0: 0000 0003 0000 0073 2600 0000 7400 7c00  .......s&...t.|.
-00000ec0: 8301 7d02 8700 6601 6401 6402 8408 7c00  ..}...f.d.d...|.
-00000ed0: 6a01 4400 8301 7d03 7c03 7c02 5f01 7c02  j.D...}.|.|._.|.
-00000ee0: 5300 2904 617b 0100 000a 2020 2020 2020  S.).a{....      
-00000ef0: 2020 4d6f 7665 2074 6869 7320 616e 6e6f    Move this anno
-00000f00: 7461 7469 6f6e 2061 6c6f 6e67 2061 2064  tation along a d
-00000f10: 6973 706c 6163 656d 656e 7420 7665 6374  isplacement vect
-00000f20: 6f72 2061 6e64 2072 6574 7572 6e20 7468  or and return th
-00000f30: 6520 7265 7375 6c74 2e0a 0a20 2020 2020  e result...     
-00000f40: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00000f50: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00000f60: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
-00000f70: 656d 656e 743a 2032 4420 6172 7261 7920  ement: 2D array 
-00000f80: 6f66 2061 6e67 6c65 730a 2020 2020 2020  of angles.      
-00000f90: 2020 2020 2020 5468 6520 6469 7370 6c61        The displa
-00000fa0: 6365 6d65 6e74 2062 7920 7768 6963 6820  cement by which 
-00000fb0: 746f 206d 6f76 6520 7468 6520 616e 6e6f  to move the anno
-00000fc0: 7461 7469 6f6e 2e0a 0a20 2020 2020 2020  tation...       
-00000fd0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00000fe0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00000ff0: 2060 7e69 6d65 7068 752e 616e 6e6f 7461   `~imephu.annota
-00001000: 7469 6f6e 2e67 656e 6572 616c 2e4c 696e  tion.general.Lin
-00001010: 6550 6174 6841 6e6e 6f74 6174 696f 6e60  ePathAnnotation`
-00001020: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00001030: 2061 6e6e 6f74 6174 696f 6e20 7265 7375   annotation resu
-00001040: 6c74 696e 6720 6672 6f6d 2074 6865 2074  lting from the t
-00001050: 7261 6e73 6c61 7469 6f6e 2e0a 2020 2020  ranslation..    
-00001060: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00001070: 0002 0000 0005 0000 0013 0000 0073 1600  .............s..
-00001080: 0000 6700 7c00 5d07 7d01 7400 7c01 8800  ..g.|.].}.t.|...
-00001090: 8302 9102 7102 5300 7221 0000 0029 0172  ....q.S.r!...).r
-000010a0: 1000 0000 7226 0000 00a9 0172 3300 0000  ....r&.....r3...
-000010b0: 7221 0000 0072 2200 0000 722a 0000 0076  r!...r"...r*...v
-000010c0: 0000 0073 0600 0000 0600 0a01 06ff 7a30  ...s..........z0
-000010d0: 4c69 6e65 5061 7468 416e 6e6f 7461 7469  LinePathAnnotati
-000010e0: 6f6e 2e74 7261 6e73 6c61 7465 2e3c 6c6f  on.translate.<lo
-000010f0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001100: 4e72 3100 0000 2904 7220 0000 0072 3300  Nr1...).r ...r3.
-00001110: 0000 da15 7472 616e 736c 6174 6564 5f61  ....translated_a
-00001120: 6e6e 6f74 6174 696f 6e5a 1374 7261 6e73  nnotationZ.trans
-00001130: 6c61 7465 645f 7665 7274 6963 6573 7221  lated_verticesr!
-00001140: 0000 0072 3400 0000 7222 0000 0072 1000  ...r4...r"...r..
-00001150: 0000 6700 0000 730c 0000 0008 0e0a 0104  ..g...s.........
-00001160: 0106 ff06 0304 017a 1c4c 696e 6550 6174  .......z.LinePat
-00001170: 6841 6e6e 6f74 6174 696f 6e2e 7472 616e  hAnnotation.tran
-00001180: 736c 6174 6529 0354 7212 0000 0072 1300  slate).Tr....r..
-00001190: 0000 2913 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-000011a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000011b0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-000011c0: 5f72 0400 0000 7208 0000 0072 0a00 0000  _r....r....r....
-000011d0: da04 626f 6f6c 7206 0000 00da 0373 7472  ..boolr......str
-000011e0: 7205 0000 00da 0566 6c6f 6174 7203 0000  r......floatr...
-000011f0: 0072 2300 0000 7209 0000 0072 2d00 0000  .r#...r....r-...
-00001200: 7207 0000 0072 0e00 0000 7210 0000 0072  r....r....r....r
-00001210: 2100 0000 7221 0000 0072 2100 0000 7222  !...r!...r!...r"
-00001220: 0000 0072 1100 0000 0e00 0000 732a 0000  ...r........s*..
-00001230: 0008 0004 0102 2002 0102 0104 fa06 0202  ...... .........
-00001240: fe02 0302 fd02 0402 fc14 0502 fb14 0602  ................
-00001250: fa02 070a f912 1516 0f16 1872 1100 0000  ...........r....
-00001260: 4e29 19da 0463 6f70 7972 0200 0000 da06  N)...copyr......
-00001270: 7479 7069 6e67 7203 0000 0072 0400 0000  typingr....r....
-00001280: 7205 0000 0072 0600 0000 da13 6173 7472  r....r......astr
-00001290: 6f70 792e 636f 6f72 6469 6e61 7465 7372  opy.coordinatesr
-000012a0: 0700 0000 7208 0000 00da 1d61 7374 726f  ....r......astro
-000012b0: 7079 2e76 6973 7561 6c69 7a61 7469 6f6e  py.visualization
-000012c0: 2e77 6373 6178 6573 7209 0000 00da 0b61  .wcsaxesr......a
-000012d0: 7374 726f 7079 2e77 6373 720a 0000 00da  stropy.wcsr.....
-000012e0: 126d 6174 706c 6f74 6c69 622e 7061 7463  .matplotlib.patc
-000012f0: 6865 7372 0b00 0000 5a0f 6d61 7470 6c6f  hesr....Z.matplo
-00001300: 746c 6962 2e70 6174 6872 0c00 0000 5a11  tlib.pathr....Z.
-00001310: 696d 6570 6875 2e61 6e6e 6f74 6174 696f  imephu.annotatio
-00001320: 6e72 0d00 0000 da0f 696d 6570 6875 2e67  nr......imephu.g
-00001330: 656f 6d65 7472 7972 0e00 0000 720f 0000  eometryr....r...
-00001340: 0072 1000 0000 7211 0000 0072 2100 0000  .r....r....r!...
-00001350: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-00001360: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
-00001370: 0000 0c00 1801 1002 0c01 0c01 0c01 0c01  ................
-00001380: 0c02 1401 1403                           ......
+00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000010: 7274 2041 6e79 2c20 4c69 7374 2c20 5475  rt Any, List, Tu
+00000020: 706c 652c 2055 6e69 6f6e 2c20 6361 7374  ple, Union, cast
+00000030: 0a0a 696d 706f 7274 206e 756d 7079 2061  ..import numpy a
+00000040: 7320 6e70 0a66 726f 6d20 6173 7472 6f70  s np.from astrop
+00000050: 7920 696d 706f 7274 2075 6e69 7473 2061  y import units a
+00000060: 7320 750a 6672 6f6d 2061 7374 726f 7079  s u.from astropy
+00000070: 2e63 6f6f 7264 696e 6174 6573 2069 6d70  .coordinates imp
+00000080: 6f72 7420 416e 676c 652c 2053 6b79 436f  ort Angle, SkyCo
+00000090: 6f72 640a 6672 6f6d 2061 7374 726f 7079  ord.from astropy
+000000a0: 2e77 6373 2069 6d70 6f72 7420 5743 530a  .wcs import WCS.
+000000b0: 0a66 726f 6d20 696d 6570 6875 2e61 6e6e  .from imephu.ann
+000000c0: 6f74 6174 696f 6e2e 6765 6e65 7261 6c2e  otation.general.
+000000d0: 6c69 6e65 5f70 6174 6820 696d 706f 7274  line_path import
+000000e0: 204c 696e 6550 6174 6841 6e6e 6f74 6174   LinePathAnnotat
+000000f0: 696f 6e0a 6672 6f6d 2069 6d65 7068 752e  ion.from imephu.
+00000100: 6765 6f6d 6574 7279 2069 6d70 6f72 7420  geometry import 
+00000110: 7472 616e 736c 6174 650a 0a0a 636c 6173  translate...clas
+00000120: 7320 5265 6374 616e 676c 6541 6e6e 6f74  s RectangleAnnot
+00000130: 6174 696f 6e28 4c69 6e65 5061 7468 416e  ation(LinePathAn
+00000140: 6e6f 7461 7469 6f6e 293a 0a20 2020 2022  notation):.    "
+00000150: 2222 416e 2061 6e6e 6f74 6174 696f 6e20  ""An annotation 
+00000160: 666f 7220 706c 6f74 7469 6e67 2061 2072  for plotting a r
+00000170: 6563 7461 6e67 6c65 206f 6e20 6120 6669  ectangle on a fi
+00000180: 6e64 6572 2063 6861 7274 2e0a 0a20 2020  nder chart...   
+00000190: 2054 6865 2072 6563 7461 6e67 6c65 2069   The rectangle i
+000001a0: 7320 6465 6669 6e65 6420 6279 2069 7473  s defined by its
+000001b0: 2063 656e 7465 722c 2077 6964 7468 2061   center, width a
+000001c0: 6e64 2068 6569 6768 742e 2054 6865 2063  nd height. The c
+000001d0: 656e 7465 7220 6d75 7374 2062 6520 6120  enter must be a 
+000001e0: 736b 790a 2020 2020 706f 7369 7469 6f6e  sky.    position
+000001f0: 2069 6e20 7269 6768 7420 6173 6365 6e73   in right ascens
+00000200: 696f 6e20 616e 6420 6465 636c 696e 6174  ion and declinat
+00000210: 696f 6e2c 2074 6865 2077 6964 7468 2061  ion, the width a
+00000220: 6e64 2068 6569 6768 7420 6d75 7374 2062  nd height must b
+00000230: 6520 616e 2061 6e67 6c65 0a20 2020 206f  e an angle.    o
+00000240: 6e20 7468 6520 736b 792e 2054 6865 2077  n the sky. The w
+00000250: 6964 7468 2069 7320 7461 6b65 6e20 746f  idth is taken to
+00000260: 2062 6520 7468 6520 6578 7465 6e73 696f   be the extensio
+00000270: 6e20 696e 2074 6865 2072 6967 6874 2061  n in the right a
+00000280: 7363 656e 7369 6f6e 2064 6972 6563 7469  scension directi
+00000290: 6f6e 2c0a 2020 2020 7468 6520 6865 6967  on,.    the heig
+000002a0: 6874 2074 6865 2065 7874 656e 7369 6f6e  ht the extension
+000002b0: 2069 6e20 7468 6520 6465 636c 696e 6174   in the declinat
+000002c0: 696f 6e20 6469 7265 6374 696f 6e2e 0a0a  ion direction...
+000002d0: 2020 2020 5468 6520 636f 726e 6572 7320      The corners 
+000002e0: 6f66 2074 6865 2072 6563 7461 6e67 6c65  of the rectangle
+000002f0: 2061 7265 206d 6170 7065 6420 746f 2074   are mapped to t
+00000300: 6865 6972 2063 6f72 7265 7370 6f6e 6469  heir correspondi
+00000310: 6e67 2070 6978 656c 2070 6f73 6974 696f  ng pixel positio
+00000320: 6e73 206f 6e0a 2020 2020 7468 6520 6669  ns on.    the fi
+00000330: 6e64 6572 2063 6861 7274 2e20 5468 6973  nder chart. This
+00000340: 2069 6d70 6c69 6573 2074 6861 7420 696e   implies that in
+00000350: 2067 656e 6572 616c 2074 6865 2066 6967   general the fig
+00000360: 7572 6520 706c 6f74 7465 6420 6f6e 2074  ure plotted on t
+00000370: 6865 2066 696e 6465 720a 2020 2020 6368  he finder.    ch
+00000380: 6172 7420 7769 6c6c 2062 6520 6120 7175  art will be a qu
+00000390: 6164 7269 6c61 7465 7261 6c2c 2062 7574  adrilateral, but
+000003a0: 206e 6f74 2065 7861 6374 6c79 2061 2072   not exactly a r
+000003b0: 6563 7461 6e67 6c65 2e0a 0a20 2020 202e  ectangle...    .
+000003c0: 2e20 6e6f 7465 3a3a 0a20 2020 2020 2020  . note::.       
+000003d0: 2054 6865 2063 656e 7465 7220 7261 7468   The center rath
+000003e0: 6572 2074 6861 6e20 2262 6f74 746f 6d20  er than "bottom 
+000003f0: 6c65 6674 2220 636f 726e 6572 2069 7320  left" corner is 
+00000400: 7370 6563 6966 6965 642c 2061 7320 7468  specified, as th
+00000410: 6973 2069 7320 6d6f 7265 0a20 2020 2020  is is more.     
+00000420: 2020 2063 6f6e 7665 6e69 656e 7420 696e     convenient in
+00000430: 2074 6865 2063 6f6e 7465 7874 206f 6620   the context of 
+00000440: 6669 6e64 6572 2063 6861 7274 732e 0a0a  finder charts...
+00000450: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00000460: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000470: 2020 6365 6e74 6572 3a20 607e 6173 7472    center: `~astr
+00000480: 6f70 792e 636f 6f72 6469 6e61 7465 732e  opy.coordinates.
+00000490: 536b 7943 6f6f 7264 600a 2020 2020 2020  SkyCoord`.      
+000004a0: 2020 5468 6520 6365 6e74 6572 206f 6620    The center of 
+000004b0: 7468 6520 7265 6374 616e 676c 652c 2069  the rectangle, i
+000004c0: 6e20 7269 6768 7420 6173 6365 6e73 696f  n right ascensio
+000004d0: 6e20 616e 6420 6465 636c 696e 6174 696f  n and declinatio
+000004e0: 6e2e 0a20 2020 2077 6964 7468 3a20 607e  n..    width: `~
+000004f0: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
+00000500: 7465 732e 416e 676c 6560 0a20 2020 2020  tes.Angle`.     
+00000510: 2020 2054 6865 2077 6964 7468 206f 6620     The width of 
+00000520: 7468 6520 7265 6374 616e 676c 6520 6173  the rectangle as
+00000530: 2061 6e20 616e 676c 6520 6f6e 2074 6865   an angle on the
+00000540: 2073 6b79 2069 6e20 7468 6520 6469 7265   sky in the dire
+00000550: 6374 696f 6e20 6f66 2074 6865 0a20 2020  ction of the.   
+00000560: 2020 2020 2072 6967 6874 2061 7363 656e       right ascen
+00000570: 7369 6f6e 2e0a 2020 2020 6865 6967 6874  sion..    height
+00000580: 3a20 607e 6173 7472 6f70 792e 636f 6f72  : `~astropy.coor
+00000590: 6469 6e61 7465 732e 416e 676c 6560 0a20  dinates.Angle`. 
+000005a0: 2020 2020 2020 2054 6865 2068 6569 6768         The heigh
+000005b0: 7420 6f66 2074 6865 2072 6563 7461 6e67  t of the rectang
+000005c0: 6c65 2061 7320 616e 2061 6e67 6c65 206f  le as an angle o
+000005d0: 6e20 7468 6520 736b 7920 696e 2074 6865  n the sky in the
+000005e0: 2064 6972 6563 7469 6f6e 206f 6620 7468   direction of th
+000005f0: 650a 2020 2020 2020 2020 6465 636c 696e  e.        declin
+00000600: 6174 696f 6e2e 0a20 2020 2077 6373 3a20  ation..    wcs: 
+00000610: 607e 6173 7472 6f70 792e 7763 732e 5743  `~astropy.wcs.WC
+00000620: 5360 0a20 2020 2020 2020 2057 4353 206f  S`.        WCS o
+00000630: 626a 6563 742e 0a20 2020 2065 6467 6563  bject..    edgec
+00000640: 6f6c 6f72 3a20 636f 6c6f 722c 2064 6566  olor: color, def
+00000650: 6175 6c74 3a20 2262 6c61 636b 220a 2020  ault: "black".  
+00000660: 2020 2020 2020 5468 6520 6564 6765 2063        The edge c
+00000670: 6f6c 6f72 2e0a 2020 2020 6661 6365 636f  olor..    faceco
+00000680: 6c6f 723a 2063 6f6c 6f72 2c20 6465 6661  lor: color, defa
+00000690: 756c 743a 2022 6e6f 6e65 220a 2020 2020  ult: "none".    
+000006a0: 2020 2020 5468 6520 6669 6c6c 696e 6720      The filling 
+000006b0: 636f 6c6f 722e 0a20 2020 202a 2a6b 7761  color..    **kwa
+000006c0: 7267 733a 2064 6963 742c 206f 7074 696f  rgs: dict, optio
+000006d0: 6e61 6c0a 2020 2020 2020 2020 4164 6469  nal.        Addi
+000006e0: 7469 6f6e 616c 206b 6579 776f 7264 2061  tional keyword a
+000006f0: 7267 756d 656e 7473 2c20 7768 6963 6820  rguments, which 
+00000700: 7769 6c6c 2062 6520 7061 7373 6564 2074  will be passed t
+00000710: 6f20 4d61 7470 6c6f 746c 6962 2773 0a20  o Matplotlib's. 
+00000720: 2020 2020 2020 2060 7e6d 6174 706c 6f74         `~matplot
+00000730: 6c69 622e 7061 7463 6865 732e 5061 7468  lib.patches.Path
+00000740: 5061 7463 6860 2070 6174 6368 2063 6f6e  Patch` patch con
+00000750: 7374 7275 6374 6f72 2e0a 2020 2020 2222  structor..    ""
+00000760: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00000770: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00000780: 662c 0a20 2020 2020 2020 2063 656e 7465  f,.        cente
+00000790: 723a 2053 6b79 436f 6f72 642c 0a20 2020  r: SkyCoord,.   
+000007a0: 2020 2020 2077 6964 7468 3a20 416e 676c       width: Angl
+000007b0: 652c 0a20 2020 2020 2020 2068 6569 6768  e,.        heigh
+000007c0: 743a 2041 6e67 6c65 2c0a 2020 2020 2020  t: Angle,.      
+000007d0: 2020 7763 733a 2057 4353 2c0a 2020 2020    wcs: WCS,.    
+000007e0: 2020 2020 6564 6765 636f 6c6f 723a 2055      edgecolor: U
+000007f0: 6e69 6f6e 5b73 7472 2c20 5475 706c 655b  nion[str, Tuple[
+00000800: 666c 6f61 742c 2066 6c6f 6174 2c20 666c  float, float, fl
+00000810: 6f61 745d 5d20 3d20 2262 6c61 636b 222c  oat]] = "black",
+00000820: 0a20 2020 2020 2020 2066 6163 6563 6f6c  .        facecol
+00000830: 6f72 3a20 556e 696f 6e5b 7374 722c 2054  or: Union[str, T
+00000840: 7570 6c65 5b66 6c6f 6174 2c20 666c 6f61  uple[float, floa
+00000850: 742c 2066 6c6f 6174 5d5d 203d 2022 6e6f  t, float]] = "no
+00000860: 6e65 222c 0a20 2020 2020 2020 202a 2a6b  ne",.        **k
+00000870: 7761 7267 733a 2041 6e79 2c0a 2020 2020  wargs: Any,.    
+00000880: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
+00000890: 2829 2e5f 5f69 6e69 745f 5f28 0a20 2020  ().__init__(.   
+000008a0: 2020 2020 2020 2020 2076 6572 7469 6365           vertice
+000008b0: 733d 5265 6374 616e 676c 6541 6e6e 6f74  s=RectangleAnnot
+000008c0: 6174 696f 6e2e 5f63 6f72 6e65 7273 2863  ation._corners(c
+000008d0: 656e 7465 722c 2077 6964 7468 2c20 6865  enter, width, he
+000008e0: 6967 6874 292c 0a20 2020 2020 2020 2020  ight),.         
+000008f0: 2020 2077 6373 3d77 6373 2c0a 2020 2020     wcs=wcs,.    
+00000900: 2020 2020 2020 2020 636c 6f73 6564 3d54          closed=T
+00000910: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00000920: 2065 6467 6563 6f6c 6f72 3d65 6467 6563   edgecolor=edgec
+00000930: 6f6c 6f72 2c0a 2020 2020 2020 2020 2020  olor,.          
+00000940: 2020 6661 6365 636f 6c6f 723d 6661 6365    facecolor=face
+00000950: 636f 6c6f 722c 0a20 2020 2020 2020 2020  color,.         
+00000960: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
+00000970: 2020 2020 2029 0a0a 2020 2020 4073 7461       )..    @sta
+00000980: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+00000990: 6620 5f63 6f72 6e65 7273 2863 656e 7465  f _corners(cente
+000009a0: 723a 2053 6b79 436f 6f72 642c 2077 6964  r: SkyCoord, wid
+000009b0: 7468 3a20 416e 676c 652c 2068 6569 6768  th: Angle, heigh
+000009c0: 743a 2041 6e67 6c65 2920 2d3e 204c 6973  t: Angle) -> Lis
+000009d0: 745b 536b 7943 6f6f 7264 5d3a 0a20 2020  t[SkyCoord]:.   
+000009e0: 2020 2020 2063 6f72 6e65 7273 3a20 4c69       corners: Li
+000009f0: 7374 5b53 6b79 436f 6f72 645d 203d 205b  st[SkyCoord] = [
+00000a00: 5d0a 2020 2020 2020 2020 6861 6c66 5f77  ].        half_w
+00000a10: 6964 7468 5f61 7263 7365 6320 3d20 7769  idth_arcsec = wi
+00000a20: 6474 682e 746f 5f76 616c 7565 2875 2e61  dth.to_value(u.a
+00000a30: 7263 7365 6329 202f 2032 0a20 2020 2020  rcsec) / 2.     
+00000a40: 2020 2068 616c 665f 6865 6967 6874 5f61     half_height_a
+00000a50: 7263 7365 6320 3d20 6865 6967 6874 2e74  rcsec = height.t
+00000a60: 6f5f 7661 6c75 6528 752e 6172 6373 6563  o_value(u.arcsec
+00000a70: 2920 2f20 320a 2020 2020 2020 2020 6469  ) / 2.        di
+00000a80: 7265 6374 696f 6e73 203d 205b 282d 312c  rections = [(-1,
+00000a90: 202d 3129 2c20 2831 2c20 2d31 292c 2028   -1), (1, -1), (
+00000aa0: 312c 2031 292c 2028 2d31 2c20 3129 5d0a  1, 1), (-1, 1)].
+00000ab0: 2020 2020 2020 2020 666f 7220 6469 7265          for dire
+00000ac0: 6374 696f 6e20 696e 2064 6972 6563 7469  ction in directi
+00000ad0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+00000ae0: 2063 656e 7465 725f 746f 5f63 6f72 6e65   center_to_corne
+00000af0: 7220 3d20 280a 2020 2020 2020 2020 2020  r = (.          
+00000b00: 2020 2020 2020 6e70 2e61 7272 6179 280a        np.array(.
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b20: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+00000b30: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00000b40: 7265 6374 696f 6e5b 305d 202a 2068 616c  rection[0] * hal
+00000b50: 665f 7769 6474 685f 6172 6373 6563 2c0a  f_width_arcsec,.
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 2020 2020 2020 2020 6469 7265 6374 696f          directio
+00000b80: 6e5b 315d 202a 2068 616c 665f 6865 6967  n[1] * half_heig
+00000b90: 6874 5f61 7263 7365 632c 0a20 2020 2020  ht_arcsec,.     
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00000bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000bc0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00000bd0: 2020 202a 2075 2e61 7263 7365 630a 2020     * u.arcsec.  
+00000be0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00000bf0: 2020 2020 2020 2020 636f 726e 6572 203d          corner =
+00000c00: 2074 7261 6e73 6c61 7465 2863 656e 7465   translate(cente
+00000c10: 722c 2063 656e 7465 725f 746f 5f63 6f72  r, center_to_cor
+00000c20: 6e65 7229 0a20 2020 2020 2020 2020 2020  ner).           
+00000c30: 2063 6f72 6e65 7273 2e61 7070 656e 6428   corners.append(
+00000c40: 636f 726e 6572 290a 2020 2020 2020 2020  corner).        
+00000c50: 7265 7475 726e 2063 6f72 6e65 7273 0a0a  return corners..
+00000c60: 2020 2020 6465 6620 726f 7461 7465 2873      def rotate(s
+00000c70: 656c 662c 2070 6976 6f74 3a20 536b 7943  elf, pivot: SkyC
+00000c80: 6f6f 7264 2c20 616e 676c 653a 2041 6e67  oord, angle: Ang
+00000c90: 6c65 2920 2d3e 2022 5265 6374 616e 676c  le) -> "Rectangl
+00000ca0: 6541 6e6e 6f74 6174 696f 6e22 3a0a 2020  eAnnotation":.  
+00000cb0: 2020 2020 2020 2222 2252 6f74 6174 6520        """Rotate 
+00000cc0: 7468 6973 2061 6e6e 6f74 6174 696f 6e20  this annotation 
+00000cd0: 6172 6f75 6e64 2061 2070 6976 6f74 2061  around a pivot a
+00000ce0: 6e64 2072 6574 7572 6e20 7468 6520 7265  nd return the re
+00000cf0: 7375 6c74 2e0a 0a20 2020 2020 2020 2054  sult...        T
+00000d00: 6865 2072 6f74 6174 696f 6e20 616e 676c  he rotation angl
+00000d10: 6520 6973 2061 6e20 616e 676c 6520 6f6e  e is an angle on
+00000d20: 2074 6865 2073 6b79 2c20 6d65 6173 7572   the sky, measur
+00000d30: 6564 2066 726f 6d20 6e6f 7274 6820 746f  ed from north to
+00000d40: 2065 6173 742e 0a0a 2020 2020 2020 2020   east...        
+00000d50: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00000d60: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000d70: 2020 2020 2020 7069 766f 743a 2060 7e61        pivot: `~a
+00000d80: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
+00000d90: 6573 2e53 6b79 436f 6f72 6460 0a20 2020  es.SkyCoord`.   
+00000da0: 2020 2020 2020 2020 2050 6f69 6e74 2061           Point a
+00000db0: 726f 756e 6420 7768 6963 6820 746f 2072  round which to r
+00000dc0: 6f74 6174 6520 7468 6520 616e 6e6f 7461  otate the annota
+00000dd0: 7469 6f6e 2e0a 2020 2020 2020 2020 616e  tion..        an
+00000de0: 676c 653a 2060 7e61 7374 726f 7079 2e63  gle: `~astropy.c
+00000df0: 6f6f 7264 696e 6174 6573 2e41 6e67 6c65  oordinates.Angle
+00000e00: 600a 2020 2020 2020 2020 2020 2020 416e  `.            An
+00000e10: 676c 6520 6f66 2072 6f74 6174 696f 6e2c  gle of rotation,
+00000e20: 206d 6561 7375 7265 6420 6672 6f6d 206e   measured from n
+00000e30: 6f72 7468 2074 6f77 6172 6473 2074 6865  orth towards the
+00000e40: 2065 6173 742e 0a0a 2020 2020 2020 2020   east...        
+00000e50: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00000e60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00000e70: 607e 696d 6570 6875 2e61 6e6e 6f74 6174  `~imephu.annotat
+00000e80: 696f 6e2e 6765 6e65 7261 6c2e 5265 6374  ion.general.Rect
+00000e90: 616e 676c 6541 6e6e 6f74 6174 696f 6e60  angleAnnotation`
+00000ea0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00000eb0: 2061 6e6e 6f74 6174 696f 6e20 7265 7375   annotation resu
+00000ec0: 6c74 696e 6720 6672 6f6d 2074 6865 2072  lting from the r
+00000ed0: 6f74 6174 696f 6e2e 0a20 2020 2020 2020  otation..       
+00000ee0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00000ef0: 7572 6e20 6361 7374 2852 6563 7461 6e67  urn cast(Rectang
+00000f00: 6c65 416e 6e6f 7461 7469 6f6e 2c20 7375  leAnnotation, su
+00000f10: 7065 7228 292e 726f 7461 7465 2870 6976  per().rotate(piv
+00000f20: 6f74 2c20 616e 676c 6529 290a 0a20 2020  ot, angle))..   
+00000f30: 2064 6566 2074 7261 6e73 6c61 7465 2873   def translate(s
+00000f40: 656c 662c 2064 6973 706c 6163 656d 656e  elf, displacemen
+00000f50: 743a 2041 6e67 6c65 2920 2d3e 2022 5265  t: Angle) -> "Re
+00000f60: 6374 616e 676c 6541 6e6e 6f74 6174 696f  ctangleAnnotatio
+00000f70: 6e22 3a0a 2020 2020 2020 2020 2222 220a  n":.        """.
+00000f80: 2020 2020 2020 2020 4d6f 7665 2074 6869          Move thi
+00000f90: 7320 616e 6e6f 7461 7469 6f6e 2061 6c6f  s annotation alo
+00000fa0: 6e67 2061 2064 6973 706c 6163 656d 656e  ng a displacemen
+00000fb0: 7420 7665 6374 6f72 2061 6e64 2072 6574  t vector and ret
+00000fc0: 7572 6e20 7468 6520 7265 7375 6c74 2e0a  urn the result..
+00000fd0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00000fe0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00000ff0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2064  ------.        d
+00001000: 6973 706c 6163 656d 656e 743a 2032 4420  isplacement: 2D 
+00001010: 6172 7261 7920 6f66 2061 6e67 6c65 730a  array of angles.
+00001020: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00001030: 6469 7370 6c61 6365 6d65 6e74 2062 7920  displacement by 
+00001040: 7768 6963 6820 746f 206d 6f76 6520 7468  which to move th
+00001050: 6520 616e 6e6f 7461 7469 6f6e 2e0a 0a20  e annotation... 
+00001060: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00001070: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00001080: 2020 2020 2020 2060 7e69 6d65 7068 752e         `~imephu.
+00001090: 616e 6e6f 7461 7469 6f6e 2e67 656e 6572  annotation.gener
+000010a0: 616c 2e52 6563 7461 6e67 6c65 416e 6e6f  al.RectangleAnno
+000010b0: 7461 7469 6f6e 600a 2020 2020 2020 2020  tation`.        
+000010c0: 2020 2020 5468 6520 616e 6e6f 7461 7469      The annotati
+000010d0: 6f6e 2072 6573 756c 7469 6e67 2066 726f  on resulting fro
+000010e0: 6d20 7468 6520 7472 616e 736c 6174 696f  m the translatio
+000010f0: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
+00001100: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
+00001110: 7374 2852 6563 7461 6e67 6c65 416e 6e6f  st(RectangleAnno
+00001120: 7461 7469 6f6e 2c20 7375 7065 7228 292e  tation, super().
+00001130: 7472 616e 736c 6174 6528 6469 7370 6c61  translate(displa
+00001140: 6365 6d65 6e74 2929 0a                   cement)).
```

### Comparing `imephu-0.2.0/src/imephu/annotation/general/__pycache__/text.cpython-310.pyc` & `imephu-0.2.1/src/imephu/annotation/general/text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,330 +1,333 @@
-00000000: 6f0d 0d0a 0000 0000 6573 c762 c414 0000  o.......es.b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
-00000050: 6d07 5a07 0100 6400 6403 6c08 5a09 6400  m.Z...d.d.l.Z.d.
-00000060: 6403 6c0a 6d02 5a0b 0100 6400 6404 6c0c  d.l.m.Z...d.d.l.
-00000070: 6d0d 5a0d 6d0e 5a0e 0100 6400 6405 6c0f  m.Z.m.Z...d.d.l.
-00000080: 6d10 5a10 0100 6400 6406 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
-00000090: 0100 6400 6407 6c13 6d14 5a14 0100 6400  ..d.d.l.m.Z...d.
-000000a0: 6408 6c15 6d16 5a16 6d17 5a17 6d18 5a18  d.l.m.Z.m.Z.m.Z.
-000000b0: 0100 4700 6409 640a 8400 640a 6514 8303  ..G.d.d...d.e...
-000000c0: 5a19 6403 5300 290b e900 0000 0029 01da  Z.d.S.)......)..
-000000d0: 0864 6565 7063 6f70 7929 05da 0341 6e79  .deepcopy)...Any
-000000e0: da07 4c69 7465 7261 6cda 0853 6571 7565  ..Literal..Seque
-000000f0: 6e63 65da 0554 7570 6c65 da05 556e 696f  nce..Tuple..Unio
-00000100: 6e4e 2902 da05 416e 676c 65da 0853 6b79  nN)...Angle..Sky
-00000110: 436f 6f72 6429 01da 0757 4353 4178 6573  Coord)...WCSAxes
-00000120: 2901 da03 5743 5329 01da 0a41 6e6e 6f74  )...WCS)...Annot
-00000130: 6174 696f 6e29 03da 0672 6f74 6174 65da  ation)...rotate.
-00000140: 1573 6b79 5f70 6f73 6974 696f 6e5f 746f  .sky_position_to
-00000150: 5f70 6978 656c da09 7472 616e 736c 6174  _pixel..translat
-00000160: 6563 0000 0000 0000 0000 0000 0000 0000  ec..............
-00000170: 0000 1100 0000 4000 0000 73ae 0000 0065  ......@...s....e
-00000180: 005a 0164 005a 0264 015a 0309 0209 0309  .Z.d.Z.d.Z......
-00000190: 0309 0464 1d64 0565 0465 0565 0665 0719  ...d.d.e.e.e.e..
-000001a0: 0065 086a 0965 0a6a 0b19 0066 0319 0064  .e.j.e.j...f...d
-000001b0: 0665 0c64 0765 0d64 0865 0465 0c65 0e65  .e.d.e.d.e.e.e.e
-000001c0: 0765 0765 0766 0319 0066 0219 0064 0965  .e.e.f...f...d.e
-000001d0: 0f64 0a19 0064 0b65 0f64 0c19 0064 0d65  .d...d.e.d...d.e
-000001e0: 1064 0e65 1166 1064 0f64 1084 055a 1264  .d.e.f.d.d...Z.d
-000001f0: 1165 1364 1264 1366 0464 1464 1584 045a  .e.d.d.f.d.d...Z
-00000200: 1464 1665 0564 1765 1564 1264 0066 0664  .d.e.d.e.d.d.f.d
-00000210: 1864 1984 045a 1664 1a65 1564 1264 0066  .d...Z.d.e.d.d.f
-00000220: 0464 1b64 1c84 045a 1764 1353 0029 1eda  .d.d...Z.d.S.)..
-00000230: 0e54 6578 7441 6e6e 6f74 6174 696f 6e61  .TextAnnotationa
-00000240: f405 0000 416e 2061 6e6e 6f74 6174 696f  ....An annotatio
-00000250: 6e20 666f 7220 6164 6469 6e67 2074 6578  n for adding tex
-00000260: 7420 746f 2061 2070 6c6f 742e 0a0a 2020  t to a plot...  
-00000270: 2020 5468 6520 7465 7874 2070 6f73 6974    The text posit
-00000280: 696f 6e20 6361 6e20 6265 2073 7065 6369  ion can be speci
-00000290: 6669 6564 2061 7320 6120 706f 7369 7469  fied as a positi
-000002a0: 6f6e 206f 6e20 7468 6520 736b 7920 2861  on on the sky (a
-000002b0: 7320 616e 2069 6e73 7461 6e63 6520 6f66  s an instance of
-000002c0: 0a20 2020 2060 7e61 7374 726f 7079 2e63  .    `~astropy.c
-000002d0: 6f6f 7264 696e 6174 6573 2e53 6b79 436f  oordinates.SkyCo
-000002e0: 6f72 6460 2920 6f72 2061 7320 6120 706f  ord`) or as a po
-000002f0: 696e 7420 696e 2061 7865 7320 636f 6f72  int in axes coor
-00000300: 6469 6e61 7465 7320 2861 7320 616e 2061  dinates (as an a
-00000310: 7272 6179 206f 660a 2020 2020 6066 6c6f  rray of.    `flo
-00000320: 6174 6020 7661 6c75 6573 2e20 4178 6573  at` values. Axes
-00000330: 2063 6f6f 7264 696e 6174 6573 2072 616e   coordinates ran
-00000340: 6765 2066 726f 6d20 2830 2c20 3029 2028  ge from (0, 0) (
-00000350: 626f 7474 6f6d 206c 6566 7420 6f66 2074  bottom left of t
-00000360: 6865 2061 7865 7329 2074 6f0a 2020 2020  he axes) to.    
-00000370: 2831 2c20 3129 2028 746f 7020 7269 6768  (1, 1) (top righ
-00000380: 7420 6f66 2074 6865 2061 7865 7329 2e0a  t of the axes)..
-00000390: 0a20 2020 2059 6f75 2063 616e 206f 6e6c  .    You can onl
-000003a0: 7920 726f 7461 7465 2061 6e64 2074 7261  y rotate and tra
-000003b0: 6e73 6c61 7465 2074 6865 2061 6e6e 6f74  nslate the annot
-000003c0: 6174 696f 6e20 6966 2074 6865 2074 6578  ation if the tex
-000003d0: 7420 706f 7369 7469 6f6e 2069 7320 7370  t position is sp
-000003e0: 6563 6966 6965 640a 2020 2020 6173 2061  ecified.    as a
-000003f0: 2070 6f73 6974 696f 6e20 6f6e 2074 6865   position on the
-00000400: 2073 6b79 2e0a 0a20 2020 202e 2e20 6e6f   sky...    .. no
-00000410: 7465 3a3a 0a20 2020 2020 2020 2054 6865  te::.        The
-00000420: 2060 726f 7461 7465 6020 6d65 7468 6f64   `rotate` method
-00000430: 2072 6f74 6174 6573 2074 6865 2074 6578   rotates the tex
-00000440: 7420 706f 7369 7469 6f6e 2c20 6275 7420  t position, but 
-00000450: 6e6f 7420 7468 6520 7465 7874 2069 7473  not the text its
-00000460: 656c 662e 2049 6620 796f 750a 2020 2020  elf. If you.    
-00000470: 2020 2020 7761 6e74 2074 6f20 726f 7461      want to rota
-00000480: 7465 2074 6865 2074 6578 7420 7261 7468  te the text rath
-00000490: 6572 2074 6861 6e20 7468 6520 7465 7874  er than the text
-000004a0: 2070 6f73 6974 696f 6e2c 2079 6f75 2073   position, you s
-000004b0: 686f 756c 6420 7573 6520 7468 650a 2020  hould use the.  
-000004c0: 2020 2020 2020 6060 726f 7461 7469 6f6e        ``rotation
-000004d0: 6060 2070 6172 616d 6574 6572 2077 6974  `` parameter wit
-000004e0: 6820 7468 6520 616e 676c 6520 696e 2064  h the angle in d
-000004f0: 6567 7265 6573 2e0a 0a0a 2020 2020 5061  egrees....    Pa
-00000500: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00000510: 2d2d 2d2d 2d2d 2d0a 2020 2020 706f 7369  -------.    posi
-00000520: 7469 6f6e 3a20 607e 6173 7472 6f70 792e  tion: `~astropy.
-00000530: 636f 6f72 6469 6e61 7465 732e 536b 7943  coordinates.SkyC
-00000540: 6f6f 7264 6020 6f72 0a20 2020 2020 2020  oord` or.       
-00000550: 2054 6865 2072 6967 6874 2061 7363 656e   The right ascen
-00000560: 7369 6f6e 2061 6e64 2064 6563 6c69 6e61  sion and declina
-00000570: 7469 6f6e 206f 6620 7468 6520 706f 696e  tion of the poin
-00000580: 7420 7768 6572 6520 746f 2070 7574 2074  t where to put t
-00000590: 6865 2074 6578 742e 0a20 2020 2073 3a20  he text..    s: 
-000005a0: 7374 720a 2020 2020 2020 2020 5468 6520  str.        The 
-000005b0: 7465 7874 2e0a 2020 2020 7763 733a 2060  text..    wcs: `
-000005c0: 7e61 7374 726f 7079 2e77 6373 2e57 4353  ~astropy.wcs.WCS
-000005d0: 600a 2020 2020 2020 2020 5743 5320 6f62  `.        WCS ob
-000005e0: 6a65 6374 2e0a 2020 2020 636f 6c6f 723a  ject..    color:
-000005f0: 2063 6f6c 6f72 2c20 6465 6661 756c 743a   color, default:
-00000600: 2022 626c 6163 6b22 0a20 2020 2020 2020   "black".       
-00000610: 2054 6865 2074 6578 7420 636f 6c6f 722e   The text color.
-00000620: 0a20 2020 2068 6f72 697a 6f6e 7461 6c61  .    horizontala
-00000630: 6c69 676e 6d65 6e74 3a20 7b22 6365 6e74  lignment: {"cent
-00000640: 6572 222c 2022 6c65 6674 222c 2022 7269  er", "left", "ri
-00000650: 6768 7422 7d2c 2064 6566 6175 6c74 3a20  ght"}, default: 
-00000660: 2263 656e 7465 7222 0a20 2020 2020 2020  "center".       
-00000670: 2054 6865 2068 6f72 697a 6f6e 7461 6c20   The horizontal 
-00000680: 616c 6967 6e6d 656e 7420 6f66 2074 6865  alignment of the
-00000690: 2074 6578 742e 0a20 2020 2076 6572 7469   text..    verti
-000006a0: 6361 6c61 6c69 676e 6d65 6e74 3a20 7b22  calalignment: {"
-000006b0: 6261 7365 6c69 6e65 222c 2022 626f 7474  baseline", "bott
-000006c0: 6f6d 222c 2022 6365 6e74 6572 222c 2022  om", "center", "
-000006d0: 6365 6e74 6572 5f62 6173 656c 696e 6522  center_baseline"
-000006e0: 2c20 2274 6f70 227d 2c20 6465 6661 756c  , "top"}, defaul
-000006f0: 743a 2022 6365 6e74 6572 220a 2020 2020  t: "center".    
-00000700: 2020 2020 5468 6520 7665 7274 6963 616c      The vertical
-00000710: 2061 6c69 676e 6d65 6e74 206f 6620 7468   alignment of th
-00000720: 6520 7465 7874 2e0a 2020 2020 636c 6970  e text..    clip
-00000730: 5f6f 6e3a 2062 6f6f 6c2c 2064 6566 6175  _on: bool, defau
-00000740: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
-00000750: 2057 6865 7468 6572 2074 6f20 636c 6970   Whether to clip
-00000760: 2074 6865 2074 6578 7420 6174 2074 6865   the text at the
-00000770: 2070 6c6f 7420 626f 756e 6461 7269 6573   plot boundaries
-00000780: 2e0a 2020 2020 2a2a 6b77 6172 6773 3a20  ..    **kwargs: 
-00000790: 6469 6374 2c20 6f70 7469 6f6e 616c 0a20  dict, optional. 
-000007a0: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
-000007b0: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-000007c0: 6e74 732c 2077 6869 6368 2077 696c 6c20  nts, which will 
-000007d0: 6265 2070 6173 7365 6420 746f 204d 6174  be passed to Mat
-000007e0: 706c 6f74 6c69 6227 730a 2020 2020 2020  plotlib's.      
-000007f0: 2020 607e 6d61 7470 6c6f 746c 6962 2e61    `~matplotlib.a
-00000800: 7865 732e 4178 6573 2e74 6578 7460 206d  xes.Axes.text` m
-00000810: 6574 686f 6420 666f 7220 6164 6469 6e67  ethod for adding
-00000820: 2074 6578 7420 746f 2070 6c6f 7420 4178   text to plot Ax
-00000830: 6573 2e0a 2020 2020 da05 626c 6163 6bda  es..    ..black.
-00000840: 0663 656e 7465 7254 da08 706f 7369 7469  .centerT..positi
-00000850: 6f6e da01 73da 0377 6373 da05 636f 6c6f  on..s..wcs..colo
-00000860: 72da 1368 6f72 697a 6f6e 7461 6c61 6c69  r..horizontalali
-00000870: 676e 6d65 6e74 2903 7212 0000 00da 046c  gnment).r......l
-00000880: 6566 74da 0572 6967 6874 da11 7665 7274  eft..right..vert
-00000890: 6963 616c 616c 6967 6e6d 656e 7429 05da  icalalignment)..
-000008a0: 0862 6173 656c 696e 65da 0662 6f74 746f  .baseline..botto
-000008b0: 6d72 1200 0000 da0f 6365 6e74 6572 5f62  mr......center_b
-000008c0: 6173 656c 696e 65da 0374 6f70 da07 636c  aseline..top..cl
-000008d0: 6970 5f6f 6eda 066b 7761 7267 7363 0800  ip_on..kwargsc..
-000008e0: 0000 0000 0000 0000 0000 0900 0000 0300  ................
-000008f0: 0000 4b00 0000 7348 0000 007c 017c 005f  ..K...sH...|.|._
-00000900: 007c 027c 005f 017c 037c 005f 0274 037c  .|.|._.|.|._.t.|
-00000910: 0883 017c 005f 047c 047c 006a 0464 013c  ...|._.|.|.j.d.<
-00000920: 007c 057c 006a 0464 023c 007c 067c 006a  .|.|.j.d.<.|.|.j
-00000930: 0464 033c 007c 077c 006a 0464 043c 0064  .d.<.|.|.j.d.<.d
-00000940: 0053 0029 054e 7216 0000 0072 1700 0000  .S.).Nr....r....
-00000950: 721a 0000 0072 1f00 0000 2905 da09 5f70  r....r....)..._p
-00000960: 6f73 6974 696f 6eda 025f 73da 045f 7763  osition.._s.._wc
-00000970: 7372 0200 0000 da07 5f6b 7761 7267 7329  sr......_kwargs)
-00000980: 09da 0473 656c 6672 1300 0000 7214 0000  ...selfr....r...
-00000990: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-000009a0: 721a 0000 0072 1f00 0000 7220 0000 00a9  r....r....r ....
-000009b0: 0072 2600 0000 fa4a 2f55 7365 7273 2f63  .r&....J/Users/c
-000009c0: 6872 6973 7469 616e 2f49 6465 6150 726f  hristian/IdeaPro
-000009d0: 6a65 6374 732f 696d 6570 6875 2f73 7263  jects/imephu/src
-000009e0: 2f69 6d65 7068 752f 616e 6e6f 7461 7469  /imephu/annotati
-000009f0: 6f6e 2f67 656e 6572 616c 2f74 6578 742e  on/general/text.
-00000a00: 7079 da08 5f5f 696e 6974 5f5f 3400 0000  py..__init__4...
-00000a10: 7310 0000 0006 0d06 0106 010a 010a 010a  s...............
-00000a20: 010a 010e 017a 1754 6578 7441 6e6e 6f74  .....z.TextAnnot
-00000a30: 6174 696f 6e2e 5f5f 696e 6974 5f5f da02  ation.__init__..
-00000a40: 6178 da06 7265 7475 726e 4e63 0200 0000  ax..returnNc....
-00000a50: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000a60: 4300 0000 7372 0000 0074 007c 006a 0183  C...sr...t.|.j..
-00000a70: 0174 026b 0272 2174 037c 006a 017c 006a  .t.k.r!t.|.j.|.j
-00000a80: 0483 027d 027c 016a 057c 0264 0119 007c  ...}.|.j.|.d...|
-00000a90: 0264 0219 007c 006a 0666 0369 007c 006a  .d...|.j.f.i.|.j
-00000aa0: 07a4 018e 0101 0064 0453 007c 016a 057c  .......d.S.|.j.|
-00000ab0: 006a 0164 0119 007c 006a 0164 0219 007c  .j.d...|.j.d...|
-00000ac0: 006a 0666 0364 037c 016a 0869 017c 006a  .j.f.d.|.j.i.|.j
-00000ad0: 07a4 018e 0101 0064 0453 0029 057a 7c41  .......d.S.).z|A
-00000ae0: 6464 2074 6865 2074 6578 7420 746f 2061  dd the text to a
-00000af0: 2066 696e 6465 7220 6368 6172 742e 0a0a   finder chart...
-00000b00: 2020 2020 2020 2020 6178 3a20 2060 7e61          ax:  `~a
-00000b10: 7374 726f 7079 2e76 6973 7561 6c69 7a61  stropy.visualiza
-00000b20: 7469 6f6e 2e77 6373 6178 6573 2e57 4353  tion.wcsaxes.WCS
-00000b30: 4178 6573 600a 2020 2020 2020 2020 2020  Axes`.          
-00000b40: 2020 5743 5320 6178 6573 206f 626a 6563    WCS axes objec
-00000b50: 742e 0a20 2020 2020 2020 2072 0100 0000  t..        r....
-00000b60: e901 0000 00da 0974 7261 6e73 666f 726d  .......transform
-00000b70: 4e29 09da 0474 7970 6572 2100 0000 7209  N)...typer!...r.
-00000b80: 0000 0072 0e00 0000 7223 0000 00da 0474  ...r....r#.....t
-00000b90: 6578 7472 2200 0000 7224 0000 00da 0974  extr"...r$.....t
-00000ba0: 7261 6e73 4178 6573 2903 7225 0000 0072  ransAxes).r%...r
-00000bb0: 2900 0000 da0b 706f 7369 7469 6f6e 5f70  ).....position_p
-00000bc0: 7872 2600 0000 7226 0000 0072 2700 0000  xr&...r&...r'...
-00000bd0: da06 6164 645f 746f 4a00 0000 7318 0000  ..add_toJ...s...
-00000be0: 000e 060e 0126 0104 0208 0108 0104 0104  .....&..........
-00000bf0: fd04 0402 fc04 050a fb7a 1554 6578 7441  .........z.TextA
-00000c00: 6e6e 6f74 6174 696f 6e2e 6164 645f 746f  nnotation.add_to
-00000c10: da05 7069 766f 74da 0561 6e67 6c65 6303  ..pivot..anglec.
-00000c20: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00000c30: 0000 0043 0000 0073 3a00 0000 7400 7c00  ...C...s:...t.|.
-00000c40: 6a01 8301 7402 7501 720b 7403 6401 8301  j...t.u.r.t.d...
-00000c50: 8201 7404 7c00 8301 7d03 7405 7c00 6a01  ..t.|...}.t.|.j.
-00000c60: 7c01 7c02 7c00 6a06 8304 7d04 7c04 7c03  |.|.|.j...}.|.|.
-00000c70: 5f01 7c03 5300 2903 611a 0200 0052 6f74  _.|.S.).a....Rot
-00000c80: 6174 6520 7468 6973 2061 6e6e 6f74 6174  ate this annotat
-00000c90: 696f 6e20 6172 6f75 6e64 2061 2070 6976  ion around a piv
-00000ca0: 6f74 2061 6e64 2072 6574 7572 6e20 7468  ot and return th
-00000cb0: 6520 7265 7375 6c74 2e0a 0a20 2020 2020  e result...     
-00000cc0: 2020 2054 6865 2072 6f74 6174 696f 6e20     The rotation 
-00000cd0: 616e 676c 6520 6973 2061 6e20 616e 676c  angle is an angl
-00000ce0: 6520 6f6e 2074 6865 2073 6b79 2c20 6d65  e on the sky, me
-00000cf0: 6173 7572 6564 2066 726f 6d20 6e6f 7274  asured from nort
-00000d00: 6820 746f 2065 6173 742e 0a0a 2020 2020  h to east...    
-00000d10: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000d20: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00000d30: 2d0a 2020 2020 2020 2020 7069 766f 743a  -.        pivot:
-00000d40: 2060 7e61 7374 726f 7079 2e63 6f6f 7264   `~astropy.coord
-00000d50: 696e 6174 6573 2e53 6b79 436f 6f72 6460  inates.SkyCoord`
-00000d60: 0a20 2020 2020 2020 2020 2020 2050 6f69  .            Poi
-00000d70: 6e74 2061 726f 756e 6420 7768 6963 6820  nt around which 
-00000d80: 746f 2072 6f74 6174 6520 7468 6520 616e  to rotate the an
-00000d90: 6e6f 7461 7469 6f6e 2e0a 2020 2020 2020  notation..      
-00000da0: 2020 616e 676c 653a 2060 7e61 7374 726f    angle: `~astro
-00000db0: 7079 2e63 6f6f 7264 696e 6174 6573 2e41  py.coordinates.A
-00000dc0: 6e67 6c65 600a 2020 2020 2020 2020 2020  ngle`.          
-00000dd0: 2020 416e 676c 6520 6f66 2072 6f74 6174    Angle of rotat
-00000de0: 696f 6e2c 206d 6561 7375 7265 6420 6672  ion, measured fr
-00000df0: 6f6d 206e 6f72 7468 2074 6f20 6561 7374  om north to east
-00000e00: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00000e10: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00000e20: 2d2d 0a20 2020 2020 2020 2060 7e69 6d65  --.        `~ime
-00000e30: 7068 752e 616e 6e6f 7461 7469 6f6e 2e67  phu.annotation.g
-00000e40: 656e 6572 616c 2e54 6578 7441 6e6e 6f74  eneral.TextAnnot
-00000e50: 6174 696f 6e60 0a20 2020 2020 2020 2020  ation`.         
-00000e60: 2020 2054 6865 2061 6e6e 6f74 6174 696f     The annotatio
-00000e70: 6e20 7265 7375 6c74 696e 6720 6672 6f6d  n resulting from
-00000e80: 2074 6865 2072 6f74 6174 696f 6e2e 0a20   the rotation.. 
-00000e90: 2020 2020 2020 207a 5654 6865 2074 6578         zVThe tex
-00000ea0: 7420 6361 6e20 6f6e 6c79 2062 6520 726f  t can only be ro
-00000eb0: 7461 7465 6420 6966 2069 7473 2070 6f73  tated if its pos
-00000ec0: 6974 696f 6e20 6973 2061 6e20 696e 7374  ition is an inst
-00000ed0: 616e 6365 206f 6620 6173 7472 6f70 792e  ance of astropy.
-00000ee0: 636f 6f72 642e 536b 7943 6f6f 7264 2e4e  coord.SkyCoord.N
-00000ef0: 2907 722d 0000 0072 2100 0000 7209 0000  ).r-...r!...r...
-00000f00: 00da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
-00000f10: 6445 7272 6f72 7202 0000 0072 0d00 0000  dErrorr....r....
-00000f20: 7223 0000 0029 0572 2500 0000 7232 0000  r#...).r%...r2..
-00000f30: 0072 3300 0000 da12 726f 7461 7465 645f  .r3.....rotated_
-00000f40: 616e 6e6f 7461 7469 6f6e 5a10 726f 7461  annotationZ.rota
-00000f50: 7465 645f 706f 7369 7469 6f6e 7226 0000  ted_positionr&..
-00000f60: 0072 2600 0000 7227 0000 0072 0d00 0000  .r&...r'...r....
-00000f70: 5c00 0000 7310 0000 000e 1102 0102 0104  \...s...........
-00000f80: ff08 0412 0106 0104 017a 1554 6578 7441  .........z.TextA
-00000f90: 6e6e 6f74 6174 696f 6e2e 726f 7461 7465  nnotation.rotate
-00000fa0: da0c 6469 7370 6c61 6365 6d65 6e74 6302  ..displacementc.
-00000fb0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00000fc0: 0000 0043 0000 0073 3400 0000 7400 7c00  ...C...s4...t.|.
-00000fd0: 6a01 8301 7402 7501 720b 7403 6401 8301  j...t.u.r.t.d...
-00000fe0: 8201 7404 7c00 8301 7d02 7405 7c00 6a01  ..t.|...}.t.|.j.
-00000ff0: 7c01 8302 7d03 7c03 7c02 5f01 7c02 5300  |...}.|.|._.|.S.
-00001000: 2903 6177 0100 000a 2020 2020 2020 2020  ).aw....        
-00001010: 4d6f 7665 2074 6869 7320 616e 6e6f 7461  Move this annota
-00001020: 7469 6f6e 2061 6c6f 6e67 2061 2064 6973  tion along a dis
-00001030: 706c 6163 656d 656e 7420 7665 6374 6f72  placement vector
-00001040: 2061 6e64 2072 6574 7572 6e20 7468 6520   and return the 
-00001050: 7265 7375 6c74 2e0a 0a20 2020 2020 2020  result...       
-00001060: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00001070: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00001080: 2020 2020 2020 2064 6973 706c 6163 656d         displacem
-00001090: 656e 743a 2032 4420 6172 7261 7920 6f66  ent: 2D array of
-000010a0: 2061 6e67 6c65 730a 2020 2020 2020 2020   angles.        
-000010b0: 2020 2020 5468 6520 6469 7370 6c61 6365      The displace
-000010c0: 6d65 6e74 2062 7920 7768 6963 6820 746f  ment by which to
-000010d0: 206d 6f76 6520 7468 6520 616e 6e6f 7461   move the annota
-000010e0: 7469 6f6e 2e0a 0a20 2020 2020 2020 2052  tion...        R
-000010f0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00001100: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2060  ------.        `
-00001110: 7e69 6d65 7068 752e 616e 6e6f 7461 7469  ~imephu.annotati
-00001120: 6f6e 2e67 656e 6572 616c 2e54 6578 7441  on.general.TextA
-00001130: 6e6e 6f74 6174 696f 6e60 0a20 2020 2020  nnotation`.     
-00001140: 2020 2020 2020 2054 6865 2061 6e6e 6f74         The annot
-00001150: 6174 696f 6e20 7265 7375 6c74 696e 6720  ation resulting 
-00001160: 6672 6f6d 2074 6865 2074 7261 6e73 6c61  from the transla
-00001170: 7469 6f6e 2e0a 2020 2020 2020 2020 7a59  tion..        zY
-00001180: 5468 6520 7465 7874 2063 616e 206f 6e6c  The text can onl
-00001190: 7920 6265 2074 7261 6e73 6c61 7465 6420  y be translated 
-000011a0: 6966 2069 7473 2070 6f73 6974 696f 6e20  if its position 
-000011b0: 6973 2061 6e20 696e 7374 616e 6365 206f  is an instance o
-000011c0: 6620 6173 7472 6f70 792e 636f 6f72 642e  f astropy.coord.
-000011d0: 536b 7943 6f6f 7264 2e4e 2906 722d 0000  SkyCoord.N).r-..
-000011e0: 0072 2100 0000 7209 0000 0072 3400 0000  .r!...r....r4...
-000011f0: 7202 0000 0072 0f00 0000 2904 7225 0000  r....r....).r%..
-00001200: 0072 3600 0000 da15 7472 616e 736c 6174  .r6.....translat
-00001210: 6564 5f61 6e6e 6f74 6174 696f 6e5a 1374  ed_annotationZ.t
-00001220: 7261 6e73 6c61 7465 645f 706f 7369 7469  ranslated_positi
-00001230: 6f6e 7226 0000 0072 2600 0000 7227 0000  onr&...r&...r'..
-00001240: 0072 0f00 0000 7700 0000 7310 0000 000e  .r....w...s.....
-00001250: 0e02 0102 0104 ff08 040c 0106 0104 017a  ...............z
-00001260: 1854 6578 7441 6e6e 6f74 6174 696f 6e2e  .TextAnnotation.
-00001270: 7472 616e 736c 6174 6529 0472 1100 0000  translate).r....
-00001280: 7212 0000 0072 1200 0000 5429 18da 085f  r....r....T)..._
-00001290: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000012a0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000012b0: 5fda 075f 5f64 6f63 5f5f 7207 0000 0072  _..__doc__r....r
-000012c0: 0900 0000 7205 0000 00da 0566 6c6f 6174  ....r......float
-000012d0: da03 6e70 74da 074e 4441 7272 6179 da02  ..npt..NDArray..
-000012e0: 6e70 da06 666c 6f61 745f da03 7374 7272  np..float_..strr
-000012f0: 0b00 0000 7206 0000 0072 0400 0000 da04  ....r....r......
-00001300: 626f 6f6c 7203 0000 0072 2800 0000 720a  boolr....r(...r.
-00001310: 0000 0072 3100 0000 7208 0000 0072 0d00  ...r1...r....r..
-00001320: 0000 720f 0000 0072 2600 0000 7226 0000  ..r....r&...r&..
-00001330: 0072 2600 0000 7227 0000 0072 1000 0000  .r&...r'...r....
-00001340: 0e00 0000 7338 0000 0008 0004 0102 2a02  ....s8........*.
-00001350: 0102 0302 0104 f618 0202 fe02 0302 fd02  ................
-00001360: 0402 fc14 0502 fb06 0602 fa02 0702 0102  ................
-00001370: ff02 f902 0a02 f602 0b0a f512 1616 1216  ................
-00001380: 1b72 1000 0000 291a da04 636f 7079 7202  .r....)...copyr.
-00001390: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
-000013a0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-000013b0: 0700 0000 da05 6e75 6d70 7972 3f00 0000  ......numpyr?...
-000013c0: da0c 6e75 6d70 792e 7479 7069 6e67 723d  ..numpy.typingr=
-000013d0: 0000 00da 1361 7374 726f 7079 2e63 6f6f  .....astropy.coo
-000013e0: 7264 696e 6174 6573 7208 0000 0072 0900  rdinatesr....r..
-000013f0: 0000 da1d 6173 7472 6f70 792e 7669 7375  ....astropy.visu
-00001400: 616c 697a 6174 696f 6e2e 7763 7361 7865  alization.wcsaxe
-00001410: 7372 0a00 0000 da0b 6173 7472 6f70 792e  sr......astropy.
-00001420: 7763 7372 0b00 0000 5a11 696d 6570 6875  wcsr....Z.imephu
-00001430: 2e61 6e6e 6f74 6174 696f 6e72 0c00 0000  .annotationr....
-00001440: da0f 696d 6570 6875 2e67 656f 6d65 7472  ..imephu.geometr
-00001450: 7972 0d00 0000 720e 0000 0072 0f00 0000  yr....r....r....
-00001460: 7210 0000 0072 2600 0000 7226 0000 0072  r....r&...r&...r
-00001470: 2600 0000 7227 0000 00da 083c 6d6f 6475  &...r'.....<modu
-00001480: 6c65 3e01 0000 0073 1400 0000 0c00 1c01  le>....s........
-00001490: 0802 0c01 1001 0c01 0c01 0c02 1401 1403  ................
+00000000: 6672 6f6d 2063 6f70 7920 696d 706f 7274  from copy import
+00000010: 2064 6565 7063 6f70 790a 6672 6f6d 2074   deepcopy.from t
+00000020: 7970 696e 6720 696d 706f 7274 2041 6e79  yping import Any
+00000030: 2c20 4c69 7465 7261 6c2c 2053 6571 7565  , Literal, Seque
+00000040: 6e63 652c 2054 7570 6c65 2c20 556e 696f  nce, Tuple, Unio
+00000050: 6e0a 0a69 6d70 6f72 7420 6e75 6d70 7920  n..import numpy 
+00000060: 6173 206e 700a 696d 706f 7274 206e 756d  as np.import num
+00000070: 7079 2e74 7970 696e 6720 6173 206e 7074  py.typing as npt
+00000080: 0a66 726f 6d20 6173 7472 6f70 792e 636f  .from astropy.co
+00000090: 6f72 6469 6e61 7465 7320 696d 706f 7274  ordinates import
+000000a0: 2041 6e67 6c65 2c20 536b 7943 6f6f 7264   Angle, SkyCoord
+000000b0: 0a66 726f 6d20 6173 7472 6f70 792e 7669  .from astropy.vi
+000000c0: 7375 616c 697a 6174 696f 6e2e 7763 7361  sualization.wcsa
+000000d0: 7865 7320 696d 706f 7274 2057 4353 4178  xes import WCSAx
+000000e0: 6573 0a66 726f 6d20 6173 7472 6f70 792e  es.from astropy.
+000000f0: 7763 7320 696d 706f 7274 2057 4353 0a0a  wcs import WCS..
+00000100: 6672 6f6d 2069 6d65 7068 752e 616e 6e6f  from imephu.anno
+00000110: 7461 7469 6f6e 2069 6d70 6f72 7420 416e  tation import An
+00000120: 6e6f 7461 7469 6f6e 0a66 726f 6d20 696d  notation.from im
+00000130: 6570 6875 2e67 656f 6d65 7472 7920 696d  ephu.geometry im
+00000140: 706f 7274 2072 6f74 6174 652c 2073 6b79  port rotate, sky
+00000150: 5f70 6f73 6974 696f 6e5f 746f 5f70 6978  _position_to_pix
+00000160: 656c 2c20 7472 616e 736c 6174 650a 0a0a  el, translate...
+00000170: 636c 6173 7320 5465 7874 416e 6e6f 7461  class TextAnnota
+00000180: 7469 6f6e 2841 6e6e 6f74 6174 696f 6e29  tion(Annotation)
+00000190: 3a0a 2020 2020 2222 2241 6e20 616e 6e6f  :.    """An anno
+000001a0: 7461 7469 6f6e 2066 6f72 2061 6464 696e  tation for addin
+000001b0: 6720 7465 7874 2074 6f20 6120 706c 6f74  g text to a plot
+000001c0: 2e0a 0a20 2020 2054 6865 2074 6578 7420  ...    The text 
+000001d0: 706f 7369 7469 6f6e 2063 616e 2062 6520  position can be 
+000001e0: 7370 6563 6966 6965 6420 6173 2061 2070  specified as a p
+000001f0: 6f73 6974 696f 6e20 6f6e 2074 6865 2073  osition on the s
+00000200: 6b79 2028 6173 2061 6e20 696e 7374 616e  ky (as an instan
+00000210: 6365 206f 660a 2020 2020 607e 6173 7472  ce of.    `~astr
+00000220: 6f70 792e 636f 6f72 6469 6e61 7465 732e  opy.coordinates.
+00000230: 536b 7943 6f6f 7264 6029 206f 7220 6173  SkyCoord`) or as
+00000240: 2061 2070 6f69 6e74 2069 6e20 6178 6573   a point in axes
+00000250: 2063 6f6f 7264 696e 6174 6573 2028 6173   coordinates (as
+00000260: 2061 6e20 6172 7261 7920 6f66 0a20 2020   an array of.   
+00000270: 2060 666c 6f61 7460 2076 616c 7565 732e   `float` values.
+00000280: 2041 7865 7320 636f 6f72 6469 6e61 7465   Axes coordinate
+00000290: 7320 7261 6e67 6520 6672 6f6d 2028 302c  s range from (0,
+000002a0: 2030 2920 2862 6f74 746f 6d20 6c65 6674   0) (bottom left
+000002b0: 206f 6620 7468 6520 6178 6573 2920 746f   of the axes) to
+000002c0: 0a20 2020 2028 312c 2031 2920 2874 6f70  .    (1, 1) (top
+000002d0: 2072 6967 6874 206f 6620 7468 6520 6178   right of the ax
+000002e0: 6573 292e 0a0a 2020 2020 596f 7520 6361  es)...    You ca
+000002f0: 6e20 6f6e 6c79 2072 6f74 6174 6520 616e  n only rotate an
+00000300: 6420 7472 616e 736c 6174 6520 7468 6520  d translate the 
+00000310: 616e 6e6f 7461 7469 6f6e 2069 6620 7468  annotation if th
+00000320: 6520 7465 7874 2070 6f73 6974 696f 6e20  e text position 
+00000330: 6973 2073 7065 6369 6669 6564 0a20 2020  is specified.   
+00000340: 2061 7320 6120 706f 7369 7469 6f6e 206f   as a position o
+00000350: 6e20 7468 6520 736b 792e 0a0a 2020 2020  n the sky...    
+00000360: 2e2e 206e 6f74 653a 3a0a 2020 2020 2020  .. note::.      
+00000370: 2020 5468 6520 6072 6f74 6174 6560 206d    The `rotate` m
+00000380: 6574 686f 6420 726f 7461 7465 7320 7468  ethod rotates th
+00000390: 6520 7465 7874 2070 6f73 6974 696f 6e2c  e text position,
+000003a0: 2062 7574 206e 6f74 2074 6865 2074 6578   but not the tex
+000003b0: 7420 6974 7365 6c66 2e20 4966 2079 6f75  t itself. If you
+000003c0: 0a20 2020 2020 2020 2077 616e 7420 746f  .        want to
+000003d0: 2072 6f74 6174 6520 7468 6520 7465 7874   rotate the text
+000003e0: 2072 6174 6865 7220 7468 616e 2074 6865   rather than the
+000003f0: 2074 6578 7420 706f 7369 7469 6f6e 2c20   text position, 
+00000400: 796f 7520 7368 6f75 6c64 2075 7365 2074  you should use t
+00000410: 6865 0a20 2020 2020 2020 2060 6072 6f74  he.        ``rot
+00000420: 6174 696f 6e60 6020 7061 7261 6d65 7465  ation`` paramete
+00000430: 7220 7769 7468 2074 6865 2061 6e67 6c65  r with the angle
+00000440: 2069 6e20 6465 6772 6565 732e 0a0a 0a20   in degrees.... 
+00000450: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00000460: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00000470: 2070 6f73 6974 696f 6e3a 2060 7e61 7374   position: `~ast
+00000480: 726f 7079 2e63 6f6f 7264 696e 6174 6573  ropy.coordinates
+00000490: 2e53 6b79 436f 6f72 6460 206f 720a 2020  .SkyCoord` or.  
+000004a0: 2020 2020 2020 5468 6520 7269 6768 7420        The right 
+000004b0: 6173 6365 6e73 696f 6e20 616e 6420 6465  ascension and de
+000004c0: 636c 696e 6174 696f 6e20 6f66 2074 6865  clination of the
+000004d0: 2070 6f69 6e74 2077 6865 7265 2074 6f20   point where to 
+000004e0: 7075 7420 7468 6520 7465 7874 2e0a 2020  put the text..  
+000004f0: 2020 733a 2073 7472 0a20 2020 2020 2020    s: str.       
+00000500: 2054 6865 2074 6578 742e 0a20 2020 2077   The text..    w
+00000510: 6373 3a20 607e 6173 7472 6f70 792e 7763  cs: `~astropy.wc
+00000520: 732e 5743 5360 0a20 2020 2020 2020 2057  s.WCS`.        W
+00000530: 4353 206f 626a 6563 742e 0a20 2020 2063  CS object..    c
+00000540: 6f6c 6f72 3a20 636f 6c6f 722c 2064 6566  olor: color, def
+00000550: 6175 6c74 3a20 2262 6c61 636b 220a 2020  ault: "black".  
+00000560: 2020 2020 2020 5468 6520 7465 7874 2063        The text c
+00000570: 6f6c 6f72 2e0a 2020 2020 686f 7269 7a6f  olor..    horizo
+00000580: 6e74 616c 616c 6967 6e6d 656e 743a 207b  ntalalignment: {
+00000590: 2263 656e 7465 7222 2c20 226c 6566 7422  "center", "left"
+000005a0: 2c20 2272 6967 6874 227d 2c20 6465 6661  , "right"}, defa
+000005b0: 756c 743a 2022 6365 6e74 6572 220a 2020  ult: "center".  
+000005c0: 2020 2020 2020 5468 6520 686f 7269 7a6f        The horizo
+000005d0: 6e74 616c 2061 6c69 676e 6d65 6e74 206f  ntal alignment o
+000005e0: 6620 7468 6520 7465 7874 2e0a 2020 2020  f the text..    
+000005f0: 7665 7274 6963 616c 616c 6967 6e6d 656e  verticalalignmen
+00000600: 743a 207b 2262 6173 656c 696e 6522 2c20  t: {"baseline", 
+00000610: 2262 6f74 746f 6d22 2c20 2263 656e 7465  "bottom", "cente
+00000620: 7222 2c20 2263 656e 7465 725f 6261 7365  r", "center_base
+00000630: 6c69 6e65 222c 2022 746f 7022 7d2c 2064  line", "top"}, d
+00000640: 6566 6175 6c74 3a20 2263 656e 7465 7222  efault: "center"
+00000650: 0a20 2020 2020 2020 2054 6865 2076 6572  .        The ver
+00000660: 7469 6361 6c20 616c 6967 6e6d 656e 7420  tical alignment 
+00000670: 6f66 2074 6865 2074 6578 742e 0a20 2020  of the text..   
+00000680: 2063 6c69 705f 6f6e 3a20 626f 6f6c 2c20   clip_on: bool, 
+00000690: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
+000006a0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+000006b0: 2063 6c69 7020 7468 6520 7465 7874 2061   clip the text a
+000006c0: 7420 7468 6520 706c 6f74 2062 6f75 6e64  t the plot bound
+000006d0: 6172 6965 732e 0a20 2020 202a 2a6b 7761  aries..    **kwa
+000006e0: 7267 733a 2064 6963 742c 206f 7074 696f  rgs: dict, optio
+000006f0: 6e61 6c0a 2020 2020 2020 2020 4164 6469  nal.        Addi
+00000700: 7469 6f6e 616c 206b 6579 776f 7264 2061  tional keyword a
+00000710: 7267 756d 656e 7473 2c20 7768 6963 6820  rguments, which 
+00000720: 7769 6c6c 2062 6520 7061 7373 6564 2074  will be passed t
+00000730: 6f20 4d61 7470 6c6f 746c 6962 2773 0a20  o Matplotlib's. 
+00000740: 2020 2020 2020 2060 7e6d 6174 706c 6f74         `~matplot
+00000750: 6c69 622e 6178 6573 2e41 7865 732e 7465  lib.axes.Axes.te
+00000760: 7874 6020 6d65 7468 6f64 2066 6f72 2061  xt` method for a
+00000770: 6464 696e 6720 7465 7874 2074 6f20 706c  dding text to pl
+00000780: 6f74 2041 7865 732e 0a20 2020 2022 2222  ot Axes..    """
+00000790: 2020 2320 6e6f 7161 3a20 4535 3031 0a0a    # noqa: E501..
+000007a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000007b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000007c0: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
+000007d0: 3a20 556e 696f 6e5b 536b 7943 6f6f 7264  : Union[SkyCoord
+000007e0: 2c20 5365 7175 656e 6365 5b66 6c6f 6174  , Sequence[float
+000007f0: 5d2c 206e 7074 2e4e 4441 7272 6179 5b6e  ], npt.NDArray[n
+00000800: 702e 666c 6f61 745f 5d5d 2c0a 2020 2020  p.float_]],.    
+00000810: 2020 2020 733a 2073 7472 2c0a 2020 2020      s: str,.    
+00000820: 2020 2020 7763 733a 2057 4353 2c0a 2020      wcs: WCS,.  
+00000830: 2020 2020 2020 636f 6c6f 723a 2055 6e69        color: Uni
+00000840: 6f6e 5b73 7472 2c20 5475 706c 655b 666c  on[str, Tuple[fl
+00000850: 6f61 742c 2066 6c6f 6174 2c20 666c 6f61  oat, float, floa
+00000860: 745d 5d20 3d20 2262 6c61 636b 222c 0a20  t]] = "black",. 
+00000870: 2020 2020 2020 2068 6f72 697a 6f6e 7461         horizonta
+00000880: 6c61 6c69 676e 6d65 6e74 3a20 4c69 7465  lalignment: Lite
+00000890: 7261 6c5b 2263 656e 7465 7222 2c20 226c  ral["center", "l
+000008a0: 6566 7422 2c20 2272 6967 6874 225d 203d  eft", "right"] =
+000008b0: 2022 6365 6e74 6572 222c 0a20 2020 2020   "center",.     
+000008c0: 2020 2076 6572 7469 6361 6c61 6c69 676e     verticalalign
+000008d0: 6d65 6e74 3a20 4c69 7465 7261 6c5b 0a20  ment: Literal[. 
+000008e0: 2020 2020 2020 2020 2020 2022 6261 7365             "base
+000008f0: 6c69 6e65 222c 2022 626f 7474 6f6d 222c  line", "bottom",
+00000900: 2022 6365 6e74 6572 222c 2022 6365 6e74   "center", "cent
+00000910: 6572 5f62 6173 656c 696e 6522 2c20 2274  er_baseline", "t
+00000920: 6f70 220a 2020 2020 2020 2020 5d20 3d20  op".        ] = 
+00000930: 2263 656e 7465 7222 2c0a 2020 2020 2020  "center",.      
+00000940: 2020 636c 6970 5f6f 6e3a 2062 6f6f 6c20    clip_on: bool 
+00000950: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+00000960: 2a2a 6b77 6172 6773 3a20 416e 792c 0a20  **kwargs: Any,. 
+00000970: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+00000980: 6c66 2e5f 706f 7369 7469 6f6e 203d 2070  lf._position = p
+00000990: 6f73 6974 696f 6e0a 2020 2020 2020 2020  osition.        
+000009a0: 7365 6c66 2e5f 7320 3d20 730a 2020 2020  self._s = s.    
+000009b0: 2020 2020 7365 6c66 2e5f 7763 7320 3d20      self._wcs = 
+000009c0: 7763 730a 2020 2020 2020 2020 7365 6c66  wcs.        self
+000009d0: 2e5f 6b77 6172 6773 203d 2064 6565 7063  ._kwargs = deepc
+000009e0: 6f70 7928 6b77 6172 6773 290a 2020 2020  opy(kwargs).    
+000009f0: 2020 2020 7365 6c66 2e5f 6b77 6172 6773      self._kwargs
+00000a00: 5b22 636f 6c6f 7222 5d20 3d20 636f 6c6f  ["color"] = colo
+00000a10: 720a 2020 2020 2020 2020 7365 6c66 2e5f  r.        self._
+00000a20: 6b77 6172 6773 5b22 686f 7269 7a6f 6e74  kwargs["horizont
+00000a30: 616c 616c 6967 6e6d 656e 7422 5d20 3d20  alalignment"] = 
+00000a40: 686f 7269 7a6f 6e74 616c 616c 6967 6e6d  horizontalalignm
+00000a50: 656e 740a 2020 2020 2020 2020 7365 6c66  ent.        self
+00000a60: 2e5f 6b77 6172 6773 5b22 7665 7274 6963  ._kwargs["vertic
+00000a70: 616c 616c 6967 6e6d 656e 7422 5d20 3d20  alalignment"] = 
+00000a80: 7665 7274 6963 616c 616c 6967 6e6d 656e  verticalalignmen
+00000a90: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
+00000aa0: 6b77 6172 6773 5b22 636c 6970 5f6f 6e22  kwargs["clip_on"
+00000ab0: 5d20 3d20 636c 6970 5f6f 6e0a 0a20 2020  ] = clip_on..   
+00000ac0: 2064 6566 2061 6464 5f74 6f28 7365 6c66   def add_to(self
+00000ad0: 2c20 6178 3a20 5743 5341 7865 7329 202d  , ax: WCSAxes) -
+00000ae0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00000af0: 2222 2241 6464 2074 6865 2074 6578 7420  """Add the text 
+00000b00: 746f 2061 2066 696e 6465 7220 6368 6172  to a finder char
+00000b10: 742e 0a0a 2020 2020 2020 2020 6178 3a20  t...        ax: 
+00000b20: 2060 7e61 7374 726f 7079 2e76 6973 7561   `~astropy.visua
+00000b30: 6c69 7a61 7469 6f6e 2e77 6373 6178 6573  lization.wcsaxes
+00000b40: 2e57 4353 4178 6573 600a 2020 2020 2020  .WCSAxes`.      
+00000b50: 2020 2020 2020 5743 5320 6178 6573 206f        WCS axes o
+00000b60: 626a 6563 742e 0a20 2020 2020 2020 2022  bject..        "
+00000b70: 2222 0a20 2020 2020 2020 2069 6620 7479  "".        if ty
+00000b80: 7065 2873 656c 662e 5f70 6f73 6974 696f  pe(self._positio
+00000b90: 6e29 203d 3d20 536b 7943 6f6f 7264 3a0a  n) == SkyCoord:.
+00000ba0: 2020 2020 2020 2020 2020 2020 706f 7369              posi
+00000bb0: 7469 6f6e 5f70 7820 3d20 736b 795f 706f  tion_px = sky_po
+00000bc0: 7369 7469 6f6e 5f74 6f5f 7069 7865 6c28  sition_to_pixel(
+00000bd0: 7365 6c66 2e5f 706f 7369 7469 6f6e 2c20  self._position, 
+00000be0: 7365 6c66 2e5f 7763 7329 0a20 2020 2020  self._wcs).     
+00000bf0: 2020 2020 2020 2061 782e 7465 7874 2870         ax.text(p
+00000c00: 6f73 6974 696f 6e5f 7078 5b30 5d2c 2070  osition_px[0], p
+00000c10: 6f73 6974 696f 6e5f 7078 5b31 5d2c 2073  osition_px[1], s
+00000c20: 656c 662e 5f73 2c20 2a2a 7365 6c66 2e5f  elf._s, **self._
+00000c30: 6b77 6172 6773 2920 2023 206e 6f71 610a  kwargs)  # noqa.
+00000c40: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000c50: 2020 2020 2020 2020 2020 6178 2e74 6578            ax.tex
+00000c60: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00000c70: 2020 2073 656c 662e 5f70 6f73 6974 696f     self._positio
+00000c80: 6e5b 305d 2c0a 2020 2020 2020 2020 2020  n[0],.          
+00000c90: 2020 2020 2020 7365 6c66 2e5f 706f 7369        self._posi
+00000ca0: 7469 6f6e 5b31 5d2c 0a20 2020 2020 2020  tion[1],.       
+00000cb0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
+00000cc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000cd0: 2020 7472 616e 7366 6f72 6d3d 6178 2e74    transform=ax.t
+00000ce0: 7261 6e73 4178 6573 2c0a 2020 2020 2020  ransAxes,.      
+00000cf0: 2020 2020 2020 2020 2020 2a2a 7365 6c66            **self
+00000d00: 2e5f 6b77 6172 6773 2c0a 2020 2020 2020  ._kwargs,.      
+00000d10: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00000d20: 2072 6f74 6174 6528 7365 6c66 2c20 7069   rotate(self, pi
+00000d30: 766f 743a 2053 6b79 436f 6f72 642c 2061  vot: SkyCoord, a
+00000d40: 6e67 6c65 3a20 416e 676c 6529 202d 3e20  ngle: Angle) -> 
+00000d50: 2254 6578 7441 6e6e 6f74 6174 696f 6e22  "TextAnnotation"
+00000d60: 3a0a 2020 2020 2020 2020 2222 2252 6f74  :.        """Rot
+00000d70: 6174 6520 7468 6973 2061 6e6e 6f74 6174  ate this annotat
+00000d80: 696f 6e20 6172 6f75 6e64 2061 2070 6976  ion around a piv
+00000d90: 6f74 2061 6e64 2072 6574 7572 6e20 7468  ot and return th
+00000da0: 6520 7265 7375 6c74 2e0a 0a20 2020 2020  e result...     
+00000db0: 2020 2054 6865 2072 6f74 6174 696f 6e20     The rotation 
+00000dc0: 616e 676c 6520 6973 2061 6e20 616e 676c  angle is an angl
+00000dd0: 6520 6f6e 2074 6865 2073 6b79 2c20 6d65  e on the sky, me
+00000de0: 6173 7572 6564 2066 726f 6d20 6e6f 7274  asured from nort
+00000df0: 6820 746f 2065 6173 742e 0a0a 2020 2020  h to east...    
+00000e00: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00000e10: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00000e20: 2d0a 2020 2020 2020 2020 7069 766f 743a  -.        pivot:
+00000e30: 2060 7e61 7374 726f 7079 2e63 6f6f 7264   `~astropy.coord
+00000e40: 696e 6174 6573 2e53 6b79 436f 6f72 6460  inates.SkyCoord`
+00000e50: 0a20 2020 2020 2020 2020 2020 2050 6f69  .            Poi
+00000e60: 6e74 2061 726f 756e 6420 7768 6963 6820  nt around which 
+00000e70: 746f 2072 6f74 6174 6520 7468 6520 616e  to rotate the an
+00000e80: 6e6f 7461 7469 6f6e 2e0a 2020 2020 2020  notation..      
+00000e90: 2020 616e 676c 653a 2060 7e61 7374 726f    angle: `~astro
+00000ea0: 7079 2e63 6f6f 7264 696e 6174 6573 2e41  py.coordinates.A
+00000eb0: 6e67 6c65 600a 2020 2020 2020 2020 2020  ngle`.          
+00000ec0: 2020 416e 676c 6520 6f66 2072 6f74 6174    Angle of rotat
+00000ed0: 696f 6e2c 206d 6561 7375 7265 6420 6672  ion, measured fr
+00000ee0: 6f6d 206e 6f72 7468 2074 6f20 6561 7374  om north to east
+00000ef0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00000f00: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00000f10: 2d2d 0a20 2020 2020 2020 2060 7e69 6d65  --.        `~ime
+00000f20: 7068 752e 616e 6e6f 7461 7469 6f6e 2e67  phu.annotation.g
+00000f30: 656e 6572 616c 2e54 6578 7441 6e6e 6f74  eneral.TextAnnot
+00000f40: 6174 696f 6e60 0a20 2020 2020 2020 2020  ation`.         
+00000f50: 2020 2054 6865 2061 6e6e 6f74 6174 696f     The annotatio
+00000f60: 6e20 7265 7375 6c74 696e 6720 6672 6f6d  n resulting from
+00000f70: 2074 6865 2072 6f74 6174 696f 6e2e 0a20   the rotation.. 
+00000f80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000f90: 2020 2069 6620 7479 7065 2873 656c 662e     if type(self.
+00000fa0: 5f70 6f73 6974 696f 6e29 2069 7320 6e6f  _position) is no
+00000fb0: 7420 536b 7943 6f6f 7264 3a0a 2020 2020  t SkyCoord:.    
+00000fc0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+00000fd0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00000fe0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00000ff0: 2020 2022 5468 6520 7465 7874 2063 616e     "The text can
+00001000: 206f 6e6c 7920 6265 2072 6f74 6174 6564   only be rotated
+00001010: 2069 6620 6974 7320 706f 7369 7469 6f6e   if its position
+00001020: 2069 7320 616e 2069 6e73 7461 6e63 6520   is an instance 
+00001030: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
+00001040: 2020 2020 2022 6173 7472 6f70 792e 636f       "astropy.co
+00001050: 6f72 642e 536b 7943 6f6f 7264 2e22 0a20  ord.SkyCoord.". 
+00001060: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00001070: 2020 2020 2072 6f74 6174 6564 5f61 6e6e       rotated_ann
+00001080: 6f74 6174 696f 6e20 3d20 6465 6570 636f  otation = deepco
+00001090: 7079 2873 656c 6629 0a20 2020 2020 2020  py(self).       
+000010a0: 2072 6f74 6174 6564 5f70 6f73 6974 696f   rotated_positio
+000010b0: 6e20 3d20 726f 7461 7465 2873 656c 662e  n = rotate(self.
+000010c0: 5f70 6f73 6974 696f 6e2c 2070 6976 6f74  _position, pivot
+000010d0: 2c20 616e 676c 652c 2073 656c 662e 5f77  , angle, self._w
+000010e0: 6373 290a 2020 2020 2020 2020 726f 7461  cs).        rota
+000010f0: 7465 645f 616e 6e6f 7461 7469 6f6e 2e5f  ted_annotation._
+00001100: 706f 7369 7469 6f6e 203d 2072 6f74 6174  position = rotat
+00001110: 6564 5f70 6f73 6974 696f 6e0a 2020 2020  ed_position.    
+00001120: 2020 2020 7265 7475 726e 2072 6f74 6174      return rotat
+00001130: 6564 5f61 6e6e 6f74 6174 696f 6e0a 0a20  ed_annotation.. 
+00001140: 2020 2064 6566 2074 7261 6e73 6c61 7465     def translate
+00001150: 2873 656c 662c 2064 6973 706c 6163 656d  (self, displacem
+00001160: 656e 743a 2041 6e67 6c65 2920 2d3e 2022  ent: Angle) -> "
+00001170: 5465 7874 416e 6e6f 7461 7469 6f6e 223a  TextAnnotation":
+00001180: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001190: 2020 2020 204d 6f76 6520 7468 6973 2061       Move this a
+000011a0: 6e6e 6f74 6174 696f 6e20 616c 6f6e 6720  nnotation along 
+000011b0: 6120 6469 7370 6c61 6365 6d65 6e74 2076  a displacement v
+000011c0: 6563 746f 7220 616e 6420 7265 7475 726e  ector and return
+000011d0: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
+000011e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000011f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00001200: 2d2d 2d0a 2020 2020 2020 2020 6469 7370  ---.        disp
+00001210: 6c61 6365 6d65 6e74 3a20 3244 2061 7272  lacement: 2D arr
+00001220: 6179 206f 6620 616e 676c 6573 0a20 2020  ay of angles.   
+00001230: 2020 2020 2020 2020 2054 6865 2064 6973           The dis
+00001240: 706c 6163 656d 656e 7420 6279 2077 6869  placement by whi
+00001250: 6368 2074 6f20 6d6f 7665 2074 6865 2061  ch to move the a
+00001260: 6e6e 6f74 6174 696f 6e2e 0a0a 2020 2020  nnotation...    
+00001270: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00001280: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00001290: 2020 2020 607e 696d 6570 6875 2e61 6e6e      `~imephu.ann
+000012a0: 6f74 6174 696f 6e2e 6765 6e65 7261 6c2e  otation.general.
+000012b0: 5465 7874 416e 6e6f 7461 7469 6f6e 600a  TextAnnotation`.
+000012c0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000012d0: 616e 6e6f 7461 7469 6f6e 2072 6573 756c  annotation resul
+000012e0: 7469 6e67 2066 726f 6d20 7468 6520 7472  ting from the tr
+000012f0: 616e 736c 6174 696f 6e2e 0a20 2020 2020  anslation..     
+00001300: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00001310: 6620 7479 7065 2873 656c 662e 5f70 6f73  f type(self._pos
+00001320: 6974 696f 6e29 2069 7320 6e6f 7420 536b  ition) is not Sk
+00001330: 7943 6f6f 7264 3a0a 2020 2020 2020 2020  yCoord:.        
+00001340: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+00001350: 6c65 6d65 6e74 6564 4572 726f 7228 0a20  lementedError(. 
+00001360: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001370: 5468 6520 7465 7874 2063 616e 206f 6e6c  The text can onl
+00001380: 7920 6265 2074 7261 6e73 6c61 7465 6420  y be translated 
+00001390: 6966 2069 7473 2070 6f73 6974 696f 6e20  if its position 
+000013a0: 6973 2061 6e20 696e 7374 616e 6365 206f  is an instance o
+000013b0: 6620 220a 2020 2020 2020 2020 2020 2020  f ".            
+000013c0: 2020 2020 2261 7374 726f 7079 2e63 6f6f      "astropy.coo
+000013d0: 7264 2e53 6b79 436f 6f72 642e 220a 2020  rd.SkyCoord.".  
+000013e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000013f0: 2020 2020 7472 616e 736c 6174 6564 5f61      translated_a
+00001400: 6e6e 6f74 6174 696f 6e20 3d20 6465 6570  nnotation = deep
+00001410: 636f 7079 2873 656c 6629 0a20 2020 2020  copy(self).     
+00001420: 2020 2074 7261 6e73 6c61 7465 645f 706f     translated_po
+00001430: 7369 7469 6f6e 203d 2074 7261 6e73 6c61  sition = transla
+00001440: 7465 2873 656c 662e 5f70 6f73 6974 696f  te(self._positio
+00001450: 6e2c 2064 6973 706c 6163 656d 656e 7429  n, displacement)
+00001460: 0a20 2020 2020 2020 2074 7261 6e73 6c61  .        transla
+00001470: 7465 645f 616e 6e6f 7461 7469 6f6e 2e5f  ted_annotation._
+00001480: 706f 7369 7469 6f6e 203d 2074 7261 6e73  position = trans
+00001490: 6c61 7465 645f 706f 7369 7469 6f6e 0a20  lated_position. 
+000014a0: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
+000014b0: 616e 736c 6174 6564 5f61 6e6e 6f74 6174  anslated_annotat
+000014c0: 696f 6e0a                                ion.
```

### Comparing `imephu-0.2.0/src/imephu/annotation/general/arrow.py` & `imephu-0.2.1/src/imephu/annotation/general/arrow.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/annotation/general/circle.py` & `imephu-0.2.1/src/imephu/annotation/general/line_path.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,108 +1,122 @@
 from copy import deepcopy
-from typing import Any, Tuple, Union, cast
+from typing import Any, Sequence, Tuple, Union
 
 from astropy.coordinates import Angle, SkyCoord
 from astropy.visualization.wcsaxes import WCSAxes
 from astropy.wcs import WCS
-from matplotlib.patches import Circle
+from matplotlib.patches import PathPatch
+from matplotlib.path import Path
 
 from imephu.annotation import Annotation
-from imephu.geometry import pixel_scales, rotate, sky_position_to_pixel, translate
+from imephu.geometry import rotate, sky_position_to_pixel, translate
 
 
-class CircleAnnotation(Annotation):
-    """An annotation for adding a circle to a plot.
+class LinePathAnnotation(Annotation):
+    """An annotation consisting of straight lines between vertices.
 
-    The radius of the circle is given as an angular distance on the sky, in the
-    direction of the right ascension. A circle is drawn irrespective of the pixel scales
-    for right ascension and declination. Hence the circle in general is not a circle on
-    the sky but just on the finder chart.
+    The path displayed by this annotation is defined by a set of vertices, which are
+    connected by straight lines on the finder chart. (The connecting lines in general
+    will refer to curved lines on the sky.)
+
+    By default the path is assumed to be closed, i.e. the last vertex is connected to
+    the first by a line. This behavior may be changed with the ``closed`` parameter.
 
     Parameters
     ----------
-    center: `~astropy.coordinates.SkyCoord`
-        The right ascension and declination of the circle's center.
-    radius: `~astropy.coordinates.Angle`
-        The radius of the circle, as an angular distance on the sky in right ascension
-        direction.
+    vertices: sequence of `~astropy.coordinates.SkyCoord`
+        The path vertices, as an array or sequence of sky coordinates (with right
+        ascension abd declination).
     wcs: `~astropy.wcs.WCS`
         WCS object.
+    closed: bool, default: True
+        Whether the the path is closed, i.e. whether the last vertex is connected to the
+        first by a line.
     edgecolor: color, default: "black"
         The edge color.
     facecolor: color, default: "none"
         The filling color.
     **kwargs: dict, optional
         Additional keyword arguments, which will be passed to Matplotlib's
-        `~matplotlib.patches.Circle` patch constructor.
+        `~matplotlib.patches.PathPatch` patch constructor.
     """
 
     def __init__(
         self,
-        center: SkyCoord,
-        radius: Angle,
+        vertices: Sequence[SkyCoord],
         wcs: WCS,
+        closed: bool = True,
         edgecolor: Union[str, Tuple[float, float, float]] = "black",
         facecolor: Union[str, Tuple[float, float, float]] = "none",
         **kwargs: Any,
     ):
-        self._center = center
-        self._radius = radius
+        if closed:
+            # Matplotlib will ignore the last vertex for a closed path; we avoid this by
+            # having that vertex twice
+            self._vertices = list(vertices)[:] + [vertices[-1]]
+        else:
+            self._vertices = list(vertices)
         self._wcs = wcs
+        self._closed = closed
         self._kwargs = deepcopy(kwargs)
         self._kwargs["edgecolor"] = edgecolor
         self._kwargs["facecolor"] = facecolor
 
     def add_to(self, ax: WCSAxes) -> None:
-        """Add the circle to a finder chart.
+        """Add the line path to a finder chart.
 
+        Parameters
+        ----------
         ax: `~astropy.visualization.wcsaxes.WCSAxes`
-            WCS axes object.
+            Plot axes.
         """
-        center_px = cast(
-            Tuple[float, float], sky_position_to_pixel(self._center, self._wcs)
-        )
-        ra_pixel_scale, _ = pixel_scales(self._wcs)
-        radius_px = float(self._radius / ra_pixel_scale)
-        circle_patch = Circle(center_px, radius_px, **self._kwargs)
-        ax.add_patch(circle_patch)
+        vertices_px = [
+            sky_position_to_pixel(vertex, self._wcs) for vertex in self._vertices
+        ]
+        path = Path(vertices_px, closed=self._closed)  # noqa
+        path_patch = PathPatch(path, **self._kwargs)
+        ax.add_patch(path_patch)
 
-    def rotate(self, pivot: SkyCoord, angle: Angle) -> "CircleAnnotation":
+    def rotate(self, pivot: SkyCoord, angle: Angle) -> "LinePathAnnotation":
         """Rotate this annotation around a pivot and return the result.
 
         The rotation angle is an angle on the sky, measured from north to east.
 
         Parameters
         ----------
         pivot: `~astropy.coordinates.SkyCoord`
             Point around which to rotate the annotation.
         angle: `~astropy.coordinates.Angle`
-            Angle of rotation, measured from north to east.
+            Angle of rotation, measured from north towards the east.
 
         Returns
         -------
-        `~imephu.annotation.general.CircleAnnotation`
+        `~imephu.annotation.general.LinePathAnnotation`
             The annotation resulting from the rotation.
         """
         rotated_annotation = deepcopy(self)
-        rotated_center = rotate(self._center, pivot, angle, self._wcs)
-        rotated_annotation._center = rotated_center
+        rotated_vertices = [
+            rotate(vertex, pivot, angle, self._wcs) for vertex in self._vertices
+        ]
+        rotated_annotation._vertices = rotated_vertices
         return rotated_annotation
 
-    def translate(self, displacement: Angle) -> "CircleAnnotation":
+    def translate(self, displacement: Angle) -> "LinePathAnnotation":
         """
         Move this annotation along a displacement vector and return the result.
 
         Parameters
         ----------
         displacement: 2D array of angles
             The displacement by which to move the annotation.
 
         Returns
         -------
-        `~imephu.annotation.general.CircleAnnotation`
+        `~imephu.annotation.general.LinePathAnnotation`
             The annotation resulting from the translation.
         """
         translated_annotation = deepcopy(self)
-        translated_center = translate(self._center, displacement)
-        translated_annotation._center = translated_center
+        translated_vertices = [
+            translate(vertex, displacement) for vertex in self._vertices
+        ]
+        translated_annotation._vertices = translated_vertices
         return translated_annotation
```

### Comparing `imephu-0.2.0/src/imephu/annotation/general/crosshairs.py` & `imephu-0.2.1/src/imephu/annotation/general/crosshairs.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/annotation/general/empty.py` & `imephu-0.2.1/src/imephu/annotation/general/empty.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/annotation/motion.py` & `imephu-0.2.1/src/imephu/annotation/motion.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/cli.py` & `imephu-0.2.1/src/imephu/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,45 +35,45 @@
     if value:
         typer.echo(f"imephu {imephu.__version__}")
         raise typer.Exit()
 
 
 @app.command()
 def main(
-    config: Optional[Path] = typer.Option(
+    config: Optional[Path] = typer.Option(  # noqa: B008
         None,
         "--config",
         "-c",
         file_okay=True,
         exists=True,
         resolve_path=True,
         help="Configuration details for the finder chart(s).",
     ),
-    output: Optional[Path] = typer.Option(
+    output: Optional[Path] = typer.Option(  # noqa: B008
         None, "--out", "-o", file_okay=True, resolve_path=True, help="Output file."
     ),
-    format: str = typer.Option(
+    format: str = typer.Option(  # noqa: B008
         "png",
         "--format",
         "-f",
         help="Image format (such as png or pdf) for the finder chart(s).",
     ),
-    version: Optional[bool] = typer.Option(
+    version: Optional[bool] = typer.Option(  # noqa: B008
         None, "--version", callback=_version_callback, help="Show the version and exit."
     ),
 ) -> None:
     """A tool for creating finder charts."""  # noqa: D401
     try:
         configuration = _read_configuration(config)
         _validate_configuration(configuration)
         configuration["__config-path"] = config
         _create_finder_charts(configuration, output, format)
     except Exception as e:
         typer.echo(str(e), err=True)
-        raise typer.Exit(code=1)
+        raise typer.Exit(code=1) from e
 
 
 def _read_configuration(config: Optional[Path]) -> Any:
     if config:
         with open(config, "r") as f:
             configuration_yaml = f.read()
     else:
```

### Comparing `imephu-0.2.0/src/imephu/salt/__pycache__/general.cpython-310.pyc` & `imephu-0.2.1/src/imephu/salt/annotation/telescope.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,431 +1,563 @@
-00000000: 6f0d 0d0a 0000 0000 a46b f161 bb1f 0000  o........k.a....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 0201 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
-00000040: 6d04 5a04 6d05 5a05 0100 6400 6403 6c06  m.Z.m.Z...d.d.l.
-00000050: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000060: 6d0a 5a0a 6d0b 5a0b 0100 6405 5a0c 6406  m.Z.m.Z...d.Z.d.
-00000070: 650d 6407 650d 6408 650d 6409 6507 640a  e.d.e.d.e.d.e.d.
-00000080: 650a 660a 640b 640c 8404 5a0e 640d 6505  e.f.d.d...Z.d.e.
-00000090: 6409 6507 640a 6509 6606 640e 640f 8404  d.e.d.e.f.d.d...
-000000a0: 5a0f 640d 6505 6409 6507 640a 6509 6606  Z.d.e.d.e.d.e.f.
-000000b0: 6410 6411 8404 5a10 640d 6505 6409 6507  d.d...Z.d.e.d.e.
-000000c0: 640a 6509 6606 6412 6413 8404 5a11 6414  d.e.f.d.d...Z.d.
-000000d0: 6504 6415 6512 6409 6507 640a 650a 6608  e.d.e.d.e.d.e.f.
-000000e0: 6416 6417 8404 5a13 6418 650d 6409 6507  d.d...Z.d.e.d.e.
-000000f0: 640a 650a 6606 6419 641a 8404 5a14 6406  d.e.f.d.d...Z.d.
-00000100: 650d 6407 650d 6408 650d 6414 6504 6415  e.d.e.d.e.d.e.d.
-00000110: 6512 6418 650d 640d 6505 6409 6507 640a  e.d.e.d.e.d.e.d.
-00000120: 6509 6612 641b 641c 8404 5a15 641d 5300  e.f.d.d...Z.d.S.
-00000130: 291e e900 0000 0029 01da 0575 6e69 7473  )......)...units
-00000140: 2902 da05 416e 676c 65da 0853 6b79 436f  )...Angle..SkyCo
-00000150: 6f72 6429 01da 0357 4353 2903 da0f 4772  ord)...WCS)...Gr
-00000160: 6f75 7041 6e6e 6f74 6174 696f 6eda 0e54  oupAnnotation..T
-00000170: 6578 7441 6e6e 6f74 6174 696f 6eda 1043  extAnnotation..C
-00000180: 6972 636c 6541 6e6e 6f74 6174 696f 6e29  ircleAnnotation)
-00000190: 0372 0100 0000 e700 0000 0000 00e0 3fe9  .r............?.
-000001a0: 0100 0000 da06 7461 7267 6574 da0d 7072  ......target..pr
-000001b0: 6f70 6f73 616c 5f63 6f64 65da 0e70 695f  oposal_code..pi_
-000001c0: 6661 6d69 6c79 5f6e 616d 65da 0377 6373  family_name..wcs
-000001d0: da06 7265 7475 726e 6304 0000 0000 0000  ..returnc.......
-000001e0: 0000 0000 0005 0000 000a 0000 0043 0000  .............C..
-000001f0: 0073 2e00 0000 7c00 9b00 6401 7c01 9b00  .s....|...d.|...
-00000200: 6402 7c02 9b00 6403 9d06 7d04 7400 6404  d.|...d...}.t.d.
-00000210: 7c04 7c03 6405 6406 6407 6408 6409 640a  |.|.d.d.d.d.d.d.
-00000220: 8d08 5300 290c 618b 0200 0052 6574 7572  ..S.).a....Retur
-00000230: 6e20 6120 7465 7874 2061 6e6e 6f74 6174  n a text annotat
-00000240: 696f 6e20 7769 7468 2074 6865 2074 6974  ion with the tit
-00000250: 6c65 2074 6f20 7468 6520 6669 6e64 6572  le to the finder
-00000260: 2063 6861 7274 2e0a 0a20 2020 2054 6865   chart...    The
-00000270: 2074 6974 6c65 2069 7320 6f66 2074 6865   title is of the
-00000280: 2066 6f72 6d20 2274 6172 6765 7420 6e61   form "target na
-00000290: 6d65 2028 7072 6f70 6f73 616c 2063 6f64  me (proposal cod
-000002a0: 653b 2073 7572 6e61 6d65 206f 6620 7468  e; surname of th
-000002b0: 6520 5072 696e 6369 7061 6c0a 2020 2020  e Principal.    
-000002c0: 496e 7665 7374 6967 6174 6f72 2922 2c20  Investigator)", 
-000002d0: 7375 6368 2061 7320 224d 6167 7261 7468  such as "Magrath
-000002e0: 6561 2028 3230 3232 2d31 2d53 4349 2d30  ea (2022-1-SCI-0
-000002f0: 3432 3b20 4164 616d 7329 222e 0a0a 2020  42; Adams)"...  
-00000300: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000310: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000320: 7461 7267 6574 3a20 7374 720a 2020 2020  target: str.    
-00000330: 2020 2020 5468 6520 6e61 6d65 206f 6620      The name of 
-00000340: 7468 6520 7461 7267 6574 2066 6f72 2077  the target for w
-00000350: 6869 6368 2074 6865 2066 696e 6465 7220  hich the finder 
-00000360: 6368 6172 7420 6973 2069 6e74 656e 6465  chart is intende
-00000370: 642e 0a20 2020 2070 726f 706f 7361 6c5f  d..    proposal_
-00000380: 636f 6465 3a20 7374 720a 2020 2020 2020  code: str.      
-00000390: 2020 5468 6520 7072 6f70 6f73 616c 2063    The proposal c
-000003a0: 6f64 6520 666f 7220 7768 6963 6820 7468  ode for which th
-000003b0: 6520 6669 6e64 6572 2063 6861 7274 2069  e finder chart i
-000003c0: 7320 696e 7465 6e64 6564 2e0a 2020 2020  s intended..    
-000003d0: 7069 5f66 616d 696c 795f 6e61 6d65 3a20  pi_family_name: 
-000003e0: 7374 720a 2020 2020 2020 2020 5468 6520  str.        The 
-000003f0: 6661 6d69 6c79 206e 616d 6520 6f66 2074  family name of t
-00000400: 6865 2050 7269 6e63 6970 616c 2049 6e76  he Principal Inv
-00000410: 6573 7469 6761 746f 722e 0a20 2020 2077  estigator..    w
-00000420: 6373 3a20 607e 6173 7472 6f70 792e 7763  cs: `~astropy.wc
-00000430: 732e 5743 5360 0a20 2020 2020 2020 2057  s.WCS`.        W
-00000440: 4353 206f 626a 6563 742e 0a0a 2020 2020  CS object...    
-00000450: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-00000460: 2d2d 2d0a 2020 2020 607e 696d 6570 6875  ---.    `~imephu
-00000470: 2e61 6e6e 6f74 6174 696f 6e2e 6765 6e65  .annotation.gene
-00000480: 7261 6c2e 5465 7874 416e 6e6f 7461 7469  ral.TextAnnotati
-00000490: 6f6e 600a 2020 2020 2020 2020 5468 6520  on`.        The 
-000004a0: 7469 746c 6520 616e 6e6f 7461 7469 6f6e  title annotation
-000004b0: 2e0a 2020 2020 7a02 2028 7a02 3b20 fa01  ..    z. (z.; ..
-000004c0: 2929 0272 0900 0000 677b 14ae 47e1 7af0  )).r....g{..G.z.
-000004d0: 3fda 0562 6c61 636b da06 6365 6e74 6572  ?..black..center
-000004e0: da06 6974 616c 6963 da04 626f 6c64 da05  ..italic..bold..
-000004f0: 6c61 7267 65a9 0672 0e00 0000 da05 636f  large..r......co
-00000500: 6c6f 72da 1368 6f72 697a 6f6e 7461 6c61  lor..horizontala
-00000510: 6c69 676e 6d65 6e74 da05 7374 796c 65da  lignment..style.
-00000520: 0677 6569 6768 74da 0473 697a 654e a901  .weight..sizeN..
-00000530: 7207 0000 0029 0572 0b00 0000 720c 0000  r....).r....r...
-00000540: 0072 0d00 0000 720e 0000 005a 0a74 6974  .r....r....Z.tit
-00000550: 6c65 5f74 6578 74a9 0072 1d00 0000 fa4a  le_text..r.....J
-00000560: 2f55 7365 7273 2f63 6872 6973 7469 616e  /Users/christian
-00000570: 2f49 6465 6150 726f 6a65 6374 732f 696d  /IdeaProjects/im
-00000580: 6570 6875 2f73 7263 2f69 6d65 7068 752f  ephu/src/imephu/
-00000590: 616e 6e6f 7461 7469 6f6e 2f73 616c 742f  annotation/salt/
-000005a0: 6765 6e65 7261 6c2e 7079 da10 7469 746c  general.py..titl
-000005b0: 655f 616e 6e6f 7461 7469 6f6e 0900 0000  e_annotation....
-000005c0: 7316 0000 0016 1802 0102 0102 0102 0102  s...............
-000005d0: 0102 0102 0102 0102 0106 f872 1f00 0000  ...........r....
-000005e0: da0b 6669 7473 5f63 656e 7465 7263 0200  ..fits_centerc..
-000005f0: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
-00000600: 0000 4300 0000 735a 0000 0074 007c 0064  ..C...sZ...t.|.d
-00000610: 017c 0174 0164 0264 0364 0464 0564 068d  .|.t.d.d.d.d.d..
-00000620: 08a0 0274 0364 0774 046a 0514 0083 01a1  ...t.d.t.j......
-00000630: 017d 0274 007c 0064 087c 0174 0164 0364  .}.t.|.d.|.t.d.d
-00000640: 0464 0564 098d 07a0 0274 0364 0a74 046a  .d.d.....t.d.t.j
-00000650: 0514 0083 01a1 017d 0374 067c 027c 0367  .......}.t.|.|.g
-00000660: 0283 0153 0029 0c61 9501 0000 5265 7475  ...S.).a....Retu
-00000670: 726e 2061 6e20 616e 6e6f 7461 7469 6f6e  rn an annotation
-00000680: 2066 6f72 2074 6865 2065 6173 7420 616e   for the east an
-00000690: 6420 6e6f 7274 6820 6469 7265 6374 696f  d north directio
-000006a0: 6e2e 0a0a 2020 2020 5061 7261 6d65 7465  n...    Paramete
-000006b0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-000006c0: 2d0a 2020 2020 6669 7473 5f63 656e 7465  -.    fits_cente
-000006d0: 723a 2060 7e61 7374 726f 7079 2e63 6f6f  r: `~astropy.coo
-000006e0: 7264 696e 6174 6573 2e53 6b79 436f 6f72  rdinates.SkyCoor
-000006f0: 6460 0a20 2020 2020 2020 2054 6865 2063  d`.        The c
-00000700: 656e 7472 616c 2070 6f73 6974 696f 6e20  entral position 
-00000710: 6f66 2074 6865 2066 696e 6465 7220 6368  of the finder ch
-00000720: 6172 742c 2069 6e20 7269 6768 7420 6173  art, in right as
-00000730: 6365 6e73 696f 6e20 616e 6420 6465 636c  cension and decl
-00000740: 696e 6174 696f 6e2e 0a20 2020 2077 6373  ination..    wcs
-00000750: 3a20 607e 6173 7472 6f70 792e 7763 732e  : `~astropy.wcs.
-00000760: 5743 5360 0a20 2020 2020 2020 2057 4353  WCS`.        WCS
-00000770: 206f 626a 6563 742e 0a0a 2020 2020 5265   object...    Re
-00000780: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00000790: 2d0a 2020 2020 607e 6173 7472 6f70 792e  -.    `~astropy.
-000007a0: 616e 6e6f 7461 7469 6f6e 2e67 656e 6572  annotation.gener
-000007b0: 616c 2e47 726f 7570 416e 6e6f 7461 7469  al.GroupAnnotati
-000007c0: 6f6e 600a 2020 2020 2020 2020 5468 6520  on`.        The 
-000007d0: 616e 6e6f 7461 7469 6f6e 2066 6f72 2074  annotation for t
-000007e0: 6865 2065 6173 7420 616e 6420 6e6f 7274  he east and nort
-000007f0: 6820 6469 7265 6374 696f 6e2e 0a20 2020  h direction..   
-00000800: 20da 0145 da05 7269 6768 7472 1300 0000   ..E..rightr....
-00000810: 7214 0000 0072 1500 0000 7216 0000 0029  r....r....r....)
-00000820: 02e7 3333 3333 3333 1340 7201 0000 00da  ..333333.@r.....
-00000830: 014e 2905 720e 0000 0072 1700 0000 7219  .N).r....r....r.
-00000840: 0000 0072 1a00 0000 721b 0000 0029 0272  ...r....r....).r
-00000850: 0100 0000 7223 0000 004e 2907 7207 0000  ....r#...N).r...
-00000860: 00da 0a4c 4947 4854 5f42 4c55 45da 0974  ...LIGHT_BLUE..t
-00000870: 7261 6e73 6c61 7465 7203 0000 00da 0175  ranslater......u
-00000880: da06 6172 636d 696e 7206 0000 0029 0472  ..arcminr....).r
-00000890: 2000 0000 720e 0000 005a 0f65 6173 745f   ...r....Z.east_
-000008a0: 616e 6e6f 7461 7469 6f6e 5a10 6e6f 7274  annotationZ.nort
-000008b0: 685f 616e 6e6f 7461 7469 6f6e 721d 0000  h_annotationr...
-000008c0: 0072 1d00 0000 721e 0000 00da 1564 6972  .r....r......dir
-000008d0: 6563 7469 6f6e 735f 616e 6e6f 7461 7469  ections_annotati
-000008e0: 6f6e 2e00 0000 7330 0000 0002 0f02 0102  on....s0........
-000008f0: 0102 0102 0102 0102 0102 0102 0104 f810  ................
-00000900: 0902 f702 0a02 0102 0102 0102 0102 0102  ................
-00000910: 0102 0104 f910 0802 f80c 0972 2900 0000  ...........r)...
-00000920: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00000930: 000a 0000 0043 0000 00f3 3a00 0000 7400  .....C....:...t.
-00000940: 7c00 6401 7401 6a02 1400 7c01 6402 6403  |.d.t.j...|.d.d.
-00000950: 8d04 7d02 7403 6404 6405 7c01 6406 6407  ..}.t.d.d.|.d.d.
-00000960: 6408 6409 640a 640b 8d08 7d03 7404 7c02  d.d.d.d...}.t.|.
-00000970: 7c03 6702 8301 5300 290d 6189 0100 000a  |.g...S.).a.....
-00000980: 2020 2020 5265 7475 726e 2061 6e20 616e      Return an an
-00000990: 6e6f 7461 7469 6f6e 2077 6974 6820 7468  notation with th
-000009a0: 6520 5361 6c74 6963 616d 2066 6965 6c64  e Salticam field
-000009b0: 206f 6620 7669 6577 2e0a 0a20 2020 2050   of view...    P
-000009c0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000009d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2060 7e61  --------.    `~a
-000009e0: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
-000009f0: 6573 2e53 6b79 436f 6f72 6460 0a20 2020  es.SkyCoord`.   
-00000a00: 2020 2020 2054 6865 2063 656e 7472 616c       The central
-00000a10: 2070 6f73 6974 696f 6e20 6f66 2074 6865   position of the
-00000a20: 2066 696e 6465 7220 6368 6172 742c 2069   finder chart, i
-00000a30: 6e20 7269 6768 7420 6173 6365 6e73 696f  n right ascensio
-00000a40: 6e20 616e 6420 6465 636c 696e 6174 696f  n and declinatio
-00000a50: 6e2e 0a20 2020 2077 6373 3a20 607e 6173  n..    wcs: `~as
-00000a60: 7472 6f70 792e 7763 732e 5743 5360 0a20  tropy.wcs.WCS`. 
-00000a70: 2020 2020 2020 2057 4353 206f 626a 6563         WCS objec
-00000a80: 742e 0a0a 2020 2020 5265 7475 726e 730a  t...    Returns.
-00000a90: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00000aa0: 607e 696d 6570 6875 2e61 6e6e 6f74 6174  `~imephu.annotat
-00000ab0: 696f 6e2e 6765 6e65 7261 6c2e 4772 6f75  ion.general.Grou
-00000ac0: 7041 6e6e 6f74 6174 696f 6e60 0a20 2020  pAnnotation`.   
-00000ad0: 2020 2020 2041 6e20 616e 6e6f 7461 7469       An annotati
-00000ae0: 6f6e 2077 6974 6820 7468 6520 5361 6c74  on with the Salt
-00000af0: 6963 616d 2066 6965 6c64 206f 6620 7669  icam field of vi
-00000b00: 6577 2e0a 2020 2020 e905 0000 00da 0567  ew..    .......g
-00000b10: 7265 656e a902 720e 0000 00da 0965 6467  reen..r......edg
-00000b20: 6563 6f6c 6f72 2902 e785 eb51 b81e 85eb  ecolor)....Q....
-00000b30: 3f72 2f00 0000 5a04 5343 414d 7213 0000  ?r/...Z.SCAMr...
-00000b40: 0072 1400 0000 7215 0000 00da 046c 6566  .r....r......lef
-00000b50: 74a9 0372 0100 0000 7201 0000 0072 0a00  t..r....r....r..
-00000b60: 0000 a906 720e 0000 0072 1900 0000 721a  ....r....r....r.
-00000b70: 0000 0072 1b00 0000 7218 0000 0072 1700  ...r....r....r..
-00000b80: 0000 4ea9 0572 0800 0000 7227 0000 0072  ..N..r....r'...r
-00000b90: 2800 0000 7207 0000 0072 0600 0000 a904  (...r....r......
-00000ba0: 7220 0000 0072 0e00 0000 5a0e 666f 765f  r ...r....Z.fov_
-00000bb0: 616e 6e6f 7461 7469 6f6e 5a0f 6e61 6d65  annotationZ.name
-00000bc0: 5f61 6e6e 6f74 6174 696f 6e72 1d00 0000  _annotationr....
-00000bd0: 721d 0000 0072 1e00 0000 da21 7361 6c74  r....r.....!salt
-00000be0: 6963 616d 5f66 6965 6c64 5f6f 665f 7669  icam_field_of_vi
-00000bf0: 6577 5f61 6e6e 6f74 6174 696f 6e53 0000  ew_annotationS..
-00000c00: 00f3 1600 0000 1610 0401 0201 0201 0201  ................
-00000c10: 0201 0201 0201 0201 06f9 0c08 7235 0000  ............r5..
-00000c20: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-00000c30: 0000 0a00 0000 4300 0000 722a 0000 0029  ......C...r*...)
-00000c40: 0d61 7f01 0000 0a20 2020 2052 6574 7572  .a.....    Retur
-00000c50: 6e20 616e 2061 6e6e 6f74 6174 696f 6e20  n an annotation 
-00000c60: 7769 7468 2074 6865 2052 5353 2066 6965  with the RSS fie
-00000c70: 6c64 206f 6620 7669 6577 2e0a 0a20 2020  ld of view...   
-00000c80: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00000c90: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2060  ----------.    `
-00000ca0: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
-00000cb0: 6174 6573 2e53 6b79 436f 6f72 6460 0a20  ates.SkyCoord`. 
-00000cc0: 2020 2020 2020 2054 6865 2063 656e 7472         The centr
-00000cd0: 616c 2070 6f73 6974 696f 6e20 6f66 2074  al position of t
-00000ce0: 6865 2066 696e 6465 7220 6368 6172 742c  he finder chart,
-00000cf0: 2069 6e20 7269 6768 7420 6173 6365 6e73   in right ascens
-00000d00: 696f 6e20 616e 6420 6465 636c 696e 6174  ion and declinat
-00000d10: 696f 6e2e 0a20 2020 2077 6373 3a20 607e  ion..    wcs: `~
-00000d20: 6173 7472 6f70 792e 7763 732e 5743 5360  astropy.wcs.WCS`
-00000d30: 0a20 2020 2020 2020 2057 4353 206f 626a  .        WCS obj
-00000d40: 6563 742e 0a0a 2020 2020 5265 7475 726e  ect...    Return
-00000d50: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00000d60: 2020 607e 696d 6570 6875 2e61 6e6e 6f74    `~imephu.annot
-00000d70: 6174 696f 6e2e 6765 6e65 7261 6c2e 4772  ation.general.Gr
-00000d80: 6f75 7041 6e6e 6f74 6174 696f 6e60 0a20  oupAnnotation`. 
-00000d90: 2020 2020 2020 2041 6e20 616e 6e6f 7461         An annota
-00000da0: 7469 6f6e 2077 6974 6820 7468 6520 5253  tion with the RS
-00000db0: 5320 6669 656c 6420 6f66 2076 6965 772e  S field of view.
-00000dc0: 0a20 2020 20e9 0400 0000 722c 0000 0072  .    .....r,...r
-00000dd0: 2d00 0000 2902 e748 e17a 14ae 47e9 3f72  -...)..H.z..G.?r
-00000de0: 3800 0000 5a03 5253 5372 1300 0000 7214  8...Z.RSSr....r.
-00000df0: 0000 0072 1500 0000 7230 0000 0072 3100  ...r....r0...r1.
-00000e00: 0000 7232 0000 004e 7233 0000 0072 3400  ..r2...Nr3...r4.
-00000e10: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000e20: 00da 1c72 7373 5f66 6965 6c64 5f6f 665f  ...rss_field_of_
-00000e30: 7669 6577 5f61 6e6e 6f74 6174 696f 6e6f  view_annotationo
-00000e40: 0000 0072 3600 0000 7239 0000 00da 0e70  ...r6...r9.....p
-00000e50: 6f73 6974 696f 6e5f 616e 676c 65da 1861  osition_angle..a
-00000e60: 7574 6f6d 6174 6564 5f70 6f73 6974 696f  utomated_positio
-00000e70: 6e5f 616e 676c 6563 0300 0000 0000 0000  n_anglec........
-00000e80: 0000 0000 0400 0000 0b00 0000 4300 0000  ............C...
-00000e90: 733a 0000 0064 017c 00a0 0074 016a 02a1  s:...d.|...t.j..
-00000ea0: 0164 029b 049d 027d 037c 0172 107c 0364  .d.....}.|.r.|.d
-00000eb0: 0337 007d 0374 0364 047c 037c 0264 0564  .7.}.t.d.|.|.d.d
-00000ec0: 0664 0764 0864 0964 0a64 0b8d 0953 0029  .d.d.d.d.d...S.)
-00000ed0: 0d61 b102 0000 5265 7475 726e 2061 2074  .a....Return a t
-00000ee0: 6578 7420 616e 6e6f 7461 7469 6f6e 2077  ext annotation w
-00000ef0: 6974 6820 7468 6520 706f 7369 7469 6f6e  ith the position
-00000f00: 2061 6e67 6c65 2e0a 0a20 2020 2054 6865   angle...    The
-00000f10: 2074 6578 7420 6f66 2074 6865 2061 6e6e   text of the ann
-00000f20: 6f74 6174 696f 6e20 6973 2022 5041 3a20  otation is "PA: 
-00000f30: 616e 676c 6520 2861 7574 6f29 222c 2077  angle (auto)", w
-00000f40: 6865 7265 2061 6e67 6c65 2069 7320 6120  here angle is a 
-00000f50: 7661 6c75 6520 696e 2064 6567 7265 6573  value in degrees
-00000f60: 2c0a 2020 2020 6769 7665 6e20 7769 7468  ,.    given with
-00000f70: 206f 6e65 2066 7261 6374 696f 6e61 6c20   one fractional 
-00000f80: 6469 6769 742c 2061 6e64 2077 6865 7265  digit, and where
-00000f90: 2022 2861 7574 6f29 2220 6973 206f 6e6c   "(auto)" is onl
-00000fa0: 7920 696e 636c 7564 6564 2069 6620 7468  y included if th
-00000fb0: 650a 2020 2020 6060 6175 746f 6d61 7465  e.    ``automate
-00000fc0: 6460 6020 7061 7261 6d65 7465 7220 6973  d`` parameter is
-00000fd0: 2060 6054 7275 6560 602e 0a0a 2020 2020   ``True``...    
-00000fe0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00000ff0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 706f  ---------.    po
-00001000: 7369 7469 6f6e 5f61 6e67 6c65 3a20 607e  sition_angle: `~
-00001010: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
-00001020: 7465 732e 416e 676c 6560 0a20 2020 2020  tes.Angle`.     
-00001030: 2020 2054 6865 2070 6f73 6974 696f 6e20     The position 
-00001040: 616e 676c 652c 2061 7320 616e 2061 6e67  angle, as an ang
-00001050: 6c65 206f 6e20 7468 6520 736b 7920 6672  le on the sky fr
-00001060: 6f6d 206e 6f72 7468 2074 6f20 6561 7374  om north to east
-00001070: 2e0a 2020 2020 6175 746f 6d61 7465 645f  ..    automated_
-00001080: 706f 7369 7469 6f6e 5f61 6e67 6c65 3a20  position_angle: 
-00001090: 626f 6f6c 0a20 2020 2020 2020 2057 6865  bool.        Whe
-000010a0: 7468 6572 2074 6865 2070 6f73 6974 696f  ther the positio
-000010b0: 6e20 616e 676c 6520 6861 7320 6265 656e  n angle has been
-000010c0: 2063 616c 6375 6c61 7465 6420 6175 746f   calculated auto
-000010d0: 6d61 7469 6361 6c6c 792e 0a20 2020 2077  matically..    w
-000010e0: 6373 3a20 607e 6173 7472 6f70 792e 7763  cs: `~astropy.wc
-000010f0: 732e 5743 5360 0a20 2020 2020 2020 2057  s.WCS`.        W
-00001100: 4353 206f 626a 6563 742e 0a0a 2020 2020  CS object...    
-00001110: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-00001120: 2d2d 2d0a 2020 2020 607e 696d 6570 6875  ---.    `~imephu
-00001130: 2e61 6e6e 6f74 6174 696f 6e2e 6765 6e65  .annotation.gene
-00001140: 7261 6c2e 5465 7874 416e 6e6f 7461 7469  ral.TextAnnotati
-00001150: 6f6e 600a 2020 2020 2020 2020 5468 6520  on`.        The 
-00001160: 616e 6e6f 7461 7469 6f6e 2066 6f72 2074  annotation for t
-00001170: 6865 2070 6f73 6974 696f 6e20 616e 676c  he position angl
-00001180: 652e 0a20 2020 207a 0550 4120 3d20 7a03  e..    z.PA = z.
-00001190: 2e31 667a 0720 2861 7574 6f29 2902 720a  .1fz. (auto)).r.
-000011a0: 0000 00e7 9cc4 20b0 7268 b1bf 7211 0000  ...... .rh..r...
-000011b0: 0072 2200 0000 da08 6261 7365 6c69 6e65  .r".....baseline
-000011c0: 7213 0000 0072 1400 0000 7215 0000 00a9  r....r....r.....
-000011d0: 0772 0e00 0000 7217 0000 0072 1800 0000  .r....r....r....
-000011e0: da11 7665 7274 6963 616c 616c 6967 6e6d  ..verticalalignm
-000011f0: 656e 7472 1900 0000 721a 0000 0072 1b00  entr....r....r..
-00001200: 0000 4e29 04da 0874 6f5f 7661 6c75 6572  ..N)...to_valuer
-00001210: 2700 0000 da06 6465 6772 6565 7207 0000  '.....degreer...
-00001220: 0029 0472 3a00 0000 723b 0000 0072 0e00  .).r:...r;...r..
-00001230: 0000 da04 7465 7874 721d 0000 0072 1d00  ....textr....r..
-00001240: 0000 721e 0000 00da 1970 6f73 6974 696f  ..r......positio
-00001250: 6e5f 616e 676c 655f 616e 6e6f 7461 7469  n_angle_annotati
-00001260: 6f6e 8b00 0000 731c 0000 0014 1504 0108  on....s.........
-00001270: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00001280: 0102 0102 0106 f772 4300 0000 da0b 7375  .......rC.....su
-00001290: 7276 6579 5f6e 616d 6563 0200 0000 0000  rvey_namec......
-000012a0: 0000 0000 0000 0200 0000 0b00 0000 4300  ..............C.
-000012b0: 0000 731a 0000 0074 0064 017c 007c 0164  ..s....t.d.|.|.d
-000012c0: 0264 0364 0464 0564 0664 0764 088d 0953  .d.d.d.d.d.d...S
-000012d0: 0029 0a61 2601 0000 5265 7475 726e 2061  .).a&...Return a
-000012e0: 2074 6578 7420 616e 6e6f 7461 7469 6f6e   text annotation
-000012f0: 2077 6974 6820 7468 6520 7375 7276 6579   with the survey
-00001300: 206e 616d 652e 0a0a 2020 2020 5061 7261   name...    Para
-00001310: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00001320: 2d2d 2d2d 2d0a 2020 2020 7375 7276 6579  -----.    survey
-00001330: 5f6e 616d 653a 2073 7472 0a20 2020 2020  _name: str.     
-00001340: 2020 2054 6865 2073 7572 7665 7920 6e61     The survey na
-00001350: 6d65 2e0a 2020 2020 7763 733a 2060 7e61  me..    wcs: `~a
-00001360: 7374 726f 7079 2e77 6373 2e57 4353 600a  stropy.wcs.WCS`.
-00001370: 2020 2020 2020 2020 5743 5320 6f62 6a65          WCS obje
-00001380: 6374 2e0a 0a20 2020 2052 6574 7572 6e73  ct...    Returns
-00001390: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-000013a0: 2060 7e69 6d65 7068 752e 616e 6e6f 7461   `~imephu.annota
-000013b0: 7469 6f6e 2e67 656e 6572 616c 2e54 6578  tion.general.Tex
-000013c0: 7441 6e6e 6f74 6174 696f 6e60 0a20 2020  tAnnotation`.   
-000013d0: 2020 2020 2054 6865 2061 6e6e 6f74 6174       The annotat
-000013e0: 696f 6e20 7769 7468 2074 6865 2073 7572  ion with the sur
-000013f0: 7665 7920 6e61 6d65 2e0a 2020 2020 2902  vey name..    ).
-00001400: 7201 0000 0072 3c00 0000 7211 0000 0072  r....r<...r....r
-00001410: 3000 0000 723d 0000 0072 1300 0000 7214  0...r=...r....r.
-00001420: 0000 0072 1500 0000 723e 0000 004e 721c  ...r....r>...Nr.
-00001430: 0000 00a9 0272 4400 0000 720e 0000 0072  .....rD...r....r
-00001440: 1d00 0000 721d 0000 0072 1e00 0000 da11  ....r....r......
-00001450: 7375 7276 6579 5f61 6e6e 6f74 6174 696f  survey_annotatio
-00001460: 6eb0 0000 0073 1600 0000 020f 0201 0201  n....s..........
-00001470: 0201 0201 0201 0201 0201 0201 0201 06f7  ................
-00001480: 7246 0000 0063 0800 0000 0000 0000 0000  rF...c..........
-00001490: 0000 0800 0000 0a00 0000 4300 0000 734a  ..........C...sJ
-000014a0: 0000 0074 0074 017c 007c 017c 027c 0764  ...t.t.|.|.|.|.d
-000014b0: 018d 0474 027c 057c 0764 028d 0274 037c  ...t.|.|.d...t.|
-000014c0: 037c 047c 0764 038d 0374 047c 067c 0764  .|.|.d...t.|.|.d
-000014d0: 048d 0274 057c 067c 0764 048d 0274 067c  ...t.|.|.d...t.|
-000014e0: 067c 0764 048d 0267 0683 0153 0029 0661  .|.d...g...S.).a
-000014f0: 3d04 0000 0a20 2020 2052 6574 7572 6e20  =....    Return 
-00001500: 6120 6772 6f75 7020 636f 6e74 6169 6e69  a group containi
-00001510: 6e67 2061 6c6c 2074 6865 2062 6173 6520  ng all the base 
-00001520: 616e 6e6f 7461 7469 6f6e 7320 666f 7220  annotations for 
-00001530: 5341 4c54 2066 696e 6465 7220 6368 6172  SALT finder char
-00001540: 7473 2e0a 0a20 2020 2054 6865 2062 6173  ts...    The bas
-00001550: 6520 616e 6e6f 7461 7469 6f6e 7320 696e  e annotations in
-00001560: 636c 7564 6520 7468 6520 7469 746c 652c  clude the title,
-00001570: 2064 6972 6563 7469 6f6e 732c 2070 6f73   directions, pos
-00001580: 6974 696f 6e20 616e 676c 652c 2073 7572  ition angle, sur
-00001590: 7665 7920 6e61 6d65 2061 6e64 0a20 2020  vey name and.   
-000015a0: 2074 6865 2052 5353 2061 6e64 2053 616c   the RSS and Sal
-000015b0: 7469 6361 6d20 6669 656c 6473 206f 6620  ticam fields of 
-000015c0: 7669 6577 2e0a 0a20 2020 2050 6172 616d  view...    Param
-000015d0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-000015e0: 2d2d 2d2d 0a20 2020 2074 6172 6765 743a  ----.    target:
-000015f0: 2073 7472 0a20 2020 2020 2020 2054 6865   str.        The
-00001600: 206e 616d 6520 6f66 2074 6865 2074 6172   name of the tar
-00001610: 6765 7420 666f 7220 7768 6963 6820 7468  get for which th
-00001620: 6520 6669 6e64 6572 2063 6861 7274 2069  e finder chart i
-00001630: 7320 696e 7465 6e64 6564 2e0a 2020 2020  s intended..    
-00001640: 7072 6f70 6f73 616c 5f63 6f64 653a 2073  proposal_code: s
-00001650: 7472 0a20 2020 2020 2020 2054 6865 2070  tr.        The p
-00001660: 726f 706f 7361 6c20 636f 6465 2066 6f72  roposal code for
-00001670: 2077 6869 6368 2074 6865 2066 696e 6465   which the finde
-00001680: 7220 6368 6172 7420 6973 2069 6e74 656e  r chart is inten
-00001690: 6465 642e 0a20 2020 2070 695f 6661 6d69  ded..    pi_fami
-000016a0: 6c79 5f6e 616d 653a 2073 7472 0a20 2020  ly_name: str.   
-000016b0: 2020 2020 2054 6865 2066 616d 696c 7920       The family 
-000016c0: 6e61 6d65 206f 6620 7468 6520 5072 696e  name of the Prin
-000016d0: 6369 7061 6c20 496e 7665 7374 6967 6174  cipal Investigat
-000016e0: 6f72 2e0a 2020 2020 706f 7369 7469 6f6e  or..    position
-000016f0: 5f61 6e67 6c65 3a20 607e 6173 7472 6f70  _angle: `~astrop
-00001700: 792e 636f 6f72 6469 6e61 7465 732e 416e  y.coordinates.An
-00001710: 676c 6560 0a20 2020 2020 2020 2054 6865  gle`.        The
-00001720: 2070 6f73 6974 696f 6e20 616e 676c 652c   position angle,
-00001730: 2061 7320 616e 2061 6e67 6c65 206f 6e20   as an angle on 
-00001740: 7468 6520 736b 7920 6672 6f6d 206e 6f72  the sky from nor
-00001750: 7468 2074 6f20 6561 7374 2e0a 2020 2020  th to east..    
-00001760: 6175 746f 6d61 7465 645f 706f 7369 7469  automated_positi
-00001770: 6f6e 5f61 6e67 6c65 3a20 626f 6f6c 0a20  on_angle: bool. 
-00001780: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-00001790: 6865 2070 6f73 6974 696f 6e20 616e 676c  he position angl
-000017a0: 6520 6861 7320 6265 656e 2063 616c 6375  e has been calcu
-000017b0: 6c61 7465 6420 6175 746f 6d61 7469 6361  lated automatica
-000017c0: 6c6c 792e 0a20 2020 2073 7572 7665 795f  lly..    survey_
-000017d0: 6e61 6d65 3a20 7374 720a 2020 2020 2020  name: str.      
-000017e0: 2020 5468 6520 7375 7276 6579 206e 616d    The survey nam
-000017f0: 652e 0a20 2020 2066 6974 735f 6365 6e74  e..    fits_cent
-00001800: 6572 3a20 607e 6173 7472 6f70 792e 636f  er: `~astropy.co
-00001810: 6f72 6469 6e61 7465 732e 536b 7943 6f6f  ordinates.SkyCoo
-00001820: 7264 600a 2020 2020 2020 2020 5468 6520  rd`.        The 
-00001830: 6365 6e74 7261 6c20 706f 7369 7469 6f6e  central position
-00001840: 206f 6620 7468 6520 6669 6e64 6572 2063   of the finder c
-00001850: 6861 7274 2c20 696e 2072 6967 6874 2061  hart, in right a
-00001860: 7363 656e 7369 6f6e 2061 6e64 2064 6563  scension and dec
-00001870: 6c69 6e61 7469 6f6e 0a20 2020 2077 6373  lination.    wcs
-00001880: 3a20 607e 6173 7472 6f70 792e 7763 732e  : `~astropy.wcs.
-00001890: 5743 5360 0a20 2020 2020 2020 2057 4353  WCS`.        WCS
-000018a0: 206f 626a 6563 742e 0a0a 2020 2020 5265   object...    Re
-000018b0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-000018c0: 2d0a 2020 2020 607e 696d 6570 6875 2e61  -.    `~imephu.a
-000018d0: 6e6e 6f74 6174 696f 6e2e 6765 6e65 7261  nnotation.genera
-000018e0: 6c2e 4772 6f75 7041 6e6e 6f74 6174 696f  l.GroupAnnotatio
-000018f0: 6e60 0a20 2020 2020 2020 2041 6e20 616e  n`.        An an
-00001900: 6e6f 7461 7469 6f6e 2077 6974 6820 616c  notation with al
-00001910: 6c20 7468 6520 5341 4c54 2062 6173 6520  l the SALT base 
-00001920: 616e 6e6f 7461 7469 6f6e 732e 0a20 2020  annotations..   
-00001930: 2029 0472 0b00 0000 720c 0000 0072 0d00   ).r....r....r..
-00001940: 0000 720e 0000 0072 4500 0000 2903 723a  ..r....rE...).r:
-00001950: 0000 0072 3b00 0000 720e 0000 0029 0272  ...r;...r....).r
-00001960: 2000 0000 720e 0000 004e 2907 7206 0000   ...r....N).r...
-00001970: 0072 1f00 0000 7246 0000 0072 4300 0000  .r....rF...rC...
-00001980: 7229 0000 0072 3500 0000 7239 0000 0029  r)...r5...r9...)
-00001990: 0872 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000019a0: 723a 0000 0072 3b00 0000 7244 0000 0072  r:...r;...rD...r
-000019b0: 2000 0000 720e 0000 0072 1d00 0000 721d   ...r....r....r.
-000019c0: 0000 0072 1e00 0000 da10 6261 7365 5f61  ...r......base_a
-000019d0: 6e6e 6f74 6174 696f 6e73 cc00 0000 7310  nnotations....s.
-000019e0: 0000 0002 1f0e 010a 010c 010a 010a 010a  ................
-000019f0: 0106 fa72 4700 0000 4e29 16da 0761 7374  ...rG...N)...ast
-00001a00: 726f 7079 7202 0000 0072 2700 0000 da13  ropyr....r'.....
-00001a10: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
-00001a20: 7465 7372 0300 0000 7204 0000 00da 0b61  tesr....r......a
-00001a30: 7374 726f 7079 2e77 6373 7205 0000 00da  stropy.wcsr.....
-00001a40: 1969 6d65 7068 752e 616e 6e6f 7461 7469  .imephu.annotati
-00001a50: 6f6e 2e67 656e 6572 616c 7206 0000 0072  on.generalr....r
-00001a60: 0700 0000 7208 0000 0072 2500 0000 da03  ....r....r%.....
-00001a70: 7374 7272 1f00 0000 7229 0000 0072 3500  strr....r)...r5.
-00001a80: 0000 7239 0000 00da 0462 6f6f 6c72 4300  ..r9.....boolrC.
-00001a90: 0000 7246 0000 0072 4700 0000 721d 0000  ..rF...rG...r...
-00001aa0: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00001ab0: da08 3c6d 6f64 756c 653e 0100 0000 732c  ..<module>....s,
-00001ac0: 0000 000c 0010 010c 0114 0204 0202 0202  ................
-00001ad0: 0102 ff02 0102 ff02 0102 ff02 0102 ff02  ................
-00001ae0: 020a fe16 2516 2516 1c1a 1c16 2532 1c    ....%.%.....%2.
+00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000010: 7274 204f 7074 696f 6e61 6c0a 0a66 726f  rt Optional..fro
+00000020: 6d20 6173 7472 6f70 7920 696d 706f 7274  m astropy import
+00000030: 2075 6e69 7473 2061 7320 750a 6672 6f6d   units as u.from
+00000040: 2061 7374 726f 7079 2e63 6f6f 7264 696e   astropy.coordin
+00000050: 6174 6573 2069 6d70 6f72 7420 416e 676c  ates import Angl
+00000060: 652c 2053 6b79 436f 6f72 640a 6672 6f6d  e, SkyCoord.from
+00000070: 2061 7374 726f 7079 2e77 6373 2069 6d70   astropy.wcs imp
+00000080: 6f72 7420 5743 530a 6672 6f6d 2069 6d65  ort WCS.from ime
+00000090: 7068 752e 616e 6e6f 7461 7469 6f6e 2e67  phu.annotation.g
+000000a0: 656e 6572 616c 2069 6d70 6f72 7420 280a  eneral import (.
+000000b0: 2020 2020 4372 6f73 7368 6169 7273 416e      CrosshairsAn
+000000c0: 6e6f 7461 7469 6f6e 2c0a 2020 2020 456d  notation,.    Em
+000000d0: 7074 7941 6e6e 6f74 6174 696f 6e2c 0a20  ptyAnnotation,. 
+000000e0: 2020 2047 726f 7570 416e 6e6f 7461 7469     GroupAnnotati
+000000f0: 6f6e 2c0a 2020 2020 5265 6374 616e 676c  on,.    Rectangl
+00000100: 6541 6e6e 6f74 6174 696f 6e2c 0a20 2020  eAnnotation,.   
+00000110: 2054 6578 7441 6e6e 6f74 6174 696f 6e2c   TextAnnotation,
+00000120: 0a29 0a66 726f 6d20 696d 6570 6875 2e73  .).from imephu.s
+00000130: 616c 742e 616e 6e6f 7461 7469 6f6e 2069  alt.annotation i
+00000140: 6d70 6f72 7420 7273 732c 2073 616c 7469  mport rss, salti
+00000150: 6361 6d0a 0a0a 6465 6620 7469 746c 655f  cam...def title_
+00000160: 616e 6e6f 7461 7469 6f6e 280a 2020 2020  annotation(.    
+00000170: 7461 7267 6574 3a20 7374 722c 2070 726f  target: str, pro
+00000180: 706f 7361 6c5f 636f 6465 3a20 7374 722c  posal_code: str,
+00000190: 2070 695f 6661 6d69 6c79 5f6e 616d 653a   pi_family_name:
+000001a0: 2073 7472 2c20 7763 733a 2057 4353 0a29   str, wcs: WCS.)
+000001b0: 202d 3e20 5465 7874 416e 6e6f 7461 7469   -> TextAnnotati
+000001c0: 6f6e 3a0a 2020 2020 2222 2252 6574 7572  on:.    """Retur
+000001d0: 6e20 6120 7465 7874 2061 6e6e 6f74 6174  n a text annotat
+000001e0: 696f 6e20 7769 7468 2074 6865 2074 6974  ion with the tit
+000001f0: 6c65 2074 6f20 7468 6520 6669 6e64 6572  le to the finder
+00000200: 2063 6861 7274 2e0a 0a20 2020 2054 6865   chart...    The
+00000210: 2074 6974 6c65 2069 7320 6f66 2074 6865   title is of the
+00000220: 2066 6f72 6d20 2274 6172 6765 7420 6e61   form "target na
+00000230: 6d65 2028 7072 6f70 6f73 616c 2063 6f64  me (proposal cod
+00000240: 653b 2073 7572 6e61 6d65 206f 6620 7468  e; surname of th
+00000250: 6520 5072 696e 6369 7061 6c0a 2020 2020  e Principal.    
+00000260: 496e 7665 7374 6967 6174 6f72 2922 2c20  Investigator)", 
+00000270: 7375 6368 2061 7320 224d 6167 7261 7468  such as "Magrath
+00000280: 6561 2028 3230 3232 2d31 2d53 4349 2d30  ea (2022-1-SCI-0
+00000290: 3432 3b20 4164 616d 7329 222e 0a0a 2020  42; Adams)"...  
+000002a0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000002b0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000002c0: 7461 7267 6574 3a20 7374 720a 2020 2020  target: str.    
+000002d0: 2020 2020 5468 6520 6e61 6d65 206f 6620      The name of 
+000002e0: 7468 6520 7461 7267 6574 2066 6f72 2077  the target for w
+000002f0: 6869 6368 2074 6865 2066 696e 6465 7220  hich the finder 
+00000300: 6368 6172 7420 6973 2069 6e74 656e 6465  chart is intende
+00000310: 642e 0a20 2020 2070 726f 706f 7361 6c5f  d..    proposal_
+00000320: 636f 6465 3a20 7374 720a 2020 2020 2020  code: str.      
+00000330: 2020 5468 6520 7072 6f70 6f73 616c 2063    The proposal c
+00000340: 6f64 6520 666f 7220 7768 6963 6820 7468  ode for which th
+00000350: 6520 6669 6e64 6572 2063 6861 7274 2069  e finder chart i
+00000360: 7320 696e 7465 6e64 6564 2e0a 2020 2020  s intended..    
+00000370: 7069 5f66 616d 696c 795f 6e61 6d65 3a20  pi_family_name: 
+00000380: 7374 720a 2020 2020 2020 2020 5468 6520  str.        The 
+00000390: 6661 6d69 6c79 206e 616d 6520 6f66 2074  family name of t
+000003a0: 6865 2050 7269 6e63 6970 616c 2049 6e76  he Principal Inv
+000003b0: 6573 7469 6761 746f 722e 0a20 2020 2077  estigator..    w
+000003c0: 6373 3a20 607e 6173 7472 6f70 792e 7763  cs: `~astropy.wc
+000003d0: 732e 5743 5360 0a20 2020 2020 2020 2057  s.WCS`.        W
+000003e0: 4353 206f 626a 6563 742e 0a0a 2020 2020  CS object...    
+000003f0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00000400: 2d2d 2d0a 2020 2020 607e 696d 6570 6875  ---.    `~imephu
+00000410: 2e61 6e6e 6f74 6174 696f 6e2e 6765 6e65  .annotation.gene
+00000420: 7261 6c2e 5465 7874 416e 6e6f 7461 7469  ral.TextAnnotati
+00000430: 6f6e 600a 2020 2020 2020 2020 5468 6520  on`.        The 
+00000440: 7469 746c 6520 616e 6e6f 7461 7469 6f6e  title annotation
+00000450: 2e0a 2020 2020 2222 220a 2020 2020 7469  ..    """.    ti
+00000460: 746c 655f 7465 7874 203d 2066 227b 7461  tle_text = f"{ta
+00000470: 7267 6574 7d20 287b 7072 6f70 6f73 616c  rget} ({proposal
+00000480: 5f63 6f64 657d 3b20 7b70 695f 6661 6d69  _code}; {pi_fami
+00000490: 6c79 5f6e 616d 657d 2922 0a20 2020 2072  ly_name})".    r
+000004a0: 6574 7572 6e20 5465 7874 416e 6e6f 7461  eturn TextAnnota
+000004b0: 7469 6f6e 280a 2020 2020 2020 2020 2830  tion(.        (0
+000004c0: 2e35 2c20 312e 3033 292c 0a20 2020 2020  .5, 1.03),.     
+000004d0: 2020 2074 6974 6c65 5f74 6578 742c 0a20     title_text,. 
+000004e0: 2020 2020 2020 2077 6373 3d77 6373 2c0a         wcs=wcs,.
+000004f0: 2020 2020 2020 2020 636f 6c6f 723d 2262          color="b
+00000500: 6c61 636b 222c 0a20 2020 2020 2020 2068  lack",.        h
+00000510: 6f72 697a 6f6e 7461 6c61 6c69 676e 6d65  orizontalalignme
+00000520: 6e74 3d22 6365 6e74 6572 222c 0a20 2020  nt="center",.   
+00000530: 2020 2020 2073 7479 6c65 3d22 6974 616c       style="ital
+00000540: 6963 222c 0a20 2020 2020 2020 2077 6569  ic",.        wei
+00000550: 6768 743d 2262 6f6c 6422 2c0a 2020 2020  ght="bold",.    
+00000560: 2020 2020 7369 7a65 3d22 6c61 7267 6522      size="large"
+00000570: 2c0a 2020 2020 2020 2020 636c 6970 5f6f  ,.        clip_o
+00000580: 6e3d 4661 6c73 652c 0a20 2020 2029 0a0a  n=False,.    )..
+00000590: 0a64 6566 2064 6972 6563 7469 6f6e 735f  .def directions_
+000005a0: 616e 6e6f 7461 7469 6f6e 2866 6974 735f  annotation(fits_
+000005b0: 6365 6e74 6572 3a20 536b 7943 6f6f 7264  center: SkyCoord
+000005c0: 2c20 7763 733a 2057 4353 2920 2d3e 2047  , wcs: WCS) -> G
+000005d0: 726f 7570 416e 6e6f 7461 7469 6f6e 3a0a  roupAnnotation:.
+000005e0: 2020 2020 2222 2252 6574 7572 6e20 616e      """Return an
+000005f0: 2061 6e6e 6f74 6174 696f 6e20 666f 7220   annotation for 
+00000600: 7468 6520 6561 7374 2061 6e64 206e 6f72  the east and nor
+00000610: 7468 2064 6972 6563 7469 6f6e 2e0a 0a20  th direction... 
+00000620: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00000630: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00000640: 2066 6974 735f 6365 6e74 6572 3a20 607e   fits_center: `~
+00000650: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
+00000660: 7465 732e 536b 7943 6f6f 7264 600a 2020  tes.SkyCoord`.  
+00000670: 2020 2020 2020 5468 6520 6365 6e74 7261        The centra
+00000680: 6c20 706f 7369 7469 6f6e 206f 6620 7468  l position of th
+00000690: 6520 6669 6e64 6572 2063 6861 7274 2c20  e finder chart, 
+000006a0: 696e 2072 6967 6874 2061 7363 656e 7369  in right ascensi
+000006b0: 6f6e 2061 6e64 2064 6563 6c69 6e61 7469  on and declinati
+000006c0: 6f6e 2e0a 2020 2020 7763 733a 2060 7e61  on..    wcs: `~a
+000006d0: 7374 726f 7079 2e77 6373 2e57 4353 600a  stropy.wcs.WCS`.
+000006e0: 2020 2020 2020 2020 5743 5320 6f62 6a65          WCS obje
+000006f0: 6374 2e0a 0a20 2020 2052 6574 7572 6e73  ct...    Returns
+00000700: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00000710: 2060 7e61 7374 726f 7079 2e61 6e6e 6f74   `~astropy.annot
+00000720: 6174 696f 6e2e 6765 6e65 7261 6c2e 4772  ation.general.Gr
+00000730: 6f75 7041 6e6e 6f74 6174 696f 6e60 0a20  oupAnnotation`. 
+00000740: 2020 2020 2020 2054 6865 2061 6e6e 6f74         The annot
+00000750: 6174 696f 6e20 666f 7220 7468 6520 6561  ation for the ea
+00000760: 7374 2061 6e64 206e 6f72 7468 2064 6972  st and north dir
+00000770: 6563 7469 6f6e 2e0a 2020 2020 2222 220a  ection..    """.
+00000780: 2020 2020 6561 7374 5f61 6e6e 6f74 6174      east_annotat
+00000790: 696f 6e20 3d20 5465 7874 416e 6e6f 7461  ion = TextAnnota
+000007a0: 7469 6f6e 280a 2020 2020 2020 2020 6669  tion(.        fi
+000007b0: 7473 5f63 656e 7465 722c 0a20 2020 2020  ts_center,.     
+000007c0: 2020 2022 4522 2c0a 2020 2020 2020 2020     "E",.        
+000007d0: 7763 733d 7763 732c 0a20 2020 2020 2020  wcs=wcs,.       
+000007e0: 2063 6f6c 6f72 3d28 302c 2030 2e35 2c20   color=(0, 0.5, 
+000007f0: 3129 2c0a 2020 2020 2020 2020 686f 7269  1),.        hori
+00000800: 7a6f 6e74 616c 616c 6967 6e6d 656e 743d  zontalalignment=
+00000810: 2272 6967 6874 222c 0a20 2020 2020 2020  "right",.       
+00000820: 2073 7479 6c65 3d22 6974 616c 6963 222c   style="italic",
+00000830: 0a20 2020 2020 2020 2077 6569 6768 743d  .        weight=
+00000840: 2262 6f6c 6422 2c0a 2020 2020 2020 2020  "bold",.        
+00000850: 7369 7a65 3d22 6c61 7267 6522 2c0a 2020  size="large",.  
+00000860: 2020 292e 7472 616e 736c 6174 6528 416e    ).translate(An
+00000870: 676c 6528 2834 2e38 2c20 3029 202a 2075  gle((4.8, 0) * u
+00000880: 2e61 7263 6d69 6e29 290a 2020 2020 6e6f  .arcmin)).    no
+00000890: 7274 685f 616e 6e6f 7461 7469 6f6e 203d  rth_annotation =
+000008a0: 2054 6578 7441 6e6e 6f74 6174 696f 6e28   TextAnnotation(
+000008b0: 0a20 2020 2020 2020 2066 6974 735f 6365  .        fits_ce
+000008c0: 6e74 6572 2c0a 2020 2020 2020 2020 224e  nter,.        "N
+000008d0: 222c 0a20 2020 2020 2020 2077 6373 3d77  ",.        wcs=w
+000008e0: 6373 2c0a 2020 2020 2020 2020 636f 6c6f  cs,.        colo
+000008f0: 723d 2830 2c20 302e 352c 2031 292c 0a20  r=(0, 0.5, 1),. 
+00000900: 2020 2020 2020 2073 7479 6c65 3d22 6974         style="it
+00000910: 616c 6963 222c 0a20 2020 2020 2020 2077  alic",.        w
+00000920: 6569 6768 743d 2262 6f6c 6422 2c0a 2020  eight="bold",.  
+00000930: 2020 2020 2020 7369 7a65 3d22 6c61 7267        size="larg
+00000940: 6522 2c0a 2020 2020 292e 7472 616e 736c  e",.    ).transl
+00000950: 6174 6528 416e 676c 6528 2830 2c20 342e  ate(Angle((0, 4.
+00000960: 3829 202a 2075 2e61 7263 6d69 6e29 290a  8) * u.arcmin)).
+00000970: 2020 2020 7265 7475 726e 2047 726f 7570      return Group
+00000980: 416e 6e6f 7461 7469 6f6e 285b 6561 7374  Annotation([east
+00000990: 5f61 6e6e 6f74 6174 696f 6e2c 206e 6f72  _annotation, nor
+000009a0: 7468 5f61 6e6e 6f74 6174 696f 6e5d 290a  th_annotation]).
+000009b0: 0a0a 6465 6620 706f 7369 7469 6f6e 5f61  ..def position_a
+000009c0: 6e67 6c65 5f61 6e6e 6f74 6174 696f 6e28  ngle_annotation(
+000009d0: 0a20 2020 2070 6f73 6974 696f 6e5f 616e  .    position_an
+000009e0: 676c 653a 2041 6e67 6c65 2c20 6175 746f  gle: Angle, auto
+000009f0: 6d61 7465 645f 706f 7369 7469 6f6e 5f61  mated_position_a
+00000a00: 6e67 6c65 3a20 626f 6f6c 2c20 7763 733a  ngle: bool, wcs:
+00000a10: 2057 4353 0a29 202d 3e20 5465 7874 416e   WCS.) -> TextAn
+00000a20: 6e6f 7461 7469 6f6e 3a0a 2020 2020 2222  notation:.    ""
+00000a30: 2252 6574 7572 6e20 6120 7465 7874 2061  "Return a text a
+00000a40: 6e6e 6f74 6174 696f 6e20 7769 7468 2074  nnotation with t
+00000a50: 6865 2070 6f73 6974 696f 6e20 616e 676c  he position angl
+00000a60: 652e 0a0a 2020 2020 5468 6520 7465 7874  e...    The text
+00000a70: 206f 6620 7468 6520 616e 6e6f 7461 7469   of the annotati
+00000a80: 6f6e 2069 7320 2250 413a 2061 6e67 6c65  on is "PA: angle
+00000a90: 2028 6175 746f 2922 2c20 7768 6572 6520   (auto)", where 
+00000aa0: 616e 676c 6520 6973 2061 2076 616c 7565  angle is a value
+00000ab0: 2069 6e20 6465 6772 6565 732c 0a20 2020   in degrees,.   
+00000ac0: 2067 6976 656e 2077 6974 6820 6f6e 6520   given with one 
+00000ad0: 6672 6163 7469 6f6e 616c 2064 6967 6974  fractional digit
+00000ae0: 2c20 616e 6420 7768 6572 6520 2228 6175  , and where "(au
+00000af0: 746f 2922 2069 7320 6f6e 6c79 2069 6e63  to)" is only inc
+00000b00: 6c75 6465 6420 6966 2074 6865 0a20 2020  luded if the.   
+00000b10: 2060 6061 7574 6f6d 6174 6564 6060 2070   ``automated`` p
+00000b20: 6172 616d 6574 6572 2069 7320 6060 5472  arameter is ``Tr
+00000b30: 7565 6060 2e0a 0a20 2020 2050 6172 616d  ue``...    Param
+00000b40: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00000b50: 2d2d 2d2d 0a20 2020 2070 6f73 6974 696f  ----.    positio
+00000b60: 6e5f 616e 676c 653a 2060 7e61 7374 726f  n_angle: `~astro
+00000b70: 7079 2e63 6f6f 7264 696e 6174 6573 2e41  py.coordinates.A
+00000b80: 6e67 6c65 600a 2020 2020 2020 2020 5468  ngle`.        Th
+00000b90: 6520 706f 7369 7469 6f6e 2061 6e67 6c65  e position angle
+00000ba0: 2c20 6173 2061 6e20 616e 676c 6520 6f6e  , as an angle on
+00000bb0: 2074 6865 2073 6b79 2066 726f 6d20 6e6f   the sky from no
+00000bc0: 7274 6820 746f 2065 6173 742e 0a20 2020  rth to east..   
+00000bd0: 2061 7574 6f6d 6174 6564 5f70 6f73 6974   automated_posit
+00000be0: 696f 6e5f 616e 676c 653a 2062 6f6f 6c0a  ion_angle: bool.
+00000bf0: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00000c00: 7468 6520 706f 7369 7469 6f6e 2061 6e67  the position ang
+00000c10: 6c65 2068 6173 2062 6565 6e20 6361 6c63  le has been calc
+00000c20: 756c 6174 6564 2061 7574 6f6d 6174 6963  ulated automatic
+00000c30: 616c 6c79 2e0a 2020 2020 7763 733a 2060  ally..    wcs: `
+00000c40: 7e61 7374 726f 7079 2e77 6373 2e57 4353  ~astropy.wcs.WCS
+00000c50: 600a 2020 2020 2020 2020 5743 5320 6f62  `.        WCS ob
+00000c60: 6a65 6374 2e0a 0a20 2020 2052 6574 7572  ject...    Retur
+00000c70: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00000c80: 2020 2060 7e69 6d65 7068 752e 616e 6e6f     `~imephu.anno
+00000c90: 7461 7469 6f6e 2e67 656e 6572 616c 2e54  tation.general.T
+00000ca0: 6578 7441 6e6e 6f74 6174 696f 6e60 0a20  extAnnotation`. 
+00000cb0: 2020 2020 2020 2054 6865 2061 6e6e 6f74         The annot
+00000cc0: 6174 696f 6e20 666f 7220 7468 6520 706f  ation for the po
+00000cd0: 7369 7469 6f6e 2061 6e67 6c65 2e0a 2020  sition angle..  
+00000ce0: 2020 2222 220a 2020 2020 7465 7874 203d    """.    text =
+00000cf0: 2066 2250 4120 3d20 7b70 6f73 6974 696f   f"PA = {positio
+00000d00: 6e5f 616e 676c 652e 746f 5f76 616c 7565  n_angle.to_value
+00000d10: 2875 2e64 6567 7265 6529 3a2e 3166 7d22  (u.degree):.1f}"
+00000d20: 0a20 2020 2069 6620 6175 746f 6d61 7465  .    if automate
+00000d30: 645f 706f 7369 7469 6f6e 5f61 6e67 6c65  d_position_angle
+00000d40: 3a0a 2020 2020 2020 2020 7465 7874 202b  :.        text +
+00000d50: 3d20 2220 2861 7574 6f29 220a 2020 2020  = " (auto)".    
+00000d60: 7265 7475 726e 2054 6578 7441 6e6e 6f74  return TextAnnot
+00000d70: 6174 696f 6e28 0a20 2020 2020 2020 2028  ation(.        (
+00000d80: 312c 202d 302e 3036 3829 2c0a 2020 2020  1, -0.068),.    
+00000d90: 2020 2020 7465 7874 2c0a 2020 2020 2020      text,.      
+00000da0: 2020 7763 733d 7763 732c 0a20 2020 2020    wcs=wcs,.     
+00000db0: 2020 2063 6f6c 6f72 3d22 626c 6163 6b22     color="black"
+00000dc0: 2c0a 2020 2020 2020 2020 686f 7269 7a6f  ,.        horizo
+00000dd0: 6e74 616c 616c 6967 6e6d 656e 743d 2272  ntalalignment="r
+00000de0: 6967 6874 222c 0a20 2020 2020 2020 2076  ight",.        v
+00000df0: 6572 7469 6361 6c61 6c69 676e 6d65 6e74  erticalalignment
+00000e00: 3d22 6261 7365 6c69 6e65 222c 0a20 2020  ="baseline",.   
+00000e10: 2020 2020 2073 7479 6c65 3d22 6974 616c       style="ital
+00000e20: 6963 222c 0a20 2020 2020 2020 2077 6569  ic",.        wei
+00000e30: 6768 743d 2262 6f6c 6422 2c0a 2020 2020  ght="bold",.    
+00000e40: 2020 2020 7369 7a65 3d22 6c61 7267 6522      size="large"
+00000e50: 2c0a 2020 2020 2020 2020 636c 6970 5f6f  ,.        clip_o
+00000e60: 6e3d 4661 6c73 652c 0a20 2020 2029 0a0a  n=False,.    )..
+00000e70: 0a64 6566 2073 7572 7665 795f 616e 6e6f  .def survey_anno
+00000e80: 7461 7469 6f6e 2873 7572 7665 793a 2073  tation(survey: s
+00000e90: 7472 2c20 7763 733a 2057 4353 2920 2d3e  tr, wcs: WCS) ->
+00000ea0: 2054 6578 7441 6e6e 6f74 6174 696f 6e3a   TextAnnotation:
+00000eb0: 0a20 2020 2022 2222 5265 7475 726e 2061  .    """Return a
+00000ec0: 2074 6578 7420 616e 6e6f 7461 7469 6f6e   text annotation
+00000ed0: 2077 6974 6820 7468 6520 7375 7276 6579   with the survey
+00000ee0: 206e 616d 652e 0a0a 2020 2020 5061 7261   name...    Para
+00000ef0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00000f00: 2d2d 2d2d 2d0a 2020 2020 7375 7276 6579  -----.    survey
+00000f10: 3a20 7374 720a 2020 2020 2020 2020 5468  : str.        Th
+00000f20: 6520 7375 7276 6579 206e 616d 652e 0a20  e survey name.. 
+00000f30: 2020 2077 6373 3a20 607e 6173 7472 6f70     wcs: `~astrop
+00000f40: 792e 7763 732e 5743 5360 0a20 2020 2020  y.wcs.WCS`.     
+00000f50: 2020 2057 4353 206f 626a 6563 742e 0a0a     WCS object...
+00000f60: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00000f70: 2d2d 2d2d 2d2d 2d0a 2020 2020 607e 696d  -------.    `~im
+00000f80: 6570 6875 2e61 6e6e 6f74 6174 696f 6e2e  ephu.annotation.
+00000f90: 6765 6e65 7261 6c2e 5465 7874 416e 6e6f  general.TextAnno
+00000fa0: 7461 7469 6f6e 600a 2020 2020 2020 2020  tation`.        
+00000fb0: 5468 6520 616e 6e6f 7461 7469 6f6e 2077  The annotation w
+00000fc0: 6974 6820 7468 6520 7375 7276 6579 206e  ith the survey n
+00000fd0: 616d 652e 0a20 2020 2022 2222 0a20 2020  ame..    """.   
+00000fe0: 2072 6574 7572 6e20 5465 7874 416e 6e6f   return TextAnno
+00000ff0: 7461 7469 6f6e 280a 2020 2020 2020 2020  tation(.        
+00001000: 2830 2c20 2d30 2e30 3638 292c 0a20 2020  (0, -0.068),.   
+00001010: 2020 2020 2073 7572 7665 792c 0a20 2020       survey,.   
+00001020: 2020 2020 2077 6373 3d77 6373 2c0a 2020       wcs=wcs,.  
+00001030: 2020 2020 2020 636f 6c6f 723d 2262 6c61        color="bla
+00001040: 636b 222c 0a20 2020 2020 2020 2068 6f72  ck",.        hor
+00001050: 697a 6f6e 7461 6c61 6c69 676e 6d65 6e74  izontalalignment
+00001060: 3d22 6c65 6674 222c 0a20 2020 2020 2020  ="left",.       
+00001070: 2076 6572 7469 6361 6c61 6c69 676e 6d65   verticalalignme
+00001080: 6e74 3d22 6261 7365 6c69 6e65 222c 0a20  nt="baseline",. 
+00001090: 2020 2020 2020 2073 7479 6c65 3d22 6974         style="it
+000010a0: 616c 6963 222c 0a20 2020 2020 2020 2077  alic",.        w
+000010b0: 6569 6768 743d 2262 6f6c 6422 2c0a 2020  eight="bold",.  
+000010c0: 2020 2020 2020 7369 7a65 3d22 6c61 7267        size="larg
+000010d0: 6522 2c0a 2020 2020 2020 2020 636c 6970  e",.        clip
+000010e0: 5f6f 6e3d 4661 6c73 652c 0a20 2020 2029  _on=False,.    )
+000010f0: 0a0a 0a64 6566 206d 6167 6e69 7475 6465  ...def magnitude
+00001100: 5f72 616e 6765 5f61 6e6e 6f74 6174 696f  _range_annotatio
+00001110: 6e28 0a20 2020 2062 616e 6470 6173 733a  n(.    bandpass:
+00001120: 2073 7472 2c0a 2020 2020 6d69 6e5f 6d61   str,.    min_ma
+00001130: 676e 6974 7564 653a 2066 6c6f 6174 2c0a  gnitude: float,.
+00001140: 2020 2020 6d61 785f 6d61 676e 6974 7564      max_magnitud
+00001150: 653a 2066 6c6f 6174 2c0a 2020 2020 7763  e: float,.    wc
+00001160: 733a 2057 4353 2c0a 2920 2d3e 2054 6578  s: WCS,.) -> Tex
+00001170: 7441 6e6e 6f74 6174 696f 6e3a 0a20 2020  tAnnotation:.   
+00001180: 2022 2222 5265 7475 726e 2061 2074 6578   """Return a tex
+00001190: 7420 616e 6e6f 7461 7469 6f6e 2077 6974  t annotation wit
+000011a0: 6820 7468 6520 6d61 676e 6974 7564 6520  h the magnitude 
+000011b0: 7261 6e67 652e 0a0a 2020 2020 5468 6520  range...    The 
+000011c0: 6d61 676e 6974 7564 6520 7261 6e67 6520  magnitude range 
+000011d0: 6973 2067 6976 656e 2061 7320 6120 7374  is given as a st
+000011e0: 7269 6e67 206f 6620 7468 6520 666f 726d  ring of the form
+000011f0: 2022 6261 6e64 7061 7373 203d 206d 696e   "bandpass = min
+00001200: 206d 6167 6e69 7475 6465 202d 0a20 2020   magnitude -.   
+00001210: 206d 6178 206d 6167 6e69 7475 6465 222c   max magnitude",
+00001220: 2077 6865 7265 2074 6865 206d 6167 6e69   where the magni
+00001230: 7475 6465 7320 6861 7665 206f 6e65 2066  tudes have one f
+00001240: 7261 6374 696f 6e61 6c20 6469 6769 742e  ractional digit.
+00001250: 2049 6620 7468 6520 6469 6666 6572 656e   If the differen
+00001260: 6365 0a20 2020 2062 6574 7765 656e 2074  ce.    between t
+00001270: 6865 206d 696e 696d 756d 2061 6e64 206d  he minimum and m
+00001280: 6178 696d 756d 206d 6167 6e69 7475 6465  aximum magnitude
+00001290: 2069 7320 6c65 7373 2074 6861 6e20 302e   is less than 0.
+000012a0: 312c 206f 6e6c 7920 7468 6520 6d61 7869  1, only the maxi
+000012b0: 6d75 6d0a 2020 2020 6d61 676e 6974 7564  mum.    magnitud
+000012c0: 6520 6973 2069 6e63 6c75 6465 642e 0a0a  e is included...
+000012d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000012e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000012f0: 2020 6261 6e64 7061 7373 3a20 6073 7472    bandpass: `str
+00001300: 600a 2020 2020 2020 2020 4261 6e64 7061  `.        Bandpa
+00001310: 7373 2066 6f72 2077 6869 6368 2074 6865  ss for which the
+00001320: 206d 6167 6e69 7475 6465 2072 616e 6765   magnitude range
+00001330: 2069 7320 6769 7665 6e2e 0a20 2020 206d   is given..    m
+00001340: 696e 5f6d 6167 6e69 7475 6465 3a20 6066  in_magnitude: `f
+00001350: 6c6f 6174 600a 2020 2020 2020 2020 4d69  loat`.        Mi
+00001360: 6e69 6d75 6d20 2862 7269 6768 7465 7374  nimum (brightest
+00001370: 2920 6d61 676e 6974 7564 652e 0a20 2020  ) magnitude..   
+00001380: 206d 6178 5f6d 6167 6e69 7475 6465 3a20   max_magnitude: 
+00001390: 6066 6c6f 6174 600a 2020 2020 2020 2020  `float`.        
+000013a0: 4d61 7869 6d75 6d20 2866 6169 6e74 6573  Maximum (faintes
+000013b0: 7429 206d 6167 6e69 7475 6465 2e0a 2020  t) magnitude..  
+000013c0: 2020 6669 7473 5f63 656e 7465 723a 2060    fits_center: `
+000013d0: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
+000013e0: 6174 6573 2e53 6b79 436f 6f72 6460 0a20  ates.SkyCoord`. 
+000013f0: 2020 2020 2020 2043 656e 7465 7220 706f         Center po
+00001400: 7369 7469 6f6e 206f 6620 7468 6520 6669  sition of the fi
+00001410: 6e64 6572 2063 6861 7274 2c20 6173 2061  nder chart, as a
+00001420: 2072 6967 6874 2061 7363 656e 7369 6f6e   right ascension
+00001430: 2061 6e64 2064 6563 6c69 6e61 7469 6f6e   and declination
+00001440: 2e0a 2020 2020 7763 733a 2060 7e61 7374  ..    wcs: `~ast
+00001450: 726f 7079 2e77 6373 2e57 4353 600a 2020  ropy.wcs.WCS`.  
+00001460: 2020 2020 2020 5743 5320 6f62 6a65 6374        WCS object
+00001470: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+00001480: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2060     -------.    `
+00001490: 7e69 6d65 7068 752e 616e 6e6f 7461 7469  ~imephu.annotati
+000014a0: 6f6e 2e67 656e 6572 616c 2e54 6578 7441  on.general.TextA
+000014b0: 6e6e 6f74 6174 696f 6e60 0a20 2020 2020  nnotation`.     
+000014c0: 2020 2054 6865 206d 6167 6e69 7475 6465     The magnitude
+000014d0: 2072 616e 6765 2061 6e6e 6f74 6174 696f   range annotatio
+000014e0: 6e2e 0a20 2020 2022 2222 0a20 2020 2069  n..    """.    i
+000014f0: 6620 6162 7328 6d61 785f 6d61 676e 6974  f abs(max_magnit
+00001500: 7564 6520 2d20 6d69 6e5f 6d61 676e 6974  ude - min_magnit
+00001510: 7564 6529 203e 2030 2e30 3939 3939 3a0a  ude) > 0.09999:.
+00001520: 2020 2020 2020 2020 7465 7874 203d 2066          text = f
+00001530: 227b 6261 6e64 7061 7373 7d20 3d20 7b6d  "{bandpass} = {m
+00001540: 696e 5f6d 6167 6e69 7475 6465 3a2e 3166  in_magnitude:.1f
+00001550: 7d20 2d20 7b6d 6178 5f6d 6167 6e69 7475  } - {max_magnitu
+00001560: 6465 3a2e 3166 7d22 0a20 2020 2065 6c73  de:.1f}".    els
+00001570: 653a 0a20 2020 2020 2020 2074 6578 7420  e:.        text 
+00001580: 3d20 6622 7b62 616e 6470 6173 737d 203d  = f"{bandpass} =
+00001590: 207b 6d61 785f 6d61 676e 6974 7564 653a   {max_magnitude:
+000015a0: 2e31 667d 220a 2020 2020 7265 7475 726e  .1f}".    return
+000015b0: 2054 6578 7441 6e6e 6f74 6174 696f 6e28   TextAnnotation(
+000015c0: 0a20 2020 2020 2020 2028 302e 352c 2030  .        (0.5, 0
+000015d0: 2e30 3229 2c0a 2020 2020 2020 2020 7465  .02),.        te
+000015e0: 7874 2c0a 2020 2020 2020 2020 7763 732c  xt,.        wcs,
+000015f0: 0a20 2020 2020 2020 2063 6f6c 6f72 3d28  .        color=(
+00001600: 302c 2030 2e35 2c20 3129 2c0a 2020 2020  0, 0.5, 1),.    
+00001610: 2020 2020 7374 796c 653d 2269 7461 6c69      style="itali
+00001620: 6322 2c0a 2020 2020 2020 2020 7765 6967  c",.        weig
+00001630: 6874 3d22 626f 6c64 222c 0a20 2020 2020  ht="bold",.     
+00001640: 2020 2073 697a 653d 226c 6172 6765 222c     size="large",
+00001650: 0a20 2020 2020 2020 2068 6f72 697a 6f6e  .        horizon
+00001660: 7461 6c61 6c69 676e 6d65 6e74 3d22 6365  talalignment="ce
+00001670: 6e74 6572 222c 0a20 2020 2020 2020 2076  nter",.        v
+00001680: 6572 7469 6361 6c61 6c69 676e 6d65 6e74  erticalalignment
+00001690: 3d22 6261 7365 6c69 6e65 222c 0a20 2020  ="baseline",.   
+000016a0: 2029 0a0a 0a64 6566 2073 6c6f 745f 616e   )...def slot_an
+000016b0: 6e6f 7461 7469 6f6e 280a 2020 2020 6365  notation(.    ce
+000016c0: 6e74 6572 3a20 536b 7943 6f6f 7264 2c20  nter: SkyCoord, 
+000016d0: 706f 7369 7469 6f6e 5f61 6e67 6c65 3a20  position_angle: 
+000016e0: 416e 676c 652c 2077 6373 3a20 5743 530a  Angle, wcs: WCS.
+000016f0: 2920 2d3e 2052 6563 7461 6e67 6c65 416e  ) -> RectangleAn
+00001700: 6e6f 7461 7469 6f6e 3a0a 2020 2020 2222  notation:.    ""
+00001710: 2252 6574 7572 6e20 616e 2061 6e6e 6f74  "Return an annot
+00001720: 6174 696f 6e20 7368 6f77 696e 6720 7468  ation showing th
+00001730: 6520 736c 6f74 2e0a 0a20 2020 2050 6172  e slot...    Par
+00001740: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00001750: 2d2d 2d2d 2d2d 0a20 2020 2063 656e 7465  ------.    cente
+00001760: 723a 2060 7e61 7374 726f 7079 2e63 6f6f  r: `~astropy.coo
+00001770: 7264 696e 6174 6573 2e53 6b79 436f 6f72  rdinates.SkyCoor
+00001780: 6460 0a20 2020 2020 2020 2054 6865 2063  d`.        The c
+00001790: 656e 7465 7220 6f66 2074 6865 2073 6c6f  enter of the slo
+000017a0: 7420 6f6e 2074 6865 2073 6b79 2c20 696e  t on the sky, in
+000017b0: 2072 6967 6874 2061 7363 656e 7369 6f6e   right ascension
+000017c0: 2061 6e64 2064 6563 6c69 6e61 7469 6f6e   and declination
+000017d0: 2e0a 2020 2020 706f 7369 7469 6f6e 5f61  ..    position_a
+000017e0: 6e67 6c65 3a20 607e 6173 7472 6f70 792e  ngle: `~astropy.
+000017f0: 636f 6f72 6469 6e61 7465 732e 416e 676c  coordinates.Angl
+00001800: 6560 0a20 2020 2020 2020 2054 6865 2070  e`.        The p
+00001810: 6f73 6974 696f 6e20 616e 676c 6520 6173  osition angle as
+00001820: 2061 6e20 616e 676c 6520 6f6e 2074 6865   an angle on the
+00001830: 2073 6b79 2c20 6d65 6173 7572 6564 2066   sky, measured f
+00001840: 726f 6d20 6e6f 7274 6820 746f 2065 6173  rom north to eas
+00001850: 742e 0a20 2020 2077 6373 3a20 607e 6173  t..    wcs: `~as
+00001860: 7472 6f70 792e 7763 732e 5743 5360 0a20  tropy.wcs.WCS`. 
+00001870: 2020 2020 2020 2057 4353 206f 626a 6563         WCS objec
+00001880: 742e 0a0a 2020 2020 5265 7475 726e 730a  t...    Returns.
+00001890: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000018a0: 607e 696d 6570 6875 2e61 6e6e 6f74 6174  `~imephu.annotat
+000018b0: 696f 6e2e 6765 6e65 7261 6c2e 5265 6374  ion.general.Rect
+000018c0: 616e 676c 6541 6e6e 6f74 6174 696f 6e60  angleAnnotation`
+000018d0: 0a20 2020 2020 2020 2054 6865 2073 6c6f  .        The slo
+000018e0: 7420 616e 6e6f 7461 7469 6f6e 2e0a 2020  t annotation..  
+000018f0: 2020 2222 220a 2020 2020 7265 7475 726e    """.    return
+00001900: 2052 6563 7461 6e67 6c65 416e 6e6f 7461   RectangleAnnota
+00001910: 7469 6f6e 280a 2020 2020 2020 2020 6365  tion(.        ce
+00001920: 6e74 6572 3d63 656e 7465 722c 0a20 2020  nter=center,.   
+00001930: 2020 2020 2077 6964 7468 3d31 202a 2075       width=1 * u
+00001940: 2e61 7263 6d69 6e20 2f20 332c 0a20 2020  .arcmin / 3,.   
+00001950: 2020 2020 2068 6569 6768 743d 3130 202a       height=10 *
+00001960: 2075 2e61 7263 6d69 6e2c 0a20 2020 2020   u.arcmin,.     
+00001970: 2020 2077 6373 3d77 6373 2c0a 2020 2020     wcs=wcs,.    
+00001980: 2020 2020 6564 6765 636f 6c6f 723d 2272      edgecolor="r
+00001990: 6564 222c 0a20 2020 2020 2020 2061 6c70  ed",.        alp
+000019a0: 6861 3d30 2e35 2c0a 2020 2020 2020 2020  ha=0.5,.        
+000019b0: 6c69 6e65 7769 6474 683d 322c 0a20 2020  linewidth=2,.   
+000019c0: 2029 2e72 6f74 6174 6528 6365 6e74 6572   ).rotate(center
+000019d0: 2c20 706f 7369 7469 6f6e 5f61 6e67 6c65  , position_angle
+000019e0: 202b 2039 3020 2a20 752e 6465 6729 0a0a   + 90 * u.deg)..
+000019f0: 0a64 6566 2062 6173 655f 616e 6e6f 7461  .def base_annota
+00001a00: 7469 6f6e 7328 0a20 2020 2074 6172 6765  tions(.    targe
+00001a10: 743a 2073 7472 2c0a 2020 2020 7072 6f70  t: str,.    prop
+00001a20: 6f73 616c 5f63 6f64 653a 2073 7472 2c0a  osal_code: str,.
+00001a30: 2020 2020 7069 5f66 616d 696c 795f 6e61      pi_family_na
+00001a40: 6d65 3a20 7374 722c 0a20 2020 2070 6f73  me: str,.    pos
+00001a50: 6974 696f 6e5f 616e 676c 653a 2041 6e67  ition_angle: Ang
+00001a60: 6c65 2c0a 2020 2020 6175 746f 6d61 7465  le,.    automate
+00001a70: 645f 706f 7369 7469 6f6e 5f61 6e67 6c65  d_position_angle
+00001a80: 3a20 626f 6f6c 2c0a 2020 2020 7375 7276  : bool,.    surv
+00001a90: 6579 3a20 4f70 7469 6f6e 616c 5b73 7472  ey: Optional[str
+00001aa0: 5d2c 0a20 2020 2066 6974 735f 6365 6e74  ],.    fits_cent
+00001ab0: 6572 3a20 536b 7943 6f6f 7264 2c0a 2020  er: SkyCoord,.  
+00001ac0: 2020 7763 733a 2057 4353 2c0a 2920 2d3e    wcs: WCS,.) ->
+00001ad0: 2047 726f 7570 416e 6e6f 7461 7469 6f6e   GroupAnnotation
+00001ae0: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+00001af0: 6120 6772 6f75 7020 636f 6e74 6169 6e69  a group containi
+00001b00: 6e67 2061 6c6c 2074 6865 2062 6173 6520  ng all the base 
+00001b10: 616e 6e6f 7461 7469 6f6e 7320 666f 7220  annotations for 
+00001b20: 5341 4c54 2066 696e 6465 7220 6368 6172  SALT finder char
+00001b30: 7473 2e0a 0a20 2020 2054 6865 2062 6173  ts...    The bas
+00001b40: 6520 616e 6e6f 7461 7469 6f6e 7320 696e  e annotations in
+00001b50: 636c 7564 6520 7468 6520 7469 746c 652c  clude the title,
+00001b60: 2064 6972 6563 7469 6f6e 732c 2070 6f73   directions, pos
+00001b70: 6974 696f 6e20 616e 676c 652c 2073 7572  ition angle, sur
+00001b80: 7665 7920 6e61 6d65 2061 6e64 0a20 2020  vey name and.   
+00001b90: 2074 6865 2052 5353 2061 6e64 2053 616c   the RSS and Sal
+00001ba0: 7469 6361 6d20 6669 656c 6473 206f 6620  ticam fields of 
+00001bb0: 7669 6577 2e0a 0a20 2020 2050 6172 616d  view...    Param
+00001bc0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00001bd0: 2d2d 2d2d 0a20 2020 2074 6172 6765 743a  ----.    target:
+00001be0: 2073 7472 0a20 2020 2020 2020 2054 6865   str.        The
+00001bf0: 206e 616d 6520 6f66 2074 6865 2074 6172   name of the tar
+00001c00: 6765 7420 666f 7220 7768 6963 6820 7468  get for which th
+00001c10: 6520 6669 6e64 6572 2063 6861 7274 2069  e finder chart i
+00001c20: 7320 696e 7465 6e64 6564 2e0a 2020 2020  s intended..    
+00001c30: 7072 6f70 6f73 616c 5f63 6f64 653a 2073  proposal_code: s
+00001c40: 7472 0a20 2020 2020 2020 2054 6865 2070  tr.        The p
+00001c50: 726f 706f 7361 6c20 636f 6465 2066 6f72  roposal code for
+00001c60: 2077 6869 6368 2074 6865 2066 696e 6465   which the finde
+00001c70: 7220 6368 6172 7420 6973 2069 6e74 656e  r chart is inten
+00001c80: 6465 642e 0a20 2020 2070 695f 6661 6d69  ded..    pi_fami
+00001c90: 6c79 5f6e 616d 653a 2073 7472 0a20 2020  ly_name: str.   
+00001ca0: 2020 2020 2054 6865 2066 616d 696c 7920       The family 
+00001cb0: 6e61 6d65 206f 6620 7468 6520 5072 696e  name of the Prin
+00001cc0: 6369 7061 6c20 496e 7665 7374 6967 6174  cipal Investigat
+00001cd0: 6f72 2e0a 2020 2020 706f 7369 7469 6f6e  or..    position
+00001ce0: 5f61 6e67 6c65 3a20 607e 6173 7472 6f70  _angle: `~astrop
+00001cf0: 792e 636f 6f72 6469 6e61 7465 732e 416e  y.coordinates.An
+00001d00: 676c 6560 0a20 2020 2020 2020 2054 6865  gle`.        The
+00001d10: 2070 6f73 6974 696f 6e20 616e 676c 652c   position angle,
+00001d20: 2061 7320 616e 2061 6e67 6c65 206f 6e20   as an angle on 
+00001d30: 7468 6520 736b 7920 6672 6f6d 206e 6f72  the sky from nor
+00001d40: 7468 2074 6f20 6561 7374 2e0a 2020 2020  th to east..    
+00001d50: 6175 746f 6d61 7465 645f 706f 7369 7469  automated_positi
+00001d60: 6f6e 5f61 6e67 6c65 3a20 626f 6f6c 0a20  on_angle: bool. 
+00001d70: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+00001d80: 6865 2070 6f73 6974 696f 6e20 616e 676c  he position angl
+00001d90: 6520 6861 7320 6265 656e 2063 616c 6375  e has been calcu
+00001da0: 6c61 7465 6420 6175 746f 6d61 7469 6361  lated automatica
+00001db0: 6c6c 792e 0a20 2020 2073 7572 7665 793a  lly..    survey:
+00001dc0: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
+00001dd0: 2020 2020 2020 2054 6865 2069 6d61 6765         The image
+00001de0: 2073 7572 7665 7920 6e61 6d65 2e0a 2020   survey name..  
+00001df0: 2020 6669 7473 5f63 656e 7465 723a 2060    fits_center: `
+00001e00: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
+00001e10: 6174 6573 2e53 6b79 436f 6f72 6460 0a20  ates.SkyCoord`. 
+00001e20: 2020 2020 2020 2054 6865 2063 656e 7472         The centr
+00001e30: 616c 2070 6f73 6974 696f 6e20 6f66 2074  al position of t
+00001e40: 6865 2066 696e 6465 7220 6368 6172 742c  he finder chart,
+00001e50: 2069 6e20 7269 6768 7420 6173 6365 6e73   in right ascens
+00001e60: 696f 6e20 616e 6420 6465 636c 696e 6174  ion and declinat
+00001e70: 696f 6e0a 2020 2020 7763 733a 2060 7e61  ion.    wcs: `~a
+00001e80: 7374 726f 7079 2e77 6373 2e57 4353 600a  stropy.wcs.WCS`.
+00001e90: 2020 2020 2020 2020 5743 5320 6f62 6a65          WCS obje
+00001ea0: 6374 2e0a 0a20 2020 2052 6574 7572 6e73  ct...    Returns
+00001eb0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00001ec0: 2060 7e69 6d65 7068 752e 616e 6e6f 7461   `~imephu.annota
+00001ed0: 7469 6f6e 2e67 656e 6572 616c 2e47 726f  tion.general.Gro
+00001ee0: 7570 416e 6e6f 7461 7469 6f6e 600a 2020  upAnnotation`.  
+00001ef0: 2020 2020 2020 416e 2061 6e6e 6f74 6174        An annotat
+00001f00: 696f 6e20 7769 7468 2061 6c6c 2074 6865  ion with all the
+00001f10: 2053 414c 5420 6261 7365 2061 6e6e 6f74   SALT base annot
+00001f20: 6174 696f 6e73 2e0a 2020 2020 2222 220a  ations..    """.
+00001f30: 2020 2020 7265 7475 726e 2047 726f 7570      return Group
+00001f40: 416e 6e6f 7461 7469 6f6e 280a 2020 2020  Annotation(.    
+00001f50: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00001f60: 2020 7469 746c 655f 616e 6e6f 7461 7469    title_annotati
+00001f70: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00001f80: 2020 2020 7461 7267 6574 3d74 6172 6765      target=targe
+00001f90: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00001fa0: 2020 2070 726f 706f 7361 6c5f 636f 6465     proposal_code
+00001fb0: 3d70 726f 706f 7361 6c5f 636f 6465 2c0a  =proposal_code,.
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fd0: 7069 5f66 616d 696c 795f 6e61 6d65 3d70  pi_family_name=p
+00001fe0: 695f 6661 6d69 6c79 5f6e 616d 652c 0a20  i_family_name,. 
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00002000: 6373 3d77 6373 2c0a 2020 2020 2020 2020  cs=wcs,.        
+00002010: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00002020: 2020 2073 7572 7665 795f 616e 6e6f 7461     survey_annota
+00002030: 7469 6f6e 2873 7572 7665 793d 7375 7276  tion(survey=surv
+00002040: 6579 2c20 7763 733d 7763 7329 2069 6620  ey, wcs=wcs) if 
+00002050: 7375 7276 6579 2065 6c73 6520 456d 7074  survey else Empt
+00002060: 7941 6e6e 6f74 6174 696f 6e28 292c 0a20  yAnnotation(),. 
+00002070: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
+00002080: 696f 6e5f 616e 676c 655f 616e 6e6f 7461  ion_angle_annota
+00002090: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+000020a0: 2020 2020 2020 706f 7369 7469 6f6e 5f61        position_a
+000020b0: 6e67 6c65 3d70 6f73 6974 696f 6e5f 616e  ngle=position_an
+000020c0: 676c 652c 0a20 2020 2020 2020 2020 2020  gle,.           
+000020d0: 2020 2020 2061 7574 6f6d 6174 6564 5f70       automated_p
+000020e0: 6f73 6974 696f 6e5f 616e 676c 653d 6175  osition_angle=au
+000020f0: 746f 6d61 7465 645f 706f 7369 7469 6f6e  tomated_position
+00002100: 5f61 6e67 6c65 2c0a 2020 2020 2020 2020  _angle,.        
+00002110: 2020 2020 2020 2020 7763 733d 7763 732c          wcs=wcs,
+00002120: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00002130: 2020 2020 2020 2020 2020 2020 6469 7265              dire
+00002140: 6374 696f 6e73 5f61 6e6e 6f74 6174 696f  ctions_annotatio
+00002150: 6e28 6669 7473 5f63 656e 7465 723d 6669  n(fits_center=fi
+00002160: 7473 5f63 656e 7465 722c 2077 6373 3d77  ts_center, wcs=w
+00002170: 6373 292c 0a20 2020 2020 2020 2020 2020  cs),.           
+00002180: 205f 6372 6f73 7368 6169 7273 5f61 6e6e   _crosshairs_ann
+00002190: 6f74 6174 696f 6e28 6669 7473 5f63 656e  otation(fits_cen
+000021a0: 7465 723d 6669 7473 5f63 656e 7465 722c  ter=fits_center,
+000021b0: 2077 6373 3d77 6373 292c 0a20 2020 2020   wcs=wcs),.     
+000021c0: 2020 2020 2020 2073 616c 7469 6361 6d2e         salticam.
+000021d0: 6669 656c 645f 6f66 5f76 6965 775f 616e  field_of_view_an
+000021e0: 6e6f 7461 7469 6f6e 2866 6974 735f 6365  notation(fits_ce
+000021f0: 6e74 6572 3d66 6974 735f 6365 6e74 6572  nter=fits_center
+00002200: 2c20 7763 733d 7763 7329 2c0a 2020 2020  , wcs=wcs),.    
+00002210: 2020 2020 2020 2020 7273 732e 6669 656c          rss.fiel
+00002220: 645f 6f66 5f76 6965 775f 616e 6e6f 7461  d_of_view_annota
+00002230: 7469 6f6e 2866 6974 735f 6365 6e74 6572  tion(fits_center
+00002240: 3d66 6974 735f 6365 6e74 6572 2c20 7763  =fits_center, wc
+00002250: 733d 7763 7329 2c0a 2020 2020 2020 2020  s=wcs),.        
+00002260: 5d0a 2020 2020 290a 0a0a 6465 6620 5f63  ].    )...def _c
+00002270: 726f 7373 6861 6972 735f 616e 6e6f 7461  rosshairs_annota
+00002280: 7469 6f6e 2866 6974 735f 6365 6e74 6572  tion(fits_center
+00002290: 3a20 536b 7943 6f6f 7264 2c20 7763 733a  : SkyCoord, wcs:
+000022a0: 2057 4353 2920 2d3e 2043 726f 7373 6861   WCS) -> Crossha
+000022b0: 6972 7341 6e6e 6f74 6174 696f 6e3a 0a20  irsAnnotation:. 
+000022c0: 2020 2072 6574 7572 6e20 4372 6f73 7368     return Crossh
+000022d0: 6169 7273 416e 6e6f 7461 7469 6f6e 280a  airsAnnotation(.
+000022e0: 2020 2020 2020 2020 6365 6e74 6572 3d66          center=f
+000022f0: 6974 735f 6365 6e74 6572 2c20 7369 7a65  its_center, size
+00002300: 3d38 202a 2075 2e61 7263 6d69 6e2c 2077  =8 * u.arcmin, w
+00002310: 6373 3d77 6373 2c20 636f 6c6f 723d 2267  cs=wcs, color="g
+00002320: 7265 656e 220a 2020 2020 290a            reen".    ).
```

### Comparing `imephu-0.2.0/src/imephu/salt/__pycache__/rss.cpython-310.pyc` & `imephu-0.2.1/src/imephu/salt/annotation/salticam.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,75 @@
-00000000: 6f0d 0d0a 0000 0000 0ca1 f161 9d04 0000  o..........a....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000c 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6404 6502 6405 6501 6406  m.Z...d.e.d.e.d.
-00000060: 6501 6407 6501 6408 6504 6409 6506 660c  e.d.e.d.e.d.e.f.
-00000070: 640a 640b 8404 5a07 640c 5300 290d e900  d.d...Z.d.S.)...
-00000080: 0000 0029 02da 0541 6e67 6c65 da08 536b  ...)...Angle..Sk
-00000090: 7943 6f6f 7264 2901 da03 5743 5329 01da  yCoord)...WCS)..
-000000a0: 1352 6563 7461 6e67 6c65 416e 6e6f 7461  .RectangleAnnota
-000000b0: 7469 6f6e da0b 6669 7473 5f63 656e 7465  tion..fits_cente
-000000c0: 72da 0a73 6c69 745f 7769 6474 68da 0b73  r..slit_width..s
-000000d0: 6c69 745f 6865 6967 6874 da0e 706f 7369  lit_height..posi
-000000e0: 7469 6f6e 5f61 6e67 6c65 da03 7763 73da  tion_angle..wcs.
-000000f0: 0672 6574 7572 6e63 0500 0000 0000 0000  .returnc........
-00000100: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
-00000110: 731c 0000 0074 007c 007c 017c 027c 0464  s....t.|.|.|.|.d
-00000120: 0164 0264 038d 06a0 017c 007c 03a1 0253  .d.d.....|.|...S
-00000130: 0029 0561 c702 0000 5265 7475 726e 2061  .).a....Return a
-00000140: 6e20 616e 6e6f 7461 7469 6f6e 2073 686f  n annotation sho
-00000150: 7769 6e67 2061 206c 6f6e 6773 6c69 742e  wing a longslit.
-00000160: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000170: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00000180: 2020 2020 6669 7473 5f63 656e 7465 723a      fits_center:
-00000190: 2060 7e61 7374 726f 7079 2e63 6f6f 7264   `~astropy.coord
-000001a0: 696e 6174 6573 2e53 6b79 436f 6f72 6460  inates.SkyCoord`
-000001b0: 0a20 2020 2020 2020 2054 6865 2063 656e  .        The cen
-000001c0: 7472 616c 2070 6f73 6974 696f 6e20 6f66  tral position of
-000001d0: 2074 6865 2066 696e 6465 7220 6368 6172   the finder char
-000001e0: 742c 2069 6e20 7269 6768 7420 6173 6365  t, in right asce
-000001f0: 6e73 696f 6e20 616e 6420 6465 636c 696e  nsion and declin
-00000200: 6174 696f 6e0a 2020 2020 736c 6974 5f77  ation.    slit_w
-00000210: 6964 7468 3a20 607e 6173 7472 6f70 792e  idth: `~astropy.
-00000220: 636f 6f72 6469 6e61 7465 732e 416e 676c  coordinates.Angl
-00000230: 6560 0a20 2020 2020 2020 2054 6865 2077  e`.        The w
-00000240: 6964 7468 206f 6620 7468 6520 736c 6974  idth of the slit
-00000250: 2c20 6173 2061 6e20 616e 676c 6520 6f6e  , as an angle on
-00000260: 2074 6865 2073 6b79 2e0a 2020 2020 736c   the sky..    sl
-00000270: 6974 5f68 6569 6768 743a 2060 7e61 7374  it_height: `~ast
-00000280: 726f 7079 2e63 6f6f 7264 696e 6174 6573  ropy.coordinates
-00000290: 2e41 6e67 6c65 600a 2020 2020 2020 2020  .Angle`.        
-000002a0: 5468 6520 6865 6967 6874 206f 6620 7468  The height of th
-000002b0: 6520 736c 6974 2c20 6173 2061 6e20 616e  e slit, as an an
-000002c0: 676c 6520 6f6e 2074 6865 2073 6b79 2e0a  gle on the sky..
-000002d0: 2020 2020 706f 7369 7469 6f6e 5f61 6e67      position_ang
-000002e0: 6c65 3a20 607e 6173 7472 6f70 792e 636f  le: `~astropy.co
-000002f0: 6f72 6469 6e61 7465 732e 416e 676c 6560  ordinates.Angle`
-00000300: 0a20 2020 2020 2020 2054 6865 2070 6f73  .        The pos
-00000310: 6974 696f 6e20 616e 676c 652c 2061 7320  ition angle, as 
-00000320: 616e 2061 6e67 6c65 206f 6e20 7468 6520  an angle on the 
-00000330: 736b 7920 6d65 6173 7572 6564 2066 726f  sky measured fro
-00000340: 6d20 6e6f 7274 6820 746f 2065 6173 742e  m north to east.
-00000350: 0a20 2020 2077 6373 3a20 607e 6173 7472  .    wcs: `~astr
-00000360: 6f70 792e 7763 732e 5743 5360 0a20 2020  opy.wcs.WCS`.   
-00000370: 2020 2020 2057 4353 206f 626a 6563 742e       WCS object.
-00000380: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00000390: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 6069    -------.    `i
-000003a0: 6d65 7068 752e 616e 6e6f 7461 7469 6f6e  mephu.annotation
-000003b0: 2e67 656e 6572 616c 2e52 6563 7461 6e67  .general.Rectang
-000003c0: 6c65 416e 6e6f 7461 7469 6f6e 600a 2020  leAnnotation`.  
-000003d0: 2020 2020 2020 5468 6520 616e 6e6f 7461        The annota
-000003e0: 7469 6f6e 2073 686f 7769 6e67 2074 6865  tion showing the
-000003f0: 206c 6f6e 6773 6c69 742e 0a20 2020 20da   longslit..    .
-00000400: 0372 6564 6700 0000 0000 00e0 3f29 0372  .redg.......?).r
-00000410: 0a00 0000 da09 6564 6765 636f 6c6f 72da  ......edgecolor.
-00000420: 0561 6c70 6861 4e29 0272 0500 0000 da06  .alphaN).r......
-00000430: 726f 7461 7465 2905 7206 0000 0072 0700  rotate).r....r..
-00000440: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000450: 00a9 0072 1000 0000 fa46 2f55 7365 7273  ...r.....F/Users
-00000460: 2f63 6872 6973 7469 616e 2f49 6465 6150  /christian/IdeaP
-00000470: 726f 6a65 6374 732f 696d 6570 6875 2f73  rojects/imephu/s
-00000480: 7263 2f69 6d65 7068 752f 616e 6e6f 7461  rc/imephu/annota
-00000490: 7469 6f6e 2f73 616c 742f 7273 732e 7079  tion/salt/rss.py
-000004a0: da13 6c6f 6e67 736c 6974 5f61 6e6e 6f74  ..longslit_annot
-000004b0: 6174 696f 6e07 0000 0073 0a00 0000 021b  ation....s......
-000004c0: 0c01 04ff 0802 02fe 7212 0000 004e 2908  ........r....N).
-000004d0: da13 6173 7472 6f70 792e 636f 6f72 6469  ..astropy.coordi
-000004e0: 6e61 7465 7372 0200 0000 7203 0000 00da  natesr....r.....
-000004f0: 0b61 7374 726f 7079 2e77 6373 7204 0000  .astropy.wcsr...
-00000500: 00da 1969 6d65 7068 752e 616e 6e6f 7461  ...imephu.annota
-00000510: 7469 6f6e 2e67 656e 6572 616c 7205 0000  tion.generalr...
-00000520: 0072 1200 0000 7210 0000 0072 1000 0000  .r....r....r....
-00000530: 7210 0000 0072 1100 0000 da08 3c6d 6f64  r....r......<mod
-00000540: 756c 653e 0100 0000 7320 0000 0010 000c  ule>....s ......
-00000550: 010c 0202 0302 0102 ff02 0202 fe02 0302  ................
-00000560: fd02 0402 fc02 0502 fb02 060e fa         .............
+00000000: 6672 6f6d 2061 7374 726f 7079 2069 6d70  from astropy imp
+00000010: 6f72 7420 756e 6974 7320 6173 2075 0a66  ort units as u.f
+00000020: 726f 6d20 6173 7472 6f70 792e 636f 6f72  rom astropy.coor
+00000030: 6469 6e61 7465 7320 696d 706f 7274 2053  dinates import S
+00000040: 6b79 436f 6f72 640a 6672 6f6d 2061 7374  kyCoord.from ast
+00000050: 726f 7079 2e77 6373 2069 6d70 6f72 7420  ropy.wcs import 
+00000060: 5743 530a 6672 6f6d 2069 6d65 7068 752e  WCS.from imephu.
+00000070: 616e 6e6f 7461 7469 6f6e 2e67 656e 6572  annotation.gener
+00000080: 616c 2069 6d70 6f72 7420 4369 7263 6c65  al import Circle
+00000090: 416e 6e6f 7461 7469 6f6e 2c20 4772 6f75  Annotation, Grou
+000000a0: 7041 6e6e 6f74 6174 696f 6e2c 2054 6578  pAnnotation, Tex
+000000b0: 7441 6e6e 6f74 6174 696f 6e0a 6672 6f6d  tAnnotation.from
+000000c0: 2069 6d65 7068 752e 6765 6f6d 6574 7279   imephu.geometry
+000000d0: 2069 6d70 6f72 7420 7472 616e 736c 6174   import translat
+000000e0: 650a 0a0a 6465 6620 6669 656c 645f 6f66  e...def field_of
+000000f0: 5f76 6965 775f 616e 6e6f 7461 7469 6f6e  _view_annotation
+00000100: 2866 6974 735f 6365 6e74 6572 3a20 536b  (fits_center: Sk
+00000110: 7943 6f6f 7264 2c20 7763 733a 2057 4353  yCoord, wcs: WCS
+00000120: 2920 2d3e 2047 726f 7570 416e 6e6f 7461  ) -> GroupAnnota
+00000130: 7469 6f6e 3a0a 2020 2020 2222 220a 2020  tion:.    """.  
+00000140: 2020 5265 7475 726e 2061 6e20 616e 6e6f    Return an anno
+00000150: 7461 7469 6f6e 2077 6974 6820 7468 6520  tation with the 
+00000160: 5361 6c74 6963 616d 2066 6965 6c64 206f  Salticam field o
+00000170: 6620 7669 6577 2e0a 0a20 2020 2050 6172  f view...    Par
+00000180: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00000190: 2d2d 2d2d 2d2d 0a20 2020 2066 6974 735f  ------.    fits_
+000001a0: 6365 6e74 6572 3a20 607e 6173 7472 6f70  center: `~astrop
+000001b0: 792e 636f 6f72 6469 6e61 7465 732e 536b  y.coordinates.Sk
+000001c0: 7943 6f6f 7264 600a 2020 2020 2020 2020  yCoord`.        
+000001d0: 5468 6520 6365 6e74 7261 6c20 706f 7369  The central posi
+000001e0: 7469 6f6e 206f 6620 7468 6520 6669 6e64  tion of the find
+000001f0: 6572 2063 6861 7274 2c20 696e 2072 6967  er chart, in rig
+00000200: 6874 2061 7363 656e 7369 6f6e 2061 6e64  ht ascension and
+00000210: 2064 6563 6c69 6e61 7469 6f6e 2e0a 2020   declination..  
+00000220: 2020 7763 733a 2060 7e61 7374 726f 7079    wcs: `~astropy
+00000230: 2e77 6373 2e57 4353 600a 2020 2020 2020  .wcs.WCS`.      
+00000240: 2020 5743 5320 6f62 6a65 6374 2e0a 0a20    WCS object... 
+00000250: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00000260: 2d2d 2d2d 2d2d 0a20 2020 2060 7e69 6d65  ------.    `~ime
+00000270: 7068 752e 616e 6e6f 7461 7469 6f6e 2e67  phu.annotation.g
+00000280: 656e 6572 616c 2e47 726f 7570 416e 6e6f  eneral.GroupAnno
+00000290: 7461 7469 6f6e 600a 2020 2020 2020 2020  tation`.        
+000002a0: 416e 2061 6e6e 6f74 6174 696f 6e20 7769  An annotation wi
+000002b0: 7468 2074 6865 2053 616c 7469 6361 6d20  th the Salticam 
+000002c0: 6669 656c 6420 6f66 2076 6965 772e 0a20  field of view.. 
+000002d0: 2020 2022 2222 0a20 2020 2066 6f76 5f61     """.    fov_a
+000002e0: 6e6e 6f74 6174 696f 6e20 3d20 4369 7263  nnotation = Circ
+000002f0: 6c65 416e 6e6f 7461 7469 6f6e 280a 2020  leAnnotation(.  
+00000300: 2020 2020 2020 6669 7473 5f63 656e 7465        fits_cente
+00000310: 722c 2035 202a 2075 2e61 7263 6d69 6e2c  r, 5 * u.arcmin,
+00000320: 2077 6373 3d77 6373 2c20 6564 6765 636f   wcs=wcs, edgeco
+00000330: 6c6f 723d 2267 7265 656e 220a 2020 2020  lor="green".    
+00000340: 290a 2020 2020 6c61 6265 6c5f 706f 7369  ).    label_posi
+00000350: 7469 6f6e 203d 2074 7261 6e73 6c61 7465  tion = translate
+00000360: 2866 6974 735f 6365 6e74 6572 2c20 282d  (fits_center, (-
+00000370: 332e 362c 2033 2e36 2920 2a20 752e 6172  3.6, 3.6) * u.ar
+00000380: 636d 696e 290a 2020 2020 6e61 6d65 5f61  cmin).    name_a
+00000390: 6e6e 6f74 6174 696f 6e20 3d20 5465 7874  nnotation = Text
+000003a0: 416e 6e6f 7461 7469 6f6e 280a 2020 2020  Annotation(.    
+000003b0: 2020 2020 6c61 6265 6c5f 706f 7369 7469      label_positi
+000003c0: 6f6e 2c0a 2020 2020 2020 2020 2253 4341  on,.        "SCA
+000003d0: 4d22 2c0a 2020 2020 2020 2020 7763 733d  M",.        wcs=
+000003e0: 7763 732c 0a20 2020 2020 2020 2073 7479  wcs,.        sty
+000003f0: 6c65 3d22 6974 616c 6963 222c 0a20 2020  le="italic",.   
+00000400: 2020 2020 2077 6569 6768 743d 2262 6f6c       weight="bol
+00000410: 6422 2c0a 2020 2020 2020 2020 7369 7a65  d",.        size
+00000420: 3d22 6c61 7267 6522 2c0a 2020 2020 2020  ="large",.      
+00000430: 2020 686f 7269 7a6f 6e74 616c 616c 6967    horizontalalig
+00000440: 6e6d 656e 743d 226c 6566 7422 2c0a 2020  nment="left",.  
+00000450: 2020 2020 2020 636f 6c6f 723d 2830 2c20        color=(0, 
+00000460: 302c 2031 292c 0a20 2020 2029 0a20 2020  0, 1),.    ).   
+00000470: 2072 6574 7572 6e20 4772 6f75 7041 6e6e   return GroupAnn
+00000480: 6f74 6174 696f 6e28 5b66 6f76 5f61 6e6e  otation([fov_ann
+00000490: 6f74 6174 696f 6e2c 206e 616d 655f 616e  otation, name_an
+000004a0: 6e6f 7461 7469 6f6e 5d29 0a              notation]).
```

### Comparing `imephu-0.2.0/src/imephu/salt/__pycache__/utils.cpython-310.pyc` & `imephu-0.2.1/src/imephu/salt/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,303 +1,304 @@
-00000000: 6f0d 0d0a 0000 0000 1cac 5262 fb12 0000  o.........Rb....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 6d0c 5a0c 0100 6400 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 0100 6502 8300 4700 6408 6409 8400 6409  ..e...G.d.d...d.
-00000090: 8302 8301 5a0f 4700 640a 640b 8400 640b  ....Z.G.d.d...d.
-000000a0: 8302 5a10 6401 5300 290c e900 0000 004e  ..Z.d.S.)......N
-000000b0: 2901 da09 6461 7461 636c 6173 7329 01da  )...dataclass)..
-000000c0: 0450 6174 6829 01da 044c 6973 7429 01da  .Path)...List)..
-000000d0: 0575 6e69 7473 2902 da05 416e 676c 65da  .units)...Angle.
-000000e0: 0853 6b79 436f 6f72 6429 01da 0b70 6172  .SkyCoord)...par
-000000f0: 7365 5374 7269 6e67 6300 0000 0000 0000  seStringc.......
-00000100: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000110: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
-00000120: 6401 5a03 6504 6505 6402 3c00 6506 6505  d.Z.e.e.d.<.e.e.
-00000130: 6403 3c00 6506 6505 6404 3c00 6506 6505  d.<.e.e.d.<.e.e.
-00000140: 6405 3c00 6406 5300 2907 da0b 4d6f 734d  d.<.d.S.)...MosM
-00000150: 6173 6b53 6c69 7461 be02 0000 4120 736c  askSlita....A sl
-00000160: 6974 2069 6e20 6120 4d4f 5320 6d61 736b  it in a MOS mask
-00000170: 2e0a 0a20 2020 2054 6865 2073 6c69 7420  ...    The slit 
-00000180: 6973 2063 6861 7261 6374 6572 6973 6564  is characterised
-00000190: 2062 7920 6974 7320 6365 6e74 6572 2070   by its center p
-000001a0: 6f73 6974 696f 6e2c 2077 6964 7468 2c20  osition, width, 
-000001b0: 6865 6967 6874 2061 6e64 2074 696c 742e  height and tilt.
-000001c0: 2054 6865 2074 696c 740a 2020 2020 7368   The tilt.    sh
-000001d0: 6f75 6c64 206e 6f74 2062 6520 636f 6e66  ould not be conf
-000001e0: 7573 6564 2077 6974 6820 7468 6520 706f  used with the po
-000001f0: 7369 7469 6f6e 2061 6e67 6c65 206f 6620  sition angle of 
-00000200: 7468 6520 4d4f 5320 6d61 736b 2e20 5468  the MOS mask. Th
-00000210: 6520 736c 6974 2077 696c 6c20 6265 0a20  e slit will be. 
-00000220: 2020 2072 6f74 6174 6564 2062 7920 7468     rotated by th
-00000230: 6520 7375 6d20 6f66 2074 6865 2070 6f73  e sum of the pos
-00000240: 6974 696f 6e20 616e 676c 6520 616e 6420  ition angle and 
-00000250: 6974 7320 7469 6c74 2e0a 0a20 2020 2041  its tilt...    A
-00000260: 7474 7269 6275 7465 730a 2020 2020 2d2d  ttributes.    --
-00000270: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 656e  --------.    cen
-00000280: 7465 723a 2060 7e61 7374 726f 7079 2e63  ter: `~astropy.c
-00000290: 6f6f 7264 696e 6174 6573 2e53 6b79 436f  oordinates.SkyCo
-000002a0: 6f72 6460 0a20 2020 2020 2020 2054 6865  ord`.        The
-000002b0: 2070 6f73 6974 696f 6e20 6f66 2074 6865   position of the
-000002c0: 2073 6c69 7420 6365 6e74 6572 2c20 6173   slit center, as
-000002d0: 2072 6967 6874 2061 7363 656e 7369 6f6e   right ascension
-000002e0: 2061 6e64 2064 6563 6c69 6e61 7469 6f6e   and declination
-000002f0: 2e0a 2020 2020 7769 6474 683a 2060 7e61  ..    width: `~a
-00000300: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
-00000310: 6573 2e41 6e67 6c65 600a 2020 2020 2020  es.Angle`.      
-00000320: 2020 5468 6520 736c 6974 2077 6964 7468    The slit width
-00000330: 2c20 6173 2061 6e20 616e 676c 6520 6f6e  , as an angle on
-00000340: 2074 6865 2073 6b79 2e0a 2020 2020 6865   the sky..    he
-00000350: 6967 6874 3a20 607e 6173 7472 6f70 792e  ight: `~astropy.
-00000360: 636f 6f72 6469 6e61 7465 732e 416e 676c  coordinates.Angl
-00000370: 6560 0a20 2020 2020 2020 2054 6865 2073  e`.        The s
-00000380: 6c69 7420 6865 6967 6874 2c20 6173 2061  lit height, as a
+00000000: 696d 706f 7274 207a 6970 6669 6c65 0a66  import zipfile.f
+00000010: 726f 6d20 6461 7461 636c 6173 7365 7320  rom dataclasses 
+00000020: 696d 706f 7274 2064 6174 6163 6c61 7373  import dataclass
+00000030: 0a66 726f 6d20 7061 7468 6c69 6220 696d  .from pathlib im
+00000040: 706f 7274 2050 6174 680a 6672 6f6d 2074  port Path.from t
+00000050: 7970 696e 6720 696d 706f 7274 204c 6973  yping import Lis
+00000060: 740a 0a66 726f 6d20 6173 7472 6f70 7920  t..from astropy 
+00000070: 696d 706f 7274 2075 6e69 7473 2061 7320  import units as 
+00000080: 750a 6672 6f6d 2061 7374 726f 7079 2e63  u.from astropy.c
+00000090: 6f6f 7264 696e 6174 6573 2069 6d70 6f72  oordinates impor
+000000a0: 7420 416e 676c 652c 2053 6b79 436f 6f72  t Angle, SkyCoor
+000000b0: 640a 6672 6f6d 2064 6566 7573 6564 786d  d.from defusedxm
+000000c0: 6c2e 6d69 6e69 646f 6d20 696d 706f 7274  l.minidom import
+000000d0: 2070 6172 7365 5374 7269 6e67 0a0a 0a40   parseString...@
+000000e0: 6461 7461 636c 6173 7328 290a 636c 6173  dataclass().clas
+000000f0: 7320 4d6f 734d 6173 6b53 6c69 743a 0a20  s MosMaskSlit:. 
+00000100: 2020 2022 2222 4120 736c 6974 2069 6e20     """A slit in 
+00000110: 6120 4d4f 5320 6d61 736b 2e0a 0a20 2020  a MOS mask...   
+00000120: 2054 6865 2073 6c69 7420 6973 2063 6861   The slit is cha
+00000130: 7261 6374 6572 6973 6564 2062 7920 6974  racterised by it
+00000140: 7320 6365 6e74 6572 2070 6f73 6974 696f  s center positio
+00000150: 6e2c 2077 6964 7468 2c20 6865 6967 6874  n, width, height
+00000160: 2061 6e64 2074 696c 742e 2054 6865 2074   and tilt. The t
+00000170: 696c 740a 2020 2020 7368 6f75 6c64 206e  ilt.    should n
+00000180: 6f74 2062 6520 636f 6e66 7573 6564 2077  ot be confused w
+00000190: 6974 6820 7468 6520 706f 7369 7469 6f6e  ith the position
+000001a0: 2061 6e67 6c65 206f 6620 7468 6520 4d4f   angle of the MO
+000001b0: 5320 6d61 736b 2e20 5468 6520 736c 6974  S mask. The slit
+000001c0: 2077 696c 6c20 6265 0a20 2020 2072 6f74   will be.    rot
+000001d0: 6174 6564 2062 7920 7468 6520 7375 6d20  ated by the sum 
+000001e0: 6f66 2074 6865 2070 6f73 6974 696f 6e20  of the position 
+000001f0: 616e 676c 6520 616e 6420 6974 7320 7469  angle and its ti
+00000200: 6c74 2e0a 0a20 2020 2041 7474 7269 6275  lt...    Attribu
+00000210: 7465 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  tes.    --------
+00000220: 2d2d 0a20 2020 2063 656e 7465 723a 2060  --.    center: `
+00000230: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
+00000240: 6174 6573 2e53 6b79 436f 6f72 6460 0a20  ates.SkyCoord`. 
+00000250: 2020 2020 2020 2054 6865 2070 6f73 6974         The posit
+00000260: 696f 6e20 6f66 2074 6865 2073 6c69 7420  ion of the slit 
+00000270: 6365 6e74 6572 2c20 6173 2072 6967 6874  center, as right
+00000280: 2061 7363 656e 7369 6f6e 2061 6e64 2064   ascension and d
+00000290: 6563 6c69 6e61 7469 6f6e 2e0a 2020 2020  eclination..    
+000002a0: 7769 6474 683a 2060 7e61 7374 726f 7079  width: `~astropy
+000002b0: 2e63 6f6f 7264 696e 6174 6573 2e41 6e67  .coordinates.Ang
+000002c0: 6c65 600a 2020 2020 2020 2020 5468 6520  le`.        The 
+000002d0: 736c 6974 2077 6964 7468 2c20 6173 2061  slit width, as a
+000002e0: 6e20 616e 676c 6520 6f6e 2074 6865 2073  n angle on the s
+000002f0: 6b79 2e0a 2020 2020 6865 6967 6874 3a20  ky..    height: 
+00000300: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
+00000310: 6e61 7465 732e 416e 676c 6560 0a20 2020  nates.Angle`.   
+00000320: 2020 2020 2054 6865 2073 6c69 7420 6865       The slit he
+00000330: 6967 6874 2c20 6173 2061 6e20 616e 676c  ight, as an angl
+00000340: 6520 6f6e 2074 6865 2073 6b79 2e0a 2020  e on the sky..  
+00000350: 2020 7469 6c74 3a20 607e 6173 7472 6f70    tilt: `~astrop
+00000360: 792e 636f 6f72 6469 6e61 7465 732e 416e  y.coordinates.An
+00000370: 676c 6560 0a20 2020 2020 2020 2054 6865  gle`.        The
+00000380: 2073 6c69 7420 7469 6c74 2c20 6173 2061   slit tilt, as a
 00000390: 6e20 616e 676c 6520 6f6e 2074 6865 2073  n angle on the s
-000003a0: 6b79 2e0a 2020 2020 7469 6c74 3a20 607e  ky..    tilt: `~
-000003b0: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
-000003c0: 7465 732e 416e 676c 6560 0a20 2020 2020  tes.Angle`.     
-000003d0: 2020 2054 6865 2073 6c69 7420 7469 6c74     The slit tilt
-000003e0: 2c20 6173 2061 6e20 616e 676c 6520 6f6e  , as an angle on
-000003f0: 2074 6865 2073 6b79 206d 6561 7375 7265   the sky measure
-00000400: 6420 6672 6f6d 206e 6f72 7468 2074 6f20  d from north to 
-00000410: 6561 7374 2e0a 2020 2020 da06 6365 6e74  east..    ..cent
-00000420: 6572 da05 7769 6474 68da 0668 6569 6768  er..width..heigh
-00000430: 74da 0474 696c 744e 2907 da08 5f5f 6e61  t..tiltN)...__na
-00000440: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000450: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000460: 5f5f 646f 635f 5f72 0700 0000 da0f 5f5f  __doc__r......__
-00000470: 616e 6e6f 7461 7469 6f6e 735f 5f72 0600  annotations__r..
-00000480: 0000 a900 7213 0000 0072 1300 0000 fa3d  ....r....r.....=
-00000490: 2f55 7365 7273 2f63 6872 6973 7469 616e  /Users/christian
-000004a0: 2f49 6465 6150 726f 6a65 6374 732f 696d  /IdeaProjects/im
-000004b0: 6570 6875 2f73 7263 2f69 6d65 7068 752f  ephu/src/imephu/
-000004c0: 7361 6c74 2f75 7469 6c73 2e70 7972 0900  salt/utils.pyr..
-000004d0: 0000 0b00 0000 730c 0000 000a 0004 0208  ......s.........
-000004e0: 1208 0108 010c 0172 0900 0000 6300 0000  .......r....c...
-000004f0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00000500: 0040 0000 0073 c400 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000510: 5a02 5500 6401 5a03 6504 6505 6402 3c00  Z.U.d.Z.e.e.d.<.
-00000520: 6506 6505 6403 3c00 6507 6504 1900 6505  e.e.d.<.e.e...e.
-00000530: 6404 3c00 6507 6508 1900 6505 6405 3c00  d.<.e.e...e.d.<.
-00000540: 6406 6509 6407 6408 6604 6409 640a 8404  d.e.d.d.f.d.d...
-00000550: 5a0a 650b 640b 650c 6407 6400 6604 640c  Z.e.d.e.d.d.f.d.
-00000560: 640d 8404 8301 5a0d 650e 6407 6504 6602  d.....Z.e.d.e.f.
-00000570: 640e 640f 8404 8301 5a0f 650e 6407 6506  d.d.....Z.e.d.e.
-00000580: 6602 6410 6411 8404 8301 5a10 650e 6407  f.d.d.....Z.e.d.
-00000590: 6507 6504 1900 6602 6412 6413 8404 8301  e.e...f.d.d.....
-000005a0: 5a11 650e 6407 6507 6508 1900 6602 6414  Z.e.d.e.e...f.d.
-000005b0: 6415 8404 8301 5a12 6406 6509 6407 6408  d.....Z.d.e.d.d.
-000005c0: 6604 6416 6417 8404 5a13 6408 5300 2918  f.d.d...Z.d.S.).
-000005d0: da07 4d6f 734d 6173 6b61 3202 0000 4120  ..MosMaska2...A 
-000005e0: 5341 4c54 204d 4f53 206d 6173 6b2e 0a0a  SALT MOS mask...
-000005f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000600: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000610: 2020 6d61 736b 5f78 6d6c 3a20 7374 720a    mask_xml: str.
-00000620: 2020 2020 2020 2020 584d 4c20 6465 6669          XML defi
-00000630: 6e69 6e67 2074 6865 204d 4f53 206d 6173  ning the MOS mas
-00000640: 6b20 636f 6e74 656e 742e 0a0a 2020 2020  k content...    
-00000650: 4174 7472 6962 7574 6573 0a20 2020 202d  Attributes.    -
-00000660: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6365  ---------.    ce
-00000670: 6e74 6572 3a20 607e 6173 7472 6f70 792e  nter: `~astropy.
-00000680: 636f 6f72 6469 6e61 7465 732e 536b 7943  coordinates.SkyC
-00000690: 6f6f 7264 600a 2020 2020 2020 2020 5468  oord`.        Th
-000006a0: 6520 706f 7369 7469 6f6e 206f 6620 7468  e position of th
-000006b0: 6520 6d61 736b 2063 656e 7465 722c 2061  e mask center, a
-000006c0: 7320 7269 6768 7420 6173 6365 6e73 696f  s right ascensio
-000006d0: 6e20 616e 6420 6465 636c 696e 6174 696f  n and declinatio
-000006e0: 6e2e 0a20 2020 2070 6f73 6974 696f 6e5f  n..    position_
-000006f0: 616e 676c 653a 2060 7e61 7374 726f 7079  angle: `~astropy
-00000700: 2e63 6f6f 7264 696e 6174 6573 2e41 6e67  .coordinates.Ang
-00000710: 6c65 600a 2020 2020 2020 2020 5468 6520  le`.        The 
-00000720: 706f 7369 7469 6f6e 2061 6e67 6c65 206f  position angle o
-00000730: 6620 7468 6520 6d61 736b 2e0a 2020 2020  f the mask..    
-00000740: 7265 6665 7265 6e63 655f 7374 6172 733a  reference_stars:
-00000750: 206c 6973 7420 6f66 2060 6173 7472 6f70   list of `astrop
-00000760: 792e 636f 6f72 6469 6e61 7465 732e 536b  y.coordinates.Sk
-00000770: 7943 6f6f 7264 600a 2020 2020 2020 2020  yCoord`.        
-00000780: 5468 6520 706f 7369 7469 6f6e 7320 6f66  The positions of
-00000790: 2074 6865 2072 6566 6572 656e 6365 2073   the reference s
-000007a0: 7461 7273 2c20 6173 2072 6967 6874 2061  tars, as right a
-000007b0: 7363 656e 7369 6f6e 7320 616e 6420 6465  scensions and de
-000007c0: 636c 696e 6174 696f 6e73 2e0a 2020 2020  clinations..    
-000007d0: 736c 6974 733a 206c 6973 7420 6f66 2060  slits: list of `
-000007e0: 4d6f 734d 6173 6b53 6c69 7460 0a20 2020  MosMaskSlit`.   
-000007f0: 2020 2020 2054 6865 2073 6c69 7473 206f       The slits o
-00000800: 6e20 7468 6520 6d61 736b 2e0a 2020 2020  n the mask..    
-00000810: da07 5f63 656e 7465 72da 0f5f 706f 7369  .._center.._posi
-00000820: 7469 6f6e 5f61 6e67 6c65 da10 5f72 6566  tion_angle.._ref
-00000830: 6572 656e 6365 5f73 7461 7273 da06 5f73  erence_stars.._s
-00000840: 6c69 7473 da08 6d61 736b 5f78 6d6c da06  lits..mask_xml..
-00000850: 7265 7475 726e 4e63 0200 0000 0000 0000  returnNc........
-00000860: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00000870: 730e 0000 007c 00a0 007c 01a1 0101 0064  s....|...|.....d
-00000880: 0053 0029 014e 2901 da0e 5f69 6e69 745f  .S.).N)..._init_
-00000890: 6672 6f6d 5f78 6d6c 2902 da04 7365 6c66  from_xml)...self
-000008a0: 721a 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-000008b0: 1400 0000 da08 5f5f 696e 6974 5f5f 4100  ......__init__A.
-000008c0: 0000 7302 0000 000e 017a 104d 6f73 4d61  ..s......z.MosMa
-000008d0: 736b 2e5f 5f69 6e69 745f 5fda 046e 616d  sk.__init__..nam
-000008e0: 6563 0100 0000 0000 0000 0000 0000 0400  ec..............
-000008f0: 0000 0800 0000 4300 0000 7394 0000 0074  ......C...s....t
-00000900: 00a0 017c 00a1 0172 2a74 00a0 027c 0064  ...|...r*t...|.d
-00000910: 01a1 028f 137d 017c 01a0 0364 02a1 01a0  .....}.|...d....
-00000920: 0464 03a1 017d 0257 0064 0404 0004 0083  .d...}.W.d......
-00000930: 0301 0074 067c 0283 0153 0031 0073 2177  ...t.|...S.1.s!w
-00000940: 0101 0001 0001 0059 0001 0074 067c 0283  .......Y...t.|..
-00000950: 0153 0074 057c 0064 0183 028f 0f7d 037c  .S.t.|.d.....}.|
-00000960: 03a0 03a1 007d 0257 0064 0404 0004 0083  .....}.W.d......
-00000970: 0301 0074 067c 0283 0153 0031 0073 4177  ...t.|...S.1.sAw
-00000980: 0101 0001 0001 0059 0001 0074 067c 0283  .......Y...t.|..
-00000990: 0153 0029 0561 2401 0000 5265 7475 726e  .S.).a$...Return
-000009a0: 2074 6865 2060 7e69 6d65 7068 752e 7361   the `~imephu.sa
-000009b0: 6c74 2e75 7469 6c73 2e4d 6f73 4d61 736b  lt.utils.MosMask
-000009c0: 2064 6566 696e 6564 2069 6e20 6120 6669   defined in a fi
-000009d0: 6c65 2e0a 0a20 2020 2020 2020 2054 6865  le...        The
-000009e0: 2066 696c 6520 6361 6e20 6265 2061 6e20   file can be an 
-000009f0: 5253 4d54 2066 696c 652c 2061 7320 7072  RSMT file, as pr
-00000a00: 6f64 7563 6564 2062 7920 5341 4c54 2773  oduced by SALT's
-00000a10: 2052 5353 2053 6c69 7420 4d61 736b 2054   RSS Slit Mask T
-00000a20: 6f6f 6c2c 206f 7220 616e 0a20 2020 2020  ool, or an.     
-00000a30: 2020 2058 4d4c 2066 696c 652e 0a0a 2020     XML file...  
-00000a40: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00000a50: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00000a60: 2d2d 2d0a 2020 2020 2020 2020 7061 7468  ---.        path
-00000a70: 3a20 607e 7061 7468 6c69 622e 5061 7468  : `~pathlib.Path
-00000a80: 600a 2020 2020 2020 2020 2020 2020 5061  `.            Pa
-00000a90: 7468 206f 6620 7468 6520 6669 6c65 2064  th of the file d
-00000aa0: 6566 696e 696e 6720 7468 6520 4d4f 5320  efining the MOS 
-00000ab0: 6d61 736b 2e0a 2020 2020 2020 2020 da01  mask..        ..
-00000ac0: 727a 0c53 6c69 746d 6173 6b2e 786d 6c7a  rz.Slitmask.xmlz
-00000ad0: 0575 7466 2d38 4e29 07da 077a 6970 6669  .utf-8N)...zipfi
-00000ae0: 6c65 da0a 6973 5f7a 6970 6669 6c65 da07  le..is_zipfile..
-00000af0: 5a69 7046 696c 65da 0472 6561 64da 0664  ZipFile..read..d
-00000b00: 6563 6f64 65da 046f 7065 6e72 1500 0000  ecode..openr....
-00000b10: 2904 721f 0000 00da 0761 7263 6869 7665  ).r......archive
-00000b20: 721a 0000 00da 0166 7213 0000 0072 1300  r......fr....r..
-00000b30: 0000 7214 0000 00da 0966 726f 6d5f 6669  ..r......from_fi
-00000b40: 6c65 4400 0000 731a 0000 000a 0c0e 0112  leD...s.........
-00000b50: 010a ff08 0610 fa08 060c fd0a 010a ff08  ................
-00000b60: 0310 fd08 037a 114d 6f73 4d61 736b 2e66  .....z.MosMask.f
-00000b70: 726f 6d5f 6669 6c65 6301 0000 0000 0000  rom_filec.......
-00000b80: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000b90: 00f3 0600 0000 7c00 6a00 5300 2902 7a17  ......|.j.S.).z.
-00000ba0: 5265 7475 726e 2074 6865 206d 6173 6b20  Return the mask 
-00000bb0: 6365 6e74 6572 2e4e 2901 7216 0000 00a9  center.N).r.....
-00000bc0: 0172 1d00 0000 7213 0000 0072 1300 0000  .r....r....r....
-00000bd0: 7214 0000 0072 0a00 0000 5900 0000 f302  r....r....Y.....
-00000be0: 0000 0006 037a 0e4d 6f73 4d61 736b 2e63  .....z.MosMask.c
-00000bf0: 656e 7465 7263 0100 0000 0000 0000 0000  enterc..........
-00000c00: 0000 0100 0000 0100 0000 4300 0000 722a  ..........C...r*
-00000c10: 0000 0029 027a 1a52 6574 7572 6e20 7468  ...).z.Return th
-00000c20: 6520 706f 7369 7469 6f6e 2061 6e67 6c65  e position angle
-00000c30: 2e4e 2901 7217 0000 0072 2b00 0000 7213  .N).r....r+...r.
-00000c40: 0000 0072 1300 0000 7214 0000 00da 0e70  ...r....r......p
-00000c50: 6f73 6974 696f 6e5f 616e 676c 655e 0000  osition_angle^..
-00000c60: 0072 2c00 0000 7a16 4d6f 734d 6173 6b2e  .r,...z.MosMask.
-00000c70: 706f 7369 7469 6f6e 5f61 6e67 6c65 6301  position_anglec.
-00000c80: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000c90: 0000 0043 0000 0072 2a00 0000 2902 7a2c  ...C...r*...).z,
-00000ca0: 5265 7475 726e 2074 6865 206c 6973 7420  Return the list 
-00000cb0: 6f66 2072 6566 6572 656e 6365 2073 7461  of reference sta
-00000cc0: 7220 706f 7369 7469 6f6e 732e 4e29 0172  r positions.N).r
-00000cd0: 1800 0000 722b 0000 0072 1300 0000 7213  ....r+...r....r.
-00000ce0: 0000 0072 1400 0000 da0f 7265 6665 7265  ...r......refere
-00000cf0: 6e63 655f 7374 6172 7363 0000 0072 2c00  nce_starsc...r,.
-00000d00: 0000 7a17 4d6f 734d 6173 6b2e 7265 6665  ..z.MosMask.refe
-00000d10: 7265 6e63 655f 7374 6172 7363 0100 0000  rence_starsc....
-00000d20: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000d30: 4300 0000 722a 0000 0029 027a 1952 6574  C...r*...).z.Ret
-00000d40: 7572 6e20 7468 6520 6c69 7374 206f 6620  urn the list of 
-00000d50: 736c 6974 732e 4e29 0172 1900 0000 722b  slits.N).r....r+
-00000d60: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000d70: 0000 da05 736c 6974 7368 0000 0072 2c00  ....slitsh...r,.
-00000d80: 0000 7a0d 4d6f 734d 6173 6b2e 736c 6974  ..z.MosMask.slit
-00000d90: 7363 0200 0000 0000 0000 0000 0000 1100  sc..............
-00000da0: 0000 0900 0000 4300 0000 73a0 0100 0074  ......C...s....t
-00000db0: 007c 0183 017d 027c 02a0 0164 01a1 017d  .|...}.|...d...}
-00000dc0: 0369 007d 047c 0344 005d 107d 057c 05a0  .i.}.|.D.].}.|..
-00000dd0: 0264 02a1 017d 067c 05a0 0264 03a1 017d  .d...}.|...d...}
-00000de0: 077c 077c 047c 063c 0071 0d74 037c 0464  .|.|.|.<.q.t.|.d
-00000df0: 0419 0083 0174 046a 0514 007d 0874 037c  .....t.j...}.t.|
-00000e00: 0464 0519 0083 0174 046a 0514 007d 0974  .d.....t.j...}.t
-00000e10: 067c 087c 0964 068d 027c 005f 0774 037c  .|.|.d...|._.t.|
-00000e20: 0464 0719 0083 0174 046a 0514 007c 005f  .d.....t.j...|._
-00000e30: 087c 02a0 0164 08a1 017d 0a67 007c 005f  .|...d...}.g.|._
-00000e40: 097c 0a44 005d 557d 0b74 037c 0b6a 0a64  .|.D.]U}.t.|.j.d
-00000e50: 0919 006a 0b83 0174 046a 0514 007d 0874  ...j...t.j...}.t
-00000e60: 037c 0b6a 0a64 0a19 006a 0b83 0174 046a  .|.j.d...j...t.j
-00000e70: 0514 007d 0974 037c 0b6a 0a64 0b19 006a  ...}.t.|.j.d...j
-00000e80: 0b83 0174 046a 0c14 007d 0c74 037c 0b6a  ...t.j...}.t.|.j
-00000e90: 0a64 0c19 006a 0b83 0174 046a 0c14 007d  .d...j...t.j...}
-00000ea0: 0d64 0d74 046a 0514 007d 0e64 0e7c 0b6a  .d.t.j...}.d.|.j
-00000eb0: 0aa0 0da1 0076 0072 9074 037c 0b6a 0a64  .....v.r.t.|.j.d
-00000ec0: 0e19 006a 0b83 0174 046a 0514 007d 0e7c  ...j...t.j...}.|
-00000ed0: 006a 09a0 0e74 0f74 067c 087c 0964 068d  .j...t.t.|.|.d..
-00000ee0: 027c 0c7c 0d7c 0e64 0f8d 04a1 0101 0071  .|.|.|.d.......q
-00000ef0: 4b7c 02a0 0164 10a1 017d 0f67 007c 005f  K|...d...}.g.|._
-00000f00: 107c 0f44 005d 227d 1074 037c 106a 0a64  .|.D.]"}.t.|.j.d
-00000f10: 0919 006a 0b83 0174 046a 0514 007d 0874  ...j...t.j...}.t
-00000f20: 037c 106a 0a64 0a19 006a 0b83 0174 046a  .|.j.d...j...t.j
-00000f30: 0514 007d 097c 006a 10a0 0e74 067c 087c  ...}.|.j...t.|.|
-00000f40: 0964 068d 02a1 0101 0071 ab64 0053 0029  .d.......q.d.S.)
-00000f50: 114e da09 7061 7261 6d65 7465 7272 1f00  .N..parameterr..
-00000f60: 0000 da05 7661 6c75 655a 0843 454e 5445  ....valueZ.CENTE
-00000f70: 5252 415a 0943 454e 5445 5244 4543 2902  RRAZ.CENTERDEC).
-00000f80: da02 7261 da03 6465 635a 0852 4f54 414e  ..ra..decZ.ROTAN
-00000f90: 474c 45da 0473 6c69 745a 0378 6365 5a03  GLE..slitZ.xceZ.
-00000fa0: 7963 6572 0b00 0000 da06 6c65 6e67 7468  ycer......length
-00000fb0: 6700 0000 0000 0000 0072 0d00 0000 2904  g........r....).
-00000fc0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000fd0: 0d00 0000 5a07 7265 6673 7461 7229 1172  ....Z.refstar).r
-00000fe0: 0800 0000 da14 6765 7445 6c65 6d65 6e74  ......getElement
-00000ff0: 7342 7954 6167 4e61 6d65 da0c 6765 7441  sByTagName..getA
-00001000: 7474 7269 6275 7465 da05 666c 6f61 74da  ttribute..float.
-00001010: 0175 da03 6465 6772 0700 0000 7216 0000  .u..degr....r...
-00001020: 0072 1700 0000 7219 0000 00da 0a61 7474  .r....r......att
-00001030: 7269 6275 7465 7372 3100 0000 da06 6172  ributesr1.....ar
-00001040: 6373 6563 da04 6b65 7973 da06 6170 7065  csec..keys..appe
-00001050: 6e64 7209 0000 0072 1800 0000 2911 721d  ndr....r....).r.
-00001060: 0000 0072 1a00 0000 da03 646f 635a 1270  ...r......docZ.p
-00001070: 6172 616d 6574 6572 5f65 6c65 6d65 6e74  arameter_element
-00001080: 73da 0a70 6172 616d 6574 6572 73da 0370  s..parameters..p
-00001090: 6172 721f 0000 00da 0376 616c 7232 0000  arr......valr2..
-000010a0: 0072 3300 0000 5a0d 736c 6974 5f65 6c65  .r3...Z.slit_ele
-000010b0: 6d65 6e74 7372 3400 0000 720b 0000 0072  mentsr4...r....r
-000010c0: 0c00 0000 720d 0000 005a 1772 6566 6572  ....r....Z.refer
-000010d0: 656e 6365 5f73 7461 725f 656c 656d 656e  ence_star_elemen
-000010e0: 7473 da03 7265 6672 1300 0000 7213 0000  ts..refr....r...
-000010f0: 0072 1400 0000 721c 0000 006d 0000 0073  .r....r....m...s
-00001100: 4800 0000 0802 0a03 0401 0801 0a01 0a01  H...............
-00001110: 0a01 1201 1201 0e01 1401 0a03 0601 0801  ................
-00001120: 1601 1601 1601 1601 0a01 0e01 1601 0601  ................
-00001130: 0201 0a01 0201 0201 0201 04fc 06ff 0a0a  ................
-00001140: 0601 0801 1601 1601 1601 04fd 7a16 4d6f  ............z.Mo
-00001150: 734d 6173 6b2e 5f69 6e69 745f 6672 6f6d  sMask._init_from
-00001160: 5f78 6d6c 2914 720e 0000 0072 0f00 0000  _xml).r....r....
-00001170: 7210 0000 0072 1100 0000 7207 0000 0072  r....r....r....r
-00001180: 1200 0000 7206 0000 0072 0400 0000 7209  ....r....r....r.
-00001190: 0000 00da 0373 7472 721e 0000 00da 0c73  .....strr......s
-000011a0: 7461 7469 636d 6574 686f 6472 0300 0000  taticmethodr....
-000011b0: 7229 0000 00da 0870 726f 7065 7274 7972  r).....propertyr
-000011c0: 0a00 0000 722d 0000 0072 2e00 0000 722f  ....r-...r....r/
-000011d0: 0000 0072 1c00 0000 7213 0000 0072 1300  ...r....r....r..
-000011e0: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000011f0: 0025 0000 0073 2400 0000 0a00 0401 0813  .%...s$.........
-00001200: 0802 0c02 0c02 1202 0203 1401 0214 1001  ................
-00001210: 0204 1001 0204 1401 0204 1401 1604 7215  ..............r.
-00001220: 0000 0029 1172 2100 0000 da0b 6461 7461  ...).r!.....data
-00001230: 636c 6173 7365 7372 0200 0000 da07 7061  classesr......pa
-00001240: 7468 6c69 6272 0300 0000 da06 7479 7069  thlibr......typi
-00001250: 6e67 7204 0000 00da 0761 7374 726f 7079  ngr......astropy
-00001260: 7205 0000 0072 3900 0000 da13 6173 7472  r....r9.....astr
-00001270: 6f70 792e 636f 6f72 6469 6e61 7465 7372  opy.coordinatesr
-00001280: 0600 0000 7207 0000 005a 1264 6566 7573  ....r....Z.defus
-00001290: 6564 786d 6c2e 6d69 6e69 646f 6d72 0800  edxml.minidomr..
-000012a0: 0000 7209 0000 0072 1500 0000 7213 0000  ..r....r....r...
-000012b0: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-000012c0: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
-000012d0: 0000 0008 000c 010c 010c 010c 0210 010c  ................
-000012e0: 0104 0310 0112 19                        .......
+000003a0: 6b79 206d 6561 7375 7265 6420 6672 6f6d  ky measured from
+000003b0: 206e 6f72 7468 2074 6f20 6561 7374 2e0a   north to east..
+000003c0: 2020 2020 2222 220a 0a20 2020 2063 656e      """..    cen
+000003d0: 7465 723a 2053 6b79 436f 6f72 640a 2020  ter: SkyCoord.  
+000003e0: 2020 7769 6474 683a 2041 6e67 6c65 0a20    width: Angle. 
+000003f0: 2020 2068 6569 6768 743a 2041 6e67 6c65     height: Angle
+00000400: 0a20 2020 2074 696c 743a 2041 6e67 6c65  .    tilt: Angle
+00000410: 0a0a 0a63 6c61 7373 204d 6f73 4d61 736b  ...class MosMask
+00000420: 3a0a 2020 2020 2222 2241 2053 414c 5420  :.    """A SALT 
+00000430: 4d4f 5320 6d61 736b 2e0a 0a20 2020 2050  MOS mask...    P
+00000440: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00000450: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206d 6173  --------.    mas
+00000460: 6b5f 786d 6c3a 2073 7472 0a20 2020 2020  k_xml: str.     
+00000470: 2020 2058 4d4c 2064 6566 696e 696e 6720     XML defining 
+00000480: 7468 6520 4d4f 5320 6d61 736b 2063 6f6e  the MOS mask con
+00000490: 7465 6e74 2e0a 0a20 2020 2041 7474 7269  tent...    Attri
+000004a0: 6275 7465 730a 2020 2020 2d2d 2d2d 2d2d  butes.    ------
+000004b0: 2d2d 2d2d 0a20 2020 2063 656e 7465 723a  ----.    center:
+000004c0: 2060 7e61 7374 726f 7079 2e63 6f6f 7264   `~astropy.coord
+000004d0: 696e 6174 6573 2e53 6b79 436f 6f72 6460  inates.SkyCoord`
+000004e0: 0a20 2020 2020 2020 2054 6865 2070 6f73  .        The pos
+000004f0: 6974 696f 6e20 6f66 2074 6865 206d 6173  ition of the mas
+00000500: 6b20 6365 6e74 6572 2c20 6173 2072 6967  k center, as rig
+00000510: 6874 2061 7363 656e 7369 6f6e 2061 6e64  ht ascension and
+00000520: 2064 6563 6c69 6e61 7469 6f6e 2e0a 2020   declination..  
+00000530: 2020 706f 7369 7469 6f6e 5f61 6e67 6c65    position_angle
+00000540: 3a20 607e 6173 7472 6f70 792e 636f 6f72  : `~astropy.coor
+00000550: 6469 6e61 7465 732e 416e 676c 6560 0a20  dinates.Angle`. 
+00000560: 2020 2020 2020 2054 6865 2070 6f73 6974         The posit
+00000570: 696f 6e20 616e 676c 6520 6f66 2074 6865  ion angle of the
+00000580: 206d 6173 6b2e 0a20 2020 2072 6566 6572   mask..    refer
+00000590: 656e 6365 5f73 7461 7273 3a20 6c69 7374  ence_stars: list
+000005a0: 206f 6620 6061 7374 726f 7079 2e63 6f6f   of `astropy.coo
+000005b0: 7264 696e 6174 6573 2e53 6b79 436f 6f72  rdinates.SkyCoor
+000005c0: 6460 0a20 2020 2020 2020 2054 6865 2070  d`.        The p
+000005d0: 6f73 6974 696f 6e73 206f 6620 7468 6520  ositions of the 
+000005e0: 7265 6665 7265 6e63 6520 7374 6172 732c  reference stars,
+000005f0: 2061 7320 7269 6768 7420 6173 6365 6e73   as right ascens
+00000600: 696f 6e73 2061 6e64 2064 6563 6c69 6e61  ions and declina
+00000610: 7469 6f6e 732e 0a20 2020 2073 6c69 7473  tions..    slits
+00000620: 3a20 6c69 7374 206f 6620 604d 6f73 4d61  : list of `MosMa
+00000630: 736b 536c 6974 600a 2020 2020 2020 2020  skSlit`.        
+00000640: 5468 6520 736c 6974 7320 6f6e 2074 6865  The slits on the
+00000650: 206d 6173 6b2e 0a20 2020 2022 2222 0a0a   mask..    """..
+00000660: 2020 2020 5f63 656e 7465 723a 2053 6b79      _center: Sky
+00000670: 436f 6f72 640a 0a20 2020 205f 706f 7369  Coord..    _posi
+00000680: 7469 6f6e 5f61 6e67 6c65 3a20 416e 676c  tion_angle: Angl
+00000690: 650a 0a20 2020 205f 7265 6665 7265 6e63  e..    _referenc
+000006a0: 655f 7374 6172 733a 204c 6973 745b 536b  e_stars: List[Sk
+000006b0: 7943 6f6f 7264 5d0a 0a20 2020 205f 736c  yCoord]..    _sl
+000006c0: 6974 733a 204c 6973 745b 4d6f 734d 6173  its: List[MosMas
+000006d0: 6b53 6c69 745d 0a0a 2020 2020 6465 6620  kSlit]..    def 
+000006e0: 5f5f 696e 6974 5f5f 2873 656c 662c 206d  __init__(self, m
+000006f0: 6173 6b5f 786d 6c3a 2073 7472 2920 2d3e  ask_xml: str) ->
+00000700: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
+00000710: 656c 662e 5f69 6e69 745f 6672 6f6d 5f78  elf._init_from_x
+00000720: 6d6c 286d 6173 6b5f 786d 6c29 0a0a 2020  ml(mask_xml)..  
+00000730: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+00000740: 2020 2020 6465 6620 6672 6f6d 5f66 696c      def from_fil
+00000750: 6528 6e61 6d65 3a20 5061 7468 2920 2d3e  e(name: Path) ->
+00000760: 2022 4d6f 734d 6173 6b22 3a0a 2020 2020   "MosMask":.    
+00000770: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+00000780: 6520 607e 696d 6570 6875 2e73 616c 742e  e `~imephu.salt.
+00000790: 7574 696c 732e 4d6f 734d 6173 6b20 6465  utils.MosMask de
+000007a0: 6669 6e65 6420 696e 2061 2066 696c 652e  fined in a file.
+000007b0: 0a0a 2020 2020 2020 2020 5468 6520 6669  ..        The fi
+000007c0: 6c65 2063 616e 2062 6520 616e 2052 534d  le can be an RSM
+000007d0: 5420 6669 6c65 2c20 6173 2070 726f 6475  T file, as produ
+000007e0: 6365 6420 6279 2053 414c 5427 7320 5253  ced by SALT's RS
+000007f0: 5320 536c 6974 204d 6173 6b20 546f 6f6c  S Slit Mask Tool
+00000800: 2c20 6f72 2061 6e0a 2020 2020 2020 2020  , or an.        
+00000810: 584d 4c20 6669 6c65 2e0a 0a20 2020 2020  XML file...     
+00000820: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00000830: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00000840: 0a20 2020 2020 2020 2070 6174 683a 2060  .        path: `
+00000850: 7e70 6174 686c 6962 2e50 6174 6860 0a20  ~pathlib.Path`. 
+00000860: 2020 2020 2020 2020 2020 2050 6174 6820             Path 
+00000870: 6f66 2074 6865 2066 696c 6520 6465 6669  of the file defi
+00000880: 6e69 6e67 2074 6865 204d 4f53 206d 6173  ning the MOS mas
+00000890: 6b2e 0a20 2020 2020 2020 2022 2222 0a20  k..        """. 
+000008a0: 2020 2020 2020 2069 6620 7a69 7066 696c         if zipfil
+000008b0: 652e 6973 5f7a 6970 6669 6c65 286e 616d  e.is_zipfile(nam
+000008c0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+000008d0: 7769 7468 207a 6970 6669 6c65 2e5a 6970  with zipfile.Zip
+000008e0: 4669 6c65 286e 616d 652c 2022 7222 2920  File(name, "r") 
+000008f0: 6173 2061 7263 6869 7665 3a0a 2020 2020  as archive:.    
+00000900: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
+00000910: 5f78 6d6c 203d 2061 7263 6869 7665 2e72  _xml = archive.r
+00000920: 6561 6428 2253 6c69 746d 6173 6b2e 786d  ead("Slitmask.xm
+00000930: 6c22 292e 6465 636f 6465 2822 7574 662d  l").decode("utf-
+00000940: 3822 290a 2020 2020 2020 2020 656c 7365  8").        else
+00000950: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00000960: 7468 206f 7065 6e28 6e61 6d65 2c20 2272  th open(name, "r
+00000970: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+00000980: 2020 2020 2020 2020 206d 6173 6b5f 786d           mask_xm
+00000990: 6c20 3d20 662e 7265 6164 2829 0a0a 2020  l = f.read()..  
+000009a0: 2020 2020 2020 7265 7475 726e 204d 6f73        return Mos
+000009b0: 4d61 736b 286d 6173 6b5f 786d 6c29 0a0a  Mask(mask_xml)..
+000009c0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+000009d0: 2020 6465 6620 6365 6e74 6572 2873 656c    def center(sel
+000009e0: 6629 202d 3e20 536b 7943 6f6f 7264 3a0a  f) -> SkyCoord:.
+000009f0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00000a00: 6e20 7468 6520 6d61 736b 2063 656e 7465  n the mask cente
+00000a10: 722e 2222 220a 2020 2020 2020 2020 7265  r.""".        re
+00000a20: 7475 726e 2073 656c 662e 5f63 656e 7465  turn self._cente
+00000a30: 720a 0a20 2020 2040 7072 6f70 6572 7479  r..    @property
+00000a40: 0a20 2020 2064 6566 2070 6f73 6974 696f  .    def positio
+00000a50: 6e5f 616e 676c 6528 7365 6c66 2920 2d3e  n_angle(self) ->
+00000a60: 2041 6e67 6c65 3a0a 2020 2020 2020 2020   Angle:.        
+00000a70: 2222 2252 6574 7572 6e20 7468 6520 706f  """Return the po
+00000a80: 7369 7469 6f6e 2061 6e67 6c65 2e22 2222  sition angle."""
+00000a90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000aa0: 7365 6c66 2e5f 706f 7369 7469 6f6e 5f61  self._position_a
+00000ab0: 6e67 6c65 0a0a 2020 2020 4070 726f 7065  ngle..    @prope
+00000ac0: 7274 790a 2020 2020 6465 6620 7265 6665  rty.    def refe
+00000ad0: 7265 6e63 655f 7374 6172 7328 7365 6c66  rence_stars(self
+00000ae0: 2920 2d3e 204c 6973 745b 536b 7943 6f6f  ) -> List[SkyCoo
+00000af0: 7264 5d3a 0a20 2020 2020 2020 2022 2222  rd]:.        """
+00000b00: 5265 7475 726e 2074 6865 206c 6973 7420  Return the list 
+00000b10: 6f66 2072 6566 6572 656e 6365 2073 7461  of reference sta
+00000b20: 7220 706f 7369 7469 6f6e 732e 2222 220a  r positions.""".
+00000b30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000b40: 656c 662e 5f72 6566 6572 656e 6365 5f73  elf._reference_s
+00000b50: 7461 7273 0a0a 2020 2020 4070 726f 7065  tars..    @prope
+00000b60: 7274 790a 2020 2020 6465 6620 736c 6974  rty.    def slit
+00000b70: 7328 7365 6c66 2920 2d3e 204c 6973 745b  s(self) -> List[
+00000b80: 4d6f 734d 6173 6b53 6c69 745d 3a0a 2020  MosMaskSlit]:.  
+00000b90: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00000ba0: 7468 6520 6c69 7374 206f 6620 736c 6974  the list of slit
+00000bb0: 732e 2222 220a 2020 2020 2020 2020 7265  s.""".        re
+00000bc0: 7475 726e 2073 656c 662e 5f73 6c69 7473  turn self._slits
+00000bd0: 0a0a 2020 2020 6465 6620 5f69 6e69 745f  ..    def _init_
+00000be0: 6672 6f6d 5f78 6d6c 2873 656c 662c 206d  from_xml(self, m
+00000bf0: 6173 6b5f 786d 6c3a 2073 7472 2920 2d3e  ask_xml: str) ->
+00000c00: 204e 6f6e 653a 0a20 2020 2020 2020 2023   None:.        #
+00000c10: 2047 6574 2074 6865 2044 4f4d 0a20 2020   Get the DOM.   
+00000c20: 2020 2020 2064 6f63 203d 2070 6172 7365       doc = parse
+00000c30: 5374 7269 6e67 286d 6173 6b5f 786d 6c29  String(mask_xml)
+00000c40: 0a0a 2020 2020 2020 2020 2320 4578 7472  ..        # Extr
+00000c50: 6163 7420 7468 6520 6d61 736b 2070 6f73  act the mask pos
+00000c60: 6974 696f 6e20 616e 6420 726f 7461 7469  ition and rotati
+00000c70: 6f6e 2061 6e67 6c65 0a20 2020 2020 2020  on angle.       
+00000c80: 2070 6172 616d 6574 6572 5f65 6c65 6d65   parameter_eleme
+00000c90: 6e74 7320 3d20 646f 632e 6765 7445 6c65  nts = doc.getEle
+00000ca0: 6d65 6e74 7342 7954 6167 4e61 6d65 2822  mentsByTagName("
+00000cb0: 7061 7261 6d65 7465 7222 290a 2020 2020  parameter").    
+00000cc0: 2020 2020 7061 7261 6d65 7465 7273 203d      parameters =
+00000cd0: 207b 7d0a 2020 2020 2020 2020 666f 7220   {}.        for 
+00000ce0: 7061 7220 696e 2070 6172 616d 6574 6572  par in parameter
+00000cf0: 5f65 6c65 6d65 6e74 733a 0a20 2020 2020  _elements:.     
+00000d00: 2020 2020 2020 206e 616d 6520 3d20 7061         name = pa
+00000d10: 722e 6765 7441 7474 7269 6275 7465 2822  r.getAttribute("
+00000d20: 6e61 6d65 2229 0a20 2020 2020 2020 2020  name").         
+00000d30: 2020 2076 616c 203d 2070 6172 2e67 6574     val = par.get
+00000d40: 4174 7472 6962 7574 6528 2276 616c 7565  Attribute("value
+00000d50: 2229 0a20 2020 2020 2020 2020 2020 2070  ").            p
+00000d60: 6172 616d 6574 6572 735b 6e61 6d65 5d20  arameters[name] 
+00000d70: 3d20 7661 6c0a 2020 2020 2020 2020 7261  = val.        ra
+00000d80: 203d 2066 6c6f 6174 2870 6172 616d 6574   = float(paramet
+00000d90: 6572 735b 2243 454e 5445 5252 4122 5d29  ers["CENTERRA"])
+00000da0: 202a 2075 2e64 6567 0a20 2020 2020 2020   * u.deg.       
+00000db0: 2064 6563 203d 2066 6c6f 6174 2870 6172   dec = float(par
+00000dc0: 616d 6574 6572 735b 2243 454e 5445 5244  ameters["CENTERD
+00000dd0: 4543 225d 2920 2a20 752e 6465 670a 2020  EC"]) * u.deg.  
+00000de0: 2020 2020 2020 7365 6c66 2e5f 6365 6e74        self._cent
+00000df0: 6572 203d 2053 6b79 436f 6f72 6428 7261  er = SkyCoord(ra
+00000e00: 3d72 612c 2064 6563 3d64 6563 290a 2020  =ra, dec=dec).  
+00000e10: 2020 2020 2020 7365 6c66 2e5f 706f 7369        self._posi
+00000e20: 7469 6f6e 5f61 6e67 6c65 203d 2066 6c6f  tion_angle = flo
+00000e30: 6174 2870 6172 616d 6574 6572 735b 2252  at(parameters["R
+00000e40: 4f54 414e 474c 4522 5d29 202a 2075 2e64  OTANGLE"]) * u.d
+00000e50: 6567 0a0a 2020 2020 2020 2020 2320 4578  eg..        # Ex
+00000e60: 7472 6163 7420 7468 6520 736c 6974 2064  tract the slit d
+00000e70: 6574 6169 6c73 0a20 2020 2020 2020 2073  etails.        s
+00000e80: 6c69 745f 656c 656d 656e 7473 203d 2064  lit_elements = d
+00000e90: 6f63 2e67 6574 456c 656d 656e 7473 4279  oc.getElementsBy
+00000ea0: 5461 674e 616d 6528 2273 6c69 7422 290a  TagName("slit").
+00000eb0: 2020 2020 2020 2020 7365 6c66 2e5f 736c          self._sl
+00000ec0: 6974 7320 3d20 5b5d 0a20 2020 2020 2020  its = [].       
+00000ed0: 2066 6f72 2073 6c69 7420 696e 2073 6c69   for slit in sli
+00000ee0: 745f 656c 656d 656e 7473 3a0a 2020 2020  t_elements:.    
+00000ef0: 2020 2020 2020 2020 7261 203d 2066 6c6f          ra = flo
+00000f00: 6174 2873 6c69 742e 6174 7472 6962 7574  at(slit.attribut
+00000f10: 6573 5b22 7863 6522 5d2e 7661 6c75 6529  es["xce"].value)
+00000f20: 202a 2075 2e64 6567 0a20 2020 2020 2020   * u.deg.       
+00000f30: 2020 2020 2064 6563 203d 2066 6c6f 6174       dec = float
+00000f40: 2873 6c69 742e 6174 7472 6962 7574 6573  (slit.attributes
+00000f50: 5b22 7963 6522 5d2e 7661 6c75 6529 202a  ["yce"].value) *
+00000f60: 2075 2e64 6567 0a20 2020 2020 2020 2020   u.deg.         
+00000f70: 2020 2077 6964 7468 203d 2066 6c6f 6174     width = float
+00000f80: 2873 6c69 742e 6174 7472 6962 7574 6573  (slit.attributes
+00000f90: 5b22 7769 6474 6822 5d2e 7661 6c75 6529  ["width"].value)
+00000fa0: 202a 2075 2e61 7263 7365 630a 2020 2020   * u.arcsec.    
+00000fb0: 2020 2020 2020 2020 6865 6967 6874 203d          height =
+00000fc0: 2066 6c6f 6174 2873 6c69 742e 6174 7472   float(slit.attr
+00000fd0: 6962 7574 6573 5b22 6c65 6e67 7468 225d  ibutes["length"]
+00000fe0: 2e76 616c 7565 2920 2a20 752e 6172 6373  .value) * u.arcs
+00000ff0: 6563 0a20 2020 2020 2020 2020 2020 2074  ec.            t
+00001000: 696c 7420 3d20 302e 3020 2a20 752e 6465  ilt = 0.0 * u.de
+00001010: 670a 2020 2020 2020 2020 2020 2020 6966  g.            if
+00001020: 2022 7469 6c74 2220 696e 2073 6c69 742e   "tilt" in slit.
+00001030: 6174 7472 6962 7574 6573 2e6b 6579 7328  attributes.keys(
+00001040: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001050: 2020 2074 696c 7420 3d20 666c 6f61 7428     tilt = float(
+00001060: 736c 6974 2e61 7474 7269 6275 7465 735b  slit.attributes[
+00001070: 2274 696c 7422 5d2e 7661 6c75 6529 202a  "tilt"].value) *
+00001080: 2075 2e64 6567 0a20 2020 2020 2020 2020   u.deg.         
+00001090: 2020 2073 656c 662e 5f73 6c69 7473 2e61     self._slits.a
+000010a0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
+000010b0: 2020 2020 2020 204d 6f73 4d61 736b 536c         MosMaskSl
+000010c0: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
+000010d0: 2020 2020 2020 2020 6365 6e74 6572 3d53          center=S
+000010e0: 6b79 436f 6f72 6428 7261 3d72 612c 2064  kyCoord(ra=ra, d
+000010f0: 6563 3d64 6563 292c 0a20 2020 2020 2020  ec=dec),.       
+00001100: 2020 2020 2020 2020 2020 2020 2077 6964               wid
+00001110: 7468 3d77 6964 7468 2c0a 2020 2020 2020  th=width,.      
+00001120: 2020 2020 2020 2020 2020 2020 2020 6865                he
+00001130: 6967 6874 3d68 6569 6768 742c 0a20 2020  ight=height,.   
+00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 2074 696c 743d 7469 6c74 2c0a 2020 2020   tilt=tilt,.    
+00001160: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00001170: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00001180: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
+00001190: 6865 2072 6566 6572 656e 6365 2073 7461  he reference sta
+000011a0: 7220 6465 7461 696c 730a 2020 2020 2020  r details.      
+000011b0: 2020 7265 6665 7265 6e63 655f 7374 6172    reference_star
+000011c0: 5f65 6c65 6d65 6e74 7320 3d20 646f 632e  _elements = doc.
+000011d0: 6765 7445 6c65 6d65 6e74 7342 7954 6167  getElementsByTag
+000011e0: 4e61 6d65 2822 7265 6673 7461 7222 290a  Name("refstar").
+000011f0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+00001200: 6665 7265 6e63 655f 7374 6172 7320 3d20  ference_stars = 
+00001210: 5b5d 0a20 2020 2020 2020 2066 6f72 2072  [].        for r
+00001220: 6566 2069 6e20 7265 6665 7265 6e63 655f  ef in reference_
+00001230: 7374 6172 5f65 6c65 6d65 6e74 733a 0a20  star_elements:. 
+00001240: 2020 2020 2020 2020 2020 2072 6120 3d20             ra = 
+00001250: 666c 6f61 7428 7265 662e 6174 7472 6962  float(ref.attrib
+00001260: 7574 6573 5b22 7863 6522 5d2e 7661 6c75  utes["xce"].valu
+00001270: 6529 202a 2075 2e64 6567 0a20 2020 2020  e) * u.deg.     
+00001280: 2020 2020 2020 2064 6563 203d 2066 6c6f         dec = flo
+00001290: 6174 2872 6566 2e61 7474 7269 6275 7465  at(ref.attribute
+000012a0: 735b 2279 6365 225d 2e76 616c 7565 2920  s["yce"].value) 
+000012b0: 2a20 752e 6465 670a 2020 2020 2020 2020  * u.deg.        
+000012c0: 2020 2020 7365 6c66 2e5f 7265 6665 7265      self._refere
+000012d0: 6e63 655f 7374 6172 732e 6170 7065 6e64  nce_stars.append
+000012e0: 2853 6b79 436f 6f72 6428 7261 3d72 612c  (SkyCoord(ra=ra,
+000012f0: 2064 6563 3d64 6563 2929 0a               dec=dec)).
```

### Comparing `imephu-0.2.0/src/imephu/salt/annotation/nir.py` & `imephu-0.2.1/src/imephu/salt/annotation/nir.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import Angle, SkyCoord
 from astropy.wcs import WCS
-
 from imephu.annotation.general import (
     CircleAnnotation,
     CrosshairsAnnotation,
     GroupAnnotation,
     LinePathAnnotation,
 )
 from imephu.geometry import translate
@@ -55,22 +54,26 @@
         r=r,
         d_horizontal=d_horizontal,
         d_vertical=d_vertical,
         center=science_bundle_center,
         wcs=wcs,
         include_fibers=include_fibers,
     )
-    sky_bundle = _sky_bundle(
-        r=r,
-        d_horizontal=d_horizontal,
-        d_vertical=d_vertical,
-        center=science_bundle_center,
-        wcs=wcs,
-        include_fibers=include_fibers,
-    ).translate((0, bundle_separaration_arcsec) * u.arcsec)
+    sky_bundle = (
+        _sky_bundle(
+            r=r,
+            d_horizontal=d_horizontal,
+            d_vertical=d_vertical,
+            center=science_bundle_center,
+            wcs=wcs,
+            include_fibers=include_fibers,
+        )
+        .rotate(science_bundle_center, 90 * u.deg)
+        .translate((0, bundle_separaration_arcsec) * u.arcsec)
+    )
     annotation = GroupAnnotation([sky_bundle, science_bundle])
     return annotation.rotate(science_bundle_center, position_angle)
 
 
 def _science_bundle(
     r: Angle,
     d_horizontal: Angle,
```

### Comparing `imephu-0.2.0/src/imephu/salt/finder_chart.py` & `imephu-0.2.1/src/imephu/salt/finder_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, BinaryIO, Generator, List, Optional, Tuple, Union
 
 from astropy import units as u
 from astropy.coordinates import Angle, SkyCoord
 from astropy.wcs import WCS
-
 from imephu.annotation.general import GroupAnnotation
 from imephu.annotation.motion import motion_annotation
 from imephu.finder_chart import FinderChart
 from imephu.salt.annotation import nir, rss, telescope
 from imephu.salt.utils import MosMask
 from imephu.utils import (
     Ephemeris,
@@ -163,19 +162,22 @@
         slit_height=slit_height,
         wcs=finder_chart.wcs,
     )
     finder_chart.add_annotation(annotation)
     return finder_chart
 
 
+DEFAULT_REF_STAR_BOX_SIZE = Angle(5 * u.arcsec)
+
+
 def rss_mos_finder_chart(
     fits: Union[str, BinaryIO, os.PathLike[Any]],
     general: GeneralProperties,
     mos_mask: MosMask,
-    reference_star_box_width: Angle = Angle(5 * u.arcsec),
+    reference_star_box_width: Angle = DEFAULT_REF_STAR_BOX_SIZE,
 ) -> FinderChart:
     """Return the finder chart for an RSS MOS observation.
 
     Parameters
     ----------
     fits: `str`, `path-like` or `binary file-like`
         FITS file to display.
@@ -433,15 +435,14 @@
     observation_annotation = _base_annotations(general, wcs)
     magnitude_range = general.target.magnitude_range
     if magnitude_range:
         magnitude_annotation = telescope.magnitude_range_annotation(
             bandpass=magnitude_range.bandpass,
             min_magnitude=magnitude_range.min_magnitude,
             max_magnitude=magnitude_range.max_magnitude,
-            fits_center=general.target.position,
             wcs=wcs,
         )
         observation_annotation.add_item(magnitude_annotation)
     if is_slot_mode:
         center = general.target.position
         slot_annotation = telescope.slot_annotation(center, general.position_angle, wcs)
         observation_annotation.add_item(slot_annotation)
```

### Comparing `imephu-0.2.0/src/imephu/schema.json` & `imephu-0.2.1/src/imephu/schema.json`

 * *Files identical despite different names*

### Comparing `imephu-0.2.0/src/imephu/service/horizons.py` & `imephu-0.2.1/src/imephu/service/horizons.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import List, Optional
 
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.units import Quantity
 from astroquery.jplhorizons import Horizons
 from dateutil.parser import parse
-
 from imephu.utils import Ephemeris, MagnitudeRange
 
 
 class HorizonsService:
     """A service for querying ephemerides from JPL Horizons.
 
     The service is initialised by calling the constructor with a start and end time,
```

### Comparing `imephu-0.2.0/src/imephu/service/survey.py` & `imephu-0.2.1/src/imephu/service/survey.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import urllib.parse
 from io import BytesIO
-from typing import BinaryIO, Protocol, NamedTuple, Callable, Dict
+from typing import BinaryIO, Callable, Dict, NamedTuple, Protocol
 
 import requests
 from astropy import units as u
 from astropy.coordinates import Angle, SkyCoord
 
 
 class SurveyError(BaseException):
@@ -14,33 +14,37 @@
 
 
 class _SurveyDetails(NamedTuple):
     identifier: str
     is_covering_position: Callable[[SkyCoord], bool]
 
 
-_always_true = lambda x: True
+def _always_true(x: SkyCoord) -> bool:
+    return True
 
 
 _DSS_DETAILS: Dict[str, _SurveyDetails] = {
     "POSS2/UKSTU Red": _SurveyDetails("poss2ukstu_red", _always_true),
-    "POSS2/UKSTU Blue":  _SurveyDetails("poss2ukstu_blue", _always_true),
+    "POSS2/UKSTU Blue": _SurveyDetails("poss2ukstu_blue", _always_true),
     "POSS2/UKSTU IR": _SurveyDetails("poss2ukstu_ir", _always_true),
     "POSS1 Red": _SurveyDetails("poss1_red", lambda p: p.dec.to_value(u.deg) > -30),
     "POSS1 Blue": _SurveyDetails("poss1_blue", lambda p: p.dec.to_value(u.deg) > -30),
     "Quick-V": _SurveyDetails("quickv", lambda p: p.dec.to_value(u.deg) > 6),
     "HST Phase2 (GSC2)": _SurveyDetails("phase2_gsc2", _always_true),
-    "HST Phase2 (GSC1)": _SurveyDetails("phase2_gsc1", lambda p: p.dec.to_value(u.deg) < -20 or p.dec.to_value(u.deg) > 6)
+    "HST Phase2 (GSC1)": _SurveyDetails(
+        "phase2_gsc1",
+        lambda p: p.dec.to_value(u.deg) < -20 or p.dec.to_value(u.deg) > 6,
+    ),
 }
 
 
 _SKYVIEW_DETAILS = {
     "2MASS-H": _SurveyDetails("2mass-h", _always_true),
     "2MASS-J": _SurveyDetails("2mass-j", _always_true),
-    "2MASS-K": _SurveyDetails("2mass-k", _always_true)
+    "2MASS-K": _SurveyDetails("2mass-k", _always_true),
 }
 
 
 class SkySurvey(Protocol):
     """A sky survey from which fits files can be requested."""
 
     def url(self, survey: str, fits_center: SkyCoord, size: Angle) -> str:
@@ -175,18 +179,21 @@
             The width and height of the FITS image, as an angle on the sky.
 
         Returns
         -------
         binary stream
             The FITS file.
         """
-        response = requests.get(self.url(survey, fits_center, size))
-        if response.status_code != 200:
-            raise SurveyError("No FITS file could be loaded.")
-        return BytesIO(response.content)
+        try:
+            response = requests.get(self.url(survey, fits_center, size))
+            if response.status_code != 200:
+                raise SurveyError("No FITS file could be loaded.")
+            return BytesIO(response.content)
+        except BaseException as e:
+            raise SurveyError("No FITS file could be loaded.") from e
 
     def is_covering_position(self, survey: str, position: SkyCoord) -> bool:
         """Return whether a position is covered by the sky survey.
 
         Parameters
         ----------
         survey: `str`
@@ -197,15 +204,14 @@
         Returns
         -------
         bool
             True if the position is covered  by the survey, False otherwise.
         """
         return self._survey_details[survey.lower()].is_covering_position(position)
 
-
     def _survey_identifier(self, survey: str) -> str:
         if survey.lower() not in self._survey_details:
             raise ValueError(f"Unknown survey: {survey}")
 
         return self._survey_details[survey.lower()].identifier
 
 
@@ -281,18 +287,21 @@
             The width and height of the FITS image, as an angle on the sky.
 
         Returns
         -------
         binary stream
             The FITS file.
         """
-        response = requests.get(self.url(survey, fits_center, size))
-        if response.status_code != 200:
-            raise SurveyError("No FITS file could be loaded.")
-        return BytesIO(response.content)
+        try:
+            response = requests.get(self.url(survey, fits_center, size))
+            if response.status_code != 200:
+                raise SurveyError("No FITS file could be loaded.")
+            return BytesIO(response.content)
+        except BaseException as e:
+            raise SurveyError("No FITS file could be loaded.") from e
 
     def is_covering_position(self, survey: str, position: SkyCoord) -> bool:
         """Return whether a position is covered by the sky survey.
 
         Parameters
         ----------
         survey: `str`
@@ -305,15 +314,15 @@
         bool
             True if the position is covered  by the survey, False otherwise.
         """
         return self._survey_details[survey.lower()].is_covering_position(position)
 
     def _survey_identifier(self, survey: str) -> str:
         if survey.lower() not in self._survey_details:
-            raise ValueError(f"Unknown survey: {survey}")
+            raise SurveyError(f"Unknown survey: {survey}")
 
         return self._survey_details[survey.lower()].identifier
 
 
 def url(survey: str, fits_center: SkyCoord, size: Angle) -> str:
     """Return the URL for requesting a FITS image from a sky survey.
 
@@ -458,8 +467,7 @@
     if survey.lower() in [s.lower() for s in _DSS_DETAILS.keys()]:
         survey_: SkySurvey = DigitizedSkySurvey()
     elif survey.lower() in [s.lower() for s in _SKYVIEW_DETAILS.keys()]:
         survey_ = SkyView(pixels=700)
     else:
         raise ValueError(f"Unknown survey: {survey}")
     return survey_.is_covering_position(survey, position)
-
```

### Comparing `imephu-0.2.0/src/imephu/utils.py` & `imephu-0.2.1/src/imephu/utils.py`

 * *Files identical despite different names*

