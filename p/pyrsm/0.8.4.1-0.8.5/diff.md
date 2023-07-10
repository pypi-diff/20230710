# Comparing `tmp/pyrsm-0.8.4.1.tar.gz` & `tmp/pyrsm-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.4.1.tar", last modified: Fri May 26 03:12:02 2023, max compression
+gzip compressed data, was "pyrsm-0.8.5.tar", last modified: Mon Jul 10 07:40:09 2023, max compression
```

## Comparing `pyrsm-0.8.4.1.tar` & `pyrsm-0.8.5.tar`

### file list

```diff
@@ -1,84 +1,153 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.576685 pyrsm-0.8.4.1/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.4.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      243 2023-05-16 06:57:58.000000 pyrsm-0.8.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-26 03:12:02.576775 pyrsm-0.8.4.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.4.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.4.1/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.564419 pyrsm-0.8.4.1/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      314 2023-05-26 03:08:41.000000 pyrsm-0.8.4.1/pyrsm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.4.1/pyrsm/basics.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.4.1/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.565243 pyrsm-0.8.4.1/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.566444 pyrsm-0.8.4.1/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/basics/salary.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.567845 pyrsm-0.8.4.1/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/data/titanic.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.568238 pyrsm-0.8.4.1/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/design/rndnames.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.571195 pyrsm-0.8.4.1/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/movie_contract.pkl
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/model/ratings.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.572969 pyrsm-0.8.4.1/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.4.1/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.4.1/pyrsm/logit.py
--rw-r--r--   0 root         (0) staff       (20)    25270 2023-05-21 21:48:34.000000 pyrsm-0.8.4.1/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.4.1/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.4.1/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.573561 pyrsm-0.8.4.1/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)       23 2023-05-18 03:04:58.000000 pyrsm-0.8.4.1/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9489 2023-05-15 05:18:12.000000 pyrsm-0.8.4.1/pyrsm/radiant/logit.py
--rw-r--r--   0 root         (0) staff       (20)    20447 2023-05-26 01:35:11.000000 pyrsm-0.8.4.1/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     1200 2023-05-23 03:10:54.000000 pyrsm-0.8.4.1/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.574261 pyrsm-0.8.4.1/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)      230 2023-05-11 03:12:37.000000 pyrsm-0.8.4.1/pyrsm/radiant/www/copy.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.4.1/pyrsm/radiant/www/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)     3597 2023-05-11 03:12:22.000000 pyrsm-0.8.4.1/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9296 2023-05-24 09:09:52.000000 pyrsm-0.8.4.1/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.4.1/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.4.1/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22603 2023-05-22 00:34:13.000000 pyrsm-0.8.4.1/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.565106 pyrsm-0.8.4.1/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-26 03:12:02.000000 pyrsm-0.8.4.1/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1838 2023-05-26 03:12:02.000000 pyrsm-0.8.4.1/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-26 03:12:02.000000 pyrsm-0.8.4.1/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      226 2023-05-26 03:12:02.000000 pyrsm-0.8.4.1/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-05-26 03:12:02.000000 pyrsm-0.8.4.1/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-05-26 03:12:02.577142 pyrsm-0.8.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 03:12:02.576409 pyrsm-0.8.4.1/tests/
--rw-r--r--   0 root         (0) staff       (20)      722 2023-05-16 05:24:37.000000 pyrsm-0.8.4.1/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.4.1/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-05-16 05:39:55.000000 pyrsm-0.8.4.1/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.4.1/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      615 2023-05-16 05:41:07.000000 pyrsm-0.8.4.1/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.4.1/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.4.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.300743 pyrsm-0.8.5/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      476 2023-07-09 01:34:00.000000 pyrsm-0.8.5/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-10 07:40:09.300825 pyrsm-0.8.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.5/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.5/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.280155 pyrsm-0.8.5/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-09 05:08:38.000000 pyrsm-0.8.5/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.282462 pyrsm-0.8.5/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-08 18:41:11.000000 pyrsm-0.8.5/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.5/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     5674 2023-07-08 23:31:10.000000 pyrsm-0.8.5/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5446 2023-07-08 22:24:23.000000 pyrsm-0.8.5/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7460 2023-07-08 22:19:48.000000 pyrsm-0.8.5/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9696 2023-07-08 23:21:46.000000 pyrsm-0.8.5/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     9944 2023-07-08 22:40:14.000000 pyrsm-0.8.5/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     8394 2023-07-08 22:20:36.000000 pyrsm-0.8.5/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)     3854 2023-07-08 23:08:05.000000 pyrsm-0.8.5/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3141 2023-07-08 23:50:35.000000 pyrsm-0.8.5/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.5/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.5/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.282734 pyrsm-0.8.5/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.5/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.284725 pyrsm-0.8.5/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/consider.pkl
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/demand_uk.pkl
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/newspaper.pkl
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/salary.pkl
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.287487 pyrsm-0.8.5/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/avengers.pkl
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/diamonds.pkl
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/publishers.pkl
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/superheroes.pkl
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/titanic.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.288179 pyrsm-0.8.5/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/design/rndnames.pkl
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.292164 pyrsm-0.8.5/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/catalog.pkl
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/direct_marketing.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/dvd.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/houseprices.pkl
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/ideal.pkl
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/ketchup.pkl
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/ratings.pkl
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ratings_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.297766 pyrsm-0.8.5/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/carpet.pkl
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city2.pkl
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/computer.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/movie.pkl
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/mp3.pkl
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/retailers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/shopping.pkl
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands.pkl
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.5/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9526 2023-07-10 04:08:57.000000 pyrsm-0.8.5/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25570 2023-07-04 04:09:06.000000 pyrsm-0.8.5/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.5/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.5/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.298728 pyrsm-0.8.5/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-07-09 05:08:44.000000 pyrsm-0.8.5/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6036 2023-07-10 07:37:12.000000 pyrsm-0.8.5/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     4945 2023-07-10 07:15:59.000000 pyrsm-0.8.5/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    10678 2023-07-10 07:32:46.000000 pyrsm-0.8.5/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)     4756 2023-07-10 07:08:33.000000 pyrsm-0.8.5/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     6006 2023-07-10 07:36:25.000000 pyrsm-0.8.5/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    14896 2023-07-10 07:11:35.000000 pyrsm-0.8.5/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.299159 pyrsm-0.8.5/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)      290 2023-07-07 20:52:09.000000 pyrsm-0.8.5/pyrsm/radiant/www/copy.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.5/pyrsm/radiant/www/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)      534 2023-07-07 22:43:29.000000 pyrsm-0.8.5/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9390 2023-07-10 01:21:40.000000 pyrsm-0.8.5/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.5/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.5/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-06-13 07:22:05.000000 pyrsm-0.8.5/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.280815 pyrsm-0.8.5/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4423 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      226 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-10 07:40:09.301169 pyrsm-0.8.5/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.300614 pyrsm-0.8.5/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.5/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.5/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.5/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.5/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.5/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.5/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.5/tests/test_utils.py
```

### Comparing `pyrsm-0.8.4.1/LICENSE` & `pyrsm-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/PKG-INFO` & `pyrsm-0.8.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.4.1
+Version: 0.8.5
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.4.1/README.md` & `pyrsm-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/bins.py` & `pyrsm-0.8.5/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/basics/consider.pkl` & `pyrsm-0.8.5/pyrsm/data/basics/consider.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/basics/demand_uk.pkl` & `pyrsm-0.8.5/pyrsm/data/basics/demand_uk.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/basics/newspaper.pkl` & `pyrsm-0.8.5/pyrsm/data/basics/newspaper.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/basics/salary.pkl` & `pyrsm-0.8.5/pyrsm/data/basics/salary.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/data/avengers.pkl` & `pyrsm-0.8.5/pyrsm/data/data/avengers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/data/diamonds.pkl` & `pyrsm-0.8.5/pyrsm/data/data/diamonds.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/data/publishers.pkl` & `pyrsm-0.8.5/pyrsm/data/data/publishers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/data/superheroes.pkl` & `pyrsm-0.8.5/pyrsm/data/data/superheroes.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/data/titanic.pkl` & `pyrsm-0.8.5/pyrsm/data/data/titanic.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/design/rndnames.pkl` & `pyrsm-0.8.5/pyrsm/data/design/rndnames.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/model/catalog.pkl` & `pyrsm-0.8.5/pyrsm/data/model/catalog.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/model/direct_marketing.pkl` & `pyrsm-0.8.5/pyrsm/data/model/direct_marketing.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/model/dvd.pkl` & `pyrsm-0.8.5/pyrsm/data/model/dvd.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/model/houseprices.pkl` & `pyrsm-0.8.5/pyrsm/data/model/houseprices.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/model/ideal.pkl` & `pyrsm-0.8.5/pyrsm/data/model/ideal.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/model/ketchup.pkl` & `pyrsm-0.8.5/pyrsm/data/model/ketchup.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/model/ratings.pkl` & `pyrsm-0.8.5/pyrsm/data/model/ratings.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/carpet.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/carpet.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/city.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/city.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/city2.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/city2.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/computer.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/computer.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/movie.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/movie.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/mp3.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/mp3.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/retailers.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/retailers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/shopping.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/shopping.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/toothpaste.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/data/multivariate/tpbrands.pkl` & `pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/logit.py` & `pyrsm-0.8.5/pyrsm/radiant/single_mean.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,148 +1,191 @@
-from typing import Union, Optional
-import pandas as pd
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib.ticker as ticker
-import statsmodels as sm
-from statsmodels.genmod.families import Binomial
-from statsmodels.genmod.families.links import logit
-import statsmodels.formula.api as smf
-from statsmodels.stats.outliers_influence import variance_inflation_factor
-from scipy import stats
-from scipy.special import expit
-from .utils import ifelse
-from .stats import weighted_mean, weighted_sd
-from .perf import auc
-from .model import sig_stars, model_fit, or_ci, or_plot, sim_prediction
-
-# from statsmodels.regression.linear_model import RegressionResults as rrs
-from .visualize import pred_plot_sm, vimp_plot_sm, extract_evars, extract_rvar
-
-
-class logistic:
-    def __init__(
-        self,
-        dataset: pd.DataFrame,
-        rvar: Optional[str] = None,
-        lev: Optional[str] = None,
-        evar: Optional[list[str]] = None,
-        form: Optional[str] = None,
-    ) -> None:
-        """
-        Initialize logistic regression model
-
-        Parameters
-        ----------
-        dataset: pandas DataFrame; dataset
-        evar: List of strings; contains the names of the columns of data to be used as explanatory variables
-        lev: String; name of the level in the response variable
-        rvar: String; name of the column to be used as the response variable
-        form: String; formula for the regression equation to use if evar and rvar are not provided
-        """
-        self.dataset = dataset
-        self.rvar = rvar
-        self.lev = lev
-        self.evar = evar
-        self.form = form
-
-        if self.form:
-            self.fitted = smf.glm(
-                formula=self.form, data=self.dataset, family=Binomial(link=logit())
-            ).fit()
-            self.evar = extract_evars(self.fitted.model, self.dataset.columns)
-            self.rvar = extract_rvar(self.fitted.model, self.dataset.columns)
-            self.lev = self.dataset.at[0, self.rvar]
-        else:
-            self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
-            self.fitted = smf.glm(
-                formula=self.form, data=self.dataset, family=Binomial(link=logit())
-            ).fit()
-
-        df = pd.DataFrame(np.exp(self.fitted.params), columns=["OR"]).dropna()
-        df["OR%"] = 100 * ifelse(df["OR"] < 1, -(1 - df["OR"]), df["OR"] - 1)
-        df["coefficient"] = self.fitted.params
-        df["std.error"] = self.fitted.params / self.fitted.tvalues
-        # wierd but this is what statsmodels uses in summary
-        df["z.value"] = self.fitted.tvalues
-        df["p.value"] = self.fitted.pvalues
-        df["  "] = sig_stars(self.fitted.pvalues)
-        self.coef = df.reset_index()
-
-    def summary(self, dec=3) -> None:
-        """
-        Summarize output from a logistic regression model
-        """
-
-        if hasattr(self.dataset, "description"):
-            data_name = self.dataset.description.split("\n")[0].split()[1].lower()
-        else:
-            data_name = "Not available"
-
-        print("Logistic regression (GLM)")
-        print(f"Data                 : {data_name}")
-        print(f"Response variable    : {self.rvar}")
-        print(f"Level                : {self.lev}")
-        print(f"Explanatory variables: {', '.join(self.evar)}")
-        print(f"Null hyp.: there is no effect x on {self.rvar}")
-        print(f"Alt. hyp.: there is an effect of x on {self.rvar}")
-
-        df = self.coef.copy()
-        df["OR"] = df["OR"].round(dec)
-        df["coefficient"] = df["coefficient"].round(2)
-        df["std.error"] = df["std.error"].round(dec)
-        df["z.value"] = df["z.value"].round(dec)
-        df["p.value"] = ifelse(
-            df["p.value"] < 0.001, "< .001", df["p.value"].round(dec)
-        )
-        df["OR%"] = [f"{round(o, max(dec-2, 0))}%" for o in df["OR%"]]
-        print(f"\n{df.to_string(index=False)}")
-        print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
-        print(f"\n{model_fit(self.fitted)}")
-
-    def ci(self, alpha=0.05, intercept=False, dec=3) -> None:
-        """
-        Confidence intervals for Odds Ratios
-        """
-        print(
-            f"\n{or_ci(self.fitted, alpha=alpha, intercept=intercept).to_string(index=False)}"
+from shiny import App, render, ui, reactive, Inputs, Outputs, Session
+import webbrowser, nest_asyncio, uvicorn
+import io
+import pyrsm as rsm
+from contextlib import redirect_stdout, redirect_stderr
+import pyrsm.radiant.utils as ru
+
+
+def ui_summary():
+    return (
+        ui.panel_conditional(
+            "input.tabs == 'Summary'",
+            ui.panel_well(
+                ui.output_ui("ui_var"),
+                ui.input_select(
+                    id="alt_hyp",
+                    label="Alternative hypothesis:",
+                    selected="two-sided",
+                    choices={
+                        "two-sided": "Two sided",
+                        "greater": "Greater than",
+                        "less": "Less than",
+                    },
+                ),
+                ui.input_slider(
+                    id="conf",
+                    label="Confidence level:",
+                    min=0,
+                    max=1,
+                    value=0.95,
+                ),
+                ui.input_numeric(
+                    id="comp_value",
+                    label="Comparison value:",
+                    value=0,
+                ),
+            ),
+        ),
+    )
+
+
+choices = {
+    "None": "None",
+    "hist": "Histogram",
+    "sim": "Simulate",
+}
+
+
+class basics_single_mean:
+    def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
+        ru.init(self, datasets, descriptions=descriptions, open=open)
+
+    def shiny_ui(self):
+        return ui.page_navbar(
+            ru.head_content(),
+            ui.nav(
+                "Basics > Single mean",
+                ui.row(
+                    ui.column(
+                        3,
+                        ru.ui_data(self),
+                        ui_summary(),
+                        ru.ui_plot(choices),
+                    ),
+                    ui.column(8, ru.ui_main_basics()),
+                ),
+            ),
+            ru.ui_help(
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-single-mean.ipynb",
+                "Single mean example notebook",
+            ),
+            ru.ui_stop(),
+            title="Radiant for Python",
+            inverse=True,
+            id="navbar_id",
         )
 
-    def plot(
-        self,
-        plots="or",
-        alpha=0.05,
-        intercept=False,
-        incl=None,
-        excl=None,
-        incl_int=[],
-        fix=True,
-        hline=False,
-        figsize=None,
-    ) -> None:
-        """
-        Plots for a logistic regression model
-        """
-        if "or" in plots:
-            or_plot(
-                self.fitted,
-                alpha=alpha,
-                intercept=intercept,
-                incl=incl,
-                excl=excl,
-                figsize=figsize,
-            )
-        if "pred" in plots:
-            pred_plot_sm(
-                self.fitted,
-                self.dataset,
-                incl=incl,
-                excl=[],
-                incl_int=incl_int,
-                fix=fix,
-                hline=hline,
-                nnv=20,
-                minq=0.025,
-                maxq=0.975,
+    def shiny_server(self, input: Inputs, output: Outputs, session: Session):
+        # --- section standard for all apps ---
+        get_data, stop_app = ru.standard_reactives(self, input, session)
+        ru.make_data_outputs(self, input, output)
+
+        # --- section unique to each app ---
+        @output(id="ui_var")
+        @render.ui
+        def ui_var():
+            isNum = get_data()["var_types"]["isNum"]
+            return ui.input_select(
+                id="var",
+                label="Variable (select one)",
+                selected=None,
+                choices=isNum,
             )
-        if "vimp" in plots:
-            vimp_plot_sm(self.fitted, self.dataset, rep=10, ax=None, ret=False)
+
+        def estimation_code():
+            data_name, code = (get_data()[k] for k in ["data_name", "code"])
+
+            args = {
+                "data": f"""{{"{data_name}": {data_name}}}""",
+                "var": input.var(),
+                "alt_hyp": input.alt_hyp(),
+                "conf": input.conf(),
+                "comp_value": input.comp_value(),
+            }
+
+            args_string = ru.drop_default_args(args, rsm.basics.single_mean)
+            return f"""rsm.basics.single_mean({args_string})""", code
+
+        def show_code():
+            sc = estimation_code()
+            return f"""{sc[1]}\nsm = {sc[0]}"""
+
+        @reactive.Calc
+        def single_mean():
+            locals()[input.datasets()] = self.datasets[
+                input.datasets()
+            ]  # get data into local scope
+            return eval(estimation_code()[0])
+
+        def summary_code():
+            return f"""sm.summary()"""
+
+        @output(id="show_summary_code")
+        @render.text
+        def show_summary_code():
+            cmd = f"""{show_code()}\n{summary_code()}"""
+            return ru.code_formatter(cmd, self)
+
+        @output(id="summary")
+        @render.text
+        def summary():
+            out = io.StringIO()
+            with redirect_stdout(out), redirect_stderr(out):
+                sm = single_mean()  # get the reactive object into local scope
+                sm.summary()
+            return out.getvalue()
+
+        def plot_code():
+            return f"""sm.plot("{input.plots()}")"""
+
+        @output(id="show_plot_code")
+        @render.text
+        def show_plot_code():
+            plots = input.plots()
+            if plots != "None":
+                cmd = f"""{show_code()}\n{plot_code()}"""
+                return ru.code_formatter(cmd, self)
+
+        @output(id="plot")
+        @render.plot
+        def plot():
+            plots = input.plots()
+            if plots != "None":
+                sm = single_mean()  # get reactive object into local scope
+                cmd = f"""{plot_code()}"""
+                return eval(cmd)
+
+
+def single_mean(
+    data_dct: dict,
+    descriptions_dct: dict = None,
+    open: bool = True,
+    host: str = "0.0.0.0",
+    port: int = 8000,
+    log_level: str = "warning",
+):
+    """
+    Launch a Radiant-for-Python app for single_mean hypothesis testing
+    """
+    rc = basics_single_mean(data_dct, descriptions_dct, open)
+    nest_asyncio.apply()
+    webbrowser.open(f"http://{host}:{port}")
+    print(f"Listening on http://{host}:{port}")
+    print(
+        "Pyrsm and Radiant are open source tools and free to use. If you\nare a student or instructor using pyrsm or Radiant for a class,\nas a favor to the developers, please send an email to\n<radiant@rady.ucsd.edu> with the name of the school and class."
+    )
+    uvicorn.run(
+        App(rc.shiny_ui(), rc.shiny_server),
+        host=host,
+        port=port,
+        log_level=log_level,
+    )
+
+
+if __name__ == "__main__":
+    import pyrsm as rsm
+
+    demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
+    single_mean(
+        {"demand_uk": demand_uk}, {"demand_uk": demand_uk_description}, open=True
+    )
```

### Comparing `pyrsm-0.8.4.1/pyrsm/model.py` & `pyrsm-0.8.5/pyrsm/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -285,29 +285,31 @@
 
     if dec is not None:
         df = df.round(dec)
 
     return df
 
 
-def predict_ci(fitted, df, alpha=0.05):
+def predict_ci(fitted, df, conf=0.95, alpha=None):
     """
     Compute predicted probabilities with confidence intervals based on a
     logistic regression model
 
     Parameters
     ----------
     fitted : Logistic regression model fitted using the statsmodels formula interface
     df : Pandas dataframe with input data for prediction
+    conf : float
+        Confidence level (0-1). Default is 0.95
     alpha : float
         Significance level (0-1). Default is 0.05
 
     Returns
     -------
-    Pandas dataframe with probability predictions and lower and upper confidence bounds
+    Pandas DataFrame with probability predictions and lower and upper confidence bounds
 
     Example
     -------
     import numpy as np
     import statsmodels.formula.api as smf
     import pandas as pd
 
@@ -326,49 +328,58 @@
     plt.clf()
     plt.plot(x1, pred["prediction"])
     plt.plot(x1, pred["2.5%"], color='black', linestyle="--", linewidth=0.5)
     plt.plot(x1, pred["97.5%"], color='black', linestyle="--", linewidth=0.5)
     plt.show()
     """
 
-    if alpha < 0 or alpha > 1:
-        raise ValueError("alpha must be a numeric value between 0 and 1")
+    if conf < 0 or conf > 1:
+        raise ValueError(
+            "Confidence level (conf) must be a numeric value between 0 and 1"
+        )
+
+    if alpha is not None:
+        raise ValueError(
+            "The alpha argument has been deprecated. Use the confidence level (conf) instead (1-alpha)."
+        )
 
     # generate predictions
     prediction = fitted.predict(df)
 
     # set up the data in df in the same was as the exog data
     # that is part of fitted.model.exog
     # use a fake response variable
     df = df.assign(__rvar__=1).copy()
     form = "__rvar__ ~ " + fitted.model.formula.split("~", 1)[1]
     exog = smf.logit(formula=form, data=df).exog
 
-    low, high = [alpha / 2, 1 - (alpha / 2)]
+    low, high = [(1.0 - conf) / 2.0, (1.0 - (1.0 - conf) / 2.0)]
     Xb = np.dot(exog, fitted.params)
     se = np.sqrt((exog.dot(fitted.cov_params()) * exog).sum(-1))
     me = stats.norm.ppf(high) * se
 
     if isinstance(fitted, sm.genmod.generalized_linear_model.GLMResultsWrapper):
         return pd.DataFrame(
             {
                 "prediction": prediction,
-                f"{low*100}%": expit(Xb - me),
-                f"{high*100}%": expit(Xb + me),
+                f"{low*100:.2f}%": expit(Xb - me),
+                f"{high*100:.2f}%": expit(Xb + me),
             }
         )
     elif isinstance(fitted, sm.regression.linear_model.RegressionResultsWrapper):
         return pd.DataFrame(
-            {"prediction": prediction, f"{low*100}%": Xb - me, f"{high*100}%": Xb + me}
+            {
+                "prediction": prediction,
+                f"{low*100:.2f}%": Xb - me,
+                f"{high*100:.2f}%": Xb + me,
+            }
         )
 
 
-def model_fit(
-    fitted, dec: int = 3, prn: bool = True, shiny=False
-) -> Union[str, pd.DataFrame]:
+def model_fit(fitted, dec: int = 3, prn: bool = True) -> Union[str, pd.DataFrame]:
     """
     Compute various model fit statistics for a fitted linear or logistic regression model
 
     Parameters
     ----------
     fitted : statmodels ols or glm object
         Regression model fitted using statsmodels
@@ -403,18 +414,15 @@
 Nr obs: {mfit.nobs.values[0]:,.0f}"""
         elif model_type == "regression":
             output = f"""R-squared: {mfit.rsq.values[0].round(dec)}, Adjusted R-squared: {mfit.rsq_adj.values[0].round(dec)}
 F-statistic: {mfit.fvalue[0].round(dec)} df({mfit.ftest_df_model.values[0]:.0f}, {mfit.ftest_df_resid.values[0]:.0f}), p.value {np.where(mfit.ftest_pval.values[0] < .001, "< 0.001", mfit.ftest_pval.values[0].round(dec))}
 Nr obs: {mfit.nobs.values[0]:,.0f}"""
         else:
             output = "Model type not supported"
-        if shiny:
-            return output
-        else:
-            print(output)
+        return output
     else:
         return mfit
 
 
 def coef_plot(
     fitted,
     alpha: float = 0.05,
```

### Comparing `pyrsm-0.8.4.1/pyrsm/notebook.py` & `pyrsm-0.8.5/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/perf.py` & `pyrsm-0.8.5/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/props.py` & `pyrsm-0.8.5/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/radiant/www/returnTextAreaBinding.js` & `pyrsm-0.8.5/pyrsm/radiant/www/returnTextAreaBinding.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/regress.py` & `pyrsm-0.8.5/pyrsm/logistic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,272 +1,262 @@
+from typing import Union, Optional
+import re
 import pandas as pd
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib.ticker as ticker
+import statsmodels as sm
+from statsmodels.genmod.families import Binomial
+from statsmodels.genmod.families.links import logit
 import statsmodels.formula.api as smf
-from typing import Optional
-from statsmodels.regression.linear_model import RegressionResults as rrs
-from shiny import App
-from .radiant.regress import model_regress
-from .utils import ifelse, format_nr, setdiff
-from .visualize import pred_plot_sm, vimp_plot_sm
-from .model import (
-    sig_stars,
-    model_fit,
-    extract_evars,
-    extract_rvar,
-    scatter_plot,
-    reg_dashboard,
-    residual_plot,
-    coef_plot,
-    coef_ci,
-    predict_ci,
-)
+from statsmodels.stats.outliers_influence import variance_inflation_factor
+from scipy import stats
+from scipy.special import expit
+from .utils import ifelse, setdiff, odir
+from .stats import weighted_mean, weighted_sd
+from .perf import auc
+from .model import sig_stars, model_fit, or_ci, or_plot, sim_prediction
 from .model import vif as calc_vif
-from .visualize import distr_plot
-from .basics import correlation
 
+# from statsmodels.regression.linear_model import RegressionResults as rrs
+from .visualize import pred_plot_sm, vimp_plot_sm, extract_evars, extract_rvar
 
-class regress:
+
+class logistic:
     def __init__(
         self,
-        dataset: pd.DataFrame,
+        data,
         rvar: Optional[str] = None,
+        lev: Optional[str] = None,
         evar: Optional[list[str]] = None,
-        int: Optional[list[str]] = None,
+        ivar: Optional[list[str]] = None,
         form: Optional[str] = None,
     ) -> None:
-
         """
-        Estimate linear regression model
+        Initialize logistic regression model
 
         Parameters
         ----------
         dataset: pandas DataFrame; dataset
         evar: List of strings; contains the names of the columns of data to be used as explanatory variables
+        lev: String; name of the level in the response variable
         rvar: String; name of the column to be used as the response variable
         form: String; formula for the regression equation to use if evar and rvar are not provided
         """
-        self.dataset = dataset
+        if isinstance(data, dict):
+            self.name = list(data.keys())[0]
+            self.data = data[self.name].copy()  # needed with pandas
+        else:
+            self.data = data.copy()  # needed with pandas
+            self.name = "Not provided"
         self.rvar = rvar
+        self.lev = lev
         self.evar = ifelse(isinstance(evar, str), [evar], evar)
-        self.int = ifelse(isinstance(int, str), [int], int)
+        self.ivar = ifelse(isinstance(ivar, str), [ivar], ivar)
         self.form = form
 
+        if self.lev is not None and self.rvar is not None:
+            self.data[self.rvar] = (self.data[self.rvar] == lev).astype(int)
+
         if self.form:
-            self.fitted = smf.ols(formula=self.form, data=self.dataset).fit()
-            self.evar = extract_evars(self.fitted.model, self.dataset.columns)
-            self.rvar = extract_rvar(self.fitted.model, self.dataset.columns)
+            self.fitted = smf.glm(
+                formula=self.form, data=self.data, family=Binomial(link=logit())
+            ).fit()
+            self.evar = extract_evars(self.fitted.model, self.data.columns)
+            self.rvar = extract_rvar(self.fitted.model, self.data.columns)
+            if self.lev is None:
+                self.lev = self.data.at[0, self.rvar]
         else:
-            self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
-            if self.int:
-                self.form += f" + {' + '.join(self.int)}"
-            self.fitted = smf.ols(self.form, data=self.dataset).fit()
-
-        df = pd.DataFrame(self.fitted.params, columns=["coefficient"]).dropna()
+            if self.evar is None or len(self.evar) == 0:
+                self.form = f"{self.rvar} ~ 1"
+            else:
+                self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
+            if self.ivar:
+                self.form += f" + {' + '.join(self.ivar)}"
+            self.fitted = smf.glm(
+                formula=self.form, data=self.data, family=Binomial(link=logit())
+            ).fit()
+        df = pd.DataFrame(np.exp(self.fitted.params), columns=["OR"]).dropna()
+        df["OR%"] = 100 * ifelse(df["OR"] < 1, -(1 - df["OR"]), df["OR"] - 1)
+        df["coefficient"] = self.fitted.params
         df["std.error"] = self.fitted.params / self.fitted.tvalues
-        df["t.value"] = self.fitted.tvalues
+        # wierd but this is what statsmodels uses in summary
+        df["z.value"] = self.fitted.tvalues
         df["p.value"] = self.fitted.pvalues
         df["  "] = sig_stars(self.fitted.pvalues)
         self.coef = df.reset_index()
 
-    def summary(
-        self,
-        ssq=False,
-        vif=False,
-        ci=False,
-        test=None,
-        dec=3,
-        name="Not provided",
-        shiny=False,
-    ) -> None:
+    def summary(self, ci=False, vif=False, test=None, dec=3) -> None:
         """
-        Summarize output from a linear regression model
-
-        parameters
-        ----------
-        ssq: Boolean; if True, include sum of squares
-        vif: Boolean; if True, include variance inflation factors
+        Summarize output from a logistic regression model
         """
-        print("Linear regression (OLS)")
-        print("Data                 :", name)
-        print("Response variable    :", self.rvar)
-        print("Explanatory variables:", ", ".join(self.evar))
-        print(f"Null hyp.: the effect of x on {self.rvar} is zero")
-        print(f"Alt. hyp.: the effect of x on {self.rvar} is not zero")
+        print("Logistic regression (GLM)")
+        print(f"Data                 : {self.name}")
+        print(f"Response variable    : {self.rvar}")
+        print(f"Level                : {self.lev}")
+        print(f"Explanatory variables: {', '.join(self.evar)}")
+        print(f"Null hyp.: There is no effect of x on {self.rvar}")
+        print(f"Alt. hyp.: There is an effect of x on {self.rvar}")
 
         df = self.coef.copy()
+        df["OR"] = df["OR"].round(dec)
         df["coefficient"] = df["coefficient"].round(2)
         df["std.error"] = df["std.error"].round(dec)
-        df["t.value"] = df["t.value"].round(dec)
+        df["z.value"] = df["z.value"].round(dec)
         df["p.value"] = ifelse(
             df["p.value"] < 0.001, "< .001", df["p.value"].round(dec)
         )
+        df["OR%"] = [f"{round(o, max(dec-2, 0))}%" for o in df["OR%"]]
+
         df = df.set_index("index")
         df.index.name = None
         print(f"\n{df.to_string()}")
         print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
-        print(f"\n{model_fit(self.fitted, shiny=shiny)}")
+        print(f"\n{model_fit(self.fitted)}")
 
         if ci:
             print("\nConfidence intervals:")
-            print(f"\n{coef_ci(self.fitted).to_string()}")
-
-        if ssq:
-            print("\nSum of squares:")
-            index = ["Regression", "Error", "Total"]
-            sum_of_squares = [
-                self.fitted.ess,
-                self.fitted.ssr,
-                self.fitted.centered_tss,
-            ]
-            sum_of_squares = pd.DataFrame(index=index).assign(
-                df=format_nr(
-                    [
-                        self.fitted.df_model,
-                        self.fitted.df_resid,
-                        self.fitted.df_model + self.fitted.df_resid,
-                    ],
-                    dec=0,
-                ),
-                SS=format_nr(sum_of_squares, dec=0),
-            )
-            print(f"\n{sum_of_squares.to_string()}")
+            df = or_ci(self.fitted).set_index("index")
+            df.index.name = None
+            print(f"\n{df.to_string()}")
 
         if vif:
-            print("\nVariance inflation factors:")
-            print(f"\n{calc_vif(self.fitted).to_string()}")
-
-        if test is not None and len(test) > 0:
-            evar = setdiff(self.evar, test)
-            if self.int is not None and len(self.int) > 0:
-                sint = [
-                    s for s in self.int for t in test if f"I({t}" in s or t not in s
-                ]
+            if self.evar is None or len(self.evar) < 2:
+                print("\nVariance Inflation Factors cannot be calculated")
             else:
-                sint = []
+                print("\nVariance inflation factors:")
+                print(f"\n{calc_vif(self.fitted).to_string()}")
 
-            form = f"{self.rvar} ~ "
-            if len(evar) == 0 and len(sint) == 0:
-                form += "1"
-            else:
-                # if len(evar) > 0:
-                # form += f"{' + '.join(evar)}"
-                # if len(sint) > 0:
-                form += f"{' + '.join(evar + sint)}"
-
-                ###### need to keep I(carat**2) in the formula even if carat is in test ######
-
-                # if self.int is not None and len(self.int) > 0:
-                #     sint = [
-                #         s for s in self.int for t in test if f"I({t}" in s or t not in s
-                #     ]
-                #     if len(sint) > 0:
-                #         form += f" + {' + '.join(sint)}"
-
-            hypothesis = [
-                f"({c} = 0)"
-                for c in self.fitted.model.exog_names
-                for v in test
-                if f"{v}:" in c or f":{v}" in c or f"{v}[T." in c or v == c
-            ]
-            print(hypothesis)
-
-            print(f"\nModel 1: {form}")
-            print(f"Model 2: {self.form}")
-            out = self.fitted.f_test(hypothesis)
-            pvalue = ifelse(out.pvalue < 0.001, "< .001", round(out.pvalue, dec))
-            print(
-                f"F-statistic: {round(out.fvalue, dec)} df ({out.df_num:.0f}, {out.df_denom:.0f}), p.value {pvalue}"
-            )
+        if test is not None and len(test) > 0:
+            self.chisq_test(test=test, dec=dec)
 
-    def predict(self, df=None, ci=False, alpha=0.05) -> pd.DataFrame:
+    def predict(self, df=None, cmd=None, dc=False, ci=False, conf=0.95) -> pd.DataFrame:
         """
         Predict values for a linear regression model
         """
         if df is None:
-            df = self.dataset
+            df = self.data
         df = df.loc[:, self.evar].copy()
+        if cmd is not None:
+            if dc:
+                for k, v in cmd.items():
+                    df[k] = v
+            else:
+                df = sim_prediction(df=df, vary=cmd)
+
         if ci:
-            return pd.concat([df, predict_ci(self.fitted, df, alpha=alpha)], axis=1)
+            if dc:
+                raise ValueError(
+                    "Confidence intervals not available when using the Data & Command option"
+                )
+            else:
+                return pd.concat([df, predict_ci(self.fitted, df, conf=conf)], axis=1)
         else:
             pred = pd.DataFrame().assign(prediction=self.fitted.predict(df))
             return pd.concat([df, pred], axis=1)
 
     def plot(
         self,
-        plots="dist",
-        nobs: int = 1000,
-        intercept=False,
+        plots="or",
         alpha=0.05,
+        intercept=False,
         incl=None,
-        excl=[],
+        excl=None,
         incl_int=[],
         fix=True,
         hline=False,
         figsize=None,
     ) -> None:
         """
-        Plots for a linear regression model
+        Plots for a logistic regression model
         """
-        dataset = self.dataset[[self.rvar] + self.evar].copy()
-        if "dist" in plots:
-            distr_plot(dataset)
-        if "corr" in plots:
-            cr = correlation(dataset)
-            cr.plot(nobs=nobs, figsize=figsize)
-        if "scatter" in plots:
-            scatter_plot(self.fitted, dataset, nobs=nobs, figsize=figsize)
-        if "dashboard" in plots:
-            reg_dashboard(self.fitted, nobs=nobs)
-        if "residual" in plots:
-            residual_plot(self.fitted, dataset, nobs=nobs, figsize=figsize)
+        if "or" in plots:
+            or_plot(
+                self.fitted,
+                alpha=alpha,
+                intercept=intercept,
+                incl=incl,
+                excl=excl,
+                figsize=figsize,
+            )
         if "pred" in plots:
             pred_plot_sm(
                 self.fitted,
-                self.dataset,
+                self.data,
                 incl=incl,
-                excl=excl,
+                excl=[],
                 incl_int=incl_int,
                 fix=fix,
                 hline=hline,
                 nnv=20,
                 minq=0.025,
                 maxq=0.975,
             )
         if "vimp" in plots:
-            vimp_plot_sm(self.fitted, self.dataset, rep=10, ax=None, ret=False)
-        if "coef" in plots:
-            coef_plot(
-                self.fitted,
-                alpha=alpha,
-                intercept=intercept,
-                incl=incl,
-                excl=excl,
-                figsize=figsize,
-            )
+            vimp_plot_sm(self.fitted, self.data, rep=10, ax=None, ret=False)
 
-    def f_test(self, vtt=None, dec=3) -> None:
+    def chisq_test(self, test=None, dec=3) -> None:
         """
-        F-test for competing models
+        Chisq-test for competing models
 
         Parameters
         ----------
-        vtt : list
+        test : list
             List of strings; contains the names of the columns of data to be tested
         """
-        if vtt is None:
-            form = f"{self.rvar} ~ 1"
-            vtt = self.evar.copy()
+        evar = setdiff(self.evar, test)
+        if self.ivar is not None and len(self.ivar) > 0:
+            sint = setdiff(self.ivar, test)
+            test += [s for t in test for s in sint if f"I({t}" not in s and t in s]
+            sint = setdiff(sint, test)
         else:
-            evar = setdiff(self.evar, vtt)
-            if len(evar) == 0:
-                form = f"{self.rvar} ~ 1"
-            else:
-                form = f"{self.rvar} ~ {' + '.join(evar)}"
+            sint = []
 
-        vtt = ifelse(isinstance(vtt, str), [vtt], vtt)
-        hypothesis = [f"({v} = 0)" for v in vtt]
-        print(f"Model 1: {form}")
-        print(f"Model 2: {self.form}")
-        out = self.fitted.f_test(hypothesis)
-        pvalue = ifelse(out.pvalue < 0.001, "< .001", round(out.pvalue, dec))
-        print(
-            f"F-statistic: {round(out.fvalue, dec)} df ({out.df_num:,.0f}, {out.df_denom:,.0f}), p.value {pvalue}"
+        form = f"{self.rvar} ~ "
+        if len(evar) == 0 and len(sint) == 0:
+            form += "1"
+        else:
+            form += f"{' + '.join(evar + sint)}"
+
+        # ensure constraints are unique
+        pattern = r"(\[T\.[^\]]*\])\:"
+        hypotheses = list(
+            set(
+                [
+                    f"({c} = 0)"
+                    for c in self.fitted.model.exog_names
+                    for v in test
+                    if f"{v}:" in c
+                    or f":{v}" in c
+                    or f"{v}[T." in c
+                    or v == c
+                    or v == re.sub(pattern, ":", c)
+                ]
+            )
         )
+
+        print(f"\nModel 1: {form}")
+        print(f"Model 2: {self.form}")
+
+        # Wald test (faster but not as accurate)
+        # out = self.fitted.wald_test(hypotheses, scalar=True)
+        # pvalue = ifelse(out.pvalue < 0.001, "< .001", round(out.pvalue, dec))
+        # print(
+        #     f"Chi-squared: {round(out.statistic, dec)} df ({out.df_denom:.0f}), p.value {pvalue}"
+        # )
+
+        # LR test of competing models (slower but more accurate)
+        sub_fitted = smf.glm(
+            formula=form, data=self.data, family=Binomial(link=logit())
+        ).fit()
+
+        lrtest = -2 * (sub_fitted.llf - self.fitted.llf)
+        df = self.fitted.df_model - sub_fitted.df_model
+        pvalue = stats.chi2.sf(lrtest, df)
+
+        # calculate pseudo R-squared values for both models
+        pr2_full = 1 - self.fitted.llf / self.fitted.llnull
+        pr2_sub = 1 - sub_fitted.llf / sub_fitted.llnull
+
+        print(f"Pseudo R-squared, Model 1 vs 2: {pr2_sub:.3f} vs {pr2_full:.3f}")
+        pvalue = ifelse(pvalue < 0.001, "< .001", round(pvalue, dec))
+        print(f"Chi-squared: {round(lrtest, dec)} df ({df:.0f}), p.value {pvalue}")
```

### Comparing `pyrsm-0.8.4.1/pyrsm/stats.py` & `pyrsm-0.8.5/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/pyrsm/utils.py` & `pyrsm-0.8.5/pyrsm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import numpy as np
 import pandas as pd
-from scipy import stats
-import inspect as ins
+import inspect
 from itertools import product
 from datetime import date, datetime
 from math import ceil
 from IPython.display import display, Markdown
 from sys import modules
 import json
 
 
 def add_description(df, md="", path=""):
     """
-    Add a description to a Pandas dataframe in markdown format
+    Add a description to a Pandas DataFrame in markdown format
 
     Parameters
     ----------
-    df : Pandas dataframe
+    df : Pandas DataFrame
     md : str
         Data description in markdown format
     path : str
         Path to a text file with the data description in markdown format
 
     Returns
     -------
-    Pandas dataframe with added description
+    Pandas DataFrame with added description
     """
 
     if path != "":
         f = open(path, "r")
         md = f.read()
         f.close()
     elif md == "":
@@ -38,15 +37,15 @@
     df._metadata.append("description")
     df.description = md
     return df
 
 
 def describe(df, prn=True):
     """
-    Print out Pandas dataframe description attribute if available. Else use Pandas'
+    Print out Pandas DataFrame description attribute if available. Else use Pandas'
     description method to provide summary statistics
     """
     if hasattr(df, "description"):
         if "ipykernel" in modules and prn:
             display(Markdown(df.description))
         elif prn:
             print(df.description)
@@ -408,15 +407,15 @@
 
     Examples
     --------
     odir(["a"])
     """
     mth = []
     attr = []
-    for i in ins.getmembers(obj):
+    for i in inspect.getmembers(obj):
         if private or not i[0].startswith("_"):
-            if ins.ismethod(i[1]) or ins.isbuiltin(i[1]):
+            if inspect.ismethod(i[1]) or inspect.isbuiltin(i[1]):
                 mth.append(i[0])
             else:
                 attr.append(i[0])
 
     return {"methods": mth, "attributes": attr}
```

### Comparing `pyrsm-0.8.4.1/pyrsm/visualize.py` & `pyrsm-0.8.5/pyrsm/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     incl_int=[],
     fix=True,
     hline=False,
     nnv=20,
     minq=0.025,
     maxq=0.975,
 ):
+
     """
     Generate prediction plots for statsmodels regression models (OLS and Logistic).
     A faster alternative to PDP plots.
 
     Parameters
     ----------
     fitted : A fitted (logistic) regression model
@@ -267,19 +268,19 @@
     elif nr_plots % 2 == 1:
         ax[-1, -1].remove()
 
 
 def pred_plot_sk(
     fitted,
     df,
-    transformed=None,
     rvar=None,
     incl=None,
     excl=[],
     incl_int=[],
+    transformed=None,
     fix=True,
     hline=False,
     nnv=20,
     minq=0.025,
     maxq=0.975,
 ):
     """
@@ -287,23 +288,23 @@
     that can handle interaction plots with categorical variables
 
     Parameters
     ----------
     fitted : A fitted sklearn model
     df : Pandas DataFrame with data used for estimation. Should include categorical variables
         in their original form (i.e., before using get_dummies)
-    transformed : List of column names that were transformed using Pandas' get_dummies. If
-        None, the function will try to determine which variables might have been transformed
     rvar : The column name for the response/target variable
     incl : A list of column names to generate prediction plots for. If None, all
         variables will be plotted
     excl : A list of column names to exclude from plotting
     incl_int : A list is ":" separated column names to plots interaction plots for.
         For example incl_int = ["a:b", "b:c"] would generate interaction plots for
         variables a x b and b x c
+    transformed : List of column names that were transformed using Pandas' get_dummies. If
+        None, the function will try to determine which variables might have been transformed
     fix : Logical or tuple
         Set the desired limited on yhat or have it calculated automatically.
         Set to False to have y-axis limits set by ggplot2 for each plot
     hline : Logical or float
         Add a horizontal line at the average of the target variable. When set to False
         no line is added. When set to a specific number, the horizontal line will be
         added at that value
@@ -311,15 +312,20 @@
         The number of values to use in simulation for numeric variables
     minq : float
         Quantile to use for the minimum value of numeric variables
     maxq : float
         Quantile to use for the maximum value of numeric variables
     """
     # features names used in the sklearn model
-    fn = fitted.feature_names_in_
+    if hasattr(fitted, "feature_names_in_"):
+        fn = fitted.feature_names_in_
+    else:
+        raise Exception(
+            "This function requires a fitted sklearn model with a named features. If you are using one-hot encoding, please use get_dummies on your dataset before fitting the model."
+        )
 
     not_transformed = [c for c in df.columns for f in fn if c == f]
     if transformed is None:
         transformed = list(
             set(
                 [
                     c
@@ -355,15 +361,17 @@
     if incl is None:
         incl = not_transformed + transformed
     else:
         incl = ifelse(isinstance(incl, str), [incl], incl)
 
     def dummify(df, trs):
         if len(trs) > 0:
-            return pd.concat([pd.get_dummies(df[trs]), df.drop(trs, axis=1)], axis=1)
+            return pd.concat(
+                [pd.get_dummies(df[trs], columns=trs), df.drop(trs, axis=1)], axis=1
+            )
         else:
             return df
 
     # margin to add above and below in plots
     plot_margin = 0.025
 
     if isinstance(hline, bool):
```

### Comparing `pyrsm-0.8.4.1/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.5/pyrsm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.4.1
+Version: 0.8.5
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.4.1/setup.cfg` & `pyrsm-0.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.4.1/tests/test_basics.py` & `pyrsm-0.8.5/tests/test_basics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from pyrsm.basics import correlation, cross_tabs
+from pyrsm.basics.correlation import correlation
+from pyrsm.basics.cross_tabs import cross_tabs
 import numpy as np
 import pandas as pd
 
 df = pd.DataFrame({"x": [0, 1, 1, 1, 0, 0, 0], "y": [2, 1, 1, 1, 2, 2, 10]})
 
 # ct.expected.iloc[0, :].round(6) == [1.714286, 1.714286, 0.571429, 4.0000]
 
@@ -17,7 +18,12 @@
 
 
 def test_crosstab():
     ct = cross_tabs(df, "x", "y")
     assert all(
         ct.expected.iloc[0, :].round(6) == [1.714286, 1.714286, 0.571429, 4.0000]
     ), "Cross tab expected values incorrect"
+
+
+if __name__ == "__main__":
+    test_correlation()
+    test_crosstab()
```

### Comparing `pyrsm-0.8.4.1/tests/test_bins.py` & `pyrsm-0.8.5/tests/test_bins.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,7 +31,14 @@
     x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, np.NaN])
     breaks = np.quantile(x[np.isnan(x) == False], np.array(range(0, 6)) / 5)
     bins = bincode(x, breaks)
     assert all(
         bins[:9] == np.array([1, 1, 2, 2, 3, 4, 4, 5, 5])
     ), "Incorrect bins with NaN returned"
     assert np.isnan(bins[-1]), "No missing value returned"
+
+
+if __name__ == "__main__":
+    test_xtile()
+    test_xtile_rev()
+    test_xtile_nan()
+    test_bincode_nan()
```

### Comparing `pyrsm-0.8.4.1/tests/test_perf.py` & `pyrsm-0.8.5/tests/test_perf.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,7 +91,23 @@
 
 def test_rome_plot_single():
     fig = ROME_plot(df, "response", "yes", "x1", qnt=10)
 
 
 def test_ROME_plot_mult():
     fig = ROME_plot(df, "response", "yes", ["x1", "x2"], qnt=10)
+
+
+if __name__ == "__main__":
+    test_calc_qnt()
+    test_calc_qnt_rev()
+    test_gains_tab()
+    test_lift_tab()
+    test_evalbin()
+    test_lift_plot_single()
+    test_lift_plot_mult()
+    test_gains_plot_single()
+    test_gains_plot_mult()
+    test_profit_plot_single()
+    test_profit_plot_mult()
+    test_rome_plot_single()
+    test_ROME_plot_mult()
```

### Comparing `pyrsm-0.8.4.1/tests/test_regression.py` & `pyrsm-0.8.5/tests/test_regression.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,7 +15,11 @@
 # sim_prediction(df, vary="x1", minq=0, maxq=1)
 # sim_prediction(df, vary="x1")
 
 
 def test_sim_prediction():
     ret = sim_prediction(df)
     assert ret.loc[0, "x3"] == "b", "Incorrectly generated simulated data"
+
+
+if __name__ == "__main__":
+    test_sim_prediction()
```

### Comparing `pyrsm-0.8.4.1/tests/test_stats.py` & `pyrsm-0.8.5/tests/test_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,16 @@
 # def test_correlation():
 #     cr, cp = correlation(df, prn=False)
 #     assert cr[1, 0].round(3) == -0.493, "Correlations incorrect"
 #     df_nan = df.copy()
 #     df_nan.loc[4, "x"] = np.NaN
 #     cr, cp = correlation(df_nan, prn=False)
 #     assert cr[1, 0].round(3) == -0.567, "Correlations with np.NaN incorrect"
+
+if __name__ == "__main__":
+    test_varprop()
+    test_seprop()
+    test_weighted_mean()
+    test_weighted_sd()
+    test_scale_df()
+    test_weighted_scale_df()
+    # test_correlation()
```

### Comparing `pyrsm-0.8.4.1/tests/test_utils.py` & `pyrsm-0.8.5/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,7 +75,20 @@
 
 def test_union():
     assert union(["a", "b", "c"], ["b", "x"]) == ["a", "b", "c", "x"], "Union incorrect"
 
 
 def test_intersect():
     assert intersect(["a", "b", "c"], ["b", "x"]) == ["b"], "Union incorrect"
+
+
+if __name__ == "__main__":
+    test_add_description()
+    test_ifelse_true()
+    test_ifelse_false()
+    test_ifelse_array()
+    test_level_list()
+    test_expand_grid()
+    test_table2data()
+    test_setdiff()
+    test_union()
+    test_intersect()
```

