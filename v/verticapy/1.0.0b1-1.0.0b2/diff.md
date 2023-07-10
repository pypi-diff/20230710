# Comparing `tmp/verticapy-1.0.0b1.tar.gz` & `tmp/verticapy-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verticapy-1.0.0b1.tar", last modified: Tue Jun 20 21:34:24 2023, max compression
+gzip compressed data, was "verticapy-1.0.0b2.tar", last modified: Mon Jul 10 13:16:57 2023, max compression
```

## Comparing `verticapy-1.0.0b1.tar` & `verticapy-1.0.0b2.tar`

### file list

```diff
@@ -1,578 +1,581 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    19328 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.361272 verticapy-1.0.0b1/verticapy/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3693 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.361272 verticapy-1.0.0b1/verticapy/_config/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_config/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6293 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_config/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_config/validators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3917 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2160 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.361272 verticapy-1.0.0b1/verticapy/_utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12398 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_display.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1680 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    73985 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_logo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4401 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1758 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_object.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2292 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.365272 verticapy-1.0.0b1/verticapy/_utils/_sql/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3787 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_cast.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_check.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5564 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_collect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3847 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_dblink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1797 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_display.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_format.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9319 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_merge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_random.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2652 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_sys.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4935 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/_utils/_sql/_vertica_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.365272 verticapy-1.0.0b1/verticapy/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/connection/connect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/connection/external.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/connection/global_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5113 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/connection/read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1734 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/connection/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5715 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/connection/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.365272 verticapy-1.0.0b1/verticapy/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.365272 verticapy-1.0.0b1/verticapy/core/parsers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10436 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/all.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5484 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/avro.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20468 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/csv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18799 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6878 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/pandas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2563 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/parsers/shp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.365272 verticapy-1.0.0b1/verticapy/core/string_sql/
--rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/string_sql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9906 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/string_sql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.365272 verticapy-1.0.0b1/verticapy/core/tablesample/
--rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/tablesample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/tablesample/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.369272 verticapy-1.0.0b1/verticapy/core/vdataframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    86125 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_aggregate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    74311 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_corr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24436 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_encoding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5346 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20773 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_fill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28658 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30554 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11984 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_join_union_sort.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35973 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_machine_learning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33120 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_math.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_multiprocessing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17839 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_normalize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9053 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_pivot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    75362 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16513 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_plotting_animated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21629 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15755 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_rolling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27363 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_sys.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7350 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13021 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_typing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7342 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15648 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/core/vdataframe/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.369272 verticapy-1.0.0b1/verticapy/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/datasets/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/airline_passengers.csv
--rw-r--r--   0 runner    (1001) docker     (123)   174821 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/amazon.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/cities.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40378 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/commodities.csv
--rw-r--r--   0 runner    (1001) docker     (123)    82078 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/gapminder.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/market.csv
--rw-r--r--   0 runner    (1001) docker     (123)   400878 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/pop_growth.csv
--rw-r--r--   0 runner    (1001) docker     (123)   367185 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/smart_meters.csv
--rw-r--r--   0 runner    (1001) docker     (123)   116752 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/titanic.csv
--rw-r--r--   0 runner    (1001) docker     (123)   406287 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/winequality.csv
--rw-r--r--   0 runner    (1001) docker     (123)   390866 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/data/world.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     9821 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/generators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18855 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/loaders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4390 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/datasets/tests_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/errors/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/geo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/hchart/
--rwxr-xr-x   0 runner    (1001) docker     (123)      690 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/hchart/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/jupyter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/jupyter/_javascript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/jupyter/extensions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/jupyter/extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1862 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/jupyter/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/jupyter/extensions/chart_magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/jupyter/extensions/sql_magic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/cluster/
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/decomposition/
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/decomposition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/delphi/
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/delphi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/ensemble/
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/ensemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/linear_model/
--rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/linear_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/memmodel/
--rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/memmodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/model_selection/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1281 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/model_selection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/naive_bayes/
--rwxr-xr-x   0 runner    (1001) docker     (123)      764 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/naive_bayes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/neighbors/
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/neighbors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/pipeline/
--rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/preprocessing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/svm/
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/svm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/tree/
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/tsa/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/tsa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/learn/vmodel/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/learn/vmodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.373272 verticapy-1.0.0b1/verticapy/machine_learning/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23033 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/cluster.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7028 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/decomposition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13555 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/ensemble.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5733 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/linear_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7937 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/naive_bayes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7846 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/preprocessing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32737 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/memmodel/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/machine_learning/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    76793 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/metrics/classification.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9212 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/metrics/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15560 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/metrics/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32727 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/cv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27013 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/param_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9934 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9541 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/kmeans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19250 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1145 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4364 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/norm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10547 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/ols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26038 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/tsa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21097 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/model_selection/variables_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/machine_learning/vertica/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7742 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/clustering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15037 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/dataprep.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28843 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/supervised.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   102564 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39245 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/cluster.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26739 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/decomposition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49160 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/ensemble.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23024 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/linear_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6681 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/model_management.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7977 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/naive_bayes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49833 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/neighbors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12316 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31328 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/preprocessing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8861 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/svm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7188 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/machine_learning/vertica/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.377272 verticapy-1.0.0b1/verticapy/plotting/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.381272 verticapy-1.0.0b1/verticapy/plotting/_highcharts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2708 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4804 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/acf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6711 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/barh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1852 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/boxplot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/candlestick.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3726 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/contour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4224 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5530 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/heatmap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6877 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.381272 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3201 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/champion_challenger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2406 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/elbow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/importance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4062 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/lof.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3047 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/logistic_reg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5761 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/model_evaluation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9000 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/pca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3899 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/regression.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2145 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/regression_tree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5058 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/stepwise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4680 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/svm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4046 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/outliers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8272 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/pie.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/range.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5549 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/scatter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2857 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_highcharts/spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.381272 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5810 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/acf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.381272 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7746 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12197 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/bubble.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4330 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3273 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/pie.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4727 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6737 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/barh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3602 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/boxplot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3001 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/contour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5108 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4164 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/heatmap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3102 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/hexbin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2369 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/hist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7993 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.385272 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8289 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/champion_challenger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/elbow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/importance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3986 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/kmeans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4719 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/lof.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6360 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/logistic_reg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7402 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/model_evaluation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8952 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/pca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4184 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/regression.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2595 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/regression_tree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4928 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/stepwise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6883 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/svm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/outliers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10252 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/pie.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3849 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/range.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6893 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/scatter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3238 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_matplotlib/spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.385272 verticapy-1.0.0b1/verticapy/plotting/_plotly/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2761 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/acf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2124 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/barh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3687 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.385272 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/champion_challenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/elbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/lof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/logistic_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/regression_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_plotly/spider.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4961 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    63291 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11132 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/plotting/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.385272 verticapy-1.0.0b1/verticapy/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.385272 verticapy-1.0.0b1/verticapy/sdk/vertica/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sdk/vertica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.389272 verticapy-1.0.0b1/verticapy/sdk/vertica/udf/
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sdk/vertica/udf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11279 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sdk/vertica/udf/gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sdk/vertica/udf/load.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2937 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sdk/vertica/udf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.389272 verticapy-1.0.0b1/verticapy/sql/
--rwxr-xr-x   0 runner    (1001) docker     (123)      935 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/create.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6474 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/dtypes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6144 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/flex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.393272 verticapy-1.0.0b1/verticapy/sql/functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8563 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/analytic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2994 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/conditional.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9095 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/date.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14963 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/math.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/null_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/random.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5681 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/regexp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5182 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/functions/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.393272 verticapy-1.0.0b1/verticapy/sql/geo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/geo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5887 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/geo/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5225 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/geo/index.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4698 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/insert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1183 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/sql/sys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.393272 verticapy-1.0.0b1/verticapy/stats/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2776 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7393 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2467 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/connect/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/connect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/connect/test_connect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/datasets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3745 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/datasets/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/geo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/geo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   153945 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/geo/test_geo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/hchart/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/hchart/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5088 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/hchart/test_hchart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/sql/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/sql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7742 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/sql/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/stats/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/stats/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23086 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/stats/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.397272 verticapy-1.0.0b1/verticapy/tests/udf/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/udf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/udf/pmath.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2489 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/udf/test_udf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.401273 verticapy-1.0.0b1/verticapy/tests/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utilities/csv_test1.csv
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utilities/csv_test2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utilities/csv_test3.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    38029 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utilities/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   315639 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utilities/titanic-passengers.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.401273 verticapy-1.0.0b1/verticapy/tests/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1501 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/utils/os_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.401273 verticapy-1.0.0b1/verticapy/tests/vDataFrame/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13815 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_combine_join_sort.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21816 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_correlation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_create.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39755 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_descriptive_statistics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31699 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_feature_engineering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6817 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_filter_sample.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28742 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    89282 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_plot_plotly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18302 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_preprocessing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23013 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.405273 verticapy-1.0.0b1/verticapy/tests/vModel/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2931 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_balance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9028 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_bisecting_kmeans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3817 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_countvectorizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2453 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_dbscan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18976 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_decision_tree_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12640 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_decision_tree_regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3056 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_delphi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18569 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_dummy_tree_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12224 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_dummy_tree_regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12627 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_elastic_net.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10335 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_iforest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_kde.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7926 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_kmeans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8857 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_knn_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7173 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_knn_regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7991 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_kprototypes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12588 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_lasso.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12726 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_linear_regression.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16380 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_linear_svc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11726 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_linear_svr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_lof.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17732 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_logistic_regression.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7714 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_mca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    62066 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_memmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13757 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_model_selection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19003 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_naive_bayes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9956 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_nearestcentroid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15627 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8791 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_onehotencoder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9202 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_pca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10022 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19395 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_randomforest_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13755 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_randomforest_regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12741 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_ridge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8734 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_svd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10874 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22751 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_xgb_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18106 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests/vModel/test_xgb_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.405273 verticapy-1.0.0b1/verticapy/tests_new/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.405273 verticapy-1.0.0b1/verticapy/tests_new/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/config/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11348 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.405273 verticapy-1.0.0b1/verticapy/tests_new/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/jupyter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/jupyter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/jupyter/extensions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/jupyter/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/memmodel/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/memmodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/metrics/test_classification_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10239 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/metrics/test_regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/model_selection/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/model_selection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/vertica/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/machine_learning/vertica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/plotting/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55249 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/base_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.409273 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_champion_challenger.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_elbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_lof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_logistic_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_acf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_barh.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_candlestick.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_pie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.413273 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.413273 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_champion_challenger.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_elbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_lof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_logistic_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_acf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_barh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hexbin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_pie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.413273 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_champion_challenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_elbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_lof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_logistic_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_acf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_barh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_pie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/tests_new/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/tests_new/sql/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/tests_new/sql/functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/sql/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/tests_new/sql/geo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/sql/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/tests_new/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/tests_new/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/udf/
--rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/udf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.417273 verticapy-1.0.0b1/verticapy/vdataframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-06-20 21:34:11.000000 verticapy-1.0.0b1/verticapy/vdataframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:34:24.361272 verticapy-1.0.0b1/verticapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-20 21:34:24.000000 verticapy-1.0.0b1/verticapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22430 2023-06-20 21:34:24.000000 verticapy-1.0.0b1/verticapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:34:24.000000 verticapy-1.0.0b1/verticapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 21:34:24.000000 verticapy-1.0.0b1/verticapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 21:34:24.000000 verticapy-1.0.0b1/verticapy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.982222 verticapy-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-07-10 13:16:57.982222 verticapy-1.0.0b2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19328 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:16:57.982222 verticapy-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.874221 verticapy-1.0.0b2/verticapy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3693 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.874221 verticapy-1.0.0b2/verticapy/_config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6070 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_config/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_config/validators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3917 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2160 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.878221 verticapy-1.0.0b2/verticapy/_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12398 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_display.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    73985 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_logo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4401 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1758 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_object.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2292 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.878221 verticapy-1.0.0b2/verticapy/_utils/_sql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3789 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_cast.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5564 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_collect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3847 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_dblink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1797 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_display.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_format.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9319 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_merge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_random.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2652 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_sys.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4935 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/_utils/_sql/_vertica_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.882221 verticapy-1.0.0b2/verticapy/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/connection/connect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/connection/external.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/connection/global_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5113 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/connection/read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1734 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/connection/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5715 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/connection/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.882221 verticapy-1.0.0b2/verticapy/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.882221 verticapy-1.0.0b2/verticapy/core/parsers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10436 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5484 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/avro.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20468 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18799 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6878 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/pandas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2563 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/parsers/shp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.882221 verticapy-1.0.0b2/verticapy/core/string_sql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/string_sql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9906 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/string_sql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.882221 verticapy-1.0.0b2/verticapy/core/tablesample/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/tablesample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/tablesample/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.890221 verticapy-1.0.0b2/verticapy/core/vdataframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    86125 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_aggregate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    74311 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_corr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24460 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_encoding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5346 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20773 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_fill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28652 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30554 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11984 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_join_union_sort.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35973 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_machine_learning.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33120 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_multiprocessing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17839 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_normalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9053 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_pivot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    76758 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16513 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_plotting_animated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21629 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15755 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_rolling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27363 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_sys.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7350 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13021 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_typing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7342 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15648 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/core/vdataframe/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.890221 verticapy-1.0.0b2/verticapy/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.894221 verticapy-1.0.0b2/verticapy/datasets/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/airline_passengers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   174821 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/amazon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/cities.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40378 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/commodities.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    82078 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/gapminder.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/market.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   400878 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/pop_growth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   367185 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/smart_meters.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   116752 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/titanic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   406287 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/winequality.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   390866 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/data/world.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9821 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/generators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18855 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/loaders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4390 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/datasets/tests_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.894221 verticapy-1.0.0b2/verticapy/errors/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/geo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/hchart/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      690 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/hchart/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/jupyter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/jupyter/_javascript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/jupyter/extensions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/jupyter/extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1862 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/jupyter/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/jupyter/extensions/chart_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/jupyter/extensions/sql_magic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/cluster/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/decomposition/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/decomposition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/delphi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/delphi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/ensemble/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/ensemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/linear_model/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/linear_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/memmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/memmodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.898221 verticapy-1.0.0b2/verticapy/learn/model_selection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1281 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/model_selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/naive_bayes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      764 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/naive_bayes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/neighbors/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/neighbors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/pipeline/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/preprocessing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/svm/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/svm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/tree/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/tsa/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/tsa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/learn/vmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/learn/vmodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.902221 verticapy-1.0.0b2/verticapy/machine_learning/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.906221 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23033 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/cluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7028 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/decomposition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13555 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/ensemble.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5733 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/linear_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7937 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/naive_bayes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7846 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/preprocessing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32737 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/memmodel/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.906221 verticapy-1.0.0b2/verticapy/machine_learning/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/metrics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    86231 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/metrics/classification.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9212 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/metrics/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15560 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/metrics/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.906221 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.906221 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32727 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/cv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27013 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/param_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9934 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10248 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/kmeans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19250 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.910221 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1145 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4364 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/norm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10547 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/ols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26038 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/tsa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21088 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/model_selection/variables_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.910221 verticapy-1.0.0b2/verticapy/machine_learning/vertica/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.914221 verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7970 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/clustering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15428 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/dataprep.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29079 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/supervised.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   103188 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39896 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/cluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27104 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/decomposition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49711 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/ensemble.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23579 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/linear_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6681 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/model_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8350 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/naive_bayes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50135 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/neighbors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12552 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31920 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/preprocessing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9083 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/svm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8120 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/machine_learning/vertica/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.914221 verticapy-1.0.0b2/verticapy/plotting/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.918221 verticapy-1.0.0b2/verticapy/plotting/_highcharts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2708 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4804 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/acf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6711 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/barh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1852 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/boxplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/candlestick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3726 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/contour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4185 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/density.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5629 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/heatmap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6941 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.918221 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3201 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/champion_challenger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2406 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/elbow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/importance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4062 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/lof.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3047 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/logistic_reg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5761 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/model_evaluation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9000 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/pca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3899 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/regression.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2145 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/regression_tree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5058 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/stepwise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4680 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/svm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4046 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/outliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8272 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/pie.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/range.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5549 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/scatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2857 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_highcharts/spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.922222 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5810 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/acf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.922222 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7746 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12197 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/bubble.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4330 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3273 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/pie.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4727 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6737 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/barh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3602 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/boxplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3001 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/contour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5108 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/density.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4164 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/heatmap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3102 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/hexbin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2369 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/hist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7993 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.926221 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8289 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/champion_challenger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/elbow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/importance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3986 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/kmeans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4719 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/lof.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6360 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/logistic_reg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7466 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/model_evaluation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8952 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/pca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4184 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/regression.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2595 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/regression_tree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4928 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/stepwise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6883 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/svm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/outliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10252 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/pie.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3849 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/range.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6893 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/scatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3238 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_matplotlib/spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.930221 verticapy-1.0.0b2/verticapy/plotting/_plotly/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/acf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3472 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/barh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3687 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.934222 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/champion_challenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/elbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/lof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/logistic_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/regression_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_plotly/spider.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4961 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63624 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11132 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/plotting/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.934222 verticapy-1.0.0b2/verticapy/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.934222 verticapy-1.0.0b2/verticapy/sdk/vertica/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sdk/vertica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.934222 verticapy-1.0.0b2/verticapy/sdk/vertica/udf/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sdk/vertica/udf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11279 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sdk/vertica/udf/gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sdk/vertica/udf/load.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2937 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sdk/vertica/udf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.938222 verticapy-1.0.0b2/verticapy/sql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      935 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6474 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/dtypes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6144 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/flex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.938222 verticapy-1.0.0b2/verticapy/sql/functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8563 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/analytic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2994 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/conditional.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9095 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/date.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14963 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/math.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/null_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/random.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5681 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/regexp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5182 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/functions/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.938222 verticapy-1.0.0b2/verticapy/sql/geo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/geo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5887 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/geo/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5225 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/geo/index.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4698 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/insert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1183 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/sql/sys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.938222 verticapy-1.0.0b2/verticapy/stats/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2776 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.938222 verticapy-1.0.0b2/verticapy/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7393 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2467 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.942222 verticapy-1.0.0b2/verticapy/tests/connect/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/connect/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/connect/test_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.942222 verticapy-1.0.0b2/verticapy/tests/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/datasets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3745 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/datasets/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.942222 verticapy-1.0.0b2/verticapy/tests/geo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/geo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   153945 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/geo/test_geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.942222 verticapy-1.0.0b2/verticapy/tests/hchart/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/hchart/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5088 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/hchart/test_hchart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.942222 verticapy-1.0.0b2/verticapy/tests/sql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/sql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7742 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/sql/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.942222 verticapy-1.0.0b2/verticapy/tests/stats/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/stats/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23086 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/stats/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.942222 verticapy-1.0.0b2/verticapy/tests/udf/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/udf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/udf/pmath.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2489 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/udf/test_udf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.946222 verticapy-1.0.0b2/verticapy/tests/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utilities/csv_test1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utilities/csv_test2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utilities/csv_test3.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38095 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utilities/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   315639 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utilities/titanic-passengers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.946222 verticapy-1.0.0b2/verticapy/tests/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1501 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/utils/os_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.950222 verticapy-1.0.0b2/verticapy/tests/vDataFrame/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13815 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_combine_join_sort.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21816 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_correlation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39755 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_descriptive_statistics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31699 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_feature_engineering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6817 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_filter_sample.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28742 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89903 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_plot_plotly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18302 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_preprocessing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23013 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests/vModel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2931 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_balance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9141 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_bisecting_kmeans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4631 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_countvectorizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3365 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_dbscan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19096 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_decision_tree_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12759 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_decision_tree_regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5009 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_delphi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18686 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_dummy_tree_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12340 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_dummy_tree_regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12735 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_elastic_net.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10448 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_iforest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3825 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8659 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_kmeans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8857 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_knn_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7290 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_knn_regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8100 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_kprototypes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12691 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_lasso.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13474 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_linear_regression.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16487 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_linear_svc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11833 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_linear_svr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3944 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_lof.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17848 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_logistic_regression.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7815 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_mca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62066 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_memmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15146 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_model_selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19111 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_naive_bayes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10069 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_nearestcentroid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15958 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8902 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_onehotencoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9303 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_pca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11513 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19515 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_randomforest_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13874 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_randomforest_regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12844 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_ridge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8835 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_svd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10874 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22862 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_xgb_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18216 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests/vModel/test_xgb_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests_new/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests_new/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11711 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests_new/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests_new/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests_new/jupyter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/jupyter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests_new/jupyter/extensions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/jupyter/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.958222 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.962222 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/memmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/memmodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.962222 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/metrics/test_classification_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10239 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/metrics/test_regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.962222 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/model_selection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/model_selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.962222 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/vertica/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/vertica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.962222 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/vertica/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/vertica/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/machine_learning/vertica/linear_model/test_linear_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.962222 verticapy-1.0.0b2/verticapy/tests_new/plotting/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56294 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/base_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.966222 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.970222 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_champion_challenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_elbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_lof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_logistic_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_acf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_barh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_candlestick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.970222 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.974222 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_champion_challenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_elbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_lof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_logistic_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_acf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_barh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hexbin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.978222 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.978222 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_champion_challenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_elbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_lof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_logistic_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_acf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_barh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.978222 verticapy-1.0.0b2/verticapy/tests_new/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.978222 verticapy-1.0.0b2/verticapy/tests_new/sql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.978222 verticapy-1.0.0b2/verticapy/tests_new/sql/functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/sql/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.978222 verticapy-1.0.0b2/verticapy/tests_new/sql/geo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/sql/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.982222 verticapy-1.0.0b2/verticapy/tests_new/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/tests_new/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.982222 verticapy-1.0.0b2/verticapy/udf/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/udf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.982222 verticapy-1.0.0b2/verticapy/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.982222 verticapy-1.0.0b2/verticapy/vdataframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-07-10 13:16:43.000000 verticapy-1.0.0b2/verticapy/vdataframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:16:57.874221 verticapy-1.0.0b2/verticapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-07-10 13:16:57.000000 verticapy-1.0.0b2/verticapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-07-10 13:16:57.000000 verticapy-1.0.0b2/verticapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:16:57.000000 verticapy-1.0.0b2/verticapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-10 13:16:57.000000 verticapy-1.0.0b2/verticapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 13:16:57.000000 verticapy-1.0.0b2/verticapy.egg-info/top_level.txt
```

### Comparing `verticapy-1.0.0b1/LICENSE.txt` & `verticapy-1.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/PKG-INFO` & `verticapy-1.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verticapy
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: VerticaPy simplifies data exploration, data cleaning, and machine learning in Vertica.
 Home-page: https://github.com/vertica/VerticaPy
 Author: Badr Ouali
 Author-email: badr.ouali@vertica.com
 Keywords: vertica python ml data science machine learning statistics database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `verticapy-1.0.0b1/README.md` & `verticapy-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/setup.py` & `verticapy-1.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="verticapy",
-    version="1.0.0-beta.1",
+    version="1.0.0-beta.2",
     author="Badr Ouali",
     author_email="badr.ouali@vertica.com",
     url="https://github.com/vertica/VerticaPy",
     keywords="vertica python ml data science machine learning statistics database",
     description=(
         "VerticaPy simplifies data exploration, data cleaning, and machine"
         " learning in Vertica."
```

### Comparing `verticapy-1.0.0b1/verticapy/__init__.py` & `verticapy-1.0.0b2/verticapy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 __author_email__: str = "badr.ouali@vertica.com"
 __description__: str = (
     "VerticaPy simplifies data exploration, data cleaning"
     " and machine learning in Vertica."
 )
 __url__: str = "https://github.com/vertica/verticapy/"
 __license__: str = "Apache License, Version 2.0"
-__version__: str = "1.0.0-beta.1"
+__version__: str = "1.0.0-beta.2"
 
 from verticapy._config.config import get_option, set_option
 from verticapy._utils._sql._vertica_version import vertica_version
 from verticapy._utils._logo import verticapy_logo_html, verticapy_logo_str
 from verticapy._help import help_start
 
 from verticapy.connection.connect import (
```

### Comparing `verticapy-1.0.0b1/verticapy/_config/__init__.py` & `verticapy-1.0.0b2/verticapy/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_config/config.py` & `verticapy-1.0.0b2/verticapy/_config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,18 +115,14 @@
         Maximum number of rows to display. If the
         specified value is invalid, max_row is not
         changed.
     mode: str
         Display mode for VerticaPy outputs, either:
             full  : VerticaPy regular display mode.
             light : Minimalist display mode.
-    overwrite_model: bool
-        If set to True, training a model with the same
-        name as an existing model overwrites the
-        existing model.
     percent_bar: bool
         If set to True, the percent of non-missing
         values is displayed.
     print_info: bool
         If set to True, information is printed each
         time the vDataFrame is modified.
     random_state: int
@@ -170,15 +166,14 @@
 register_option(Option("cache", True, "", bool_validator))
 register_option(Option("interactive", False, "", bool_validator))
 register_option(Option("count_on", False, "", bool_validator))
 register_option(Option("footer_on", True, "", bool_validator))
 register_option(Option("max_columns", 50, "", st_positive_int_validator))
 register_option(Option("max_rows", 100, "", st_positive_int_validator))
 register_option(Option("mode", "full", "", in_validator(["full", "light"])))
-register_option(Option("overwrite_model", True, "", bool_validator))
 register_option(Option("percent_bar", False, "", bool_validator))
 register_option(Option("print_info", True, "", bool_validator))
 register_option(Option("save_query_profile", True, "", bool_validator))
 register_option(Option("sql_on", False, "", bool_validator))
 register_option(Option("random_state", None, "", optional_positive_int_validator))
 register_option(Option("temp_schema", "public", "", str_validator))
 register_option(Option("time_on", False, "", bool_validator))
```

### Comparing `verticapy-1.0.0b1/verticapy/_config/validators.py` & `verticapy-1.0.0b2/verticapy/_config/validators.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_help.py` & `verticapy-1.0.0b2/verticapy/_help.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_typing.py` & `verticapy-1.0.0b2/verticapy/_typing.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/__init__.py` & `verticapy-1.0.0b2/verticapy/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_display.py` & `verticapy-1.0.0b2/verticapy/_utils/_display.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_gen.py` & `verticapy-1.0.0b2/verticapy/_utils/_gen.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-import random
+import uuid
 from typing import Optional
 
 from verticapy._utils._sql._format import quote_ident
 
 from verticapy.connection.connect import current_cursor
 
 
@@ -41,12 +41,12 @@
     """
     current_cursor().execute("SELECT CURRENT_SESSION(), USERNAME();")
     current_session, username = current_cursor().fetchone()
     session_user = f"{current_session}_{username}"
     L = session_user.split("_")
     L[0] = "".join(filter(str.isalnum, L[0]))
     L[1] = "".join(filter(str.isalnum, L[1]))
-    random_int = random.randint(0, 10e9)
-    name = f'"_verticapy_tmp_{name.lower()}_{L[0]}_{L[1]}_{random_int}_"'
+    universal_unique_id = str(uuid.uuid1()).replace("-", "")
+    name = f'"_verticapy_tmp_{name.lower()}_{L[0]}_{L[1]}_{universal_unique_id}_"'
     if schema:
         name = f"{quote_ident(schema)}.{name}"
     return name
```

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_logo.py` & `verticapy-1.0.0b2/verticapy/_utils/_logo.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_map.py` & `verticapy-1.0.0b2/verticapy/_utils/_map.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_object.py` & `verticapy-1.0.0b2/verticapy/_utils/_object.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_parsers.py` & `verticapy-1.0.0b2/verticapy/_utils/_parsers.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/__init__.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_cast.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_cast.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     map_dict = {
         "vmap": f"MAPTOSTRING({column})",
         "binary": f"TO_HEX({column})",
         "spatial": f"ST_AsText({column})",
     }
     if category in map_dict:
-        return map_dict[column]
+        return map_dict[category]
     return column
 
 
 def to_dtype_category(
     expr: type,
 ) -> Literal["float", "int", "text", "date", "complex", "undefined"]:
     """
```

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_check.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_check.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_collect.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_collect.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_dblink.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_dblink.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_display.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_display.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_format.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_format.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_merge.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_merge.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_random.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_random.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_sys.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_sys.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/_utils/_sql/_vertica_version.py` & `verticapy-1.0.0b2/verticapy/_utils/_sql/_vertica_version.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/connection/__init__.py` & `verticapy-1.0.0b2/verticapy/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/connection/connect.py` & `verticapy-1.0.0b2/verticapy/connection/connect.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/connection/external.py` & `verticapy-1.0.0b2/verticapy/connection/external.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/connection/global_connection.py` & `verticapy-1.0.0b2/verticapy/connection/global_connection.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/connection/read.py` & `verticapy-1.0.0b2/verticapy/connection/read.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/connection/utils.py` & `verticapy-1.0.0b2/verticapy/connection/utils.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/connection/write.py` & `verticapy-1.0.0b2/verticapy/connection/write.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/__init__.py` & `verticapy-1.0.0b2/verticapy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/__init__.py` & `verticapy-1.0.0b2/verticapy/core/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/_utils.py` & `verticapy-1.0.0b2/verticapy/core/parsers/_utils.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/all.py` & `verticapy-1.0.0b2/verticapy/core/parsers/all.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/avro.py` & `verticapy-1.0.0b2/verticapy/core/parsers/avro.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/csv.py` & `verticapy-1.0.0b2/verticapy/core/parsers/csv.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/json.py` & `verticapy-1.0.0b2/verticapy/core/parsers/json.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/pandas.py` & `verticapy-1.0.0b2/verticapy/core/parsers/pandas.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/parsers/shp.py` & `verticapy-1.0.0b2/verticapy/core/parsers/shp.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/string_sql/__init__.py` & `verticapy-1.0.0b2/verticapy/core/string_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/string_sql/base.py` & `verticapy-1.0.0b2/verticapy/core/string_sql/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/tablesample/__init__.py` & `verticapy-1.0.0b2/verticapy/core/tablesample/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/tablesample/base.py` & `verticapy-1.0.0b2/verticapy/core/tablesample/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/__init__.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_aggregate.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_aggregate.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_corr.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_corr.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_encoding.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
                 query=query,
                 title="Computing the equal frequency histogram bins.",
                 method="fetchall",
                 sql_push_ext=self._parent._vars["sql_push_ext"],
                 symbol=self._parent._vars["symbol"],
             )
             result = [elem[0] for elem in result]
-        elif self.isnum() and method in ("same_width", "auto"):
+        elif self.isnum() and not (self.isbool()) and method in ("same_width", "auto"):
             if not h or h <= 0:
                 if nbins <= 0:
                     h = self.numh()
                 else:
                     h = (self.max() - self.min()) * 1.01 / nbins
                 if h > 0.01:
                     h = round(h, 2)
```

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_eval.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_eval.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_fill.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_fill.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_filter.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,15 +659,15 @@
         Returns
         -------
         vDataFrame
             vDataFrame of the search
         """
         order_by, usecols, expr = format_type(order_by, usecols, expr, dtype=list)
         if isinstance(conditions, Iterable) and not isinstance(conditions, str):
-            conditions = " AND ".join([f"({elem})" for elem in conditions])
+            conditions = " AND ".join([f"({c})" for c in conditions])
         if conditions:
             conditions = f" WHERE {conditions}"
         all_cols = ", ".join(["*"] + expr)
         query = f"SELECT {all_cols} FROM {self}{conditions}"
         result = create_new_vdf(query)
         if usecols:
             result = result.select(usecols)
```

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_io.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_io.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_join_union_sort.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_join_union_sort.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_machine_learning.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_machine_learning.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_math.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_math.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_multiprocessing.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_normalize.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_normalize.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_pivot.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_pivot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_plotting.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 import math
-from typing import Callable, Literal, Optional, Union
+import warnings
 from collections.abc import Iterable
+from typing import Callable, Literal, Optional, Union
 import numpy as np
 
 import verticapy._config.config as conf
 from verticapy._utils._object import get_vertica_mllib
 from verticapy._typing import (
     ArrayLike,
     ColorType,
@@ -162,14 +163,19 @@
         Returns
         -------
         obj
             Plotting Object.
         """
         columns = format_type(columns, dtype=list)
         columns, of = self.format_colnames(columns, of, expected_nb_of_cols=[1, 2])
+        if not (isinstance(max_cardinality, Iterable)):
+            max_cardinality = (max_cardinality, max_cardinality)
+        if not (isinstance(h, Iterable)):
+            h = (h, h)
+
         if len(columns) == 1:
             return self[columns[0]].bar(
                 method=method,
                 of=of,
                 max_cardinality=max_cardinality[0],
                 h=h[0],
                 **style_kwargs,
@@ -277,14 +283,19 @@
         Returns
         -------
         obj
             Plotting Object.
         """
         columns = format_type(columns, dtype=list)
         columns, of = self.format_colnames(columns, of, expected_nb_of_cols=[1, 2])
+        if not (isinstance(max_cardinality, Iterable)):
+            max_cardinality = (max_cardinality, max_cardinality)
+        if not (isinstance(h, Iterable)):
+            h = (h, h)
+
         if len(columns) == 1:
             return self[columns[0]].barh(
                 method=method,
                 of=of,
                 max_cardinality=max_cardinality[0],
                 h=h[0],
                 chart=chart,
@@ -408,18 +419,14 @@
                 sum     : Sum of the vDataColumn 'of'.
                 q%      : q Quantile of the vDataColumn 'of'
                           (ex: 50% to get the median).
             It can also be a cutomized aggregation, for example:
             AVG(column1) + 5
         of: str, optional
             The  vDataColumn used to compute the  aggregation.
-        max_cardinality: tuple, optional
-            Maximum number of distinct elements for vDataColumns
-            to be used as categorical. For these elements, no
-            h is picked or computed.
         h: tuple, optional
             Interval width of the  input vDataColumns. Optimized
             h  will be  computed if  the  parameter  is empty or
             invalid.
         chart: PlottingObject, optional
             The chart object to plot on.
         **style_kwargs
@@ -1788,14 +1795,18 @@
             or of a date-like type. Optimized  h will be computed
             if the parameter is empty or invalid.
         max_cardinality: int, optional
             Maximum number of distinct elements for vDataColumns
             to be used as categorical.
             The less frequent  elements are gathered together
             to create a new category : 'Others'.
+            This parameter is used to discretize the vDataColumn
+            'by' when the main input nvDataColumn is nnumerical.
+            Otherwise, it  is  used  to   discretize    all the
+            vDataColumn inputs.
         cat_priority: PythonScalar / ArrayLike, optional
             ArrayLike list of the different categories to consider
             when drawing the box plot.  The other categories are
             filtered.
         chart: PlottingObject, optional
             The chart object to plot on.
         **style_kwargs
@@ -1803,30 +1814,56 @@
             functions.
 
         Returns
         -------
         obj
             Plotting Object.
         """
-        vpy_plt, kwargs = self._parent.get_plotting_lib(
-            class_name="Histogram",
-            chart=chart,
-            style_kwargs=style_kwargs,
-        )
-        return vpy_plt.Histogram(
-            vdf=self._parent,
-            columns=[self._alias],
-            by=by,
-            method=method,
-            of=of,
-            h=h,
-            h_by=h_by,
-            max_cardinality=max_cardinality,
-            cat_priority=cat_priority,
-        ).draw(**kwargs)
+        if self.isnum() and not (self.isbool()):
+            vpy_plt, kwargs = self._parent.get_plotting_lib(
+                class_name="Histogram",
+                chart=chart,
+                style_kwargs=style_kwargs,
+            )
+            return vpy_plt.Histogram(
+                vdf=self._parent,
+                columns=[self._alias],
+                by=by,
+                method=method,
+                of=of,
+                h=h,
+                h_by=h_by,
+                max_cardinality=max_cardinality,
+                cat_priority=cat_priority,
+            ).draw(**kwargs)
+        else:
+            warning_message = (
+                f"The Virtual Column {self._alias} is not "
+                "numerical. A bar chart will be drawn instead."
+            )
+            warnings.warn(warning_message, Warning)
+            if by:
+                return self._parent.bar(
+                    columns=[self._alias, by],
+                    method=method,
+                    of=of,
+                    max_cardinality=(max_cardinality, max_cardinality),
+                    h=(h, h),
+                    chart=chart,
+                    **style_kwargs,
+                )
+            else:
+                return self.bar(
+                    method=method,
+                    of=of,
+                    max_cardinality=max_cardinality,
+                    h=h,
+                    chart=chart,
+                    **style_kwargs,
+                )
 
     @save_verticapy_logs
     def density(
         self,
         by: Optional[str] = None,
         bandwidth: PythonNumber = 1.0,
         kernel: Literal["gaussian", "logistic", "sigmoid", "silverman"] = "gaussian",
```

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_plotting_animated.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_plotting_animated.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_read.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_read.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_rolling.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_rolling.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_sys.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_sys.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_text.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_text.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_typing.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_typing.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/_utils.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/_utils.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/core/vdataframe/base.py` & `verticapy-1.0.0b2/verticapy/core/vdataframe/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/__init__.py` & `verticapy-1.0.0b2/verticapy/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/__init__.py` & `verticapy-1.0.0b2/verticapy/datasets/data/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/airline_passengers.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/airline_passengers.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/amazon.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/amazon.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/cities.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/cities.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/commodities.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/commodities.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/gapminder.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/gapminder.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/iris.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/iris.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/market.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/market.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/pop_growth.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/pop_growth.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/smart_meters.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/smart_meters.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/titanic.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/winequality.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/winequality.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/data/world.csv` & `verticapy-1.0.0b2/verticapy/datasets/data/world.csv`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/generators.py` & `verticapy-1.0.0b2/verticapy/datasets/generators.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/loaders.py` & `verticapy-1.0.0b2/verticapy/datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/datasets/tests_loaders.py` & `verticapy-1.0.0b2/verticapy/datasets/tests_loaders.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/errors/__init__.py` & `verticapy-1.0.0b2/verticapy/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/geo/__init__.py` & `verticapy-1.0.0b2/verticapy/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/hchart/__init__.py` & `verticapy-1.0.0b2/verticapy/hchart/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/jupyter/__init__.py` & `verticapy-1.0.0b2/verticapy/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/jupyter/_javascript.py` & `verticapy-1.0.0b2/verticapy/jupyter/_javascript.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/jupyter/extensions/__init__.py` & `verticapy-1.0.0b2/verticapy/jupyter/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/jupyter/extensions/_utils.py` & `verticapy-1.0.0b2/verticapy/jupyter/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/jupyter/extensions/chart_magic.py` & `verticapy-1.0.0b2/verticapy/jupyter/extensions/chart_magic.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/jupyter/extensions/sql_magic.py` & `verticapy-1.0.0b2/verticapy/jupyter/extensions/sql_magic.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/cluster/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/decomposition/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/delphi/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/delphi/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/ensemble/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/linear_model/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/memmodel/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/memmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/metrics/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/model_selection/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/naive_bayes/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/naive_bayes/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/neighbors/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/neighbors/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/pipeline/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/preprocessing/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/svm/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/svm/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/tools/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/tree/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/tsa/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/tsa/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/learn/vmodel/__init__.py` & `verticapy-1.0.0b2/verticapy/learn/vmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/base.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/cluster.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/cluster.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/decomposition.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/decomposition.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/ensemble.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/ensemble.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/linear_model.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/linear_model.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/naive_bayes.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/preprocessing.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/preprocessing.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/memmodel/tree.py` & `verticapy-1.0.0b2/verticapy/machine_learning/memmodel/tree.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/metrics/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/metrics/classification.py` & `verticapy-1.0.0b2/verticapy/machine_learning/metrics/classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 from typing import Callable, Literal, Optional, Union, TYPE_CHECKING
-
 import numpy as np
-
 from verticapy._typing import (
     ArrayLike,
     NoneType,
     PythonNumber,
     PythonScalar,
     SQLRelation,
 )
@@ -1653,15 +1651,14 @@
     """
     if average == "weighted":
         confusion_list = _compute_classes_tn_fn_fp_tp(
             y_true, y_score[1], input_relation, labels
         )
         weights = [args[1] + args[3] for args in confusion_list]
     else:
-        # micro is not feasible using AUC.
         weights = [1.0 for args in labels]
     nbins_kw = {"nbins": nbins} if not isinstance(nbins, NoneType) else {}
     scores = [
         weights[i]
         * metric(
             y_true,
             y_score[0].format(labels[i]),
@@ -1670,14 +1667,76 @@
             **nbins_kw,
         )
         for i in range(len(labels))
     ]
     return sum(scores) / sum(weights)
 
 
+def _compute_micro_multiclass_metric(
+    y_true: str,
+    y_score: ArrayLike,
+    input_relation: SQLRelation,
+    labels: ArrayLike,
+    nbins: int,
+    fun_sql_name: Optional[str],
+):
+    if fun_sql_name == "roc":
+        X = ["decision_boundary", "false_positive_rate", "true_positive_rate"]
+    elif fun_sql_name == "prc":
+        X = ["decision_boundary", "recall", "precision"]
+    labels_query = ""
+    for i in range(len(labels)):
+        labels_query += f"""
+                    WHEN {labels[i]} THEN {y_score[i]}"""
+    decode_query = f"""
+                    SELECT
+                    CASE WHEN {y_true} = distinct_values.value THEN 1 ELSE 0 END AS decoded_value,
+                    CASE distinct_values.value
+                    {labels_query}
+                    ELSE NULL
+                    END AS prob_value
+                    FROM
+                    {input_relation},
+                    (SELECT DISTINCT {y_true} AS value FROM {input_relation}) AS distinct_values"""
+
+    query = f"""
+            SELECT
+                {', '.join(X)}
+            FROM
+                (SELECT
+                    {fun_sql_name.upper()}(
+                            obs, prob 
+                            USING PARAMETERS 
+                            num_bins = {nbins}) OVER() 
+                FROM (
+                SELECT
+                t.decoded_value as obs,
+                t.prob_value::float as prob
+                FROM (
+                {decode_query}) AS t) AS subquery
+            ) x
+            """
+    # The following query does exactly what is required except that I have to tell it that the distinct values are 0,1,2
+    query_result = _executeSQL(
+        query=query,
+        title=f"Computing the",
+        method="fetchall",
+    )
+    result = [
+        [item[0] for item in query_result],
+        [item[1] for item in query_result],
+        [item[2] for item in query_result],
+    ]
+    if fun_sql_name == "prc":
+        result[0] = [0] + result[0] + [1]
+        result[1] = [1] + result[1] + [0]
+        result[2] = [0] + result[2] + [1]
+    return result
+
+
 def _get_yscore(
     y_score: Union[str, ArrayLike],
     labels: Optional[ArrayLike] = None,
     pos_label: Optional[PythonScalar] = None,
 ) -> str:
     """
     Returns the 'y_score' to use to compute the final metric.
@@ -1779,14 +1838,137 @@
             average=average,
             labels=labels,
             nbins=nbins,
         )
 
 
 @save_verticapy_logs
+def average_precision_score(
+    y_true: str,
+    y_score: Union[str, ArrayLike],
+    input_relation: SQLRelation,
+    average: Literal[None, "micro", "macro", "scores", "weighted"] = None,
+    labels: Optional[ArrayLike] = None,
+    pos_label: Optional[PythonScalar] = None,
+    nbins: int = 10000,
+) -> float:
+    """
+    Computes the Average precision Score.
+
+    Parameters
+    ----------
+    y_true: str
+        Response column.
+    y_score: str |  ArrayLike
+        Prediction.
+    input_relation: SQLRelation
+        Relation to use for scoring. This relation can
+        be a view, table, or a customized relation (if
+        an alias is used at the end of the relation).
+        For example: (SELECT ... FROM ...) x
+    average: str, optional
+        The method used to  compute the final score for
+        multiclass-classification.
+            micro    : positive  and   negative  values
+                       globally.
+            macro    : average  of  the  score of  each
+                       class.
+            scores   : scores  for   all  the  classes.
+            weighted : weighted average of the score of
+                       each class.
+        If  empty,  the  behaviour  is  similar to  the
+        'scores' option.
+    labels: ArrayLike, optional
+        List   of   the  response  column   categories.
+    pos_label: PythonScalar, optional
+        To  compute  the metric, one of  the  response
+        column classes must be the positive class. The
+        parameter 'pos_label' represents this class.
+    nbins: int, optional
+        An integer value that determines the number of
+        decision boundaries.
+        Decision boundaries  are set at equally spaced
+        intervals between 0 and 1, inclusive.
+        Greater  values  for nbins give  more  precise
+        estimations  of the AUC,  but can  potentially
+        decrease  performance.  The  maximum value  is
+        999,999.  If negative,  the  maximum value  is
+        used.
+
+    Returns
+    -------
+    float
+        score.
+    """
+    if not isinstance(pos_label, NoneType) or isinstance(labels, NoneType):
+        recall, precision = _compute_function_metrics(
+            y_true=y_true,
+            y_score=_get_yscore(y_score, labels, pos_label),
+            input_relation=input_relation,
+            pos_label=pos_label,
+            nbins=nbins,
+            fun_sql_name="prc",
+        )[1:]
+        return -np.sum(np.diff(recall) * np.array(precision)[:-1])
+    else:
+        _check_labels(y_true=y_true, labels=labels, input_relation=input_relation)
+    if average == "micro":
+        _, recall, precision = _compute_micro_multiclass_metric(
+            y_true, y_score, input_relation, labels, nbins, fun_sql_name="prc"
+        )
+        return -np.sum(np.diff(recall) * np.array(precision)[:-1])
+    elif average == "macro":
+        aps = 0
+        for i, label in enumerate(labels):
+            aps += average_precision_score(
+                y_true=y_true,
+                y_score=y_score[i],
+                input_relation=input_relation,
+                average=None,
+                labels=None,
+                pos_label=label,
+                nbins=nbins,
+            )
+        return aps / len(labels)
+    elif average == "weighted":
+        aps = 0
+        all_weights = 0
+        for i, label in enumerate(labels):
+            weight = len(input_relation[input_relation[y_true] == label])
+            aps += weight * average_precision_score(
+                y_true=y_true,
+                y_score=y_score[i],
+                input_relation=input_relation,
+                average=None,
+                labels=None,
+                pos_label=label,
+                nbins=nbins,
+            )
+            all_weights += weight
+        return aps / all_weights
+    else:
+        aps = []
+        for i, label in enumerate(labels):
+            aps.append(
+                average_precision_score(
+                    y_true=y_true,
+                    y_score=y_score[i],
+                    input_relation=input_relation,
+                    average=None,
+                    labels=None,
+                    pos_label=label,
+                    nbins=nbins,
+                )
+            )
+        return aps
+
+    return None
+
+
+@save_verticapy_logs
 def roc_auc_score(
     y_true: str,
     y_score: Union[str, ArrayLike],
     input_relation: SQLRelation,
     average: Literal[None, "binary", "micro", "macro", "scores", "weighted"] = None,
     labels: Optional[ArrayLike] = None,
     pos_label: Optional[PythonScalar] = None,
@@ -1840,36 +2022,83 @@
         used.
 
     Returns
     -------
     float
         score.
     """
-    if not isinstance(pos_label, NoneType) or isinstance(labels, NoneType):
+    if (
+        not isinstance(pos_label, NoneType)
+        or isinstance(labels, NoneType)
+        and isinstance(y_score, str)
+    ):
         false_positive, true_positive = _compute_function_metrics(
             y_true=y_true,
             y_score=_get_yscore(y_score, labels, pos_label),
             input_relation=input_relation,
             pos_label=pos_label,
             nbins=nbins,
             fun_sql_name="roc",
         )[1:]
         return _compute_area(true_positive, false_positive)
+    elif average == "micro":
+        _check_labels(y_true=y_true, labels=labels, input_relation=input_relation)
+        _, false_positive, true_positive = _compute_micro_multiclass_metric(
+            y_true, y_score, input_relation, labels, nbins, fun_sql_name="roc"
+        )
+        return _compute_area(true_positive, false_positive)
+    elif average == "macro":
+        _check_labels(y_true=y_true, labels=labels, input_relation=input_relation)
+        fpr = {}
+        tpr = {}
+        for i in range(len(y_score)):
+            fpr[i], tpr[i] = _compute_function_metrics(
+                y_true=y_true,
+                y_score=y_score[i],
+                input_relation=input_relation,
+                pos_label=labels[i],
+                nbins=nbins,
+                fun_sql_name="roc",
+            )[1:]
+
+        fpr_grid = np.linspace(0.0, 1.0, nbins)
+        mean_tpr = np.zeros_like(fpr_grid)
+
+        for i in range(len(y_score)):
+            sorted_pairs = sorted(zip(fpr[i], tpr[i]))
+            fpr_sorted, tpr_sorted = zip(*sorted_pairs)
+            mean_tpr += np.interp(
+                fpr_grid, fpr_sorted, tpr_sorted
+            )  # linear interpolation
+
+        # Average it and compute AUC
+        mean_tpr /= len(y_score)
+        roc_auc = _compute_area(mean_tpr.tolist()[::-1], fpr_grid.tolist()[::-1])
+        return roc_auc
     else:
         return _compute_multiclass_metric(
             metric=roc_auc_score,
             y_true=y_true,
             y_score=y_score,
             input_relation=input_relation,
             average=average,
             labels=labels,
             nbins=nbins,
         )
 
 
+def _check_labels(y_true, labels, input_relation):
+    distinct_values = _executeSQL(
+        query=f"SELECT DISTINCT {y_true} AS value FROM {input_relation}",
+        method="fetchall",
+    )
+    if set(item[0] for item in distinct_values) != set(labels):
+        raise ValueError("Mismatch between distinct values and provided labels")
+
+
 @save_verticapy_logs
 def prc_auc_score(
     y_true: str,
     y_score: Union[str, ArrayLike],
     input_relation: SQLRelation,
     average: Literal[None, "binary", "micro", "macro", "scores", "weighted"] = None,
     labels: Optional[ArrayLike] = None,
@@ -1935,23 +2164,56 @@
             y_score=_get_yscore(y_score, labels, pos_label),
             input_relation=input_relation,
             pos_label=pos_label,
             nbins=nbins,
             fun_sql_name="prc",
         )[1:]
         return _compute_area(precision, recall)
+    elif average == "micro":
+        _check_labels(y_true=y_true, labels=labels, input_relation=input_relation)
+        _, recall, precision = _compute_micro_multiclass_metric(
+            y_true, y_score, input_relation, labels, nbins, fun_sql_name="prc"
+        )
+        return _compute_area(precision, recall)
+    elif average == "macro":
+        _check_labels(y_true=y_true, labels=labels, input_relation=input_relation)
+        recall = {}
+        precision = {}
+        for i in range(len(y_score)):
+            recall[i], precision[i] = _compute_function_metrics(
+                y_true=y_true,
+                y_score=y_score[i],
+                input_relation=input_relation,
+                pos_label=labels[i],
+                nbins=nbins,
+                fun_sql_name="prc",
+            )[1:]
+
+        recall_grid = np.linspace(0.0, 1.0, nbins)
+        mean_precision = np.zeros_like(recall_grid)
+
+        for i in range(len(y_score)):
+            sorted_pairs = sorted(zip(recall[i], precision[i]))
+            recall_sorted, precision_sorted = zip(*sorted_pairs)
+            mean_precision += np.interp(recall_grid, recall_sorted, precision_sorted)
+        mean_precision /= len(y_score)
+        prc_auc = _compute_area(
+            mean_precision.tolist()[::-1], recall_grid.tolist()[::-1]
+        )
+        return prc_auc
     else:
         return _compute_multiclass_metric(
             metric=prc_auc_score,
             y_true=y_true,
             y_score=y_score,
             input_relation=input_relation,
             average=average,
             labels=labels,
             nbins=nbins,
+            fun_sql_name="prc",
         )
 
 
 # Logloss Metric.
 
 
 @save_verticapy_logs
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/metrics/plotting.py` & `verticapy-1.0.0b2/verticapy/machine_learning/metrics/plotting.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/metrics/regression.py` & `verticapy-1.0.0b2/verticapy/machine_learning/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/cv.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/cv.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/param_gen.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/param_gen.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/hp_tuning/plotting.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/hp_tuning/plotting.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/kmeans.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/kmeans.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,17 +117,32 @@
         loop = L
     i = None
     for i in loop:
         model_name = gen_tmp_name(schema=schema, name="kmeans")
         if use_kprototype:
             if init == "kmeanspp":
                 init = "random"
-            model = KPrototypes(model_name, i, init, max_iter, tol, gamma)
+            model = KPrototypes(
+                name=model_name,
+                overwrite_model=True,
+                n_cluster=i,
+                init=init,
+                max_iter=max_iter,
+                tol=tol,
+                gama=gamma,
+            )
         else:
-            model = KMeans(model_name, i, init, max_iter, tol)
+            model = KMeans(
+                name=model_name,
+                overwrite_model=True,
+                n_cluster=i,
+                init=init,
+                max_iter=max_iter,
+                tol=tol,
+            )
         model.fit(input_relation, X)
         score = model.elbow_score_
         if score > elbow_score_stop:
             return i
         model.drop()
     print(
         f"\u26A0 The K was not found. The last K (= {i}) "
@@ -229,17 +244,32 @@
         loop = tqdm(L)
     else:
         loop = L
     for i in loop:
         if use_kprototype:
             if init == "kmeanspp":
                 init = "random"
-            model = KPrototypes(model_name, i, init, max_iter, tol, gamma)
+            model = KPrototypes(
+                name=model_name,
+                overwrite_model=True,
+                n_cluster=i,
+                init=init,
+                max_iter=max_iter,
+                tol=tol,
+                gamma=gamma,
+            )
         else:
-            model = KMeans(model_name, i, init, max_iter, tol)
+            model = KMeans(
+                name=model_name,
+                overwrite_model=True,
+                n_cluster=i,
+                init=init,
+                max_iter=max_iter,
+                tol=tol,
+            )
         model.fit(input_relation, X)
         elbow_score += [float(model.elbow_score_)]
         between_cluster_ss += [float(model.between_cluster_ss_)]
         total_ss += [float(model.total_ss_)]
         total_within_cluster_ss += [float(model.total_within_cluster_ss_)]
         model.drop()
     if show:
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/model_validation.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/model_validation.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/norm.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/norm.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/ols.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/ols.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/statistical_tests/tsa.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/statistical_tests/tsa.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/model_selection/variables_selection.py` & `verticapy-1.0.0b2/verticapy/machine_learning/model_selection/variables_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,15 +409,15 @@
     Returns
     -------
     TableSample
         result of the stepwise.
     """
     X = format_type(X, dtype=list)
     assert len(X) >= 1, ValueError("Vector X must have at least one element.")
-    if not conf.get_option("overwrite_model"):
+    if not estimator.overwrite_model:
         estimator._is_already_stored(raise_error=True)
     avg = _executeSQL(
         f"SELECT /*+LABEL('stepwise')*/ AVG({y}) FROM {input_relation}",
         method="fetchfirstelem",
         print_time_sql=False,
     )
     fun = aic_score if criterion == "aic" else bic_score
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/__init__.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/clustering.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     Automatically creates k different groups with which to
     generalize the data.
 
     Parameters
     ----------
     name: str
         Name of the model.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same name
+        as an existing model overwrites the existing model.
     n_cluster: int, optional
         Number  of clusters. If empty, an optimal number  of
         clusters  are determined using multiple  k-means
         models.
     init: str / list, optional
         The method for finding the initial cluster  centers.
             kmeanspp : Uses   the    k-means++   method   to
@@ -116,14 +119,15 @@
 
     # System & Special Methods.
 
     @save_verticapy_logs
     def __init__(
         self,
         name: str,
+        overwrite_model: bool = False,
         n_cluster: Optional[int] = None,
         init: Union[Literal["kmeanspp", "random"], ArrayLike] = "kmeanspp",
         max_iter: int = 300,
         tol: float = 1e-4,
         use_kprototype: bool = False,
         gamma: float = 1.0,
         preprocess_data: bool = True,
@@ -132,14 +136,15 @@
             "normalize_min_cat": 0,
             "outliers_threshold": 3.0,
             "na_method": "drop",
         },
         print_info: bool = True,
     ) -> None:
         self.model_name = name
+        self.overwrite_model = overwrite_model
         self.parameters = {
             "n_cluster": n_cluster,
             "init": init,
             "max_iter": max_iter,
             "tol": tol,
             "use_kprototype": use_kprototype,
             "gamma": gamma,
@@ -157,15 +162,15 @@
         Parameters
         ----------
         input_relation: SQLRelation
             Training Relation.
         X: SQLColumns, optional
             List of the predictors.
         """
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         if self.parameters["print_info"]:
             print(f"\033[1m\033[4mStarting AutoClustering\033[0m\033[0m\n")
         if self.parameters["preprocess_data"]:
             model_preprocess = AutoDataPrep(**self.parameters["preprocess_dict"])
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/dataprep.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/dataprep.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 import verticapy._config.config as conf
 from verticapy._typing import NoneType, TimeInterval, SQLColumns, SQLRelation
 from verticapy._utils._gen import gen_tmp_name
 from verticapy._utils._sql._collect import save_verticapy_logs
 from verticapy._utils._sql._format import format_type
 from verticapy._utils._sql._sys import _executeSQL
 
+from verticapy.sql.drop import drop
+
 
 from verticapy.core.vdataframe.base import vDataFrame
 
 from verticapy.machine_learning.vertica.base import VerticaModel
 from verticapy.machine_learning.vertica.decomposition import PCA
 
 
@@ -39,14 +41,18 @@
     column type.
 
     Parameters
     ----------
     name: str, optional
         Name of the model in which to store the output
         relation in the Vertica database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     cat_method: str, optional
         Method for encoding categorical features. This
         can  be set to 'label' for label encoding  and
         'ooe' for One-Hot Encoding.
     num_method: str, optional
         [Only used for non-time series datasets]
         Method  for  encoding numerical features.  This
@@ -151,33 +157,31 @@
 
     # System & Special Methods.
 
     @save_verticapy_logs
     def __init__(
         self,
         name: Optional[str] = None,
+        overwrite_model: Optional[bool] = False,
         cat_method: Literal["label", "ooe"] = "ooe",
         num_method: Literal["same_freq", "same_width", "none"] = "none",
         nbins: int = 20,
         outliers_threshold: float = 4.0,
         na_method: Literal["auto", "drop"] = "auto",
         cat_topk: int = 10,
         normalize: bool = True,
         normalize_min_cat: int = 6,
         id_method: Literal["none", "drop"] = "drop",
         apply_pca: bool = False,
         rule: TimeInterval = "auto",
         identify_ts: bool = True,
         save: bool = True,
     ) -> None:
-        self.model_name = name
-        if not self.model_name:
-            self.model_name = gen_tmp_name(
-                schema=conf.get_option("temp_schema"), name="autodataprep"
-            )
+        super().__init__(name, overwrite_model)
+
         self.parameters = {
             "cat_method": cat_method,
             "num_method": num_method,
             "nbins": nbins,
             "outliers_threshold": outliers_threshold,
             "na_method": na_method,
             "cat_topk": cat_topk,
@@ -186,14 +190,23 @@
             "normalize_min_cat": normalize_min_cat,
             "apply_pca": apply_pca,
             "id_method": id_method,
             "identify_ts": identify_ts,
             "save": save,
         }
 
+    def drop(self) -> bool:
+        """
+        Drops the model from the Vertica database.
+        """
+        # it could be stored as a model or a table
+        dropped_model = super().drop()
+        dropped_table = drop(self.model_name, method="table")
+        return dropped_model or dropped_table
+
     # Model Fitting Method.
 
     def fit(
         self,
         input_relation: SQLRelation,
         X: Optional[SQLColumns] = None,
         ts: Optional[str] = None,
@@ -212,15 +225,15 @@
             Time series  vDataColumn used to order the
             data.
             The vDataColumn type must be date-like (date,
             datetime, timestamp...).
         by: SQLColumns, optional
             vDataColumns used in the partition.
         """
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         current_print_info = conf.get_option("print_info")
         conf.set_option("print_info", False)
         if by and not ts:
             raise ValueError("Parameter 'by' must be empty if 'ts' is not defined.")
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/automl/supervised.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/automl/supervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,18 @@
     Tests multiple models to find those that maximize
     the input score.
 
     Parameters
     ----------
     name: str
         Name of the model.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     estimator: list / 'native' / 'all' / 'fast' / object
         List  of Vertica  estimators with a fit  method.
         Alternatively,  you can specify 'native' for all
         native  Vertica models, 'all' for all  VerticaPy
         models, and 'fast' for quick modeling.
     estimator_type: str, optional
         Estimator Type.
@@ -247,14 +251,15 @@
 
     # System & Special Methods.
 
     @save_verticapy_logs
     def __init__(
         self,
         name: str,
+        overwrite_model: bool = False,
         estimator: Union[list, str] = "fast",
         estimator_type: Literal["auto", "regressor", "binary", "multi"] = "auto",
         metric: str = "auto",
         cv: int = 3,
         pos_label: Optional[PythonScalar] = None,
         cutoff: float = -1,
         nbins: int = 100,
@@ -268,14 +273,15 @@
         preprocess_data: bool = True,
         preprocess_dict: dict = {"identify_ts": False},
         print_info: bool = True,
     ) -> None:
         if optimized_grid not in [0, 1, 2]:
             raise ValueError("Optimized Grid must be an integer between 0 and 2.")
         self.model_name = name
+        self.overwrite_model = overwrite_model
         self.parameters = {
             "estimator": estimator,
             "estimator_type": estimator_type,
             "metric": metric,
             "cv": cv,
             "pos_label": pos_label,
             "cutoff": cutoff,
@@ -352,15 +358,15 @@
         input_relation: SQLRelation
             Training Relation.
         X: SQLColumns, optional
             List of the predictors.
         y: str, optional
             Response column.
         """
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         if isinstance(X, NoneType):
             if not y:
                 exclude_columns = []
             else:
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/base.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,21 +159,23 @@
                 x == col
             ):
                 return idx
 
     # System & Special Methods.
 
     @abstractmethod
-    def __init__(self) -> None:
+    def __init__(self, name: str, overwrite_model: bool = False) -> None:
         """Must be overridden in the child class"""
-        return None
-        # self.X = None
-        # self.parameters = {}
-        # for att in self._attributes:
-        #    setattr(self, att, None)
+        self.model_name = name
+        self.overwrite_model = overwrite_model
+
+        if not self.model_name:
+            self.model_name = gen_tmp_name(
+                schema=conf.get_option("temp_schema"), name=self._model_type
+            )
 
     def __repr__(self) -> str:
         """
         Returns the model Representation.
         """
         return f"<{self._model_type}>"
 
@@ -255,15 +257,15 @@
         )
         if res:
             model_type = res[0]
             res = True
         else:
             res = False
         if raise_error and res:
-            raise NameError(f"The model '{model_name}' already exists !")
+            raise NameError(f"The model '{model_name}' already exists!")
         if return_model_type:
             return model_type
         return res
 
     # Attributes Methods.
 
     def get_attributes(self, attr_name: Optional[str] = None) -> Any:
@@ -674,20 +676,24 @@
     def _vertica_predict_sql(self) -> str:
         """Must be overridden in child class"""
         raise NotImplementedError
 
     # System & Special Methods.
 
     @abstractmethod
-    def __init__(self) -> None:
+    def __init__(self, name: str, overwrite_model: bool = False) -> None:
         """Must be overridden in the child class"""
-        super().__init__()
+        super().__init__(name, overwrite_model)
         # self.test_relation = None
         # self.y = None
 
+    @property
+    def _model_category(self) -> Literal["SUPERVISED"]:
+        return "SUPERVISED"
+
     # Model Fitting Method.
 
     def fit(
         self,
         input_relation: SQLRelation,
         X: SQLColumns,
         y: str,
@@ -708,15 +714,15 @@
                 Relation used to test the model.
 
         Returns
         -------
         str
             model's summary.
         """
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         X = format_type(X, dtype=list)
         self.X = quote_ident(X)
         self.y = quote_ident(y)
         id_column, id_column_name = "", gen_tmp_name(name="id_column")
@@ -1199,17 +1205,17 @@
     @property
     def classes_(self) -> np.ndarray:
         return np.array([0, 1])
 
     # System & Special Methods.
 
     @abstractmethod
-    def __init__(self) -> None:
+    def __init__(self, name: str, overwrite_model: bool = False) -> None:
         """Must be overridden in the child class"""
-        super().__init__()
+        super().__init__(name, overwrite_model)
 
     # Attributes Methods.
 
     def _is_binary_classifier(self) -> Literal[True]:
         """
         Returns True if the model is a Binary Classifier.
         """
@@ -1733,17 +1739,17 @@
         )
 
 
 class MulticlassClassifier(Supervised):
     # System & Special Methods.
 
     @abstractmethod
-    def __init__(self) -> None:
+    def __init__(self, name: str, overwrite_model: bool = False) -> None:
         """Must be overridden in the child class"""
-        super().__init__()
+        super().__init__(name, overwrite_model)
         # self.classes_ = None
 
     def _check_pos_label(self, pos_label: PythonScalar) -> PythonScalar:
         """
         Checks if the pos_label is correct.
         """
         if isinstance(pos_label, NoneType) and self._is_binary_classifier():
@@ -2573,17 +2579,17 @@
         )
 
 
 class Regressor(Supervised):
     # System & Special Methods.
 
     @abstractmethod
-    def __init__(self) -> None:
+    def __init__(self, name: str, overwrite_model: bool = False) -> None:
         """Must be overridden in the child class"""
-        super().__init__()
+        super().__init__(name, overwrite_model)
 
     # Model Evaluation Methods.
 
     def regression_report(
         self,
         metrics: Union[
             str,
@@ -2792,17 +2798,21 @@
             return vdf.copy().eval(name, self.deploySQL(X=X))
 
 
 class Unsupervised(VerticaModel):
     # System & Special Methods.
 
     @abstractmethod
-    def __init__(self) -> None:
+    def __init__(self, name: str, overwrite_model: bool = False) -> None:
         """Must be overridden in the child class"""
-        super().__init__()
+        super().__init__(name, overwrite_model)
+
+    @property
+    def _model_category(self) -> Literal["UNSUPERVISED"]:
+        return "UNSUPERVISED"
 
     # Model Fitting Method.
 
     def fit(
         self, input_relation: SQLRelation, X: Optional[SQLColumns] = None
     ) -> Optional[str]:
         """
@@ -2817,15 +2827,15 @@
             numerical columns are used.
 
         Returns
         -------
         str
                 model's summary.
         """
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         id_column, id_column_name = "", gen_tmp_name(name="id_column")
         if self._model_type in ("BisectingKMeans", "IsolationForest") and isinstance(
             conf.get_option("random_state"), int
         ):
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/cluster.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,17 +68,17 @@
     def _vertica_predict_sql(self) -> str:
         """Must be overridden in child class"""
         raise NotImplementedError
 
     # System & Special Methods.
 
     @abstractmethod
-    def __init__(self) -> None:
+    def __init__(self, name: str, overwrite_model: bool = False) -> None:
         """Must be overridden in the child class"""
-        super().__init__()
+        super().__init__(name, overwrite_model)
 
     # Prediction / Transformation Methods.
 
     def predict(
         self,
         vdf: SQLRelation,
         X: Optional[SQLColumns] = None,
@@ -202,17 +202,21 @@
     which each observation belongs to the cluster with the
     nearest mean (cluster centers or cluster centroid),
     serving as a prototype of  the cluster.  This results
     in a partitioning of the data space into Voronoi cells.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of  the model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_cluster: int, optional
         Number of clusters
     init: str / list, optional
         The  method  used to find the initial  cluster
         centers.
                 kmeanspp : Uses   the  KMeans++  method   to
                        initialize the centers.
@@ -237,18 +241,14 @@
         return "KMEANS"
 
     @property
     def _vertica_predict_sql(self) -> Literal["APPLY_KMEANS"]:
         return "APPLY_KMEANS"
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLUSTERING"]:
         return "CLUSTERING"
 
     @property
     def _model_type(self) -> Literal["KMeans"]:
         return "KMeans"
 
@@ -266,22 +266,22 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         n_cluster: int = 8,
         init: Union[Literal["kmeanspp", "random"], list] = "kmeanspp",
         max_iter: int = 300,
         tol: float = 1e-4,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_cluster": n_cluster,
             "init": init,
             "max_iter": max_iter,
             "tol": tol,
         }
 
@@ -393,17 +393,21 @@
     Creates a KPrototypes object by using the Vertica
     k-prototypes algorithm. The algorithm combines
     the k-means and k-modes  algorithms  in order to
     handle both numerical and  categorical data.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the model. The model is stored in  the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_cluster: int, optional
         Number of clusters.
     init: str / list, optional
         The  method  used  to  find the  initial  cluster
         centers.
             random: The centers are initialized randomly.
         You  can  also provide a list of initial  cluster
@@ -452,22 +456,23 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         n_cluster: int = 8,
         init: Union[Literal["random"], list] = "random",
         max_iter: int = 300,
         tol: float = 1e-4,
         gamma: float = 1.0,
     ) -> None:
-        super().__init__(name)
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_cluster": n_cluster,
             "init": init,
             "max_iter": max_iter,
             "tol": tol,
             "gamma": gamma,
         }
@@ -512,17 +517,21 @@
     centroid),  which serves  as a  prototype  of the
     cluster.  This  results  in a partitioning of the
     data space into  Voronoi cells. Bisecting k-means
     combines k-means  and hierarchical clustering.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model.  The  model is stored in
         the database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_cluster: int, optional
         Number of clusters
     bisection_iterations: int, optional
         The number of iterations the bisecting KMeans
         algorithm  performs for each bisection  step.
         This   corresponds  to  how   many  times  a
         standalone  KMeans  algorithm runs  in  each
@@ -577,18 +586,14 @@
         return "BISECTING_KMEANS"
 
     @property
     def _vertica_predict_sql(self) -> Literal["APPLY_BISECTING_KMEANS"]:
         return "APPLY_BISECTING_KMEANS"
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLUSTERING"]:
         return "CLUSTERING"
 
     @property
     def _model_type(self) -> Literal["BisectingKMeans"]:
         return "BisectingKMeans"
 
@@ -611,25 +616,26 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         n_cluster: int = 8,
         bisection_iterations: int = 1,
         split_method: Literal["size", "sum_squares"] = "sum_squares",
         min_divisible_cluster_size: int = 2,
         distance_method: Literal["euclidean"] = "euclidean",
         init: Union[Literal["kmeanspp", "pseudo", "random"], list] = "kmeanspp",
         max_iter: int = 300,
         tol: float = 1e-4,
     ) -> None:
-        super().__init__(name)
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_cluster": n_cluster,
             "bisection_iterations": bisection_iterations,
             "split_method": str(split_method).lower(),
             "min_divisible_cluster_size": min_divisible_cluster_size,
             "distance_method": str(distance_method).lower(),
             "init": init,
@@ -804,18 +810,22 @@
                      can find non-linear clusters. It is a very
                      powerful algorithm for outlier  detection
                      and clustering. A table is created at
                      the end of the learning phase.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the model.  This is  not a  built-in
         model, so this name is  used to build the
         final table.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     eps: float, optional
         The radius of a  neighborhood with respect to
         some point.
     min_samples: int, optional
         Minimum number  of points required to  form a
         dense region.
     p: int, optional
@@ -853,18 +863,22 @@
     def _attributes(self) -> list[str]:
         return ["n_cluster_", "n_noise_", "p_"]
 
     # System & Special Methods.
 
     @save_verticapy_logs
     def __init__(
-        self, name: str, eps: float = 0.5, min_samples: int = 5, p: int = 2
+        self,
+        name: str = None,
+        overwrite_model: bool = False,
+        eps: float = 0.5,
+        min_samples: int = 5,
+        p: int = 2,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {"eps": eps, "min_samples": min_samples, "p": p}
 
     def drop(self) -> bool:
         """
         Drops the model from the Vertica database.
         """
         try:
@@ -901,15 +915,15 @@
             create the final relation.
         index: str, optional
             Index  used to identify each row  separately.
             It is highly  recommanded to have one already
             in the main table to avoid creating temporary
             tables.
         """
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         if isinstance(input_relation, vDataFrame):
             if isinstance(X, NoneType):
                 X = input_relation.numcol()
             input_relation = input_relation.current_relation()
@@ -1153,35 +1167,30 @@
         return ""
 
     @property
     def _vertica_predict_sql(self) -> Literal[""]:
         return ""
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLASSIFIER"]:
         return "CLASSIFIER"
 
     @property
     def _model_type(self) -> Literal["NearestCentroid"]:
         return "NearestCentroid"
 
     @property
     def _attributes(self) -> list[str]:
         return ["clusters_", "classes_", "p_"]
 
     # System & Special Methods.
 
     @save_verticapy_logs
-    def __init__(self, name: str, p: int = 2) -> None:
-        super().__init__()
-        self.model_name = name
+    def __init__(self, name: str = None, p: int = 2) -> None:
+        super().__init__(name)
         self.parameters = {"p": p}
 
     def drop(self) -> bool:
         """
         NearestCentroid models are not stored in the Vertica DB.
         """
         return False
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/decomposition.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/decomposition.py`

 * *Files 7% similar despite different names*

```diff
@@ -396,17 +396,21 @@
 class PCA(Decomposition):
     """
     Creates a PCA  (Principal Component Analysis) object
     using the Vertica PCA algorithm.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the  model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_components: int, optional
         The  number of  components to keep in the model.
         If  this value  is not provided,  all components
         are kept.  The  maximum number of components  is
         the number of  non-zero singular values returned
         by the internal call to SVD. This number is less
         than or equal to SVD  (number of columns, number
@@ -431,18 +435,14 @@
         return "APPLY_PCA"
 
     @property
     def _vertica_inverse_transform_sql(self) -> Literal["APPLY_INVERSE_PCA"]:
         return "APPLY_INVERSE_PCA"
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["DECOMPOSITION"]:
         return "DECOMPOSITION"
 
     @property
     def _model_type(self) -> Literal["PCA"]:
         return "PCA"
 
@@ -452,21 +452,21 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         n_components: int = 0,
         scale: bool = False,
         method: Literal["lapack"] = "lapack",
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_components": n_components,
             "scale": scale,
             "method": str(method).lower(),
         }
 
     # Attributes Methods.
@@ -511,17 +511,21 @@
     using  the Vertica PCA  algorithm. MCA is a PCA applied
     to a complete disjunctive table.  The  input relation is
     transformed to a TCDT (transformed  complete  disjunctive
     table) before applying the PCA.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model.  The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     """
 
     # Properties.
 
     @property
     def _is_native(self) -> Literal[False]:
         return False
@@ -539,31 +543,27 @@
         return "APPLY_PCA"
 
     @property
     def _vertica_inverse_transform_sql(self) -> Literal["APPLY_INVERSE_PCA"]:
         return "APPLY_INVERSE_PCA"
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["DECOMPOSITION"]:
         return "DECOMPOSITION"
 
     @property
     def _model_type(self) -> Literal["MCA"]:
         return "MCA"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
-    def __init__(self, name: str) -> None:
-        super().__init__(name)
+    def __init__(self, name: str = None, overwrite_model: bool = False) -> None:
+        super().__init__(name, overwrite_model)
         self.parameters = {}
 
     # Plotting Methods.
 
     def plot_contrib(
         self, dimension: int = 1, chart: Optional[PlottingObject] = None, **style_kwargs
     ) -> PlottingObject:
@@ -757,17 +757,21 @@
 class SVD(Decomposition):
     """
     Creates  an  SVD  (Singular  Value  Decomposition)
     object using the Vertica SVD algorithm.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_components: int, optional
         The number  of components to keep in the model.
         If this value  is not provided,  all components
         are kept.  The maximum number of  components is
         the number of non-zero singular values returned
         by  the  internal call to SVD. This  number  is
         less  than or equal to SVD (number of  columns,
@@ -788,18 +792,14 @@
         return "APPLY_SVD"
 
     @property
     def _vertica_inverse_transform_sql(self) -> Literal["APPLY_INVERSE_SVD"]:
         return "APPLY_INVERSE_SVD"
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["DECOMPOSITION"]:
         return "DECOMPOSITION"
 
     @property
     def _model_type(self) -> Literal["SVD"]:
         return "SVD"
 
@@ -808,18 +808,21 @@
         return ["vectors_", "values_", "explained_variance_"]
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
-        self, name: str, n_components: int = 0, method: Literal["lapack"] = "lapack"
+        self,
+        name: str = None,
+        overwrite_model: bool = False,
+        n_components: int = 0,
+        method: Literal["lapack"] = "lapack",
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_components": n_components,
             "method": str(method).lower(),
         }
 
     # Attributes Methods.
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/ensemble.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -348,28 +348,32 @@
 
 
 """
 Algorithms used for regression.
 """
 
 
-class RandomForestRegressor(RandomForest, Regressor):
+class RandomForestRegressor(Regressor, RandomForest):
     """
     Creates a RandomForestRegressor object using the
     Vertica RF_REGRESSOR function. It is an ensemble
     learning method for regression  that operates by
     constructing a multitude of decision trees  at
     training-time and outputting a class with the
     mode.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_estimators: int, optional
         The number of trees  in the forest, an integer
         between 1 and 1000, inclusive.
     max_features: int / str, optional
         The  number  of randomly chosen features  from
         which  to pick the best feature to split a
         given  tree node. It can be an integer or  one
@@ -412,18 +416,14 @@
         return "RF_REGRESSOR"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_RF_REGRESSOR"]:
         return "PREDICT_RF_REGRESSOR"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["RandomForestRegressor"]:
         return "RandomForestRegressor"
 
@@ -438,26 +438,26 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         n_estimators: int = 10,
         max_features: Union[Literal["auto", "max"], int] = "auto",
         max_leaf_nodes: PythonNumber = 1e9,
         sample: float = 0.632,
         max_depth: int = 5,
         min_samples_leaf: int = 1,
         min_info_gain: PythonNumber = 0.0,
         nbins: int = 32,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_estimators": n_estimators,
             "max_features": max_features,
             "max_leaf_nodes": int(max_leaf_nodes),
             "sample": sample,
             "max_depth": max_depth,
             "min_samples_leaf": min_samples_leaf,
@@ -501,24 +501,28 @@
         """
         if self.n_estimators_ == 1:
             return self.trees_[0]
         else:
             return mm.RandomForestRegressor(self.trees_)
 
 
-class XGBRegressor(XGBoost, Regressor):
+class XGBRegressor(Regressor, XGBoost):
     """
     Creates  an  XGBRegressor  object  using the  Vertica
     XGB_REGRESSOR algorithm.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the  model.  The  model  is  stored
         in the DB.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     max_ntree: int, optional
         Maximum  number  of trees that  can be  created.
     max_depth: int, optional
         Maximum depth  of each tree, an  integer between 1
         and 20, inclusive.
     nbins: int, optional
         Number of bins used to find splits in each column,
@@ -567,18 +571,14 @@
         return "XGB_REGRESSOR"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_XGB_REGRESSOR"]:
         return "PREDICT_XGB_REGRESSOR"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["XGBRegressor"]:
         return "XGBRegressor"
 
@@ -595,29 +595,29 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         max_ntree: int = 10,
         max_depth: int = 5,
         nbins: int = 32,
         split_proposal_method: Literal["local", "global"] = "global",
         tol: float = 0.001,
         learning_rate: float = 0.1,
         min_split_loss: float = 0.0,
         weight_reg: float = 0.0,
         sample: float = 1.0,
         col_sample_by_tree: float = 1.0,
         col_sample_by_node: float = 1.0,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         params = {
             "max_ntree": max_ntree,
             "max_depth": max_depth,
             "nbins": nbins,
             "split_proposal_method": str(split_proposal_method).lower(),
             "tol": tol,
             "learning_rate": learning_rate,
@@ -676,27 +676,31 @@
 
 
 """
 Algorithms used for classification.
 """
 
 
-class RandomForestClassifier(RandomForest, MulticlassClassifier):
+class RandomForestClassifier(MulticlassClassifier, RandomForest):
     """
     Creates a RandomForestClassifier object using the
     Vertica  RF_CLASSIFIER function. It is an ensemble
     learning method for classification that operates
     by constructing a multitude of decision trees  at
     training-time and outputting a class with the mode.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_estimators: int, optional
         The number of trees  in the forest, an integer
         between 1 and 1000, inclusive.
     max_features: int / str, optional
         The  number  of randomly chosen features  from
         which  to pick the best feature to split  a
         given  tree node. It can be an integer or  one
@@ -739,18 +743,14 @@
         return "RF_CLASSIFIER"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_RF_CLASSIFIER"]:
         return "PREDICT_RF_CLASSIFIER"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLASSIFIER"]:
         return "CLASSIFIER"
 
     @property
     def _model_type(self) -> Literal["RandomForestClassifier"]:
         return "RandomForestClassifier"
 
@@ -766,26 +766,26 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         n_estimators: int = 10,
         max_features: Union[Literal["auto", "max"], int] = "auto",
         max_leaf_nodes: PythonNumber = 1e9,
         sample: float = 0.632,
         max_depth: int = 5,
         min_samples_leaf: int = 1,
         min_info_gain: PythonNumber = 0.0,
         nbins: int = 32,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_estimators": n_estimators,
             "max_features": max_features,
             "max_leaf_nodes": int(max_leaf_nodes),
             "sample": sample,
             "max_depth": max_depth,
             "min_samples_leaf": min_samples_leaf,
@@ -845,24 +845,28 @@
         """
         if self.n_estimators_ == 1:
             return self.trees_[0]
         else:
             return mm.RandomForestClassifier(self.trees_, self.classes_)
 
 
-class XGBClassifier(XGBoost, MulticlassClassifier):
+class XGBClassifier(MulticlassClassifier, XGBoost):
     """
     Creates  an  XGBClassifier  object using the  Vertica
     XGB_CLASSIFIER algorithm.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the  model. The model  is  stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     max_ntree: int, optional
         Maximum  number  of trees that can be  created.
     max_depth: int, optional
         Maximum depth  of each tree, an  integer between 1
         and 20, inclusive.
     nbins: int, optional
         Number of bins used to find splits in each column,
@@ -911,18 +915,14 @@
         return "XGB_CLASSIFIER"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_XGB_CLASSIFIER"]:
         return "PREDICT_XGB_CLASSIFIER"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLASSIFIER"]:
         return "CLASSIFIER"
 
     @property
     def _model_type(self) -> Literal["XGBClassifier"]:
         return "XGBClassifier"
 
@@ -940,29 +940,29 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         max_ntree: int = 10,
         max_depth: int = 5,
         nbins: int = 32,
         split_proposal_method: Literal["local", "global"] = "global",
         tol: float = 0.001,
         learning_rate: float = 0.1,
         min_split_loss: float = 0.0,
         weight_reg: float = 0.0,
         sample: float = 1.0,
         col_sample_by_tree: float = 1.0,
         col_sample_by_node: float = 1.0,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         params = {
             "max_ntree": max_ntree,
             "max_depth": max_depth,
             "nbins": nbins,
             "split_proposal_method": str(split_proposal_method).lower(),
             "tol": tol,
             "learning_rate": learning_rate,
@@ -1057,17 +1057,21 @@
 class IsolationForest(Clustering, Tree):
     """
     Creates an IsolationForest object using the Vertica
     IFOREST algorithm.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of  the model. The model  is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_estimators: int, optional
         The number  of  trees in the forest,  an integer
         between 1 and 1000, inclusive.
     max_depth: int, optional
         Maximum  depth of each tree,  an integer between
         1 and 100, inclusive.
     nbins: int, optional
@@ -1092,18 +1096,14 @@
         return "IFOREST"
 
     @property
     def _vertica_predict_sql(self) -> Literal["APPLY_IFOREST"]:
         return "APPLY_IFOREST"
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["ANOMALY_DETECTION"]:
         return "ANOMALY_DETECTION"
 
     @property
     def _model_type(self) -> Literal["IsolationForest"]:
         return "IsolationForest"
 
@@ -1113,23 +1113,23 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         n_estimators: int = 100,
         max_depth: int = 10,
         nbins: int = 32,
         sample: float = 0.632,
         col_sample_by_tree: float = 1.0,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_estimators": n_estimators,
             "max_depth": max_depth,
             "nbins": nbins,
             "sample": sample,
             "col_sample_by_tree": col_sample_by_tree,
         }
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/linear_model.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/linear_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -289,17 +289,21 @@
     Linear Regression  algorithm. The Elastic Net
     is a regularized regression method that linearly
     combines the L1 and L2 penalties of the Lasso and
     Ridge methods.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the  model.  The model is stored in
         the database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     tol: float, optional
         Determines  whether the algorithm has reached
         the specified accuracy result.
     C: PythonNumber, optional
         The regularization parameter value. The value
         must be zero or non-negative.
     max_iter: int, optional
@@ -329,41 +333,37 @@
         return "LINEAR_REG"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_LINEAR_REG"]:
         return "PREDICT_LINEAR_REG"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["LinearRegression"]:
         return "LinearRegression"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         tol: float = 1e-6,
         C: PythonNumber = 1.0,
         max_iter: int = 100,
         solver: Literal["newton", "bfgs", "cgd"] = "cgd",
         l1_ratio: float = 0.5,
         fit_intercept: bool = True,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         if vertica_version()[0] < 12 and not fit_intercept:
             raise VersionError(
                 "The parameter 'fit_intercept' can be activated for "
                 "Vertica versions greater or equal to 12."
             )
         self.parameters = {
             "penalty": "enet",
@@ -381,17 +381,21 @@
     Creates  a  Lasso  object using the  Vertica
     Linear  Regression  algorithm.
     Lasso is a regularized regression method
     that uses an L1 penalty.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The  model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     tol: float, optional
         Determines  whether the  algorithm has reached
         the specified accuracy result.
     C: PythonNumber, optional
         The regularization  parameter value. The value
         must be zero or non-negative.
     max_iter: int, optional
@@ -418,40 +422,36 @@
         return "LINEAR_REG"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_LINEAR_REG"]:
         return "PREDICT_LINEAR_REG"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["LinearRegression"]:
         return "LinearRegression"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         tol: float = 1e-6,
         C: PythonNumber = 1.0,
         max_iter: int = 100,
         solver: Literal["newton", "bfgs", "cgd"] = "cgd",
         fit_intercept: bool = True,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         if vertica_version()[0] < 12 and not fit_intercept:
             raise VersionError(
                 "The parameter 'fit_intercept' can be activated for "
                 "Vertica versions greater or equal to 12."
             )
         self.parameters = {
             "penalty": "l1",
@@ -466,17 +466,21 @@
 class LinearRegression(Regressor, LinearModel):
     """
     Creates a LinearRegression object using the Vertica
     Linear Regression algorithm.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The  model is stored  in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     tol: float, optional
         Determines whether the  algorithm has reached the
         specified accuracy result.
     max_iter: int, optional
         Determines the  maximum number of  iterations the
         algorithm performs before achieving the specified
         accuracy result.
@@ -499,39 +503,35 @@
         return "LINEAR_REG"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_LINEAR_REG"]:
         return "PREDICT_LINEAR_REG"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["LinearRegression"]:
         return "LinearRegression"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         tol: float = 1e-6,
         max_iter: int = 100,
         solver: Literal["newton", "bfgs"] = "newton",
         fit_intercept: bool = True,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         if vertica_version()[0] < 12 and not fit_intercept:
             raise VersionError(
                 "The parameter 'fit_intercept' can be activated for "
                 "Vertica versions greater or equal to 12."
             )
         self.parameters = {
             "penalty": "none",
@@ -547,17 +547,21 @@
     Creates  a  Ridge  object using the  Vertica
     Linear  Regression  algorithm.
     Ridge is a regularized regression method
     which uses an L2 penalty.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     tol: float, optional
         Determines whether  the algorithm has reached
         the specified accuracy result.
     C: PythonNumber, optional
         The regularization parameter value. The value
         must be zero or non-negative.
     max_iter: int, optional
@@ -583,40 +587,36 @@
         return "LINEAR_REG"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_LINEAR_REG"]:
         return "PREDICT_LINEAR_REG"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["LinearRegression"]:
         return "LinearRegression"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         tol: float = 1e-6,
         C: PythonNumber = 1.0,
         max_iter: int = 100,
         solver: Literal["newton", "bfgs"] = "newton",
         fit_intercept: bool = True,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         if vertica_version()[0] < 12 and not fit_intercept:
             raise VersionError(
                 "The parameter 'fit_intercept' can be activated for "
                 "Vertica versions greater or equal to 12."
             )
         self.parameters = {
             "penalty": "l2",
@@ -636,17 +636,21 @@
 class LogisticRegression(BinaryClassifier, LinearModelClassifier):
     """
     Creates a LogisticRegression  object using the Vertica
     Logistic Regression algorithm.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model.  The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     penalty: str, optional
         Determines the method of regularization.
             None : No Regularization.
             l1   : L1 Regularization.
             l2   : L2 Regularization.
             enet : Combination between L1 and L2.
     tol: float, optional
@@ -682,44 +686,40 @@
         return "LOGISTIC_REG"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_LOGISTIC_REG"]:
         return "PREDICT_LOGISTIC_REG"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLASSIFIER"]:
         return "CLASSIFIER"
 
     @property
     def _model_type(self) -> Literal["LogisticRegression"]:
         return "LogisticRegression"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         penalty: Literal["none", "l1", "l2", "enet", None] = "none",
         tol: float = 1e-6,
         C: PythonNumber = 1.0,
         max_iter: int = 100,
         solver: Literal["newton", "bfgs", "cgd"] = "newton",
         l1_ratio: float = 0.5,
         fit_intercept: bool = True,
     ) -> None:
-        super().__init__()
+        super().__init__(name, overwrite_model)
         penalty = str(penalty).lower()
         solver = str(solver).lower()
-        self.model_name = name
         if vertica_version()[0] < 12 and not fit_intercept:
             raise VersionError(
                 "The parameter 'fit_intercept' can be activated for "
                 "Vertica versions greater or equal to 12."
             )
         self.parameters = {
             "penalty": penalty,
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/model_management.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/model_management.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/naive_bayes.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/naive_bayes.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,17 +39,21 @@
     Naive  Bayes  algorithm.  It is a "probabilistic
     classifier"  based  on  applying Bayes' theorem
     with strong (naïve) independence assumptions
     between the features.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of  the  model.  The  model is stored
         in the database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     alpha: float, optional
         A  float  that  specifies  use  of  Laplace
         smoothing if the event model is categorical,
         multinomial, or Bernoulli.
     nbtype: str, optional
         Naive Bayes type.
         - auto        : Vertica NaiveBayes objects
@@ -78,18 +82,14 @@
         return "NAIVE_BAYES"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_NAIVE_BAYES"]:
         return "PREDICT_NAIVE_BAYES"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLASSIFIER"]:
         return "CLASSIFIER"
 
     @property
     def _model_type(self) -> Literal["NaiveBayes"]:
         return "NaiveBayes"
 
@@ -99,22 +99,22 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         alpha: PythonNumber = 1.0,
         nbtype: Literal[
             "auto", "bernoulli", "categorical", "multinomial", "gaussian"
         ] = "auto",
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {"alpha": alpha, "nbtype": str(nbtype).lower()}
 
     # Attributes Methods.
 
     def _compute_attributes(self) -> None:
         """
         Computes the model's attributes.
@@ -201,30 +201,36 @@
             self.classes_,
         )
 
 
 class BernoulliNB(NaiveBayes):
     """NaiveBayes with parameter nbtype = 'bernoulli'"""
 
-    def __init__(self, name: str, alpha: float = 1.0) -> None:
-        super().__init__(name, alpha, nbtype="bernoulli")
+    def __init__(
+        self, name: str = None, overwrite_model: bool = False, alpha: float = 1.0
+    ) -> None:
+        super().__init__(name, overwrite_model, alpha, nbtype="bernoulli")
 
 
 class CategoricalNB(NaiveBayes):
     """NaiveBayes with parameter nbtype = 'categorical'"""
 
-    def __init__(self, name: str, alpha: float = 1.0) -> None:
-        super().__init__(name, alpha, nbtype="categorical")
+    def __init__(
+        self, name: str = None, overwrite_model: bool = False, alpha: float = 1.0
+    ) -> None:
+        super().__init__(name, overwrite_model, alpha, nbtype="categorical")
 
 
 class GaussianNB(NaiveBayes):
     """NaiveBayes with parameter nbtype = 'gaussian'"""
 
-    def __init__(self, name: str) -> None:
-        super().__init__(name, nbtype="gaussian")
+    def __init__(self, name: str = None, overwrite_model: bool = False) -> None:
+        super().__init__(name, overwrite_model, nbtype="gaussian")
 
 
 class MultinomialNB(NaiveBayes):
     """NaiveBayes with parameter nbtype = 'multinomial'"""
 
-    def __init__(self, name: str, alpha: float = 1.0) -> None:
-        super().__init__(name, alpha, nbtype="multinomial")
+    def __init__(
+        self, name: str = None, overwrite_model: bool = False, alpha: float = 1.0
+    ) -> None:
+        super().__init__(name, overwrite_model, alpha, nbtype="multinomial")
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/neighbors.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/neighbors.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,35 +100,30 @@
         return ""
 
     @property
     def _vertica_predict_sql(self) -> Literal[""]:
         return ""
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["KNeighborsRegressor"]:
         return "KNeighborsRegressor"
 
     @property
     def _attributes(self) -> list[str]:
         return ["n_neighbors_", "p_"]
 
     # System & Special Methods.
 
     @save_verticapy_logs
-    def __init__(self, name: str, n_neighbors: int = 5, p: int = 2) -> None:
-        super().__init__()
-        self.model_name = name
+    def __init__(self, name: str = None, n_neighbors: int = 5, p: int = 2) -> None:
+        super().__init__(name)
         self.parameters = {"n_neighbors": n_neighbors, "p": p}
 
     def drop(self) -> bool:
         """
         KNN models are not stored in the Vertica DB.
         """
         return False
@@ -316,35 +311,30 @@
         return ""
 
     @property
     def _vertica_predict_sql(self) -> Literal[""]:
         return ""
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLASSIFIER"]:
         return "CLASSIFIER"
 
     @property
     def _model_type(self) -> Literal["KNeighborsClassifier"]:
         return "KNeighborsClassifier"
 
     @property
     def _attributes(self) -> list[str]:
         return ["classes_", "n_neighbors_", "p_"]
 
     # System & Special Methods.
 
     @save_verticapy_logs
-    def __init__(self, name: str, n_neighbors: int = 5, p: int = 2) -> None:
-        super().__init__()
-        self.model_name = name
+    def __init__(self, name: str = None, n_neighbors: int = 5, p: int = 2) -> None:
+        super().__init__(name)
         self.parameters = {"n_neighbors": n_neighbors, "p": p}
 
     def drop(self) -> bool:
         """
         KNN models are not stored in the Vertica DB.
         """
         return False
@@ -733,17 +723,21 @@
     """
     [Beta Version]
     Creates a KernelDensity object.
     This object uses pure SQL to compute the final score.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. This is not a built-in model, so
         this name is used  to build the final table.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     bandwidth: PythonNumber, optional
         The bandwidth of the kernel.
     kernel: str, optional
         The kernel used during the learning phase.
             gaussian  : Gaussian Kernel.
             logistic  : Logistic Kernel.
             sigmoid   : Sigmoid Kernel.
@@ -783,14 +777,16 @@
     def _vertica_fit_sql(self) -> Literal["RF_REGRESSOR"]:
         return "RF_REGRESSOR"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_RF_REGRESSOR"]:
         return "PREDICT_RF_REGRESSOR"
 
+    # This is an exception. Although KernelDensity is a subclass of Regressor,
+    # but it is UNSUPERVISED.
     @property
     def _model_category(self) -> Literal["UNSUPERVISED"]:
         return "UNSUPERVISED"
 
     @property
     def _model_subcategory(self) -> Literal["PREPROCESSING"]:
         return "PREPROCESSING"
@@ -800,27 +796,27 @@
         return "KernelDensity"
 
     # System & Special Methods.
 
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         bandwidth: PythonNumber = 1.0,
         kernel: Literal["gaussian", "logistic", "sigmoid", "silverman"] = "gaussian",
         p: int = 2,
         max_leaf_nodes: PythonNumber = 1e9,
         max_depth: int = 5,
         min_samples_leaf: int = 1,
         nbins: int = 5,
         xlim: Optional[list] = None,
         **kwargs,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "nbins": nbins,
             "p": p,
             "bandwidth": bandwidth,
             "kernel": str(kernel).lower(),
             "max_leaf_nodes": int(max_leaf_nodes),
             "max_depth": int(max_depth),
@@ -957,15 +953,15 @@
         input_relation: SQLRelation
             Training relation.
         X: list, optional
             List of the predictors.
         """
         X = format_type(X, dtype=list)
         X = quote_ident(X)
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         if isinstance(input_relation, vDataFrame):
             if not X:
                 X = input_relation.numcol()
             vdf = input_relation
@@ -1156,18 +1152,22 @@
                      distance,  it  is  highly  sensitive  to
                      unnormalized data.
                      A  table  is created at the  end of
                      the learning phase.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the  model.  This is not a  built-in
         model, so this name is used to build the
         final table.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     n_neighbors: int, optional
         Number of neighbors to consider when computing
         the score.
     p: int, optional
         The p of the p-distances (distance metric used
         during the model computation).
     """
@@ -1201,17 +1201,22 @@
     @property
     def _attributes(self) -> list[str]:
         return ["n_neighbors_", "p_", "n_errors_", "cnt_"]
 
     # System & Special Methods.
 
     @save_verticapy_logs
-    def __init__(self, name: str, n_neighbors: int = 20, p: int = 2) -> None:
-        super().__init__()
-        self.model_name = name
+    def __init__(
+        self,
+        name: str = None,
+        overwrite_model: bool = False,
+        n_neighbors: int = 20,
+        p: int = 2,
+    ) -> None:
+        super().__init__(name, overwrite_model)
         self.parameters = {"n_neighbors": n_neighbors, "p": p}
 
     def drop(self) -> bool:
         """
         Drops the model from the Vertica database.
         """
         try:
@@ -1263,15 +1268,15 @@
                 Index  used to seperately identify each row.
             To avoid the creation of temporary tables,
             it is recommended that you already have an
             index in the main table.
         """
         X, key_columns = format_type(X, key_columns, dtype=list)
         X = quote_ident(X)
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         self.key_columns = quote_ident(key_columns)
         if isinstance(input_relation, vDataFrame):
             self.input_relation = input_relation.current_relation()
             if not X:
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/pipeline.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     Parameters
     ----------
     steps: list
         List of (name, transform)  tuples (implementing
         fit/transform) that  are chained, in  the order
         in which they are chained, where the last object
         is an estimator.
+    overwrite_model: bool, optional
+        If set to True, training a model in the pipeline with the same
+        name as an existing model overwrites the existing model.
     """
 
     # Properties.
 
     @property
     def _is_native(self) -> Literal[False]:
         return False
@@ -79,16 +82,17 @@
     @property
     def _attributes(self) -> None:
         raise NotImplementedError
 
     # System & Special Methods.
 
     @save_verticapy_logs
-    def __init__(self, steps: list) -> None:
+    def __init__(self, steps: list, overwrite_model: bool = False) -> None:
         self.steps = []
+        self.overwrite_model = overwrite_model
         for idx, s in enumerate(steps):
             if len(s) != 2:
                 raise ValueError(
                     "The steps of the Pipeline must be composed of 2 elements "
                     f"(name, transform). Found {len(s)}."
                 )
             elif not isinstance(s[0], str):
@@ -190,15 +194,15 @@
             model.
         """
         X = format_type(X, dtype=list)
         if isinstance(input_relation, str):
             vdf = vDataFrame(input_relation)
         else:
             vdf = input_relation
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         X_new = copy.deepcopy(X)
         current_vdf = vdf
         for idx, step in enumerate(self.steps):
             if (idx == len(self.steps) - 1) and (y):
                 step[1].fit(current_vdf, X_new, y, test_relation)
             else:
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/preprocessing.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -403,16 +403,20 @@
 class CountVectorizer(VerticaModel):
     """
     Creates a Text Index that counts the occurences
     of each word in the data.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     lowercase: bool, optional
         Converts  all  the elements to lowercase  before
         processing.
     max_df: float, optional
         Keeps  the words that represent less than  this
         float in the total dictionary distribution.
     min_df: float, optional
@@ -463,24 +467,24 @@
         return ["stop_words_", "vocabulary_", "n_errors_"]
 
     # System & Special Methods.
 
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         lowercase: bool = True,
         max_df: float = 1.0,
         min_df: float = 0.0,
         max_features: int = -1,
         ignore_special: bool = True,
         max_text_size: int = 2000,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "lowercase": lowercase,
             "max_df": max_df,
             "min_df": min_df,
             "max_features": max_features,
             "ignore_special": ignore_special,
             "max_text_size": max_text_size,
@@ -570,15 +574,15 @@
         input_relation: SQLRelation
                 Training relation.
         X: SQLColumns
                 List of the predictors. If empty, all the
             columns are used.
         """
         X = format_type(X, dtype=list)
-        if conf.get_option("overwrite_model"):
+        if self.overwrite_model:
             self.drop()
         else:
             self._is_already_stored(raise_error=True)
         if isinstance(input_relation, vDataFrame):
             if isinstance(X, NoneType):
                 X = input_relation.get_columns()
             self.input_relation = input_relation.current_relation()
@@ -641,16 +645,20 @@
 
 class Scaler(Preprocessing):
     """
     Creates a Vertica Scaler object.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     method: str, optional
         Method used to normalize.
                 zscore        : Normalization   using   the   Z-Score.
                             (x - avg) / std
                 robust_zscore : Normalization using the Robust Z-Score.
                                 (x - median) / (1.4826 * mad)
                 minmax        : Normalization  using  the  Min  &  Max.
@@ -668,18 +676,14 @@
         return "APPLY_NORMALIZE"
 
     @property
     def _vertica_inverse_transform_sql(self) -> Literal["REVERSE_NORMALIZE"]:
         return "REVERSE_NORMALIZE"
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["PREPROCESSING"]:
         return "PREPROCESSING"
 
     @property
     def _model_type(self) -> Literal["Scaler"]:
         return "Scaler"
 
@@ -693,18 +697,20 @@
             return ["mean_", "std_"]
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
-        self, name: str, method: Literal["zscore", "robust_zscore", "minmax"] = "zscore"
+        self,
+        name: str = None,
+        overwrite_model: bool = False,
+        method: Literal["zscore", "robust_zscore", "minmax"] = "zscore",
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {"method": str(method).lower()}
 
     # Attributes Methods.
 
     def _compute_attributes(self) -> None:
         """
         Computes the model's attributes.
@@ -738,53 +744,57 @@
 class StandardScaler(Scaler):
     """i.e. Scaler with param method = 'zscore'"""
 
     @property
     def _attributes(self) -> list[str]:
         return ["mean_", "std_"]
 
-    def __init__(self, name: str) -> None:
-        super().__init__(name, "zscore")
+    def __init__(self, name: str = None, overwrite_model: bool = False) -> None:
+        super().__init__(name, overwrite_model, "zscore")
 
 
 class RobustScaler(Scaler):
     """i.e. Scaler with param method = 'robust_zscore'"""
 
     @property
     def _attributes(self) -> list[str]:
         return ["median_", "mad_"]
 
-    def __init__(self, name: str) -> None:
-        super().__init__(name, "robust_zscore")
+    def __init__(self, name: str = None, overwrite_model: bool = False) -> None:
+        super().__init__(name, overwrite_model, "robust_zscore")
 
 
 class MinMaxScaler(Scaler):
     """i.e. Scaler with param method = 'minmax'"""
 
     @property
     def _attributes(self) -> list[str]:
         return ["min_", "max_"]
 
-    def __init__(self, name: str) -> None:
-        super().__init__(name, "minmax")
+    def __init__(self, name: str = None, overwrite_model: bool = False) -> None:
+        super().__init__(name, overwrite_model, "minmax")
 
 
 """
 Algorithms used for encoding.
 """
 
 
 class OneHotEncoder(Preprocessing):
     """
     Creates a Vertica OneHotEncoder object.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     extra_levels: dict, optional
         Additional levels in each  category that are not
         in the input relation.
     drop_first: bool, optional
         If set to True,  treats the first level of the
         categorical variable as the reference level.
         Otherwise, every level of the categorical variable
@@ -827,18 +837,14 @@
         return "APPLY_ONE_HOT_ENCODER"
 
     @property
     def _vertica_inverse_transform_sql(self) -> Literal[""]:
         return ""
 
     @property
-    def _model_category(self) -> Literal["UNSUPERVISED"]:
-        return "UNSUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["PREPROCESSING"]:
         return "PREPROCESSING"
 
     @property
     def _model_type(self) -> Literal["OneHotEncoder"]:
         return "OneHotEncoder"
 
@@ -848,24 +854,24 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         extra_levels: Optional[dict] = None,
         drop_first: bool = True,
         ignore_null: bool = True,
         separator: str = "_",
         column_naming: Literal["indices", "values", "values_relaxed"] = "indices",
         null_column_name: str = "null",
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "extra_levels": format_type(extra_levels, dtype=dict),
             "drop_first": drop_first,
             "ignore_null": ignore_null,
             "separator": separator,
             "column_naming": str(column_naming).lower(),
             "null_column_name": null_column_name,
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/svm.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/svm.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,17 +39,21 @@
     Creates  a  LinearSVR  object  using the Vertica  SVM
     (Support Vector Machine)  algorithm.  This  algorithm
     finds the hyperplane used to approximate distribution
     of the data.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The model is stored in
         the database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     tol: float, optional
         Tolerance for stopping criteria. This is
         used to control accuracy.
     C: float, optional
         Weight  for  misclassification  cost. The
         algorithm minimizes the regularization
         cost and the misclassification cost.
@@ -83,41 +87,37 @@
         return "SVM_REGRESSOR"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_SVM_REGRESSOR"]:
         return "PREDICT_SVM_REGRESSOR"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["REGRESSOR"]:
         return "REGRESSOR"
 
     @property
     def _model_type(self) -> Literal["LinearSVR"]:
         return "LinearSVR"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         tol: float = 1e-4,
         C: float = 1.0,
         intercept_scaling: float = 1.0,
         intercept_mode: Literal["regularized", "unregularized"] = "regularized",
         acceptable_error_margin: float = 0.1,
         max_iter: int = 100,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "tol": tol,
             "C": C,
             "intercept_scaling": intercept_scaling,
             "intercept_mode": str(intercept_mode).lower(),
             "acceptable_error_margin": acceptable_error_margin,
             "max_iter": max_iter,
@@ -148,17 +148,21 @@
     categories, an SVM training algorithm builds a
     model that assigns new examples to one category
     or  the other,  making it  a  non-probabilistic
     binary linear classifier.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name  of the  model. The model is stored
         in the database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     tol: float, optional
         Tolerance for stopping criteria. This is
         used to control accuracy.
     C: float, optional
         Weight for misclassification cost.  The
         algorithm minimizes the regularization cost
         and the misclassification cost.
@@ -195,41 +199,37 @@
         return "SVM_CLASSIFIER"
 
     @property
     def _vertica_predict_sql(self) -> Literal["PREDICT_SVM_CLASSIFIER"]:
         return "PREDICT_SVM_CLASSIFIER"
 
     @property
-    def _model_category(self) -> Literal["SUPERVISED"]:
-        return "SUPERVISED"
-
-    @property
     def _model_subcategory(self) -> Literal["CLASSIFIER"]:
         return "CLASSIFIER"
 
     @property
     def _model_type(self) -> Literal["LinearSVC"]:
         return "LinearSVC"
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         tol: float = 1e-4,
         C: float = 1.0,
         intercept_scaling: float = 1.0,
         intercept_mode: Literal["regularized", "unregularized"] = "regularized",
         class_weight: Union[Literal["auto", "none"], list] = [1, 1],
         max_iter: int = 100,
     ) -> None:
-        super().__init__()
-        self.model_name = name
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "tol": tol,
             "C": C,
             "intercept_scaling": intercept_scaling,
             "intercept_mode": str(intercept_mode).lower(),
             "class_weight": class_weight,
             "max_iter": max_iter,
```

### Comparing `verticapy-1.0.0b1/verticapy/machine_learning/vertica/tree.py` & `verticapy-1.0.0b2/verticapy/machine_learning/vertica/tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,17 +32,21 @@
 
 class DecisionTreeRegressor(RandomForestRegressor):
     """
     A DecisionTreeRegressor consisting of a single tree.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     max_features: str / int, optional
         The number of randomly  chosen features from which
         to pick the best feature  to split on a given tree
         node.  It  can  be  an integer  or one of the  two
         following methods:
             auto : square root of the total number of
                    predictors.
@@ -70,23 +74,24 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         max_features: Union[Literal["auto", "max"], int] = "auto",
         max_leaf_nodes: PythonNumber = 1e9,
         max_depth: int = 100,
         min_samples_leaf: int = 1,
         min_info_gain: PythonNumber = 0.0,
         nbins: int = 32,
     ) -> None:
-        super().__init__(name)
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_estimators": 1,
             "max_features": max_features,
             "max_leaf_nodes": int(max_leaf_nodes),
             "sample": 1.0,
             "max_depth": max_depth,
             "min_samples_leaf": min_samples_leaf,
@@ -99,25 +104,29 @@
     """
     A regressor that overfits the training data.
     These models are typically used as a control
     to compare with your other models.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The model is stored
         in the database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     """
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
-    def __init__(self, name: str) -> None:
-        super().__init__(name)
+    def __init__(self, name: str = None, overwrite_model: bool = False) -> None:
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_estimators": 1,
             "max_features": "max",
             "max_leaf_nodes": int(1e9),
             "sample": 1.0,
             "max_depth": 100,
             "min_samples_leaf": 1,
@@ -133,17 +142,21 @@
 
 class DecisionTreeClassifier(RandomForestClassifier):
     """
     A DecisionTreeClassifier consisting of a single tree.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of the model. The model is stored in the
         database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     max_features: str / int, optional
         The number of randomly  chosen features from which
         to pick the best feature  to split on a given tree
         node.  It  can  be  an integer  or one of the  two
         following methods.
             auto : square root of the total number of
                    predictors.
@@ -171,23 +184,24 @@
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
     def __init__(
         self,
-        name: str,
+        name: str = None,
+        overwrite_model: bool = False,
         max_features: Union[Literal["auto", "max"], int] = "auto",
         max_leaf_nodes: PythonNumber = 1e9,
         max_depth: int = 100,
         min_samples_leaf: int = 1,
         min_info_gain: PythonNumber = 0.0,
         nbins: int = 32,
     ) -> None:
-        super().__init__(name)
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_estimators": 1,
             "max_features": max_features,
             "max_leaf_nodes": int(max_leaf_nodes),
             "sample": 1.0,
             "max_depth": max_depth,
             "min_samples_leaf": min_samples_leaf,
@@ -200,25 +214,29 @@
     """
     A classifier that overfits the training data.
     These models are  typically used as a control
     to compare with your other models.
 
     Parameters
     ----------
-    name: str
+    name: str, optional
         Name of  the  model. The model is stored
         in the database.
+    overwrite_model: bool, optional
+        If set to True, training a model with the same
+        name as an existing model overwrites the
+        existing model.
     """
 
     # System & Special Methods.
 
     @check_minimum_version
     @save_verticapy_logs
-    def __init__(self, name: str) -> None:
-        super().__init__(name)
+    def __init__(self, name: str = None, overwrite_model: bool = False) -> None:
+        super().__init__(name, overwrite_model)
         self.parameters = {
             "n_estimators": 1,
             "max_features": "max",
             "max_leaf_nodes": int(1e9),
             "sample": 1.0,
             "max_depth": 100,
             "min_samples_leaf": 1,
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/acf.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/acf.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/bar.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/bar.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/barh.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/barh.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/base.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/boxplot.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/boxplot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/candlestick.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/candlestick.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/contour.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/contour.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     # Formatting Methods.
 
     def _get_narrow_vars(self) -> tuple:
         n, m = self.data["X"].shape
         data = []
         for i in range(n):
             for j in range(m):
-                data += [[i, j, self.data["Z"][i][j]]]
+                data += [[j, i, self.data["Z"][i][j]]]
         return data
 
     # Styling Methods.
 
     def _init_style(self) -> None:
         self.init_style = {
             "chart": {
@@ -72,19 +72,19 @@
                     "function () {return '<b>[' + this.series.xAxis."
                     "categories[this.point.x] + ', ' + this.series.yAxis"
                     ".categories[this.point.y] + ']</b>: ' + this.point"
                     ".value + '</b>';}"
                 )
             },
             "xAxis": {
-                "categories": np.round(self.data["X"][:, 0], 3).tolist(),
+                "categories": np.round(self.data["X"][0], 3).tolist(),
                 "title": {"text": self.layout["columns"][0]},
             },
             "yAxis": {
-                "categories": np.round(self.data["Y"][0], 3).tolist(),
+                "categories": np.round(self.data["Y"][:, 0], 3).tolist(),
                 "title": {"text": self.layout["columns"][1]},
             },
             "legend": {
                 "align": "right",
                 "layout": "vertical",
                 "margin": 0,
                 "verticalAlign": "top",
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/density.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/density.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,18 +115,17 @@
         self,
         chart: Optional[HChart] = None,
         **style_kwargs,
     ) -> HChart:
         """
         Draws a multi-density plot using the HC API.
         """
-        labels = self._clean_quotes(self.layout["labels"])
         chart, style_kwargs = self._get_chart(chart, style_kwargs=style_kwargs)
         chart.set_dict_options(self.init_style)
         chart.set_dict_options(style_kwargs)
         m = self.data["X"].shape[1]
         for i in range(m):
             data = np.column_stack(
                 (self.data["X"][:, i], self.data["Y"][:, i])
             ).tolist()
-            chart.add_data_set(data, "area", labels[i])
+            chart.add_data_set(data, "area", str(self.layout["labels"][i]))
         return chart
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/heatmap.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
             y_label = self.layout["columns"][1]
         elif "method_of" in self.layout:
             y_label = self.layout["method_of"]
         else:
             y_label = ""
         if isinstance(self.layout["y_labels"], list):
             y_labels = copy.deepcopy(self.layout["y_labels"])
-            y_labels.reverse()
         else:
             y_labels = self.layout["y_labels"]
         self.init_style = {
             "chart": {
                 "type": "heatmap",
                 "marginTop": 40,
                 "marginBottom": 80,
@@ -161,13 +160,17 @@
         )
         chart.set_dict_options(self.init_style)
         chart.set_dict_options(style_kwargs)
         X = np.flip(self.data["X"], axis=1)
         data = []
         for i in range(len(self.layout["x_labels"])):
             for j in range(len(self.layout["y_labels"])):
-                data += [[i, j, round(X[i, j], self.layout["mround"])]]
+                if "mround" in self.layout:
+                    Xij = round(X[i, j], self.layout["mround"])
+                else:
+                    Xij = X[i, j]
+                data += [[i, j, Xij]]
         chart.add_data_set(data, **self.init_style_matrix)
         chart.set_dict_options(
             {"colorAxis": self._get_cmap_style(style_kwargs=style_kwargs)}
         )
         return chart
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/line.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/line.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,16 +146,17 @@
         if self.layout["kind"] == "step":
             step_kwargs = kind_kwargs
         else:
             step_kwargs = {}
             chart.set_dict_options(kind_kwargs)
         if self.layout["has_category"]:
             uniques = np.unique(self.data["z"])
+            X = np.array([int(int_string) for int_string in self.data["x"]])
             for c in uniques:
-                x = self._to_datetime(self.data["x"][self.data["z"] == c])
+                x = self._to_datetime(X[self.data["z"] == c])
                 y = self.data["Y"][:, 0][self.data["z"] == c]
                 data = np.column_stack((x, y)).tolist()
                 chart.add_data_set(data, kind, str(c), **step_kwargs)
         else:
             x = self._to_datetime(self.data["x"])
             y = self.data["Y"][:, 0]
             data = np.column_stack((x, y)).tolist()
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/champion_challenger.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/champion_challenger.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/elbow.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/elbow.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/importance.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/importance.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/lof.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/lof.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/logistic_reg.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/logistic_reg.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/model_evaluation.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/pca.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/pca.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/regression.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/regression.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/regression_tree.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/regression_tree.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/stepwise.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/stepwise.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/machine_learning/svm.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/machine_learning/svm.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/outliers.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/outliers.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/pie.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/pie.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/range.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/range.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/scatter.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/scatter.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_highcharts/spider.py` & `verticapy-1.0.0b2/verticapy/plotting/_highcharts/spider.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/acf.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/acf.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/bar.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/bar.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/base.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/bubble.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/bubble.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/line.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/line.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/animated/pie.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/animated/pie.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/bar.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/bar.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/barh.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/barh.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/base.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/boxplot.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/boxplot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/contour.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/contour.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/density.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/density.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/heatmap.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/heatmap.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/hexbin.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/hexbin.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/hist.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/line.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/line.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/champion_challenger.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/champion_challenger.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/elbow.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/elbow.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/importance.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/importance.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         ax: Optional[Axes] = None,
         **style_kwargs,
     ) -> Axes:
         """
         Draws a coefficient importance bar chart using the Matplotlib API.
         """
         n = len(self.data["importance"])
-        x_label = self.layout["x_label"] if "x_label" in self.layout else "Importance"
+        x_label = (
+            self.layout["x_label"] if "x_label" in self.layout else "Importance (%)"
+        )
         y_label = self.layout["y_label"] if "y_label" in self.layout else "Features"
         ax, fig, style_kwargs = self._get_ax_fig(
             ax,
             size=(12, int(n / 2) + 1),
             set_axis_below=True,
             grid=True,
             style_kwargs=style_kwargs,
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/kmeans.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/kmeans.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/lof.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/lof.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/logistic_reg.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/logistic_reg.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/model_evaluation.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/model_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         ax.fill_between(
             self.data["x"],
             self.data["y"],
             self.data["z"],
             **self.init_style,
         )
         ax.set_xlabel(self.layout["x_label"])
+        ax.set_ylabel("Values")
         ax.set_title(self.layout["title"])
         ax.legend(loc="center left", bbox_to_anchor=[1, 0.5])
         ax.set_ylim(0, 1)
         ax.set_xlim(0, 1)
         return ax
 
 
@@ -256,10 +257,11 @@
             label=self.layout["z_label"],
         )
         c1 = mpatches.Patch(
             color=self._get_final_color(style_kwargs=style_kwargs, idx=1),
             label=self.layout["y_label"],
         )
         ax.legend(handles=[c0, c1], loc="center left", bbox_to_anchor=[1, 0.5])
+        ax.set_ylabel("Values")
         ax.set_xlim(0, 1)
         ax.set_ylim(0)
         return ax
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/pca.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/pca.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/regression.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/regression.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/regression_tree.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/regression_tree.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/stepwise.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/stepwise.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/machine_learning/svm.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/machine_learning/svm.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/outliers.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/outliers.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/pie.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/pie.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/range.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/range.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/scatter.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/scatter.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_matplotlib/spider.py` & `verticapy-1.0.0b2/verticapy/plotting/_matplotlib/spider.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-from verticapy.plotting._plotly.bar import BarChart
+from verticapy.plotting._plotly.bar import BarChart, BarChart2D
 from verticapy.plotting._plotly.pie import PieChart, NestedPieChart
-from verticapy.plotting._plotly.barh import HorizontalBarChart
+from verticapy.plotting._plotly.barh import HorizontalBarChart, HorizontalBarChart2D
 from verticapy.plotting._plotly.scatter import ScatterPlot
 from verticapy.plotting._plotly.boxplot import BoxPlot
 from verticapy.plotting._plotly.heatmap import HeatMap
 from verticapy.plotting._plotly.contour import ContourPlot
 from verticapy.plotting._plotly.density import DensityPlot, MultiDensityPlot
 from verticapy.plotting._plotly.spider import SpiderChart
 from verticapy.plotting._plotly.range import RangeCurve
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/acf.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/acf.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/bar.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/hist.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,63 +12,61 @@
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 from typing import Literal, Optional
 
-import plotly.express as px
+
 from plotly.graph_objs._figure import Figure
+import plotly.graph_objects as go
 
 from verticapy.plotting._plotly.base import PlotlyBase
 
 
-class BarChart(PlotlyBase):
+class Histogram(PlotlyBase):
     # Properties.
 
     @property
     def _category(self) -> Literal["chart"]:
         return "chart"
 
     @property
-    def _kind(self) -> Literal["bar"]:
-        return "bar"
+    def _kind(self) -> Literal["hist"]:
+        return "hist"
 
     @property
-    def _compute_method(self) -> Literal["1D"]:
-        return "1D"
+    def _compute_method(self) -> Literal["hist"]:
+        return "hist"
 
     # Styling Methods.
 
     def _init_style(self) -> None:
-        self.init_trace_style = {"marker_color": self.get_colors(idx=0)}
-        self.init_layout_style = {
-            "yaxis_title": self.layout["method"],
-            "xaxis_title": self.layout["column"],
-            "width": 100 + 100 * len(self.layout["labels"]),
-            "height": 500,
-        }
+        self.init_style = {"width": 800, "height": 450}
 
     # Draw.
 
     def draw(
         self,
         fig: Optional[Figure] = None,
         **style_kwargs,
     ) -> Figure:
         """
-        Draws a bar chart using the Plotly API.
+        Draws an histogram using the Plotly API.
         """
-        fig_base = self._get_fig(fig)
-        fig = px.bar(x=self.layout["labels"], y=self.data["y"])
-        if self.data["is_categorical"]:
-            fig.update_xaxes(type="category")
-        params = self._update_dict(self.init_layout_style, style_kwargs)
-        fig.update_layout(**params)
-        fig.update_traces(**self.init_trace_style)
-        fig_base.add_trace(fig.data[0])
-        fig_base.update_layout(fig.layout)
-        return fig_base
-
-
-class BarChart2D(PlotlyBase):
-    ...
+        fig = self._get_fig(fig)
+        key = "categories" if self.layout["has_category"] else "columns"
+        fig.add_trace(
+            go.Bar(
+                x=self.data[self.layout[key][0]]["x"],
+                y=self.data[self.layout[key][0]]["y"],
+                width=self.data["width"],
+                offset=0,
+            )
+        )
+        fig.update_layout(yaxis_title=self.layout["method_of"])
+        if len(self.layout["columns"]) == 1:
+            fig.update_layout(xaxis_title=self.layout["columns"][0])
+        else:
+            title = self.layout["by"]
+        fig.update_layout(**self._update_dict(self.init_style, style_kwargs))
+        return fig
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/barh.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/spider.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,63 +12,84 @@
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 from typing import Literal, Optional
 
-import plotly.express as px
+import plotly.graph_objects as go
 from plotly.graph_objs._figure import Figure
 
 from verticapy.plotting._plotly.base import PlotlyBase
 
 
-class HorizontalBarChart(PlotlyBase):
+class SpiderChart(PlotlyBase):
     # Properties.
 
     @property
     def _category(self) -> Literal["chart"]:
         return "chart"
 
     @property
-    def _kind(self) -> Literal["bar"]:
-        return "bar"
+    def _kind(self) -> Literal["spider"]:
+        return "spider"
 
     @property
-    def _compute_method(self) -> Literal["1D"]:
-        return "1D"
+    def _compute_method(self) -> Literal["2D"]:
+        return "2D"
 
     # Styling Methods.
 
     def _init_style(self) -> None:
-        self.init_trace_style = {"marker_color": self.get_colors(idx=0)}
-        self.init_layout_style = {
-            "xaxis_title": self.layout["method"],
-            "yaxis_title": self.layout["column"],
-            # "width": 500 ,
-            "height": 100 * len(self.layout["labels"]),
+        self.init_style = {
+            "width": 500,
+            "height": 500,
+            "legend": dict(
+                title=self.layout["columns"][1]
+                if len(self.layout["columns"]) > 1
+                else None
+            ),
+            "title": self.layout["columns"][0],
+            "annotations": [
+                dict(
+                    x=0.5,
+                    y=-0.1,
+                    xref="paper",
+                    yref="paper",
+                    text=f"(Method: {self.layout['method_of'].title()})",
+                    showarrow=False,
+                )
+            ],
         }
 
     # Draw.
 
     def draw(
         self,
         fig: Optional[Figure] = None,
         **style_kwargs,
     ) -> Figure:
         """
-        Draws a horizontal bar chart using the Plotly API.
+        Draws a spider plot using the Plotly API.
         """
-        fig_base = self._get_fig(fig)
-        fig = px.bar(y=self.layout["labels"], x=self.data["y"], orientation="h")
-        if self.data["is_categorical"]:
-            fig.update_yaxes(type="category")
-        params = self._update_dict(self.init_layout_style, style_kwargs)
-        fig.update_layout(**params)
-        fig.update_traces(**self.init_trace_style)
-        fig_base.add_trace(fig.data[0])
-        fig_base.update_layout(fig.layout)
-        return fig_base
-
-
-class HorizontalBarChart2D(PlotlyBase):
-    ...
+        fig = self._get_fig(fig)
+        for i in range(self.data["X"].shape[1]):
+            fig.add_trace(
+                go.Scatterpolar(
+                    r=self.data["X"][:, i].flatten(),
+                    theta=self.layout["x_labels"],
+                    fill="toself",
+                    name=self.layout["y_labels"][i],
+                )
+            )
+        fig.update_layout(
+            polar=dict(
+                radialaxis=dict(
+                    visible=True,
+                    nticks=5,
+                ),
+                angularaxis=dict(type="category"),
+            ),
+            showlegend=True,
+        )
+        fig.update_layout(**self._update_dict(self.init_style, style_kwargs))
+        return fig
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/base.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/boxplot.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/boxplot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/contour.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/contour.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         Draws a contour plot using the Plotly API.
         """
         fig_base = self._get_fig(fig)
         x_title = self.layout["columns"][0]
         y_title = self.layout["columns"][1]
         fig = go.Figure(
             data=go.Contour(
-                z=np.transpose(self.data["Z"]),
+                z=self.data["Z"],
                 x=np.unique(self.data["X"]),
                 y=np.unique(self.data["Y"]),
                 hovertemplate=f"{x_title}: "
                 "%{x:.2f} <br> "
                 f"{y_title}:"
                 " %{y:.2f} <extra></extra> <br> Color: %{z:.2f}",
                 **self._get_color_style(style_kwargs),
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/density.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/density.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     # Styling Methods.
 
     def _init_style(self) -> None:
         self.init_style = {
             "width": 700,
             "height": 500,
             "autosize": False,
-            "xaxis_title": self.layout["x_label"],
+            "xaxis_title": self._clean_quotes(self.layout["x_label"]),
             "yaxis_title": self.layout["y_label"],
             "xaxis": dict(
                 showline=True,
                 linewidth=1,
                 linecolor="black",
                 mirror=True,
                 zeroline=False,
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/heatmap.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/heatmap.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/hist.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/regression.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,61 +12,81 @@
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 from typing import Literal, Optional
 
-
-from plotly.graph_objs._figure import Figure
 import plotly.graph_objects as go
+from plotly.graph_objs._figure import Figure
 
 from verticapy.plotting._plotly.base import PlotlyBase
 
 
-class Histogram(PlotlyBase):
+class RegressionPlot(PlotlyBase):
     # Properties.
 
     @property
-    def _category(self) -> Literal["chart"]:
-        return "chart"
+    def _category(self) -> Literal["plot"]:
+        return "plot"
 
     @property
-    def _kind(self) -> Literal["hist"]:
-        return "hist"
+    def _kind(self) -> Literal["regression"]:
+        return "regression"
 
     @property
-    def _compute_method(self) -> Literal["hist"]:
-        return "hist"
+    def _compute_method(self) -> Literal["sample"]:
+        return "sample"
+
+    @property
+    def _dimension_bounds(self) -> tuple[int, int]:
+        return (2, 3)
 
     # Styling Methods.
 
     def _init_style(self) -> None:
-        self.init_style = {"width": 800, "height": 450}
+        self.init_style = {
+            "mode": "markers",
+            "marker_line_width": 2,
+            "marker_size": 10,
+            "marker_line_color": "black",
+        }
+        self.init_layout_style = {
+            "yaxis_title": self.layout["columns"][1],
+            "xaxis_title": self.layout["columns"][0],
+            "width": 700,
+            "height": 600,
+        }
 
     # Draw.
 
     def draw(
         self,
         fig: Optional[Figure] = None,
         **style_kwargs,
     ) -> Figure:
         """
-        Draws an histogram using the Plotly API.
+        Draws a regression plot using the Plotly API.
         """
         fig = self._get_fig(fig)
-        key = "categories" if self.layout["has_category"] else "columns"
-        fig.add_trace(
-            go.Bar(
-                x=self.data[self.layout[key][0]]["x"],
-                y=self.data[self.layout[key][0]]["y"],
-                width=self.data["width"],
-                offset=0,
+        x = self.data["X"][:, 0]
+        y = self.data["X"][:, 1]
+        min_reg_x, max_reg_x = min(x), max(x)
+        y0 = self.data["coef"][0]
+        slope = self.data["coef"][1]
+        if len(self.layout["columns"]) == 2:
+            fig = fig.add_trace(
+                go.Scatter(x=x, y=y, **self.init_style, name="Scatter Points")
+            )
+            fig.add_trace(
+                go.Scatter(
+                    x=[min_reg_x, max_reg_x],
+                    y=[y0 + slope * min_reg_x, y0 + slope * max_reg_x],
+                    mode="lines",
+                    line_shape="linear",
+                    name="Regression Line",
+                )
             )
-        )
-        fig.update_layout(yaxis_title=self.layout["method_of"])
-        if len(self.layout["columns"]) == 1:
-            fig.update_layout(xaxis_title=self.layout["columns"][0])
+            fig.update_layout(**self._update_dict(self.init_layout_style, style_kwargs))
         else:
-            title = self.layout["by"]
-        fig.update_layout(**self._update_dict(self.init_style, style_kwargs))
+            raise ValueError("The number of predictors is too big to draw the plot.")
         return fig
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/line.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/line.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/champion_challenger.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/champion_challenger.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/elbow.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/elbow.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/importance.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/importance.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/kmeans.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/kmeans.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/lof.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/lof.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/logistic_reg.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/logistic_reg.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/model_evaluation.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/pca.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/pca.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/regression.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/bar.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,81 +12,108 @@
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 from typing import Literal, Optional
 
+import plotly.express as px
 import plotly.graph_objects as go
 from plotly.graph_objs._figure import Figure
 
 from verticapy.plotting._plotly.base import PlotlyBase
 
 
-class RegressionPlot(PlotlyBase):
+class BarChart(PlotlyBase):
     # Properties.
 
     @property
-    def _category(self) -> Literal["plot"]:
-        return "plot"
+    def _category(self) -> Literal["chart"]:
+        return "chart"
 
     @property
-    def _kind(self) -> Literal["regression"]:
-        return "regression"
+    def _kind(self) -> Literal["bar"]:
+        return "bar"
 
     @property
-    def _compute_method(self) -> Literal["sample"]:
-        return "sample"
-
-    @property
-    def _dimension_bounds(self) -> tuple[int, int]:
-        return (2, 3)
+    def _compute_method(self) -> Literal["1D"]:
+        return "1D"
 
     # Styling Methods.
 
     def _init_style(self) -> None:
-        self.init_style = {
-            "mode": "markers",
-            "marker_line_width": 2,
-            "marker_size": 10,
-            "marker_line_color": "black",
+        self.init_trace_style = {"marker_color": self.get_colors(idx=0)}
+        self.init_layout_style = {
+            "yaxis_title": self.layout["method"],
+            "xaxis_title": self.layout["column"],
+            "width": 100 + 100 * len(self.layout["labels"]),
+            "height": 500,
         }
+
+    # Draw.
+
+    def draw(
+        self,
+        fig: Optional[Figure] = None,
+        **style_kwargs,
+    ) -> Figure:
+        """
+        Draws a bar chart using the Plotly API.
+        """
+        fig_base = self._get_fig(fig)
+        fig = px.bar(x=self.layout["labels"], y=self.data["y"])
+        if self.data["is_categorical"]:
+            fig.update_xaxes(type="category")
+        params = self._update_dict(self.init_layout_style, style_kwargs)
+        fig.update_layout(**params)
+        fig.update_traces(**self.init_trace_style)
+        fig_base.add_trace(fig.data[0])
+        fig_base.update_layout(fig.layout)
+        return fig_base
+
+
+class BarChart2D(PlotlyBase):
+    @property
+    def _category(self) -> Literal["chart"]:
+        return "chart"
+
+    @property
+    def _kind(self) -> Literal["bar"]:
+        return "bar"
+
+    @property
+    def _compute_method(self) -> Literal["2D"]:
+        return "2D"
+
+    # Styling Methods.
+    def _init_style(self) -> None:
         self.init_layout_style = {
-            "yaxis_title": self.layout["columns"][1],
+            "yaxis_title": self.layout["method"],
+            "legend_title_text": self.layout["columns"][1],
             "xaxis_title": self.layout["columns"][0],
-            "width": 700,
-            "height": 600,
+            "width": (150 + 40 * len(self.layout["x_labels"]))
+            * 0.8
+            * len(self.layout["y_labels"]),
+            "height": 500,
         }
 
     # Draw.
 
     def draw(
         self,
         fig: Optional[Figure] = None,
         **style_kwargs,
     ) -> Figure:
         """
-        Draws a regression plot using the Plotly API.
+        Draws a 2D BarChart using the Matplotlib API.
         """
-        fig = self._get_fig(fig)
-        x = self.data["X"][:, 0]
-        y = self.data["X"][:, 1]
-        min_reg_x, max_reg_x = min(x), max(x)
-        y0 = self.data["coef"][0]
-        slope = self.data["coef"][1]
-        if len(self.layout["columns"]) == 2:
-            fig = fig.add_trace(
-                go.Scatter(x=x, y=y, **self.init_style, name="Scatter Points")
-            )
-            fig.add_trace(
-                go.Scatter(
-                    x=[min_reg_x, max_reg_x],
-                    y=[y0 + slope * min_reg_x, y0 + slope * max_reg_x],
-                    mode="lines",
-                    line_shape="linear",
-                    name="Regression Line",
-                )
+        fig_base = self._get_fig(fig)
+        for i in range(len(self.layout["y_labels"])):
+            fig = go.Bar(
+                name=self.layout["y_labels"][i],
+                x=self.layout["x_labels"],
+                y=self.data["X"][:, i],
             )
-            fig.update_layout(**self._update_dict(self.init_layout_style, style_kwargs))
-        else:
-            raise ValueError("The number of predictors is too big to draw the plot.")
-        return fig
+            fig_base.add_trace(fig)
+        params = self._update_dict(self.init_layout_style, style_kwargs)
+        fig_base.update_layout(**params)
+        return fig_base  # self.data,self.layout
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/regression_tree.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/regression_tree.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/stepwise.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/stepwise.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/machine_learning/svm.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/machine_learning/svm.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/outliers.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/outliers.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/pie.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/pie.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/range.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/range.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/scatter.py` & `verticapy-1.0.0b2/verticapy/plotting/_plotly/scatter.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_plotly/spider.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_scatter.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,86 +10,77 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-from typing import Literal, Optional
+# Vertica
+from verticapy.tests_new.plotting.base_test_files import (
+    ScatterVDF2DPlot,
+    ScatterVDF3DPlot,
+)
 
-import plotly.graph_objects as go
-from plotly.graph_objs._figure import Figure
 
-from verticapy.plotting._plotly.base import PlotlyBase
+class TestHighchartsScatterVDF2DPlot(ScatterVDF2DPlot):
+    """
+    Testing different attributes of 2D scatter plot on a vDataFrame
+    """
 
-
-class SpiderChart(PlotlyBase):
-    # Properties.
-
-    @property
-    def _category(self) -> Literal["chart"]:
-        return "chart"
-
-    @property
-    def _kind(self) -> Literal["spider"]:
-        return "spider"
-
-    @property
-    def _compute_method(self) -> Literal["2D"]:
-        return "2D"
-
-    # Styling Methods.
-
-    def _init_style(self) -> None:
-        self.init_style = {
-            "width": 500,
-            "height": 500,
-            "legend": dict(
-                title=self.layout["columns"][1]
-                if len(self.layout["columns"]) > 1
-                else None
-            ),
-            "title": self.layout["columns"][0],
-            "annotations": [
-                dict(
-                    x=0.5,
-                    y=-0.1,
-                    xref="paper",
-                    yref="paper",
-                    text=f"(Method: {self.layout['method_of'].title()})",
-                    showarrow=False,
-                )
+    def test_properties_all_unique_values_for_by(self, dummy_scatter_vd):
+        """
+        Test if all unique valies are inside the plot
+        """
+        # Arrange
+        # Act
+        result = dummy_scatter_vd.scatter(
+            [
+                self.COL_NAME_2,
+                self.COL_NAME_3,
             ],
-        }
+            by=self.COL_NAME_4,
+        )
+        # Assert
+        assert len(result.data_temp) == len(
+            self.all_categories
+        ), "Some unique values were not found in the plot"
+
+    def test_data_total_number_of_points(self, dummy_scatter_vd):
+        """
+        Test if all datapoints were plotted
+        """
+        # Arrange
+        # Act
+        # Assert - checking if correct object created
+        assert sum(len(item.data) for item in self.result.data_temp) == len(
+            dummy_scatter_vd
+        ), "Number of points not consistent with data"
 
-    # Draw.
 
-    def draw(
+class TestHighchartsScatterVDF3DPlot(ScatterVDF3DPlot):
+    """
+    Testing different attributes of 3D scatter plot on a vDataFrame
+    """
+
+    def test_properties_all_unique_values_for_by_3d_plot(
         self,
-        fig: Optional[Figure] = None,
-        **style_kwargs,
-    ) -> Figure:
-        """
-        Draws a spider plot using the Plotly API.
-        """
-        fig = self._get_fig(fig)
-        for i in range(self.data["X"].shape[1]):
-            fig.add_trace(
-                go.Scatterpolar(
-                    r=self.data["X"][:, i].flatten(),
-                    theta=self.layout["x_labels"],
-                    fill="toself",
-                    name=self.layout["y_labels"][i],
-                )
-            )
-        fig.update_layout(
-            polar=dict(
-                radialaxis=dict(
-                    visible=True,
-                    nticks=5,
-                ),
-                angularaxis=dict(type="category"),
-            ),
-            showlegend=True,
-        )
-        fig.update_layout(**self._update_dict(self.init_style, style_kwargs))
-        return fig
+    ):
+        """
+        Test if all unique values plotted
+        """
+        # Arrange
+        # Act
+        # Assert
+        assert len(self.result.data_temp) == len(
+            self.all_categories
+        ), "Some unique values were not found in the plot"
+
+    def test_data_total_number_of_points_3d_plot(self, dummy_scatter_vd):
+        """
+        Test if all datapoints were plotted
+        """
+        # Arrange
+        # Act
+        # Assert - checking if correct object created
+        assert sum(len(item.data) for item in self.result.data_temp) == len(
+            dummy_scatter_vd
+        ), "Number of points not consistent with data"
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/_utils.py` & `verticapy-1.0.0b2/verticapy/plotting/_utils.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/plotting/base.py` & `verticapy-1.0.0b2/verticapy/plotting/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,26 +458,26 @@
         method, aggregate, aggregate_fun, is_standard = self._map_method(method, of)
         if not is_standard:
             other_columns = ", " + ", ".join(
                 vdc._parent.get_columns(exclude_columns=[vdc._alias])
             )
         # depending on the cardinality, the type, the vDataColumn
         # can be treated as categorical or not
-        cardinality, count, is_numeric, is_date, is_categorical = (
-            vdc.nunique(True),
-            vdc._parent.shape()[0],
-            vdc.isnum() and not vdc.isbool(),
-            (vdc.category() == "date"),
-            False,
-        )
+        cardinality = vdc.nunique(True)
+        count = vdc._parent.shape()[0]
+        is_numeric = vdc.isnum() and not vdc.isbool()
+        is_date = vdc.isdate()
+        is_bool = vdc.isbool()
+        cast = "::int" if is_bool else ""
+        is_categorical = False
         # case when categorical
         if (((cardinality <= max_cardinality) or not is_numeric) or pie) and not (
             is_date
         ):
-            if (is_numeric) and not pie:
+            if ((is_numeric) and not pie) or (is_bool):
                 query = f"""
                     SELECT 
                         {vdc},
                         {aggregate}
                     FROM {vdc._parent} 
                     WHERE {vdc} IS NOT NULL 
                     GROUP BY {vdc} 
@@ -614,15 +614,15 @@
                 h = float(vdc.max() - vdc.min()) / nbins
             if (vdc.ctype == "int") or (h == 0):
                 h = max(1.0, h)
             query_result = _executeSQL(
                 query=f"""
                     SELECT
                         /*+LABEL('plotting._matplotlib._compute_plot_params')*/
-                        FLOOR({vdc} / {h}) * {h},
+                        FLOOR({vdc}{cast} / {h}) * {h},
                         {aggregate} 
                     FROM {vdc._parent}
                     WHERE {vdc} IS NOT NULL
                     GROUP BY 1
                     ORDER BY 1""",
                 title="Computing the histogram heights",
                 method="fetchall",
@@ -673,21 +673,31 @@
         max_cardinality: int = 8,
         cat_priority: Union[None, PythonScalar, ArrayLike] = None,
     ) -> None:
         if not columns:
             columns = vdf.numcol()
         else:
             columns = format_type(columns, dtype=list)
-        if not columns:
-            raise ValueError("No numerical columns found to compute the statistics.")
-        columns, by = vdf.format_colnames(columns, by)
+        columns_ = []
+        for col in columns:
+            if vdf[col].isnum() and not (vdf[col].isbool()):
+                columns_ += [col]
+            elif conf.get_option("print_info"):
+                warning_message = (
+                    f"The Virtual Column {col} is not numerical."
+                    " Its histogram will not be drawn."
+                )
+                warnings.warn(warning_message, Warning)
+        if not columns_:
+            raise ValueError("No quantitative feature to plot.")
+        columns_, by = vdf.format_colnames(columns_, by)
         method, aggregate, aggregate_fun, is_standard = self._map_method(method, of)
-        self._init_check(dim=len(columns), is_standard=is_standard)
-        if by and len(columns) == 1:
-            column = columns[0]
+        self._init_check(dim=len(columns_), is_standard=is_standard)
+        if by and len(columns_) == 1:
+            column = columns_[0]
             cols = [column]
             if not h or h <= 0:
                 h = vdf[column].numh()
             data, categories = {"width": h}, []
             vdf_tmp = vdf[by].isin(cat_priority) if cat_priority else vdf.copy()
             if vdf_tmp[by].isnum():
                 vdf_tmp[by].discretize(h=h_by)
@@ -706,32 +716,25 @@
                     h=h,
                 )
                 categories += [category]
                 data[category] = copy.deepcopy(self.data)
         else:
             h_, categories = [], None
             if isinstance(h, NoneType) or h <= 0:
-                for idx, column in enumerate(columns):
+                for idx, column in enumerate(columns_):
                     h_ += [vdf[column].numh()]
                 h = min(h_)
             data, cols = {"width": h}, []
-            for idx, column in enumerate(columns):
+            for idx, column in enumerate(columns_):
                 if vdf[column].isnum():
                     self._compute_plot_params(
                         vdf[column], method=method, of=of, max_cardinality=1, h=h
                     )
                     cols += [column]
                     data[self._clean_quotes(column)] = copy.deepcopy(self.data)
-                else:
-                    if vdf._vars["display"]["print_info"]:
-                        warning_message = (
-                            f"The Virtual Column {column} is not numerical."
-                            " Its histogram will not be drawn."
-                        )
-                        warnings.warn(warning_message, Warning)
         self.data = data
         self.layout = {
             "columns": self._clean_quotes(cols),
             "categories": categories,
             "by": self._clean_quotes(by),
             "method": method,
             "method_of": method + f"({of})" if of else method,
@@ -770,17 +773,20 @@
             expr = [
                 f"MIN({columns[0]})",
                 f"APPROXIMATE_PERCENTILE({columns[0]} USING PARAMETERS percentile = {q[0]})",
                 f"APPROXIMATE_MEDIAN({columns[0]})",
                 f"APPROXIMATE_PERCENTILE({columns[0]} USING PARAMETERS percentile = {q[1]})",
                 f"MAX({columns[0]})",
             ]
-            if vdf[by].isnum():
+            if vdf[by].isnum() and not (vdf[by].isbool()):
                 _by = vdf[by].discretize(h=h, return_enum_trans=True)
                 is_num_transf = True
+            elif vdf[by].isbool():
+                _by = ("{}::varchar", "varchar", "text")
+                is_num_transf = False
             else:
                 _by = vdf[by].discretize(
                     k=max_cardinality, method="topk", return_enum_trans=True
                 )
                 is_num_transf = False
             _by = _by[0].replace("{}", by) + f" AS {by}"
             vdf_tmp = vdf.copy()
@@ -886,14 +892,15 @@
         columns, of = vdf.format_colnames(columns, of)
         is_column_date = [False, False]
         timestampadd = ["", ""]
         matrix = []
         for idx, column in enumerate(columns):
             is_numeric = vdf[column].isnum() and (vdf[column].nunique(True) > 2)
             is_date = vdf[column].isdate()
+            cast = "::int" if vdf[column].isbool() else ""
             where = []
             if is_numeric:
                 if isinstance(h[idx], NoneType):
                     interval = vdf[column].numh()
                     if interval > 0.01:
                         interval = round(interval, 2)
                     elif interval > 0.0001:
@@ -906,28 +913,28 @@
                     interval = h[idx]
                 if vdf[column].category() == "int":
                     floor_end = "-1"
                     interval = int(max(math.floor(interval), 1))
                 else:
                     floor_end = ""
                 expr = f"""'[' 
-                          || FLOOR({column} 
+                          || FLOOR({column}{cast}
                                  / {interval}) 
                                  * {interval} 
                           || ';' 
-                          || (FLOOR({column} 
+                          || (FLOOR({column}{cast}
                                   / {interval}) 
                                   * {interval} 
                                   + {interval}{floor_end}) 
                           || ']'"""
                 if (interval > 1) or (vdf[column].category() == "float"):
                     matrix += [expr]
                 else:
-                    matrix += [f"FLOOR({column}) || ''"]
-                order_by = f"""ORDER BY MIN(FLOOR({column} 
+                    matrix += [f"FLOOR({column}{cast}) || ''"]
+                order_by = f"""ORDER BY MIN(FLOOR({column}{cast} 
                                           / {interval}) * {interval}) ASC"""
                 where += [f"{column} IS NOT NULL"]
             elif is_date:
                 if isinstance(h[idx], NoneType):
                     interval = vdf[column].numh()
                 else:
                     interval = max(math.floor(h[idx]), 1)
```

### Comparing `verticapy-1.0.0b1/verticapy/plotting/sql.py` & `verticapy-1.0.0b2/verticapy/plotting/sql.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sdk/__init__.py` & `verticapy-1.0.0b2/verticapy/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sdk/vertica/__init__.py` & `verticapy-1.0.0b2/verticapy/sdk/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sdk/vertica/udf/__init__.py` & `verticapy-1.0.0b2/verticapy/sdk/vertica/udf/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sdk/vertica/udf/gen.py` & `verticapy-1.0.0b2/verticapy/sdk/vertica/udf/gen.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sdk/vertica/udf/load.py` & `verticapy-1.0.0b2/verticapy/sdk/vertica/udf/load.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sdk/vertica/udf/utils.py` & `verticapy-1.0.0b2/verticapy/sdk/vertica/udf/utils.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/__init__.py` & `verticapy-1.0.0b2/verticapy/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/create.py` & `verticapy-1.0.0b2/verticapy/sql/create.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/drop.py` & `verticapy-1.0.0b2/verticapy/sql/drop.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/dtypes.py` & `verticapy-1.0.0b2/verticapy/sql/dtypes.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/flex.py` & `verticapy-1.0.0b2/verticapy/sql/flex.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/__init__.py` & `verticapy-1.0.0b2/verticapy/sql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/analytic.py` & `verticapy-1.0.0b2/verticapy/sql/functions/analytic.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/conditional.py` & `verticapy-1.0.0b2/verticapy/sql/functions/conditional.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/date.py` & `verticapy-1.0.0b2/verticapy/sql/functions/date.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/math.py` & `verticapy-1.0.0b2/verticapy/sql/functions/math.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/null_handling.py` & `verticapy-1.0.0b2/verticapy/sql/functions/null_handling.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/random.py` & `verticapy-1.0.0b2/verticapy/sql/functions/random.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/regexp.py` & `verticapy-1.0.0b2/verticapy/sql/functions/regexp.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/functions/string.py` & `verticapy-1.0.0b2/verticapy/sql/functions/string.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/geo/__init__.py` & `verticapy-1.0.0b2/verticapy/sql/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/geo/functions.py` & `verticapy-1.0.0b2/verticapy/sql/geo/functions.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/geo/index.py` & `verticapy-1.0.0b2/verticapy/sql/geo/index.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/insert.py` & `verticapy-1.0.0b2/verticapy/sql/insert.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/sql/sys.py` & `verticapy-1.0.0b2/verticapy/sql/sys.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/stats/__init__.py` & `verticapy-1.0.0b2/verticapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/base.py` & `verticapy-1.0.0b2/verticapy/tests/base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/conftest.py` & `verticapy-1.0.0b2/verticapy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/connect/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/connect/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/connect/test_connect.py` & `verticapy-1.0.0b2/verticapy/tests/connect/test_connect.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/datasets/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/datasets/test_datasets.py` & `verticapy-1.0.0b2/verticapy/tests/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/geo/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/geo/test_geo.py` & `verticapy-1.0.0b2/verticapy/tests/geo/test_geo.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/hchart/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/hchart/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/hchart/test_hchart.py` & `verticapy-1.0.0b2/verticapy/tests/hchart/test_hchart.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/sql/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/sql/test_sql.py` & `verticapy-1.0.0b2/verticapy/tests/sql/test_sql.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/stats/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/stats/test_stats.py` & `verticapy-1.0.0b2/verticapy/tests/stats/test_stats.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/udf/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/udf/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/udf/test_udf.py` & `verticapy-1.0.0b2/verticapy/tests/udf/test_udf.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/utilities/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/utilities/test_utilities.py` & `verticapy-1.0.0b2/verticapy/tests/utilities/test_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,14 +607,15 @@
         )
         assert drop("public.titanic_verticapy_test_json")
         drop("public.titanic_verticapy_test_json_2")
 
     def test_read_csv(self):
         path = os.path.dirname(verticapy.__file__) + "/datasets/data/titanic.csv"
         # with schema
+        drop("public.titanic_verticapy_test_csv", method="table")
         result = read_csv(
             path, table_name="titanic_verticapy_test_csv", schema="public"
         )
         assert result.shape() == (1234, 14)
         drop("public.titanic_verticapy_test_csv", method="table")
         # temporary table
         result = read_csv(
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/utilities/titanic-passengers.json` & `verticapy-1.0.0b2/verticapy/tests/utilities/titanic-passengers.json`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/utils/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/utils/log.py` & `verticapy-1.0.0b2/verticapy/tests/utils/log.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/utils/os_utils.py` & `verticapy-1.0.0b2/verticapy/tests/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_combine_join_sort.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_combine_join_sort.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_correlation.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_correlation.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_create.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_create.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_descriptive_statistics.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_feature_engineering.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_feature_engineering.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_filter_sample.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_filter_sample.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_plot.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_plot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_plot_plotly.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_plot_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,78 +164,89 @@
     )
 
 
 @pytest.fixture(scope="class")
 def regression_plot_result(load_plotly, dummy_scatter_vd):
     model = LinearRegression("LR_churn")
     model.fit(dummy_scatter_vd, ["x"], "y")
-    return model.plot()
+    yield model.plot()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def local_outlier_factor_3d_plot_result(load_plotly, dummy_scatter_vd):
     model = LocalOutlierFactor("lof_test_3d")
     model.fit(dummy_scatter_vd, ["X", "Y", "Z"])
-    return model.plot()
+    yield model.plot()
+    model.drop()
+    drop("lof_test_3d", method="table")
 
 
 @pytest.fixture(scope="class")
 def local_outlier_factor_plot_result(load_plotly, dummy_scatter_vd):
-    model = LocalOutlierFactor("lof_test")
+    model = LocalOutlierFactor("lof_test_fixture")
     model.fit(dummy_scatter_vd, ["X", "Y"])
-    return model.plot()
+    yield model.plot()
+    model.drop()
+    drop("lof_test_fixture", method="table")
 
 
 @pytest.fixture(scope="class")
 def logistic_regression_plot_result(load_plotly, titanic_vd):
     model = LogisticRegression("log_reg_test")
     model.fit(titanic_vd, ["fare"], "survived")
-    return model.plot()
+    yield model.plot()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def logistic_regression_plot_for_3d_result(load_plotly, titanic_vd):
-    model = LogisticRegression("log_reg_test")
+    model = LogisticRegression("log_reg_test_3d")
     model.fit(titanic_vd, ["fare", "age"], "survived")
-    return model.plot()
+    yield model.plot()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def importance_plot_result(load_plotly, iris_vd):
     model = RandomForestClassifier("importance_test")
     model.fit(
         iris_vd,
         ["PetalLengthCm", "PetalWidthCm", "SepalWidthCm", "SepalLengthCm"],
         "Species",
     )
-    return model.features_importance()
+    yield model.features_importance()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def pca_circle_plot_result(load_plotly, iris_vd):
     model = PCA("pca_circle_test")
     model.drop()
     model.fit(iris_vd)
-    return model.plot_circle()
+    yield model.plot_circle()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def roc_plot_result(load_plotly, titanic_vd):
     model = RandomForestClassifier("roc_plot_test")
     model.drop()
     model.fit(titanic_vd, ["age", "fare", "sex"], "survived")
-    return model.roc_curve()
+    yield model.roc_curve()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def cutoff_curve_plot_result(load_plotly, iris_vd):
     model = RandomForestClassifier("cutoff_curve_plot_test")
     model.drop()
     model.fit(iris_vd, ["PetalLengthCm", "PetalWidthCm"], "Species")
-    return model.cutoff_curve(pos_label="Iris-virginica")
+    yield model.cutoff_curve(pos_label="Iris-virginica")
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def prc_curve_plot_result(load_plotly, dummy_probability_data):
     return prc_curve("y_true", "y_score", dummy_probability_data)
 
 
@@ -247,55 +258,60 @@
 @pytest.fixture(scope="class")
 def voronoi_plot_result(load_plotly, iris_vd):
     model = KMeans(name="test_KMeans_iris")
     model.fit(
         iris_vd,
         ["PetalLengthCm", "PetalWidthCm"],
     )
-    return model.plot_voronoi()
+    yield model.plot_voronoi()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def svm_plot_result(load_plotly, iris_one_hot_vd):
     model = LinearSVC(name="public.SVC_iris")
     model.fit(iris_one_hot_vd, ["PetalLengthCm"], "Species_Iris-setosa")
-    return model.plot()
+    yield model.plot()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def svm_2d_plot_result(load_plotly, iris_one_hot_vd):
-    model = LinearSVC(name="public.SVC_iris")
+    model = LinearSVC(name="public.SVC_iris_2")
     model.fit(
         iris_one_hot_vd, ["PetalLengthCm", "SepalLengthCm"], "Species_Iris-setosa"
     )
-    return model.plot()
+    yield model.plot()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def svm_3d_plot_result(load_plotly, iris_one_hot_vd):
-    model = LinearSVC(name="public.SVC_iris")
+    model = LinearSVC(name="public.SVC_iris_3")
     model.fit(
         iris_one_hot_vd,
         ["PetalLengthCm", "SepalLengthCm", "PetalWidthCm"],
         "Species_Iris-setosa",
     )
-    return model.plot()
+    yield model.plot()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def champion_challenger_plot_result(load_plotly, titanic_vd):
     model = AutoML("model_automl", lmax=10, print_info=False)
     model.fit(
         titanic_vd,
         [
             "age",
         ],
         "survived",
     )
-    return model.plot()
+    yield model.plot()
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def stepwise_plot_result(load_plotly, titanic_vd):
     model = LogisticRegression(
         name="test_LR_titanic", tol=1e-4, max_iter=100, solver="Newton"
     )
@@ -307,15 +323,16 @@
             "fare",
             "parch",
             "pclass",
         ],
         y="survived",
         direction="backward",
     )
-    return stepwise_result.step_wise_
+    yield stepwise_result.step_wise_
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def hist_plot_result(load_plotly, titanic_vd):
     return titanic_vd["age"].hist()
 
 
@@ -332,19 +349,20 @@
     iris_one_hot["Species"].one_hot_encode(drop_first=False)
     yield iris_one_hot
     drop(name="public.iris")
 
 
 @pytest.fixture(scope="class")
 def regression_tree_plot_result(load_plotly, titanic_vd):
-    model = DecisionTreeRegressor(name="model_titanic")
+    model = DecisionTreeRegressor(name="model_titanic_fixture")
     x_col = "fare"
     y_col = "age"
     model.fit(titanic_vd, x_col, y_col)
-    return model.plot(), x_col, y_col
+    yield model.plot(), x_col, y_col
+    model.drop()
 
 
 @pytest.fixture(scope="class")
 def elbow_plot_result(load_plotly, iris_vd):
     return elbow(input_relation=iris_vd, X=["PetalLengthCm", "PetalWidthCm"])
 
 
@@ -1248,17 +1266,15 @@
 
     # ToDO - Change below after quotation bug fixed
     def test_properties_x_axis_title(self, load_plotly, dummy_dist_vd):
         # Arrange
         # Act
         result = dummy_dist_vd["0"].density()
         # Assert -
-        assert (
-            result.layout["xaxis"]["title"]["text"] == '"0"'
-        ), "X axis title incorrect"
+        assert result.layout["xaxis"]["title"]["text"] == "0", "X axis title incorrect"
 
     def test_properties_y_axis_title(self, load_plotly, dummy_dist_vd):
         # Arrange
         # Act
         result = dummy_dist_vd["0"].density()
         # Assert
         assert (
@@ -1754,22 +1770,23 @@
         ), "Discrepancy between points plotted and total number ofp oints"
 
     def test_additional_options_custom_height(self, load_plotly, dummy_scatter_vd):
         # rrange
         custom_height = 650
         custom_width = 700
         # Act
-        model = LinearRegression("LR_churn")
+        model = LinearRegression("LR_churn_h")
         model.fit(dummy_scatter_vd, ["X"], "Y")
         result = model.plot(height=custom_height, width=custom_width)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningLOFPlot:
     @pytest.fixture(autouse=True)
     def result_2d(self, local_outlier_factor_plot_result):
         self.result = local_outlier_factor_plot_result
 
@@ -1869,14 +1886,16 @@
         model.fit(dummy_scatter_vd, ["X", "Y"])
         result = model.plot(height=custom_height, width=custom_width)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
+        drop("lof_test", method="table")
 
 
 class TestMachineLearningLogisticRegressionPlot:
     @pytest.fixture(autouse=True)
     def result_2d(self, logistic_regression_plot_result):
         self.result_2d = logistic_regression_plot_result
 
@@ -1948,22 +1967,23 @@
         ), "Either line or the two scatter plots are missing"
 
     def test_additional_options_custom_height(self, load_plotly, titanic_vd):
         # rrange
         custom_height = 650
         custom_width = 700
         # Act
-        model = LogisticRegression("log_reg_test")
+        model = LogisticRegression("log_reg_test_h")
         model.fit(titanic_vd, ["fare"], "survived")
         result = model.plot(height=custom_height, width=custom_width)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningImportanceBarChart:
     @pytest.fixture(autouse=True)
     def result(self, importance_plot_result):
         self.result = importance_plot_result
 
@@ -2001,26 +2021,27 @@
         assert len(self.result.data[0]["x"]) == total_items, "Some columns missing"
 
     def test_additional_options_custom_height(self, load_plotly, iris_vd):
         # rrange
         custom_height = 650
         custom_width = 700
         # Act
-        model = RandomForestClassifier("importance_test")
+        model = RandomForestClassifier("importance_test_2")
         model.fit(
             iris_vd,
             ["PetalLengthCm", "PetalWidthCm", "SepalWidthCm", "SepalLengthCm"],
             "Species",
         )
         result = model.features_importance(height=custom_height, width=custom_width)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningPCACirclePlot:
     @pytest.fixture(autouse=True)
     def result(self, pca_circle_plot_result):
         self.result = pca_circle_plot_result
 
@@ -2067,14 +2088,15 @@
         model.fit(iris_vd)
         result = model.plot_circle(height=custom_height, width=custom_width)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningROCCurve:
     @pytest.fixture(autouse=True)
     def result(self, roc_plot_result):
         self.result = roc_plot_result
 
@@ -2128,14 +2150,15 @@
         model.fit(titanic_vd, ["age", "fare", "sex"], "survived")
         result = model.roc_curve(height=custom_height, width=custom_width)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningCutoffCurve:
     @pytest.fixture(autouse=True)
     def result(self, cutoff_curve_plot_result):
         self.result = cutoff_curve_plot_result
 
@@ -2184,14 +2207,15 @@
             pos_label="Iris-virginica", width=custom_width, height=custom_height
         )
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningPRCCurve:
     @pytest.fixture(autouse=True)
     def result(self, prc_curve_plot_result):
         self.result = prc_curve_plot_result
 
@@ -2365,14 +2389,15 @@
         # Act
         result = model.plot_voronoi(width=custom_width, height=custom_height)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningRegressionTreePlot:
     @pytest.fixture(autouse=True)
     def result(self, regression_tree_plot_result):
         self.result, self.x_col, self.y_col = regression_tree_plot_result
 
@@ -2446,14 +2471,15 @@
             width=custom_width,
         )
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningSVMClassifierPlot:
     @pytest.fixture(autouse=True)
     def result(self, svm_plot_result, svm_2d_plot_result, svm_3d_plot_result):
         self.result = svm_plot_result
         self.result_2d = svm_2d_plot_result
@@ -2513,41 +2539,43 @@
         # Assert
         assert len(self.result_3d.data) == total_items, "Some elements missing"
 
     def test_additional_options_custom_height(self, load_plotly, iris_one_hot_vd):
         # rrange
         custom_height = 650
         custom_width = 700
-        model = LinearSVC(name="public.SVC_iris")
+        model = LinearSVC(name="public.SVC_iris_h")
         model.fit(iris_one_hot_vd, ["PetalLengthCm"], "Species_Iris-setosa")
         # Act
         result = model.plot(width=custom_width, height=custom_height)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
     def test_additional_options_custom_height_for_2d(
         self, load_plotly, iris_one_hot_vd
     ):
         # rrange
         custom_height = 650
         custom_width = 700
-        model = LinearSVC(name="public.SVC_iris")
+        model = LinearSVC(name="public.SVC_iris_2d")
         model.fit(
             iris_one_hot_vd, ["PetalLengthCm", "SepalWidthCm"], "Species_Iris-setosa"
         )
         # Act
         result = model.plot(width=custom_width, height=custom_height)
         # Assert
         assert (
             result.layout["height"] == custom_height
             and result.layout["width"] == custom_width
         ), "Custom height and width not working"
+        model.drop()
 
 
 class TestMachineLearningChampionChallengerPlot:
     @pytest.fixture(autouse=True)
     def result(self, champion_challenger_plot_result):
         self.result = champion_challenger_plot_result
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_preprocessing.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_preprocessing.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vDataFrame/test_vDF_utilities.py` & `verticapy-1.0.0b2/verticapy/tests/vDataFrame/test_vDF_utilities.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/__init__.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_balance.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_balance.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_bisecting_kmeans.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_bisecting_kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,7 +253,11 @@
         assert res[0] == res_py[0]
         assert res[1] == res_py[1]
         vdf = vDataFrame("public.bsk_data")
         vdf["prediction_sql"] = mmodel.predict_sql(["col1", "col2", "col3", "col4"])
         model.predict(vdf, name="prediction_vertica_sql")
         score = vdf.score("prediction_sql", "prediction_vertica_sql", metric="accuracy")
         assert score == pytest.approx(1.0)
+
+    def test_optional_name(self):
+        model = BisectingKMeans()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_countvectorizer.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_countvectorizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 
 # Pytest
 import pytest
 
+# Other Modules
+from vertica_python.errors import QueryError
+
 # VerticaPy
 from verticapy import (
     drop,
     set_option,
 )
 from verticapy.connection import current_cursor
 from verticapy.datasets import load_titanic
@@ -109,7 +112,28 @@
         model_class = CountVectorizer(
             "model_test_vdf",
         )
         model_class.drop()
         model_class.fit(titanic_vd, ["name"])
         assert model_class.transform().shape() == (1841, 4)
         model_class.drop()
+
+    def test_AutoDataPrep_overwrite_model(self, titanic_vd):
+        model = CountVectorizer("test_overwrite_model")
+        model.drop()
+        model.fit(titanic_vd, ["name"])
+
+        # overwrite_model is false by default
+        with pytest.raises(QueryError) as exception_info:
+            model.fit(titanic_vd)
+        assert "throwErrorFunctionDoesNotMatchCandidates" in str(exception_info.value)
+
+        # overwriting the model when overwrite_model is specified true
+        model = CountVectorizer("test_overwrite_model", overwrite_model=True)
+        model.fit(titanic_vd, ["name"])
+
+        # cleaning up
+        model.drop()
+
+    def test_optional_name(self):
+        model = CountVectorizer()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_dbscan.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression_tree.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,81 +10,64 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-
 # Pytest
 import pytest
 
-# Other Modules
-import matplotlib.pyplot as plt
+# Vertica
+from verticapy.tests_new.plotting.base_test_files import LearningRegressionTreePlot
+
 
-# VerticaPy
-import verticapy
-from verticapy import (
-    drop,
-    set_option,
-)
-from verticapy.connection import current_cursor
-from verticapy.datasets import load_titanic
-from verticapy.learn.cluster import DBSCAN
-
-set_option("print_info", False)
-
-
-@pytest.fixture(scope="module")
-def titanic_vd():
-    titanic = load_titanic()
-    yield titanic
-    drop(
-        name="public.titanic",
-    )
-
-
-@pytest.fixture(scope="module")
-def model(titanic_vd):
-    model_class = DBSCAN(
-        "DBSCAN_model_test",
-    )
-    model_class.drop()
-    model_class.fit("public.titanic", ["age", "fare"])
-    yield model_class
-    model_class.drop()
-
-
-class TestDBSCAN:
-    def test_repr(self, model):
-        assert model.__repr__() == "<DBSCAN>"
-
-    def test_get_params(self, model):
-        assert model.get_params() == {"eps": 0.5, "min_samples": 5, "p": 2}
-
-    def test_get_predict(self, titanic_vd, model):
-        titanic_copy = model.predict()
-
-        assert titanic_copy["dbscan_cluster"].min() == pytest.approx(-1, abs=1e-6)
-
-    def test_get_attributes(self, model):
-        result = model.get_attributes()
-        assert result == ["n_cluster_", "n_noise_", "p_"]
-
-    def test_get_plot(self, model):
-        result = model.plot()
-        assert len(result.get_default_bbox_extra_artists()) == 9
-        plt.close("all")
-
-    def test_set_params(self, model):
-        model.set_params({"p": 1})
-
-        assert model.get_params()["p"] == 1
-
-    def test_model_from_vDF(self, titanic_vd):
-        model_test = DBSCAN("dbscan_from_vDF")
-        model_test.drop()
-        model_test.fit(titanic_vd, ["age", "fare"], "survived")
-        assert model_test.predict()["dbscan_cluster"].min() == pytest.approx(
-            -1, abs=1e-6
+class TestPlotlyMachineLearningRegressionTreePlot(LearningRegressionTreePlot):
+    """
+    Testing different attributes of Regression Tree plot
+    """
+
+    def test_properties_observations_label(self):
+        """
+        Test plot title
+        """
+        # Arrange
+        test_title = "Observations"
+        # Act
+        # Assert
+        assert self.result.data[0]["name"] == test_title, "X axis label incorrect"
+
+    def test_properties_prediction_label(self):
+        """
+        Test plot title
+        """
+        # Arrange
+        test_title = "Prediction"
+        # Act
+        # Assert
+        assert self.result.data[1]["name"] == test_title, "Y axis label incorrect"
+
+    def test_properties_hover_label(self):
+        """
+        Test hover labels
+        """
+        # Arrange
+        test_title = (
+            f"{self.COL_NAME_1}: %" "{x} <br>" f"{self.COL_NAME_2}: %" "{y} <br>"
         )
-        model_test.drop()
+        # Act
+        # Assert
+        assert (
+            self.result.data[0]["hovertemplate"] == test_title
+        ), "Hover information incorrect"
+
+    def test_properties_no_of_elements(self):
+        """
+        Test number of elements
+        """
+        # Arrange
+        total_items = 2
+        # Act
+        # Assert
+        assert len(self.result.data) == pytest.approx(
+            total_items, abs=1
+        ), "Some elements missing"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_decision_tree_classifier.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_decision_tree_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,7 +494,11 @@
             "Bus",
             "Train",
         ]
 
     def test_plot_tree(self, model):
         result = model.plot_tree()
         assert model.to_graphviz() == result.source.strip()
+
+    def test_optional_name(self):
+        model = DecisionTreeClassifier()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_decision_tree_regressor.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_decision_tree_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,7 +359,11 @@
             "0.000000",
             "1.000000",
         ]
 
     def test_plot_tree(self, model):
         result = model.plot_tree()
         assert model.to_graphviz() == result.source.strip()
+
+    def test_optional_name(self):
+        model = DecisionTreeRegressor()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_delphi.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_dbscan.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,91 +16,99 @@
 """
 
 # Pytest
 import pytest
 
 # Other Modules
 import matplotlib.pyplot as plt
+from vertica_python.errors import DuplicateObject
 
 # VerticaPy
-from verticapy import set_option, drop
-from verticapy.datasets import load_winequality, load_amazon, load_titanic
-from verticapy.learn.delphi import AutoML, AutoDataPrep, AutoClustering
+import verticapy
+from verticapy import (
+    drop,
+    set_option,
+)
+from verticapy.connection import current_cursor
+from verticapy.datasets import load_titanic
+from verticapy.learn.cluster import DBSCAN
 
 set_option("print_info", False)
-set_option("random_state", 0)
-
-
-@pytest.fixture(scope="module")
-def amazon_vd():
-    amazon = load_amazon()
-    yield amazon
-    drop(name="public.amazon")
 
 
 @pytest.fixture(scope="module")
 def titanic_vd():
     titanic = load_titanic()
     yield titanic
-    drop(name="public.titanic")
+    drop(
+        name="public.titanic",
+    )
 
 
 @pytest.fixture(scope="module")
-def winequality_vd():
-    winequality = load_winequality()
-    yield winequality
-    drop(name="public.winequality")
+def model(titanic_vd):
+    model_class = DBSCAN(
+        "DBSCAN_model_test",
+    )
+    model_class.drop()
+    model_class.fit("public.titanic", ["age", "fare"])
+    yield model_class
+    model_class.drop()
+
+
+class TestDBSCAN:
+    def test_repr(self, model):
+        assert model.__repr__() == "<DBSCAN>"
+
+    def test_get_params(self, model):
+        assert model.get_params() == {"eps": 0.5, "min_samples": 5, "p": 2}
+
+    def test_get_predict(self, titanic_vd, model):
+        titanic_copy = model.predict()
+
+        assert titanic_copy["dbscan_cluster"].min() == pytest.approx(-1, abs=1e-6)
+
+    def test_get_attributes(self, model):
+        result = model.get_attributes()
+        assert result == ["n_cluster_", "n_noise_", "p_"]
+
+    def test_get_plot(self, model):
+        result = model.plot()
+        assert len(result.get_default_bbox_extra_artists()) == 9
+        plt.close("all")
 
+    def test_set_params(self, model):
+        model.set_params({"p": 1})
 
-class TestDelphi:
-    def test_AutoML(self, titanic_vd):
-        model = AutoML(
-            "AutoML_test_ml",
-        )
-        model.drop()
-        model.fit(titanic_vd, y="survived")
-        assert model.model_grid_["avg_score"][0] < 0.1
-        assert len(model.plot().get_default_bbox_extra_artists()) < 30
-        plt.close("all")
-        assert len(model.plot("stepwise").get_default_bbox_extra_artists()) < 200
-        plt.close("all")
-        model.drop()
+        assert model.get_params()["p"] == 1
 
-    def test_AutoDataPrep(self, titanic_vd, amazon_vd):
-        model = AutoDataPrep(
-            "AutoML_test_dp",
+    def test_model_from_vDF(self, titanic_vd):
+        model_test = DBSCAN("dbscan_from_vDF")
+        model_test.drop()
+        model_test.fit(titanic_vd, ["age", "fare"], "survived")
+        assert model_test.predict()["dbscan_cluster"].min() == pytest.approx(
+            -1, abs=1e-6
         )
-        model.drop()
-        model.fit(titanic_vd)
-        assert model.final_relation_.shape() == (1234, 56)
-        model.drop()
-        model2 = AutoDataPrep("AutoML_test_dp_2", num_method="same_freq")
-        model2.drop()
-        model2.fit(titanic_vd)
-        assert model2.final_relation_.shape() == (1234, 101)
-        model2.drop()
-        model3 = AutoDataPrep(
-            "AutoML_test_dp_3",
-            num_method="same_width",
-            na_method="drop",
-            apply_pca=True,
-        )
-        model3.drop()
-        model3.fit(titanic_vd)
-        assert model3.final_relation_.shape() == (112, 122)
-        model3.drop()
-        model4 = AutoDataPrep(
-            "AutoML_test_dp_4",
-        )
-        model4.drop()
-        model4.fit(amazon_vd)
-        assert model4.final_relation_.shape() == (6318, 3)
-        model4.drop()
-
-    def test_AutoClustering(self, titanic_vd):
-        model = AutoClustering(
-            "AutoML_test_cluster",
+        model_test.drop()
+
+    def test_overwrite_model(self, titanic_vd):
+        model = DBSCAN("test_overwrite_model")
+        model.drop()  # to isulate this test from any previous left over
+        model.fit(titanic_vd, ["age", "fare"], "survived")
+
+        # overwrite_model is false by default
+        with pytest.raises(DuplicateObject) as exception_info:
+            model.fit(titanic_vd, ["age", "fare"], "survived")
+        assert 'Object "test_overwrite_model" already exists' in str(
+            exception_info.value
         )
+
+        # overwriting the model when overwrite_model is specified true
+        model = DBSCAN("test_overwrite_model", overwrite_model=True)
+        model.fit(titanic_vd, ["age", "fare"], "survived")
+
+        # cleaning up
         model.drop()
-        model.fit(titanic_vd)
-        assert model.model_.parameters["n_cluster"] < 100
-        model.drop()
+
+    def test_optional_name(self):
+        model = DBSCAN()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_dummy_tree_classifier.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_dummy_tree_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,7 +479,11 @@
             "Bus",
             "Train",
         ]
 
     def test_plot_tree(self, model):
         result = model.plot_tree()
         assert model.to_graphviz() == result.source.strip()
+
+    def test_optional_name(self):
+        model = DummyTreeClassifier()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_dummy_tree_regressor.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_dummy_tree_regressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,7 +344,11 @@
             "0.000000",
             "1.000000",
         ]
 
     def test_plot_tree(self, model):
         result = model.plot_tree()
         assert model.to_graphviz() == result.source.strip()
+
+    def test_optional_name(self):
+        model = DummyTreeRegressor()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_elastic_net.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_elastic_net.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,7 +329,11 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'enet_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "enet_from_vDF"
 
         model_test.drop()
+
+    def test_optional_name(self):
+        model = ElasticNet()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_iforest.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_iforest.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,7 +307,11 @@
             "3.000000",
             "3.000000",
         ]
 
     def test_plot_tree(self, model):
         result = model.plot_tree()
         assert model.to_graphviz() == result.source.strip()
+
+    def test_optional_name(self):
+        model = IsolationForest()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_kde.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_lof.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 """
 
 # Pytest
 import pytest
 
 # Other Modules
 import matplotlib.pyplot as plt
+from vertica_python.errors import DuplicateObject
 
 # VerticaPy
 from verticapy import (
     drop,
     set_option,
 )
 from verticapy.connection import current_cursor
 from verticapy.datasets import load_titanic
-from verticapy.learn.neighbors import KernelDensity
+from verticapy.learn.neighbors import LocalOutlierFactor
 
 set_option("print_info", False)
 
 
 @pytest.fixture(scope="module")
 def titanic_vd():
     titanic = load_titanic()
@@ -40,71 +41,86 @@
     drop(
         name="public.titanic",
     )
 
 
 @pytest.fixture(scope="module")
 def model(titanic_vd):
-    model_class = KernelDensity(
-        "KernelDensity_model_test",
+    model_class = LocalOutlierFactor(
+        "lof_model_test",
     )
     model_class.drop()
     model_class.fit("public.titanic", ["age", "fare"])
     yield model_class
     model_class.drop()
 
 
-class TestKernelDensity:
+class TestLocalOutlierFactor:
     def test_repr(self, model):
-        assert model.__repr__() == "<KernelDensity>"
+        assert model.__repr__() == "<LocalOutlierFactor>"
 
     def test_get_params(self, model):
-        assert model.get_params() == {
-            "bandwidth": 1,
-            "kernel": "gaussian",
-            "max_depth": 5,
-            "max_leaf_nodes": 1000000000,
-            "min_samples_leaf": 1,
-            "nbins": 5,
-            "p": 2,
-            "xlim": [],
-        }
+        assert model.get_params() == {"n_neighbors": 20, "p": 2}
 
     def test_get_predict(self, titanic_vd, model):
-        titanic_copy = model.predict(titanic_vd.copy(), name="kde")
+        titanic_copy = model.predict()
 
-        assert titanic_copy["kde"].mean() == pytest.approx(
-            1.82115211838814e-06, abs=1e-6
+        assert titanic_copy["lof_score"].mean() == pytest.approx(
+            1.17226637499694, abs=1e-6
         )
 
-    def test_get_vertica_attributes(self, model):
-        result = model.get_vertica_attributes()
-        assert result["attr_name"][0] == "tree_count"
+    def test_get_attributes(self, model):
+        result = model.get_attributes()
+        assert result == ["n_neighbors_", "p_", "n_errors_", "cnt_"]
 
     def test_get_plot(self, model):
-        result = model.plot()
-        assert len(result.get_default_bbox_extra_artists()) == 8
+        result = model.plot(color=["r", "b"])
+        assert len(result.get_default_bbox_extra_artists()) == 9
         plt.close("all")
-        model_test = KernelDensity("model_test_plot_kde_plot")
+        model_test = LocalOutlierFactor("model_test_plot_lof")
         model_test.drop()
         model_test.fit("public.titanic", ["age"])
-        result = model_test.plot()
+        result = model_test.plot(color=["r", "b"])
         assert len(result.get_default_bbox_extra_artists()) == 9
         model_test.drop()
 
+        model_test = LocalOutlierFactor("model_test_plot_lof_2")
+        model_test.drop()
+        model_test.fit("public.titanic", ["age", "fare", "pclass"])
+        result = model_test.plot(color=["r", "b"])
+        assert len(result.get_default_bbox_extra_artists()) == 3
+        model_test.drop()
+
     def test_set_params(self, model):
         model.set_params({"p": 1})
 
         assert model.get_params()["p"] == 1
 
     def test_model_from_vDF(self, titanic_vd):
-        model_test = KernelDensity(
-            "KernelDensity_from_vDF_tmp",
+        model_test = LocalOutlierFactor(
+            "lof_from_vDF_tmp",
         )
         model_test.drop()
         model_test.fit(titanic_vd, ["age", "fare"])
-        titanic_copy = model_test.predict(titanic_vd.copy(), name="kde")
-
-        assert titanic_copy["kde"].mean() == pytest.approx(
-            1.82115211838814e-06, abs=1e-6
+        assert model_test.predict()["lof_score"].mean() == pytest.approx(
+            1.17226637499694, abs=1e-6
         )
         model_test.drop()
+
+    def test_overwrite_model(self, titanic_vd):
+        model = LocalOutlierFactor("test_overwrite_model")
+        model.drop()  # to isulate this test from any previous left over
+        model.fit(titanic_vd, ["age", "fare"])
+
+        # overwrite_model is false by default
+        with pytest.raises(DuplicateObject) as exception_info:
+            model.fit(titanic_vd, ["age", "fare"])
+        assert 'Object "test_overwrite_model" already exists' in str(
+            exception_info.value
+        )
+
+        # overwriting the model when overwrite_model is specified true
+        model = LocalOutlierFactor("test_overwrite_model", overwrite_model=True)
+        model.fit(titanic_vd, ["age", "fare"])
+
+        # cleaning up
+        model.drop()
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_kmeans.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_kprototypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,217 +18,222 @@
 # Pytest
 import pytest
 
 # Other Modules
 import matplotlib.pyplot as plt
 
 # VerticaPy
+from verticapy.tests.conftest import get_version
 from verticapy import drop, set_option
 from verticapy.connection import current_cursor
-from verticapy.datasets import load_iris, load_winequality
-from verticapy.learn.cluster import KMeans
+from verticapy.datasets import load_iris
+from verticapy.learn.cluster import KPrototypes
 
 set_option("print_info", False)
 
 
 @pytest.fixture(scope="module")
 def iris_vd():
     iris = load_iris()
     yield iris
     drop(
         name="public.iris",
     )
 
 
 @pytest.fixture(scope="module")
-def winequality_vd():
-    winequality = load_winequality()
-    yield winequality
-    drop(
-        name="public.winequality",
-    )
-
-
-@pytest.fixture(scope="module")
 def model(iris_vd):
-    model_class = KMeans(
-        "kmeans_model_test",
+    model_class = KPrototypes(
+        "kprototypes_model_test",
         n_cluster=3,
         max_iter=10,
-        init=[[7.2, 3.0, 5.8, 1.6], [6.9, 3.1, 4.9, 1.5], [5.7, 4.4, 1.5, 0.4]],
+        init=[
+            [7.2, 3.0, 5.8, 1.6, "Iris-setosa"],
+            [6.9, 3.1, 4.9, 1.5, "Iris-versicolor"],
+            [5.7, 4.4, 1.5, 0.4, "Iris-virginica"],
+        ],
     )
     model_class.drop()
-    model_class.fit(
-        "public.iris",
-        ["SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm"],
-    )
+    model_class.fit(iris_vd)
     yield model_class
     model_class.drop()
 
 
-class TestKMeans:
+version = get_version()
+
+
+@pytest.mark.skipif(
+    version[0] < 12 or (version[0] == 12 and version[1] == 0 and version[2] < 3),
+    reason="requires vertica 12.0.3 or higher",
+)
+class TestKPrototypes:
     def test_repr(self, model):
-        assert model.__repr__() == "<KMeans>"
+        assert model.__repr__() == "<KPrototypes>"
 
     def test_deploySQL(self, model):
-        expected_sql = 'APPLY_KMEANS("SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm" USING PARAMETERS model_name = \'kmeans_model_test\', match_by_pos = \'true\')'
+        expected_sql = 'APPLY_KPROTOTYPES("SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm", "Species" USING PARAMETERS model_name = \'kprototypes_model_test\', match_by_pos = \'true\')'
         result_sql = model.deploySQL()
 
         assert result_sql == expected_sql
 
     def test_drop(self):
-        current_cursor().execute("DROP MODEL IF EXISTS kmeans_model_test_drop")
-        model_test = KMeans(
-            "kmeans_model_test_drop",
-        )
-        model_test.fit("public.iris", ["SepalLengthCm", "SepalWidthCm"])
+        current_cursor().execute("DROP MODEL IF EXISTS kprototypes_model_test_drop")
+        model_test = KPrototypes("kprototypes_model_test_drop", n_cluster=3)
+        model_test.fit("public.iris", ["SepalLengthCm", "SepalWidthCm", "Species"])
 
         current_cursor().execute(
-            "SELECT model_name FROM models WHERE model_name = 'kmeans_model_test_drop'"
+            "SELECT model_name FROM models WHERE model_name = 'kprototypes_model_test_drop'"
         )
-        assert current_cursor().fetchone()[0] == "kmeans_model_test_drop"
+        assert current_cursor().fetchone()[0] == "kprototypes_model_test_drop"
 
         model_test.drop()
         current_cursor().execute(
-            "SELECT model_name FROM models WHERE model_name = 'kmeans_model_test_drop'"
+            "SELECT model_name FROM models WHERE model_name = 'kprototypes_model_test_drop'"
         )
         assert current_cursor().fetchone() is None
 
     def test_get_vertica_attributes(self, model):
         m_att = model.get_vertica_attributes()
 
         assert m_att["attr_name"] == ["centers", "metrics"]
         assert m_att["attr_fields"] == [
-            "sepallengthcm, sepalwidthcm, petallengthcm, petalwidthcm",
+            "sepallengthcm, sepalwidthcm, petallengthcm, petalwidthcm, species",
             "metrics",
         ]
         assert m_att["#_of_rows"] == [3, 1]
 
         m_att_centers = model.get_vertica_attributes(attr_name="centers")
 
         assert m_att_centers["sepallengthcm"] == [
             pytest.approx(5.006),
-            pytest.approx(5.90161290322581),
-            pytest.approx(6.85),
+            pytest.approx(5.9156862745098),
+            pytest.approx(6.62244897959184),
         ]
 
     def test_get_params(self, model):
         assert model.get_params() == {
             "max_iter": 10,
             "tol": 0.0001,
             "n_cluster": 3,
             "init": [
-                [7.2, 3.0, 5.8, 1.6],
-                [6.9, 3.1, 4.9, 1.5],
-                [5.7, 4.4, 1.5, 0.4],
+                [7.2, 3.0, 5.8, 1.6, "Iris-setosa"],
+                [6.9, 3.1, 4.9, 1.5, "Iris-versicolor"],
+                [5.7, 4.4, 1.5, 0.4, "Iris-virginica"],
             ],
+            "gamma": 1.0,
         }
 
     def test_get_predict(self, iris_vd, model):
         iris_copy = iris_vd.copy()
 
         model.predict(
             iris_copy,
-            X=["SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm"],
+            X=[
+                "SepalLengthCm",
+                "SepalWidthCm",
+                "PetalLengthCm",
+                "PetalWidthCm",
+                "Species",
+            ],
             name="pred",
         )
 
         assert iris_copy["pred"].mode() == 1
         assert iris_copy["pred"].distinct() == [0, 1, 2]
 
     def test_set_params(self, model):
         model.set_params({"max_iter": 20})
         assert model.get_params()["max_iter"] == 20
 
     def test_model_from_vDF(self, iris_vd):
-        current_cursor().execute("DROP MODEL IF EXISTS kmeans_vDF")
-        model_test = KMeans("kmeans_vDF", init="random")
-        model_test.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm"])
+        current_cursor().execute("DROP MODEL IF EXISTS kprototypes_vDF")
+        model_test = KPrototypes("kprototypes_vDF", n_cluster=3, init="random")
+        model_test.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm", "Species"])
         current_cursor().execute(
-            "SELECT model_name FROM models WHERE model_name = 'kmeans_vDF'"
+            "SELECT model_name FROM models WHERE model_name = 'kprototypes_vDF'"
         )
-        assert current_cursor().fetchone()[0] == "kmeans_vDF"
+        assert current_cursor().fetchone()[0] == "kprototypes_vDF"
         model_test.drop()
 
     def test_init_method(self):
-        model_test_kmeanspp = KMeans("kmeanspp_test", init="kmeanspp")
-        model_test_kmeanspp.drop()
-        model_test_kmeanspp.fit("public.iris")
-
-        current_cursor().execute(
-            "SELECT model_name FROM models WHERE model_name = 'kmeanspp_test'"
-        )
-        assert current_cursor().fetchone()[0] == "kmeanspp_test"
-        model_test_kmeanspp.drop()
-
-        model_test_random = KMeans("random_test", init="random")
+        model_test_random = KPrototypes("random_test", n_cluster=3, init="random")
         model_test_random.drop()
         model_test_random.fit("public.iris")
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'random_test'"
         )
         assert current_cursor().fetchone()[0] == "random_test"
         model_test_random.drop()
 
-    def test_get_plot(self, winequality_vd):
+    def test_get_plot(self, iris_vd):
         current_cursor().execute("DROP MODEL IF EXISTS model_test_plot")
-        model_test = KMeans(
+        model_test = KPrototypes(
             "model_test_plot",
+            n_cluster=3,
         )
-        model_test.fit(winequality_vd, ["alcohol", "quality"])
+        model_test.fit(iris_vd, ["SepalLengthCm", "PetalWidthCm"])
         result = model_test.plot(color="b")
         assert len(result.get_default_bbox_extra_artists()) > 8
         plt.close("all")
         model_test.drop()
+        # TODO: test for categorical inputs.
 
     def test_to_python(self, model):
         current_cursor().execute(
-            "SELECT APPLY_KMEANS(5.006, 3.418, 1.464, 0.244 USING PARAMETERS model_name = '{}', match_by_pos=True)".format(
+            "SELECT APPLY_KPROTOTYPES(5.006, 3.418, 1.464, 0.244, 'Iris-setosa' USING PARAMETERS model_name = '{0}', match_by_pos=True)".format(
                 model.model_name
             )
         )
         prediction = current_cursor().fetchone()[0]
         assert prediction == pytest.approx(
-            model.to_python()([[5.006, 3.418, 1.464, 0.244]])[0]
+            model.to_python()([[5.006, 3.418, 1.464, 0.244, "Iris-setosa"]])[0]
         )
         assert 0.0 == pytest.approx(
             model.to_python(return_distance_clusters=True)(
                 [[5.006, 3.418, 1.464, 0.244]]
             )[0][0]
         )
 
     def test_to_sql(self, model):
         current_cursor().execute(
-            "SELECT APPLY_KMEANS(5.006, 3.418, 1.464, 0.244 USING PARAMETERS model_name = '{}', match_by_pos=True)::float, {}::float".format(
-                model.model_name, model.to_sql([5.006, 3.418, 1.464, 0.244])
+            "SELECT APPLY_KPROTOTYPES(5.006, 3.418, 1.464, 0.244, 'Iris-setosa' USING PARAMETERS model_name = '{0}', match_by_pos=True)::float, {1}::float".format(
+                model.model_name,
+                model.to_sql([5.006, 3.418, 1.464, 0.244, "'Iris-setosa'"]),
             )
         )
         prediction = current_cursor().fetchone()
         assert prediction[0] == pytest.approx(prediction[1])
 
     def test_to_memmodel(self, model, iris_vd):
         mmodel = model.to_memmodel()
-        res = mmodel.predict([[5.006, 3.418, 1.464, 0.244], [3.0, 11.0, 1993.0, 0.0]])
+        res = mmodel.predict(
+            [
+                [5.006, 3.418, 1.464, 0.244, "Iris-setosa"],
+                [3.0, 11.0, 1993.0, 0.0, "Iris-setosa"],
+            ]
+        )
         res_py = model.to_python()(
-            [[5.006, 3.418, 1.464, 0.244], [3.0, 11.0, 1993.0, 0.0]]
+            [
+                [5.006, 3.418, 1.464, 0.244, "Iris-setosa"],
+                [3.0, 11.0, 1993.0, 0.0, "Iris-setosa"],
+            ]
         )
         assert res[0] == res_py[0]
         assert res[1] == res_py[1]
         vdf = iris_vd.copy()
         vdf["prediction_sql"] = mmodel.predict_sql(
-            ["SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm"]
+            [
+                "SepalLengthCm",
+                "SepalWidthCm",
+                "PetalLengthCm",
+                "PetalWidthCm",
+                "Species",
+            ]
         )
         model.predict(vdf, name="prediction_vertica_sql")
         score = vdf.score("prediction_sql", "prediction_vertica_sql", metric="accuracy")
-        assert score == pytest.approx(1.0)
+        assert score == pytest.approx(0.993333333333333)  # can we do better?
 
-    def test_get_voronoi_plot(self, iris_vd):
-        current_cursor().execute("DROP MODEL IF EXISTS model_test_plot")
-        model_test = KMeans(
-            "model_test_plot",
-        )
-        model_test.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm"])
-        result = model_test.plot_voronoi(color="b")
-        assert len(result.gca().get_default_bbox_extra_artists()) == 21
-        plt.close("all")
-        model_test.drop()
+    def test_optional_name(self):
+        model = KPrototypes()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_knn_classifier.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_knn_regressor.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_knn_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,7 +183,11 @@
         model_test = KNeighborsRegressor(
             "knn_from_vDF",
         )
         model_test.drop()
         model_test.fit(titanic_vd, ["age"], "survived")
         assert model_test.score() == pytest.approx(-0.122616967579114)
         model_test.drop()
+
+    def test_optional_name(self):
+        model = KNeighborsRegressor()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_kprototypes.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_kmeans.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,218 +18,234 @@
 # Pytest
 import pytest
 
 # Other Modules
 import matplotlib.pyplot as plt
 
 # VerticaPy
-from verticapy.tests.conftest import get_version
 from verticapy import drop, set_option
 from verticapy.connection import current_cursor
-from verticapy.datasets import load_iris
-from verticapy.learn.cluster import KPrototypes
+from verticapy.datasets import load_iris, load_winequality
+from verticapy.learn.cluster import KMeans
 
 set_option("print_info", False)
 
 
 @pytest.fixture(scope="module")
 def iris_vd():
     iris = load_iris()
     yield iris
     drop(
         name="public.iris",
     )
 
 
 @pytest.fixture(scope="module")
+def winequality_vd():
+    winequality = load_winequality()
+    yield winequality
+    drop(
+        name="public.winequality",
+    )
+
+
+@pytest.fixture(scope="module")
 def model(iris_vd):
-    model_class = KPrototypes(
-        "kprototypes_model_test",
+    model_class = KMeans(
+        "kmeans_model_test",
         n_cluster=3,
         max_iter=10,
-        init=[
-            [7.2, 3.0, 5.8, 1.6, "Iris-setosa"],
-            [6.9, 3.1, 4.9, 1.5, "Iris-versicolor"],
-            [5.7, 4.4, 1.5, 0.4, "Iris-virginica"],
-        ],
+        init=[[7.2, 3.0, 5.8, 1.6], [6.9, 3.1, 4.9, 1.5], [5.7, 4.4, 1.5, 0.4]],
     )
     model_class.drop()
-    model_class.fit(iris_vd)
+    model_class.fit(
+        "public.iris",
+        ["SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm"],
+    )
     yield model_class
     model_class.drop()
 
 
-version = get_version()
-
-
-@pytest.mark.skipif(
-    version[0] < 12 or (version[0] == 12 and version[1] == 0 and version[2] < 3),
-    reason="requires vertica 12.0.3 or higher",
-)
-class TestKPrototypes:
+class TestKMeans:
     def test_repr(self, model):
-        assert model.__repr__() == "<KPrototypes>"
+        assert model.__repr__() == "<KMeans>"
 
     def test_deploySQL(self, model):
-        expected_sql = 'APPLY_KPROTOTYPES("SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm", "Species" USING PARAMETERS model_name = \'kprototypes_model_test\', match_by_pos = \'true\')'
+        expected_sql = 'APPLY_KMEANS("SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm" USING PARAMETERS model_name = \'kmeans_model_test\', match_by_pos = \'true\')'
         result_sql = model.deploySQL()
 
         assert result_sql == expected_sql
 
     def test_drop(self):
-        current_cursor().execute("DROP MODEL IF EXISTS kprototypes_model_test_drop")
-        model_test = KPrototypes("kprototypes_model_test_drop", n_cluster=3)
-        model_test.fit("public.iris", ["SepalLengthCm", "SepalWidthCm", "Species"])
+        current_cursor().execute("DROP MODEL IF EXISTS kmeans_model_test_drop")
+        model_test = KMeans(
+            "kmeans_model_test_drop",
+        )
+        model_test.fit("public.iris", ["SepalLengthCm", "SepalWidthCm"])
 
         current_cursor().execute(
-            "SELECT model_name FROM models WHERE model_name = 'kprototypes_model_test_drop'"
+            "SELECT model_name FROM models WHERE model_name = 'kmeans_model_test_drop'"
         )
-        assert current_cursor().fetchone()[0] == "kprototypes_model_test_drop"
+        assert current_cursor().fetchone()[0] == "kmeans_model_test_drop"
 
         model_test.drop()
         current_cursor().execute(
-            "SELECT model_name FROM models WHERE model_name = 'kprototypes_model_test_drop'"
+            "SELECT model_name FROM models WHERE model_name = 'kmeans_model_test_drop'"
         )
         assert current_cursor().fetchone() is None
 
     def test_get_vertica_attributes(self, model):
         m_att = model.get_vertica_attributes()
 
         assert m_att["attr_name"] == ["centers", "metrics"]
         assert m_att["attr_fields"] == [
-            "sepallengthcm, sepalwidthcm, petallengthcm, petalwidthcm, species",
+            "sepallengthcm, sepalwidthcm, petallengthcm, petalwidthcm",
             "metrics",
         ]
         assert m_att["#_of_rows"] == [3, 1]
 
         m_att_centers = model.get_vertica_attributes(attr_name="centers")
 
         assert m_att_centers["sepallengthcm"] == [
             pytest.approx(5.006),
-            pytest.approx(5.9156862745098),
-            pytest.approx(6.62244897959184),
+            pytest.approx(5.90161290322581),
+            pytest.approx(6.85),
         ]
 
     def test_get_params(self, model):
         assert model.get_params() == {
             "max_iter": 10,
             "tol": 0.0001,
             "n_cluster": 3,
             "init": [
-                [7.2, 3.0, 5.8, 1.6, "Iris-setosa"],
-                [6.9, 3.1, 4.9, 1.5, "Iris-versicolor"],
-                [5.7, 4.4, 1.5, 0.4, "Iris-virginica"],
+                [7.2, 3.0, 5.8, 1.6],
+                [6.9, 3.1, 4.9, 1.5],
+                [5.7, 4.4, 1.5, 0.4],
             ],
-            "gamma": 1.0,
         }
 
     def test_get_predict(self, iris_vd, model):
         iris_copy = iris_vd.copy()
 
         model.predict(
             iris_copy,
-            X=[
-                "SepalLengthCm",
-                "SepalWidthCm",
-                "PetalLengthCm",
-                "PetalWidthCm",
-                "Species",
-            ],
+            X=["SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm"],
             name="pred",
         )
 
         assert iris_copy["pred"].mode() == 1
         assert iris_copy["pred"].distinct() == [0, 1, 2]
 
     def test_set_params(self, model):
         model.set_params({"max_iter": 20})
         assert model.get_params()["max_iter"] == 20
 
     def test_model_from_vDF(self, iris_vd):
-        current_cursor().execute("DROP MODEL IF EXISTS kprototypes_vDF")
-        model_test = KPrototypes("kprototypes_vDF", n_cluster=3, init="random")
-        model_test.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm", "Species"])
+        current_cursor().execute("DROP MODEL IF EXISTS kmeans_vDF")
+        model_test = KMeans("kmeans_vDF", init="random")
+        model_test.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm"])
         current_cursor().execute(
-            "SELECT model_name FROM models WHERE model_name = 'kprototypes_vDF'"
+            "SELECT model_name FROM models WHERE model_name = 'kmeans_vDF'"
         )
-        assert current_cursor().fetchone()[0] == "kprototypes_vDF"
+        assert current_cursor().fetchone()[0] == "kmeans_vDF"
         model_test.drop()
 
     def test_init_method(self):
-        model_test_random = KPrototypes("random_test", n_cluster=3, init="random")
+        model_test_kmeanspp = KMeans("kmeanspp_test", init="kmeanspp")
+        model_test_kmeanspp.drop()
+        model_test_kmeanspp.fit("public.iris")
+
+        current_cursor().execute(
+            "SELECT model_name FROM models WHERE model_name = 'kmeanspp_test'"
+        )
+        assert current_cursor().fetchone()[0] == "kmeanspp_test"
+        model_test_kmeanspp.drop()
+
+        model_test_random = KMeans("random_test", init="random")
         model_test_random.drop()
         model_test_random.fit("public.iris")
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'random_test'"
         )
         assert current_cursor().fetchone()[0] == "random_test"
         model_test_random.drop()
 
-    def test_get_plot(self, iris_vd):
+    def test_get_plot(self, winequality_vd):
         current_cursor().execute("DROP MODEL IF EXISTS model_test_plot")
-        model_test = KPrototypes(
+        model_test = KMeans(
             "model_test_plot",
-            n_cluster=3,
         )
-        model_test.fit(iris_vd, ["SepalLengthCm", "PetalWidthCm"])
+        model_test.fit(winequality_vd, ["alcohol", "quality"])
         result = model_test.plot(color="b")
         assert len(result.get_default_bbox_extra_artists()) > 8
         plt.close("all")
         model_test.drop()
-        # TODO: test for categorical inputs.
 
     def test_to_python(self, model):
         current_cursor().execute(
-            "SELECT APPLY_KPROTOTYPES(5.006, 3.418, 1.464, 0.244, 'Iris-setosa' USING PARAMETERS model_name = '{0}', match_by_pos=True)".format(
+            "SELECT APPLY_KMEANS(5.006, 3.418, 1.464, 0.244 USING PARAMETERS model_name = '{}', match_by_pos=True)".format(
                 model.model_name
             )
         )
         prediction = current_cursor().fetchone()[0]
         assert prediction == pytest.approx(
-            model.to_python()([[5.006, 3.418, 1.464, 0.244, "Iris-setosa"]])[0]
+            model.to_python()([[5.006, 3.418, 1.464, 0.244]])[0]
         )
         assert 0.0 == pytest.approx(
             model.to_python(return_distance_clusters=True)(
                 [[5.006, 3.418, 1.464, 0.244]]
             )[0][0]
         )
 
     def test_to_sql(self, model):
         current_cursor().execute(
-            "SELECT APPLY_KPROTOTYPES(5.006, 3.418, 1.464, 0.244, 'Iris-setosa' USING PARAMETERS model_name = '{0}', match_by_pos=True)::float, {1}::float".format(
-                model.model_name,
-                model.to_sql([5.006, 3.418, 1.464, 0.244, "'Iris-setosa'"]),
+            "SELECT APPLY_KMEANS(5.006, 3.418, 1.464, 0.244 USING PARAMETERS model_name = '{}', match_by_pos=True)::float, {}::float".format(
+                model.model_name, model.to_sql([5.006, 3.418, 1.464, 0.244])
             )
         )
         prediction = current_cursor().fetchone()
         assert prediction[0] == pytest.approx(prediction[1])
 
     def test_to_memmodel(self, model, iris_vd):
         mmodel = model.to_memmodel()
-        res = mmodel.predict(
-            [
-                [5.006, 3.418, 1.464, 0.244, "Iris-setosa"],
-                [3.0, 11.0, 1993.0, 0.0, "Iris-setosa"],
-            ]
-        )
+        res = mmodel.predict([[5.006, 3.418, 1.464, 0.244], [3.0, 11.0, 1993.0, 0.0]])
         res_py = model.to_python()(
-            [
-                [5.006, 3.418, 1.464, 0.244, "Iris-setosa"],
-                [3.0, 11.0, 1993.0, 0.0, "Iris-setosa"],
-            ]
+            [[5.006, 3.418, 1.464, 0.244], [3.0, 11.0, 1993.0, 0.0]]
         )
         assert res[0] == res_py[0]
         assert res[1] == res_py[1]
         vdf = iris_vd.copy()
         vdf["prediction_sql"] = mmodel.predict_sql(
-            [
-                "SepalLengthCm",
-                "SepalWidthCm",
-                "PetalLengthCm",
-                "PetalWidthCm",
-                "Species",
-            ]
+            ["SepalLengthCm", "SepalWidthCm", "PetalLengthCm", "PetalWidthCm"]
         )
         model.predict(vdf, name="prediction_vertica_sql")
         score = vdf.score("prediction_sql", "prediction_vertica_sql", metric="accuracy")
-        assert score == pytest.approx(0.993333333333333)  # can we do better?
+        assert score == pytest.approx(1.0)
+
+    def test_get_voronoi_plot(self, iris_vd):
+        current_cursor().execute("DROP MODEL IF EXISTS model_test_plot")
+        model_test = KMeans(
+            "model_test_plot",
+        )
+        model_test.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm"])
+        result = model_test.plot_voronoi(color="b")
+        assert len(result.gca().get_default_bbox_extra_artists()) == 21
+        plt.close("all")
+        model_test.drop()
+
+    def test_overwrite_model(self, iris_vd):
+        model = KMeans("test_overwrite_model")
+        model.drop()  # to isulate this test from any previous left over
+        model.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm"])
+
+        # overwrite_model is false by default
+        with pytest.raises(NameError) as exception_info:
+            model.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm"])
+        assert exception_info.match("The model 'test_overwrite_model' already exists!")
+
+        # overwriting the model when overwrite_model is specified true
+        model = KMeans("test_overwrite_model", overwrite_model=True)
+        model.fit(iris_vd, ["SepalLengthCm", "SepalWidthCm"])
+
+        # cleaning up
+        model.drop()
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_lasso.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_lasso.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,7 +328,11 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'lasso_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "lasso_from_vDF"
 
         model_test.drop()
+
+    def test_optional_name(self):
+        model = Lasso()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_linear_regression.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_linear_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -326,7 +326,24 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'linreg_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "linreg_from_vDF"
 
         model_test.drop()
+
+    def test_overwrite_model(self, winequality_vd):
+        model = LinearRegression("test_overwrite_model")
+        model.drop()  # to isulate this test from any previous left over
+        model.fit(winequality_vd, ["alcohol"], "quality")
+
+        # overwrite_model is false by default
+        with pytest.raises(NameError) as exception_info:
+            model.fit(winequality_vd, ["alcohol"], "quality")
+        assert exception_info.match("The model 'test_overwrite_model' already exists!")
+
+        # overwriting the model when overwrite_model is specified true
+        model = LinearRegression("test_overwrite_model", overwrite_model=True)
+        model.fit(winequality_vd, ["alcohol"], "quality")
+
+        # cleaning up
+        model.drop()
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_linear_svc.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_linear_svc.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,7 +409,11 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'lsvc_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "lsvc_from_vDF"
 
         model_test.drop()
+
+    def test_optional_name(self):
+        model = LinearSVC()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_linear_svr.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_linear_svr.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,7 +315,11 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'lsvr_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "lsvr_from_vDF"
 
         model_test.drop()
+
+    def test_optional_name(self):
+        model = LinearSVR()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_logistic_regression.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_logistic_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,7 +439,11 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'logreg_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "logreg_from_vDF"
 
         model_test.drop()
+
+    def test_optional_name(self):
+        model = LogisticRegression()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_mca.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_mca.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,7 +195,11 @@
         )
         model_test.fit(market_vd.cdt())
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'mca_vDF'"
         )
         assert current_cursor().fetchone()[0] == "mca_vDF"
         model_test.drop()
+
+    def test_optional_name(self):
+        model = MCA()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_memmodel.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_memmodel.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_model_selection.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_model_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -381,7 +381,56 @@
         assert result["importance"][-4] == pytest.approx(99.2744192911641096, 1e-4)
         plt.close("all")
         model = LinearRegression("LR_stepwise_test")
         model.drop()
         assert result["importance"][-1] == pytest.approx(0.7255807088358904, 1e-4)
         assert result["importance"][-4] == pytest.approx(99.2744192911641096, 1e-4)
         plt.close("all")
+
+    def test_overwrite_model(self, titanic_vd):
+        titanic = titanic_vd.copy()
+        titanic["boat"].fillna(method="0ifnull")
+        model = LogisticRegression("stepwise_overwrite_model_test")
+        model.drop()
+        model.fit(titanic_vd, ["age", "fare"], "survived")
+
+        # overwrite_model is false by default
+        with pytest.raises(NameError) as exception_info:
+            result = stepwise(
+                model,
+                titanic,
+                ["age", "fare", "boat", "pclass"],
+                "survived",
+                "bic",
+                "backward",
+                100,
+                3,
+                True,
+                "pearson",
+                True,
+                True,
+            )
+        assert exception_info.match(
+            "The model 'stepwise_overwrite_model_test' already exists!"
+        )
+
+        # overwriting the model when overwrite_model is specified true
+        model = LogisticRegression(
+            "stepwise_overwrite_model_test", overwrite_model=True
+        )
+        result = stepwise(
+            model,
+            titanic,
+            ["age", "fare", "boat", "pclass"],
+            "survived",
+            "aic",
+            "forward",
+            100,
+            3,
+            True,
+            "spearman",
+            True,
+            True,
+        )
+
+        # cleaning up
+        model.drop()
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_naive_bayes.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_naive_bayes.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,7 +507,11 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'nb_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "nb_from_vDF"
 
         model_test.drop()
+
+    def test_optional_name(self):
+        model = NaiveBayes()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_nearestcentroid.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_nearestcentroid.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,7 +245,11 @@
         )
         model_test.drop()
         model_test.fit(titanic_vd, ["age"], "survived")
         assert model_test.score(cutoff=0.9, metric="accuracy") == pytest.approx(
             0.6078234704112337
         )
         model_test.drop()
+
+    def test_optional_name(self):
+        model = NearestCentroid()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_normalizer.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,7 +350,17 @@
         )
         model_test.fit(winequality_vd, ["alcohol", "quality"])
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'norm_vDF'"
         )
         assert current_cursor().fetchone()[0] == "norm_vDF"
         model_test.drop()
+
+    def test_optional_name(self):
+        model = Scaler()
+        assert model.model_name is not None
+        model = StandardScaler()
+        assert model.model_name is not None
+        model = RobustScaler()
+        assert model.model_name is not None
+        model = MinMaxScaler()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_onehotencoder.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_onehotencoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,7 +201,11 @@
         model_test = OneHotEncoder("ohe_vDF", drop_first=False)
         model_test.fit(titanic_vd, ["pclass", "embarked"])
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'ohe_vDF'"
         )
         assert current_cursor().fetchone()[0] == "ohe_vDF"
         model_test.drop()
+
+    def test_optional_name(self):
+        model = OneHotEncoder()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_pca.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,7 +222,11 @@
         )
         model_test.fit(winequality_vd, ["alcohol", "quality"])
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'pca_vDF'"
         )
         assert current_cursor().fetchone()[0] == "pca_vDF"
         model_test.drop()
+
+    def test_optional_name(self):
+        model = PCA()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_pipeline.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,7 +277,57 @@
             winequality_vd, ["citric_acid", "residual_sugar", "alcohol"], "quality"
         )
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name IN ('std_model_test_vdf', 'linreg_model_test_vdf')"
         )
         assert len(current_cursor().fetchall()) == 2
         model_test.drop()
+
+    def test_overwrite_model(self, winequality_vd):
+        model = Pipeline(
+            [
+                (
+                    "ScalerWine",
+                    Scaler(
+                        "std_test_overwrite_model",
+                    ),
+                ),
+                (
+                    "LinearRegressionWine",
+                    LinearRegression(
+                        "linreg_test_overwrite_model",
+                    ),
+                ),
+            ]
+        )
+        model.drop()
+        model.fit(winequality_vd, ["alcohol"], "quality")
+
+        # overwrite_model is false by default
+        with pytest.raises(NameError) as exception_info:
+            model.fit(winequality_vd, ["alcohol"], "quality")
+        assert exception_info.match(
+            "The model 'std_test_overwrite_model' already exists!"
+        )
+
+        # overwriting the model when overwrite_model is specified true
+        model = Pipeline(
+            [
+                (
+                    "ScalerWine",
+                    Scaler(
+                        "std_test_overwrite_model",
+                    ),
+                ),
+                (
+                    "LinearRegressionWine",
+                    LinearRegression(
+                        "linreg_test_overwrite_model",
+                    ),
+                ),
+            ],
+            overwrite_model=True,
+        )
+        model.fit(winequality_vd, ["alcohol"], "quality")
+
+        # cleaning up
+        model.drop()
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_randomforest_classifier.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_randomforest_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,7 +510,11 @@
             "Bus",
             "Train",
         ]
 
     def test_plot_tree(self, model):
         result = model.plot_tree()
         assert model.to_graphviz() == result.source.strip()
+
+    def test_optional_name(self):
+        model = RandomForestClassifier()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_randomforest_regressor.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_randomforest_regressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,7 +394,11 @@
             "0.000000",
             "1.000000",
         ]
 
     def test_plot_tree(self, model):
         result = model.plot_tree()
         assert model.to_graphviz() == result.source.strip()
+
+    def test_optional_name(self):
+        model = RandomForestRegressor()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_ridge.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_ridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,7 +333,11 @@
 
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'ridge_from_vDF'"
         )
         assert current_cursor().fetchone()[0] == "ridge_from_vDF"
 
         model_test.drop()
+
+    def test_optional_name(self):
+        model = Ridge()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_svd.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_svd.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,7 +218,11 @@
         )
         model_test.fit(winequality_vd, ["alcohol", "quality"])
         current_cursor().execute(
             "SELECT model_name FROM models WHERE model_name = 'SVD_vDF'"
         )
         assert current_cursor().fetchone()[0] == "SVD_vDF"
         model_test.drop()
+
+    def test_optional_name(self):
+        model = SVD()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_tools.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_tools.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_xgb_classifier.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_xgb_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,7 +600,11 @@
         y_test_vertica = model.to_python()(X_test)
         y_test_python = model_python.predict(X_test)
         result = (y_test_vertica - y_test_python) ** 2
         result = result.sum() / len(result)
         assert result == 0.0
         model.drop()
         os.remove(path)
+
+    def test_optional_name(self):
+        model = XGBClassifier()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests/vModel/test_xgb_regressor.py` & `verticapy-1.0.0b2/verticapy/tests/vModel/test_xgb_regressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,7 +510,11 @@
         model_python.load_model(path)
         y_test_python = model_python.predict(X_test)
         result = (y_test_vertica - y_test_python) ** 2
         result = result.sum() / len(result)
         assert result == pytest.approx(0.0, abs=1.0e-11)
         model.drop()
         os.remove(path)
+
+    def test_optional_name(self):
+        model = XGBRegressor()
+        assert model.model_name is not None
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/config/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/config/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/conftest.py` & `verticapy-1.0.0b2/verticapy/tests_new/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Standard Python Modules
 import random
 import tempfile
 import string
+from contextlib import contextmanager
 
 # Pytest
 import pytest
 
 # Other Modules
 from scipy.special import erfinv
 import numpy as np
@@ -412,14 +413,27 @@
     input_relation = np.column_stack((y_true, y_pred))
     vdf = vDataFrame(input_relation, usecols=["y_t", "y_s"])
     yield vdf, y_true, y_pred, labels
 
 
 @pytest.fixture(scope="module")
 def winequality_vpy(schema_loader):
+    with winequality_vpy_main(schema_loader) as result:
+        yield result
+
+
+@pytest.fixture(scope="function")
+def winequality_vpy_fun(schema_loader):
+    with winequality_vpy_main(schema_loader) as result:
+        yield result
+
+
+# @pytest.fixture(scope="function")
+@contextmanager
+def winequality_vpy_main(schema_loader):
     """
     Create a dummy vDataFrame for winequality data
     """
     winequality = load_winequality(schema_loader, "winequality")
     yield winequality
     drop(
         name=f"{schema_loader}.winequality",
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/connection/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/datasets/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/jupyter/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/jupyter/extensions/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/jupyter/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/machine_learning/memmodel/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/machine_learning/memmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/machine_learning/metrics/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/machine_learning/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/machine_learning/metrics/test_classification_metrics.py` & `verticapy-1.0.0b2/verticapy/tests_new/machine_learning/metrics/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/machine_learning/metrics/test_regression_metrics.py` & `verticapy-1.0.0b2/verticapy/tests_new/machine_learning/metrics/test_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/machine_learning/model_selection/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/machine_learning/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/machine_learning/vertica/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/machine_learning/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/base_test_files.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/base_test_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,48 @@
             of=of_col,
             method=method,
         )
         # Assert - checking if correct object created
         assert isinstance(result, plotting_library_object), "Wrong object created"
 
 
+class VDFBarPlot2D(BasicPlotTests):
+    """
+    Testing different attributes of Bar plot on a vDataFrame
+    """
+
+    # Testing variables
+
+    COL_NAME_VDF_1 = "cats"
+    COL_NAME_VDF_2 = "binary"
+
+    @pytest.fixture(autouse=True)
+    def data(self, dummy_dist_vd):
+        """
+        Load test data
+        """
+        self.data = dummy_dist_vd
+
+    @property
+    def cols(self):
+        """
+        Store labels for X,Y,Z axis to check.
+        """
+        return [self.COL_NAME_VDF_1, "density"]
+
+    def create_plot(self):
+        """
+        Create the plot
+        """
+        return (
+            self.data.bar,
+            {"columns": [self.COL_NAME_VDF_1, self.COL_NAME_VDF_2]},
+        )
+
+
 class VDCBarhPlot(BasicPlotTests):
     """
     Testing different attributes of HHorizontal Bar plot on a vDataColumn
     """
 
     # Testing variables
     COL_NAME = "check 2"
@@ -396,15 +430,27 @@
         """
         return (
             self.data.barh,
             {"columns": self.COL_NAME_VDF_1},
         )
 
 
-# Testing variables
+class VDFBarhPlot2D(VDFBarPlot2D):
+    """
+    Testing different attributes of HHorizontal Bar plot on a vDataFrame
+    """
+
+    def create_plot(self):
+        """
+        Create the plot
+        """
+        return (
+            self.data.barh,
+            {"columns": [self.COL_NAME_VDF_1, self.COL_NAME_VDF_2]},
+        )
 
 
 class VDCBoxPlot(BasicPlotTests):
     """
     Testing different attributes of Box plot on a vDataColumn
     """
 
@@ -1597,14 +1643,16 @@
         # Act
         result = model.plot_voronoi(
             max_nb_points,
             plot_crosses,
         )
         # Assert - checking if correct object created
         assert isinstance(result, plotting_library_object), "Wrong object created"
+        # cleanup
+        model.drop()
 
 
 class LOFPlot2D(BasicPlotTests):
     """
     Testing different attributes of 2D LOF plot
     """
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/conftest.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/conftest.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/conftest.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/conftest.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_champion_challenger.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_champion_challenger.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_elbow.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_elbow.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_importance.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_importance.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_lof.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_lof.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_logistic_reg.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_logistic_reg.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_model_evaluation.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_model_evaluation.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_pca.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_pca.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression_tree.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_regression_tree.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_stepwise.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_stepwise.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_svm.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/machine_learning/test_highcharts_svm.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_acf.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_acf.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_bar.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_bar.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_barh.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_barh.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_base.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_boxplot.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_boxplot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_candlestick.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_candlestick.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_contour.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_contour.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_density.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_density.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,32 +28,17 @@
 
 class TestHighchartsVDCDensityPlot(VDCDensityPlot):
     """
     Testing different attributes of Density plot on a vDataColumn
     """
 
 
-@pytest.mark.skip("Error in this highchart plot")
 class TestHighchartVDCDensityMultiPlot(VDCDensityMultiPlot):
     """
     Testing different attributes of Multiple Density plots on a vDataColumn
     """
 
-    def test_properties_multiple_plots_produced_for_multiplot(
-        self,
-    ):
-        """
-        Test if two plots created
-        """
-        # Arrange
-        number_of_plots = 2
-        # Act
-        # Assert
-        assert (
-            len(self.result.lines) == number_of_plots
-        ), "Two plots not produced for two classes"
-
 
 class TestHighchartsVDFDensityPlot(VDFDensityPlot):
     """
     Testing different attributes of Density plot on a vDataFrame
     """
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_heatmap.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_heatmap.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_hist.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_hist.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_line.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_line.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_outliers.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_outliers.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_pie.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_pie.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_range.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_range.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_scatter.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_acf.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,77 +10,58 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
+# Pytest
+import pytest
+
 # Vertica
-from verticapy.tests_new.plotting.base_test_files import (
-    ScatterVDF2DPlot,
-    ScatterVDF3DPlot,
-)
+from verticapy.tests_new.plotting.base_test_files import ACFPlot
 
 
-class TestHighchartsScatterVDF2DPlot(ScatterVDF2DPlot):
+class TestMatplotlibVDFACFPlot(ACFPlot):
     """
-    Testing different attributes of 2D scatter plot on a vDataFrame
+    Testing different attributes of ACF plot on a vDataFrame
     """
 
-    def test_properties_all_unique_values_for_by(self, dummy_scatter_vd):
+    @pytest.mark.skip(reason="Matplotlib does not have a y-axis")
+    def test_properties_yaxis_label(self):
         """
-        Test if all unique valies are inside the plot
+        Testing y-axis label
         """
-        # Arrange
-        # Act
-        result = dummy_scatter_vd.scatter(
-            [
-                self.COL_NAME_2,
-                self.COL_NAME_3,
-            ],
-            by=self.COL_NAME_4,
-        )
-        # Assert
-        assert len(result.data_temp) == len(
-            self.all_categories
-        ), "Some unique values were not found in the plot"
 
-    def test_data_total_number_of_points(self, dummy_scatter_vd):
+    def test_properties_vertical_lines_for_custom_lag(self, amazon_vd):
         """
-        Test if all datapoints were plotted
+        Test to check number of vertical lines
         """
         # Arrange
+        lag_number = 24
         # Act
-        # Assert - checking if correct object created
-        assert sum(len(item.data) for item in self.result.data_temp) == len(
-            dummy_scatter_vd
-        ), "Number of points not consistent with data"
-
-
-class TestHighchartsScatterVDF3DPlot(ScatterVDF3DPlot):
-    """
-    Testing different attributes of 3D scatter plot on a vDataFrame
-    """
+        result = amazon_vd.acf(
+            ts="date",
+            column="number",
+            p=lag_number - 1,
+            by=["state"],
+            unit="month",
+            method="spearman",
+        )
+        # Assert
+        assert (
+            len(result.get_lines()[0].get_xdata()) - 2 == lag_number
+        ), "Number of vertical lines inconsistent"
 
-    def test_properties_all_unique_values_for_by_3d_plot(
+    def test_data_all_scatter_points(
         self,
     ):
         """
-        Test if all unique values plotted
+        Test to check if all points plotted
         """
         # Arrange
+        lag_number = 13
         # Act
         # Assert
-        assert len(self.result.data_temp) == len(
-            self.all_categories
-        ), "Some unique values were not found in the plot"
-
-    def test_data_total_number_of_points_3d_plot(self, dummy_scatter_vd):
-        """
-        Test if all datapoints were plotted
-        """
-        # Arrange
-        # Act
-        # Assert - checking if correct object created
-        assert sum(len(item.data) for item in self.result.data_temp) == len(
-            dummy_scatter_vd
-        ), "Number of points not consistent with data"
+        assert (
+            len(self.result.get_lines()[0].get_xdata()) - 2 == lag_number
+        ), "Number of lag points inconsistent"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/highcharts/test_highcharts_spider.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/highcharts/test_highcharts_spider.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/conftest.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/conftest.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_champion_challenger.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_champion_challenger.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_elbow.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_elbow.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_importance.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_importance.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,32 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-# Pytest
-import pytest
-
 # Verticapy
 from verticapy.tests_new.plotting.base_test_files import ImportanceBarChartPlot
 
 
-class TestMatplotlibMachineLearningImportanceBarChart(ImportanceBarChartPlot):
+class TestPlotlyMachineLearningImportanceBarChartPlot(ImportanceBarChartPlot):
     """
     Testing different attributes of Importance Bar Chart plot
     """
 
     @property
     def cols(self):
         """
         Store labels for X,Y,Z axis to check.
         """
         return ["Importance (%)", "Features"]
 
-    @pytest.mark.skip(reason="Need to add '%' sign to x axis")
-    def test_properties_xaxis_label(self):
-        """
-        Testing x-axis title
-        """
-
     def test_data_no_of_columns(self):
         """
-        Test if four columns are produced
+        Test if all columns used
         """
         # Arrange
         total_items = 4
         # Act
         # Assert
-        assert len(self.result.containers[0]) == total_items, "Some columns missing"
+        assert len(self.result.data[0]["x"]) == total_items, "Some columns missing"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_kmeans.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,7 +116,9 @@
         result = model.plot_voronoi(
             [COL_NAME_1, COL_NAME_2],
             max_nb_points,
             plot_crosses,
         )
         # Assert - checking if correct object created
         assert isinstance(result, plotting_library_object), "Wrong object created"
+        # cleanup
+        model.drop()
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_lof.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_lof.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_logistic_reg.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_logistic_reg.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_model_evaluation.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_kmeans.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,49 +14,26 @@
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Pytest
 import pytest
 
 # Verticapy
-from verticapy.tests_new.plotting.base_test_files import (
-    ROCPlot,
-    CutoffCurvePlot,
-    PRCPlot,
-    LiftChartPlot,
-)
+from verticapy.tests_new.plotting.base_test_files import VornoiPlot
 
 
-class TestMatplotlibMachineLearningROCPlot(ROCPlot):
+class TestPlotlyMachineLearningKmeansPlot(VornoiPlot):
     """
-    Testing different attributes of ROC plot
+    Testing different attributes of Importance Bar Chart plot
     """
 
-
-class TestMatplotlibMachineLearningCutoffCurvePlot(CutoffCurvePlot):
-    """
-    Testing different attributes of Curve plot
-    """
-
-    @pytest.mark.skip(reason="Need to fix y axis")
-    def test_properties_yaxis_label(self):
-        """
-        Testing y-axis title
-        """
-
-
-class TestMatplotlibMachineLearningPRCPlot(PRCPlot):
-    """
-    Testing different attributes of PRC plot
-    """
-
-
-class TestMatplotlibMachineLearningLiftChartPlot(LiftChartPlot):
-    """
-    Testing different attributes of Lift Chart plot
-    """
-
-    @pytest.mark.skip(reason="Need to fix y axis")
-    def test_properties_yaxis_label(self):
+    def test_properties_no_of_elements(self):
         """
-        Testing y-axis title
+        Test if all objects plotted
         """
+        # Arrange
+        total_items = 20
+        # Act
+        # Assert
+        assert len(self.result.data) == pytest.approx(
+            total_items, abs=5
+        ), "Some elements missing"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_pca.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_pca.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression_tree.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_regression_tree.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_stepwise.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_stepwise.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_svm.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_svm.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_acf.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_acf.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,31 +10,41 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-# Pytest
-import pytest
-
 # Vertica
 from verticapy.tests_new.plotting.base_test_files import ACFPlot
 
 
-class TestMatplotlibVDFACFPlot(ACFPlot):
+class TestPlotlyVDFACFPlot(ACFPlot):
     """
     Testing different attributes of ACF plot on a vDataFrame
     """
 
-    @pytest.mark.skip(reason="Matplotlib does not have a y-axis")
-    def test_properties_yaxis_label(self):
+    @property
+    def cols(self):
+        """
+        Store labels for X,Y,Z axis to check.
         """
-        Testing y-axis label
+        return ["Lag", "Value"]
+
+    def test_properties_scatter_points_and_confidence(self):
         """
+        Check if all 3 elements are plotted
+        """
+        # Arrange
+        total_elements = 3
+        # Act
+        # Assert - checking if all plotting objects were created
+        assert (
+            len(self.result.data) == total_elements
+        ), "Some elements of plot are missing"
 
     def test_properties_vertical_lines_for_custom_lag(self, amazon_vd):
         """
         Test to check number of vertical lines
         """
         # Arrange
         lag_number = 24
@@ -45,23 +55,42 @@
             p=lag_number - 1,
             by=["state"],
             unit="month",
             method="spearman",
         )
         # Assert
         assert (
-            len(result.get_lines()[0].get_xdata()) - 2 == lag_number
+            len(result.layout["shapes"]) == lag_number
         ), "Number of vertical lines inconsistent"
 
+    def test_properties_mode_lines(self, amazon_vd):
+        """
+        Test to check number of vertical lines for kind=line
+        """
+        # Arrange
+        mode = "lines+markers"
+        # Act
+        result = amazon_vd.acf(
+            ts="date",
+            column="number",
+            p=12,
+            by=["state"],
+            unit="month",
+            method="spearman",
+            kind="line",
+        )
+        # Assert
+        assert result.data[-1]["mode"] == mode, "Number of vertical lines inconsistent"
+
     def test_data_all_scatter_points(
         self,
     ):
         """
         Test to check if all points plotted
         """
         # Arrange
         lag_number = 13
         # Act
         # Assert
         assert (
-            len(self.result.get_lines()[0].get_xdata()) - 2 == lag_number
+            len(self.result.data[0]["x"]) == lag_number
         ), "Number of lag points inconsistent"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_bar.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_bar.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_barh.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_barh.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Vertica
-from verticapy.tests_new.plotting.base_test_files import VDCBarhPlot, VDFBarhPlot
+from verticapy.tests_new.plotting.base_test_files import (
+    VDCBarhPlot,
+    VDFBarhPlot,
+    VDFBarhPlot2D,
+)
 
 
 class TestMatplotlibVDCBarhPlot(VDCBarhPlot):
     """
     Testing different attributes of HHorizontal Bar plot on a vDataColumn
     """
 
@@ -85,7 +89,20 @@
     def test_all_categories_created(self):
         """
         Test all categories
         """
         assert set(
             self.result.get_yticklabels()[i].get_text() for i in range(3)
         ).issubset(set(["A", "B", "C"]))
+
+
+class TestMatplotlibVDFBarhPlot2D(VDFBarhPlot2D):
+    """
+    Testing different attributes of HHorizontal Bar plot on a vDataFrame
+    """
+
+    @property
+    def cols(self):
+        """
+        Store labels for X,Y,Z axis to check.
+        """
+        return ["density", self.COL_NAME_VDF_1]
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_base.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_boxplot.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_boxplot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_contour.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_contour.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_density.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_density.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_heatmap.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_heatmap.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hexbin.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hexbin.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hist.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_hist.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_line.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_line.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_outliers.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_outliers.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_pie.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_pie.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_range.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_range.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_scatter.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_scatter.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/matplotlib/test_matplotlib_spider.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/test_matplotlib_spider.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/conftest.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/conftest.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_champion_challenger.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_champion_challenger.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_elbow.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_elbow.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_importance.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_pca.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,31 +11,24 @@
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Verticapy
-from verticapy.tests_new.plotting.base_test_files import ImportanceBarChartPlot
+from verticapy.tests_new.plotting.base_test_files import PCACirclePlot
 
 
-class TestPlotlyMachineLearningImportanceBarChartPlot(ImportanceBarChartPlot):
+class TestPlotlyMachineLearningPCACirclePlot(PCACirclePlot):
     """
-    Testing different attributes of Importance Bar Chart plot
+    Testing different attributes of PCA circle plot
     """
 
-    @property
-    def cols(self):
-        """
-        Store labels for X,Y,Z axis to check.
-        """
-        return ["Importance (%)", "Features"]
-
     def test_data_no_of_columns(self):
         """
-        Test if all columns used
+        Test all columns
         """
         # Arrange
-        total_items = 4
+        total_items = 3
         # Act
         # Assert
-        assert len(self.result.data[0]["x"]) == total_items, "Some columns missing"
+        assert len(self.result.data) == total_items, "Some columns missing"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_kmeans.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/matplotlib/machine_learning/test_matplotlib_importance.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,36 @@
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Pytest
 import pytest
 
 # Verticapy
-from verticapy.tests_new.plotting.base_test_files import VornoiPlot
+from verticapy.tests_new.plotting.base_test_files import ImportanceBarChartPlot
 
 
-class TestPlotlyMachineLearningKmeansPlot(VornoiPlot):
+class TestMatplotlibMachineLearningImportanceBarChart(ImportanceBarChartPlot):
     """
     Testing different attributes of Importance Bar Chart plot
     """
 
-    def test_properties_no_of_elements(self):
+    @property
+    def cols(self):
         """
-        Test if all objects plotted
+        Store labels for X,Y,Z axis to check.
+        """
+        return ["Importance (%)", "Features"]
+
+    def test_properties_xaxis_label(self):
+        """
+        Testing x-axis title
+        """
+
+    def test_data_no_of_columns(self):
+        """
+        Test if four columns are produced
         """
         # Arrange
-        total_items = 20
+        total_items = 4
         # Act
         # Assert
-        assert len(self.result.data) == pytest.approx(
-            total_items, abs=5
-        ), "Some elements missing"
+        assert len(self.result.containers[0]) == total_items, "Some columns missing"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_lof.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_lof.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_logistic_reg.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_logistic_reg.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_model_evaluation.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_model_evaluation.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_pca.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,24 +11,36 @@
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Verticapy
-from verticapy.tests_new.plotting.base_test_files import PCACirclePlot
+from verticapy.tests_new.plotting.base_test_files import LearningRegressionPlot
 
 
-class TestPlotlyMachineLearningPCACirclePlot(PCACirclePlot):
+class TestPlotlyMachineLearningRegressionPlot(LearningRegressionPlot):
     """
-    Testing different attributes of PCA circle plot
+    Testing different attributes of Regression plot
     """
 
-    def test_data_no_of_columns(self):
+    def test_properties_scatter_and_line_plot(self):
         """
-        Test all columns
+        Test two items exist
         """
         # Arrange
-        total_items = 3
+        total_items = 2
         # Act
         # Assert
-        assert len(self.result.data) == total_items, "Some columns missing"
+        assert len(self.result.data) == total_items, "Either line or scatter missing"
+
+    def test_data_all_scatter_points(self, dummy_scatter_vd):
+        """
+        Test all datapoints
+        """
+        # Arrange
+        no_of_points = len(dummy_scatter_vd)
+        # Act
+        # Assert
+        assert (
+            len(self.result.data[0]["x"]) == no_of_points
+        ), "Discrepancy between points plotted and total number of points"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_stepwise.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,37 +10,45 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
+# Pytest
+import pytest
+
 # Verticapy
-from verticapy.tests_new.plotting.base_test_files import LearningRegressionPlot
+from verticapy.tests_new.plotting.base_test_files import StepwisePlot
 
 
-class TestPlotlyMachineLearningRegressionPlot(LearningRegressionPlot):
+class TestPlotlyMachineLearningStepwisePlot(StepwisePlot):
     """
-    Testing different attributes of Regression plot
+    Testing different attributes of Stepwise plot
     """
 
-    def test_properties_scatter_and_line_plot(self):
+    def test_properties_no_of_elements(self):
         """
-        Test two items exist
+        Test all objects
         """
         # Arrange
-        total_items = 2
+        total_items = 8
         # Act
         # Assert
-        assert len(self.result.data) == total_items, "Either line or scatter missing"
+        assert len(self.result.data) == pytest.approx(
+            total_items, abs=1
+        ), "Some elements missing"
 
-    def test_data_all_scatter_points(self, dummy_scatter_vd):
+    def test_data_start_and_end(self):
         """
-        Test all datapoints
+        Test start and end objects
         """
         # Arrange
-        no_of_points = len(dummy_scatter_vd)
+        start = "Start"
+        end = "End"
         # Act
         # Assert
-        assert (
-            len(self.result.data[0]["x"]) == no_of_points
-        ), "Discrepancy between points plotted and total number of points"
+        assert start in [
+            self.result.data[i]["name"] for i in range(len(self.result.data))
+        ] and end in [
+            self.result.data[i]["name"] for i in range(len(self.result.data))
+        ], "Some elements missing"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_regression_tree.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_contour.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,64 +10,59 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-# Pytest
-import pytest
-
 # Vertica
-from verticapy.tests_new.plotting.base_test_files import LearningRegressionTreePlot
+from verticapy.tests_new.plotting.base_test_files import VDFContourPlot
 
 
-class TestPlotlyMachineLearningRegressionTreePlot(LearningRegressionTreePlot):
+class TestPlotlyVDFContourPlot(VDFContourPlot):
     """
-    Testing different attributes of Regression Tree plot
+    Testing different attributes of Contour plot on a vDataFrame
     """
 
-    def test_properties_observations_label(self):
+    def test_data_count_xaxis_default_bins(
+        self,
+    ):
         """
-        Test plot title
+        Testing default bins
         """
         # Arrange
-        test_title = "Observations"
         # Act
         # Assert
-        assert self.result.data[0]["name"] == test_title, "X axis label incorrect"
+        assert self.result.data[0]["x"].shape[0] == 100, "The default bins are not 100."
 
-    def test_properties_prediction_label(self):
+    def test_data_count_xaxis_custom_bins(self, dummy_dist_vd):
         """
-        Test plot title
+        Test different bin sizes
         """
         # Arrange
-        test_title = "Prediction"
-        # Act
-        # Assert
-        assert self.result.data[1]["name"] == test_title, "Y axis label incorrect"
+        custom_bins = 200
+
+        def func(param_a, param_b):
+            return param_b + param_a * 0
 
-    def test_properties_hover_label(self):
-        """
-        Test hover labels
-        """
-        # Arrange
-        test_title = (
-            f"{self.COL_NAME_1}: %" "{x} <br>" f"{self.COL_NAME_2}: %" "{y} <br>"
-        )
         # Act
+        result = dummy_dist_vd.contour(
+            columns=[self.COL_NAME_1, self.COL_NAME_2], nbins=custom_bins, func=func
+        )
         # Assert
         assert (
-            self.result.data[0]["hovertemplate"] == test_title
-        ), "Hover information incorrect"
+            result.data[0]["x"].shape[0] == custom_bins
+        ), "The custom bins option is not working."
 
-    def test_properties_no_of_elements(self):
+    def test_data_x_axis_range(self, dummy_dist_vd):
         """
-        Test number of elements
+        Test x-axis range
         """
         # Arrange
-        total_items = 2
+        x_min = dummy_dist_vd[self.COL_NAME_1].min()
+        x_max = dummy_dist_vd[self.COL_NAME_1].max()
         # Act
         # Assert
-        assert len(self.result.data) == pytest.approx(
-            total_items, abs=1
-        ), "Some elements missing"
+        assert (
+            self.result.data[0]["x"].min() == x_min
+            and self.result.data[0]["x"].max() == x_max
+        ), "The range in data is not consistent with plot"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_stepwise.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_line.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,45 +10,78 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-# Pytest
+import random
 import pytest
 
-# Verticapy
-from verticapy.tests_new.plotting.base_test_files import StepwisePlot
 
+# Vertica
+from verticapy.tests_new.plotting.base_test_files import VDCLinePlot, VDFLinePlot
 
-class TestPlotlyMachineLearningStepwisePlot(StepwisePlot):
+
+class TestPlotlyVDCLinePlot(VDCLinePlot):
     """
-    Testing different attributes of Stepwise plot
+    Testing different attributes of Line plot on a vDataColumn
     """
 
-    def test_properties_no_of_elements(self):
+    @pytest.mark.skip(reason="Need to change from time to time column name")
+    def test_properties_xaxis_label(self):
+        """
+        Testing x-axis title
+        """
+
+    def test_data_count_of_all_values(self, dummy_line_data_vd):
+        """
+        Testing total points
+        """
+        # Arrange
+        total_count = dummy_line_data_vd.shape()[0]
+        # Act
+        assert (
+            self.result.data[0]["x"].shape[0] + self.result.data[1]["x"].shape[0]
+            == total_count
+        ), "The total values in the plot are not equal to the values in the dataframe."
+
+    def test_data_spot_check(self, dummy_line_data_vd):
         """
-        Test all objects
+        Spot check one data point
         """
         # Arrange
-        total_items = 8
         # Act
-        # Assert
-        assert len(self.result.data) == pytest.approx(
-            total_items, abs=1
-        ), "Some elements missing"
+        assert (
+            str(
+                dummy_line_data_vd[self.TIME_COL][
+                    random.randint(0, len(dummy_line_data_vd)) - 1
+                ]
+            )
+            in self.result.data[0]["x"]
+        ), "Two time values that exist in the data do not exist in the plot"
 
-    def test_data_start_and_end(self):
+    def test_additional_options_marker_on(self, dummy_line_data_vd):
         """
-        Test start and end objects
+        Test marker option
         """
         # Arrange
-        start = "Start"
-        end = "End"
         # Act
-        # Assert
-        assert start in [
-            self.result.data[i]["name"] for i in range(len(self.result.data))
-        ] and end in [
-            self.result.data[i]["name"] for i in range(len(self.result.data))
-        ], "Some elements missing"
+        result = dummy_line_data_vd[self.COL_NAME_1].plot(
+            ts=self.TIME_COL, by=self.COL_NAME_2, markers=True
+        )
+        # Assert - checking if correct object created
+        assert set(result.data[0]["mode"]) == set(
+            "lines+markers"
+        ), "Markers not turned on"
+
+
+class TestPlotlyVDFLinePlot(VDFLinePlot):
+    """
+    Testing different attributes of Line plot on a vDataFrame
+    """
+
+    @pytest.mark.skip(reason="Need to change from time to time column name")
+    def test_properties_xaxis_label(self):
+        """
+        Testing x-axis title
+        """
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_svm.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/machine_learning/test_plotly_svm.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_acf.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_outliers.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,87 +10,87 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
+# Pytest
+import pytest
+
 # Vertica
-from verticapy.tests_new.plotting.base_test_files import ACFPlot
+from verticapy.tests_new.plotting.base_test_files import OutliersPlot2D, OutliersPlot
 
 
-class TestPlotlyVDFACFPlot(ACFPlot):
+class TestPlotlyOutliersPlot(OutliersPlot):
     """
-    Testing different attributes of ACF plot on a vDataFrame
+    Testing different attributes of outliers plot on a vDataColumn
     """
 
-    @property
-    def cols(self):
+    @pytest.mark.skip(reason="Y axis label not applied to plotly plot")
+    def test_properties_yaxis_label(self):
         """
-        Store labels for X,Y,Z axis to check.
+        Testing y-axis title
         """
-        return ["Lag", "Value"]
 
-    def test_properties_scatter_points_and_confidence(self):
+    def test_properties_xaxis_label(self):
         """
-        Check if all 3 elements are plotted
+        Testing x-axis title
         """
         # Arrange
-        total_elements = 3
+        column_name = self.COL_NAME_1
         # Act
-        # Assert - checking if all plotting objects were created
-        assert (
-            len(self.result.data) == total_elements
-        ), "Some elements of plot are missing"
+        # Assert -
+        assert self.result.data[0]["x"][0] == column_name, "X axis label incorrect"
 
-    def test_properties_vertical_lines_for_custom_lag(self, amazon_vd):
+    def test_data_all_scatter_points_for_1d(
+        self,
+        dummy_dist_vd,
+    ):
         """
-        Test to check number of vertical lines
+        Test if all points are plotted
         """
         # Arrange
-        lag_number = 24
+        total_points = len(dummy_dist_vd[self.COL_NAME_1])
         # Act
-        result = amazon_vd.acf(
-            ts="date",
-            column="number",
-            p=lag_number - 1,
-            by=["state"],
-            unit="month",
-            method="spearman",
+        result = dummy_dist_vd.outliers_plot(
+            columns=[self.COL_NAME_1], max_nb_points=10000
         )
-        # Assert
+        plot_points_count = sum(data["y"].shape[0] for data in result.data)
         assert (
-            len(result.layout["shapes"]) == lag_number
-        ), "Number of vertical lines inconsistent"
+            plot_points_count == total_points
+        ), "All points are not plotted for 1d plot"
 
-    def test_properties_mode_lines(self, amazon_vd):
+
+class TestPlotlyOutliersPlot2D(OutliersPlot2D):
+    """
+    Testing different attributes of outliers plot on a vDataFrame
+    """
+
+    def test_data_all_scatter_points_for_2d(self, dummy_dist_vd):
         """
-        Test to check number of vertical lines for kind=line
+        Test if all points ar eplotted
         """
         # Arrange
-        mode = "lines+markers"
+        total_points = len(dummy_dist_vd[self.COL_NAME_1])
         # Act
-        result = amazon_vd.acf(
-            ts="date",
-            column="number",
-            p=12,
-            by=["state"],
-            unit="month",
-            method="spearman",
-            kind="line",
+        result = dummy_dist_vd.outliers_plot(
+            columns=[self.COL_NAME_1, self.COL_NAME_2], max_nb_points=10000
         )
-        # Assert
-        assert result.data[-1]["mode"] == mode, "Number of vertical lines inconsistent"
+        assert result.data[-1]["y"].shape[0] + result.data[-2]["y"].shape[
+            0
+        ] == pytest.approx(
+            total_points, abs=1
+        ), "All points are not plotted for 2d plot"
 
-    def test_data_all_scatter_points(
+    def test_data_all_information_plotted_for_2d(
         self,
     ):
         """
-        Test to check if all points plotted
+        Test if all four elements plotted
         """
         # Arrange
-        lag_number = 13
+        total_elements = 4
         # Act
-        # Assert
         assert (
-            len(self.result.data[0]["x"]) == lag_number
-        ), "Number of lag points inconsistent"
+            len(self.result.data) == total_elements
+        ), "The total number of elements plotted is not correct"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_bar.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Vertica
-from verticapy.tests_new.plotting.base_test_files import VDCBarPlot, VDFBarPlot
+from verticapy.tests_new.plotting.base_test_files import (
+    VDCBarPlot,
+    VDFBarPlot,
+    VDFBarPlot2D,
+)
 
 
 class TestPlotlyVDCBarPlot(VDCBarPlot):
     """
     Testing different attributes of Bar plot on a vDataColumn
     """
 
@@ -81,7 +85,13 @@
         """
         ### Checking if the density was plotted correctly
         nums = dummy_dist_vd.to_pandas()[self.COL_NAME_VDF_1].value_counts()
         total = len(dummy_dist_vd)
         assert set(self.result.data[0]["y"]).issubset(
             set([nums["A"] / total, nums["B"] / total, nums["C"] / total])
         )
+
+
+class TestPlotlyVDFBarPlot2D(VDFBarPlot2D):
+    """
+    Testing different attributes of 2D Bar plot on a vDataFrame
+    """
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_barh.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_barh.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Vertica
 from verticapy.tests_new.plotting.base_test_files import (
     VDCBarhPlot,
     VDFBarhPlot,
+    VDFBarhPlot2D,
     get_yaxis_label,
     get_xaxis_label,
 )
 
 
 class TestPlotlyVDCBarhPlot(VDCBarhPlot):
     """
@@ -119,7 +120,20 @@
         )
 
     def test_all_categories_created(self):
         """
         Test if all categories exist in plot
         """
         assert set(self.result.data[0]["y"]).issubset(set(["A", "B", "C"]))
+
+
+class TestPlotlyVDFBarhPlot2D(VDFBarhPlot2D):
+    """
+    Testing different attributes of HHorizontal Bar plot on a vDataFrame
+    """
+
+    @property
+    def cols(self):
+        """
+        Store labels for X,Y,Z axis to check.
+        """
+        return ["density", self.COL_NAME_VDF_1]
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_base.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_base.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_boxplot.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_boxplot.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_contour.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_spider.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,58 +11,53 @@
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
 # Vertica
-from verticapy.tests_new.plotting.base_test_files import VDFContourPlot
+from verticapy.tests_new.plotting.base_test_files import VDCSpiderPlot
 
 
-class TestPlotlyVDFContourPlot(VDFContourPlot):
+class TestPlotlyVDCSpiderPlot(VDCSpiderPlot):
     """
-    Testing different attributes of Contour plot on a vDataFrame
+    Testing different attributes of Spider plot on a vDataColumn
     """
 
-    def test_data_count_xaxis_default_bins(
+    def test_properties_method_title_at_bottom(
         self,
     ):
         """
-        Testing default bins
+        Test method title
         """
         # Arrange
+        method_text = "(Method: Density)"
         # Act
-        # Assert
-        assert self.result.data[0]["x"].shape[0] == 100, "The default bins are not 100."
+        # Assert -
+        assert (
+            self.result.layout["annotations"][0]["text"] == method_text
+        ), "Method title incorrect"
 
-    def test_data_count_xaxis_custom_bins(self, dummy_dist_vd):
+    def test_properties_multiple_plots_produced_for_multiplot(
+        self,
+    ):
         """
-        Test different bin sizes
+        Test if multiple plots produced
         """
         # Arrange
-        custom_bins = 200
-
-        def func(param_a, param_b):
-            return param_b + param_a * 0
-
+        number_of_plots = 2
         # Act
-        result = dummy_dist_vd.contour(
-            columns=[self.COL_NAME_1, self.COL_NAME_2], nbins=custom_bins, func=func
-        )
         # Assert
         assert (
-            result.data[0]["x"].shape[0] == custom_bins
-        ), "The custom bins option is not working."
+            len(self.by_result.data) == number_of_plots
+        ), "Two traces not produced for two classes of binary"
 
-    def test_data_x_axis_range(self, dummy_dist_vd):
+    def test_data_all_categories(self, dummy_dist_vd):
         """
-        Test x-axis range
+        Test all categories
         """
         # Arrange
-        x_min = dummy_dist_vd[self.COL_NAME_1].min()
-        x_max = dummy_dist_vd[self.COL_NAME_1].max()
+        no_of_category = dummy_dist_vd["cats"].nunique()
         # Act
-        # Assert
         assert (
-            self.result.data[0]["x"].min() == x_min
-            and self.result.data[0]["x"].max() == x_max
-        ), "The range in data is not consistent with plot"
+            self.result.data[0]["r"].shape[0] == no_of_category
+        ), "The number of categories in the data differ from the plot"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_density.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_density.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,36 +42,18 @@
         # Act
         assert pytest.approx(self.result.data[0]["x"].min(), 4) == pytest.approx(
             x_min, 4
         ) and pytest.approx(self.result.data[0]["x"].max(), 4) == pytest.approx(
             x_max, 4
         ), "The range in data is not consistent with plot"
 
-    @pytest.mark.skip(reason="Need to remove extra quootation marks")
-    def test_properties_xaxis_label(self):
-        """
-        Testing x-axis title
-        """
-
 
 class TestplotlyVDCDensityMultiPlot(VDCDensityMultiPlot):
     """
     Testing different attributes of Multiple Density plots on a vDataColumn
     """
 
-    @pytest.mark.skip(reason="Need to remove extra quootation marks")
-    def test_properties_xaxis_label(self):
-        """
-        Testing x-axis title
-        """
-
 
 class TestPlotlyVDFDensityPlot(VDFDensityPlot):
     """
     Testing different attributes of Density plot on a vDataFrame
     """
-
-    @pytest.mark.skip(reason="Need to remove extra quootation marks")
-    def test_properties_xaxis_label(self):
-        """
-        Testing x-axis title
-        """
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_heatmap.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_heatmap.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_hist.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_hist.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_outliers.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_range.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,87 +10,82 @@
 Unless  required  by applicable  law or  agreed to in
 writing, software  distributed  under the  License is
 distributed on an  "AS IS" BASIS,  WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the  License for the specific  language governing
 permissions and limitations under the License.
 """
-# Pytest
-import pytest
-
 # Vertica
-from verticapy.tests_new.plotting.base_test_files import OutliersPlot2D, OutliersPlot
+from verticapy.tests_new.plotting.base_test_files import VDCRangeCurve, VDFRangeCurve
 
 
-class TestPlotlyOutliersPlot(OutliersPlot):
+class TestPlotlyVDCRangeCurve(VDCRangeCurve):
     """
-    Testing different attributes of outliers plot on a vDataColumn
+    Testing different attributes of range curve plot on a vDataColumn
     """
 
-    @pytest.mark.skip(reason="Y axis label not applied to plotly plot")
-    def test_properties_yaxis_label(self):
+    def test_data_x_axis(self, dummy_date_vd):
         """
-        Testing y-axis title
+        Test data of x-axis
         """
+        # Arrange
+        test_set = set(dummy_date_vd.to_numpy()[:, 0])
+        # Act
+        result = dummy_date_vd[self.COL_NAME_1].range_plot(ts=self.TIME_COL)
+        assert set(result.data[0]["x"]).issubset(
+            test_set
+        ), "There is descripancy between x axis values for the bounds"
 
-    def test_properties_xaxis_label(self):
+    def test_data_x_axis_for_median(self, dummy_date_vd):
         """
-        Testing x-axis title
+        Test median value
         """
         # Arrange
-        column_name = self.COL_NAME_1
+        test_set = set(dummy_date_vd.to_numpy()[:, 0])
         # Act
-        # Assert -
-        assert self.result.data[0]["x"][0] == column_name, "X axis label incorrect"
+        assert set(self.result.data[1]["x"]).issubset(
+            test_set
+        ), "There is descripancy between x axis values for the median"
 
-    def test_data_all_scatter_points_for_1d(
-        self,
-        dummy_dist_vd,
-    ):
+    def test_additional_options_turn_off_median(self, dummy_date_vd):
         """
-        Test if all points are plotted
+        Test when median is turned off
         """
         # Arrange
-        total_points = len(dummy_dist_vd[self.COL_NAME_1])
         # Act
-        result = dummy_dist_vd.outliers_plot(
-            columns=[self.COL_NAME_1], max_nb_points=10000
+        result = dummy_date_vd[self.COL_NAME_1].range_plot(
+            ts=self.TIME_COL, plot_median=False
         )
-        plot_points_count = sum(data["y"].shape[0] for data in result.data)
+        # Assert
         assert (
-            plot_points_count == total_points
-        ), "All points are not plotted for 1d plot"
+            len(result.data) == 1
+        ), "Median is still showing even after it is turned off"
 
-
-class TestPlotlyOutliersPlot2D(OutliersPlot2D):
-    """
-    Testing different attributes of outliers plot on a vDataFrame
-    """
-
-    def test_data_all_scatter_points_for_2d(self, dummy_dist_vd):
+    def test_additional_options_turn_on_median(
+        self,
+    ):
         """
-        Test if all points ar eplotted
+        Test when median is turned on
         """
         # Arrange
-        total_points = len(dummy_dist_vd[self.COL_NAME_1])
         # Act
-        result = dummy_dist_vd.outliers_plot(
-            columns=[self.COL_NAME_1, self.COL_NAME_2], max_nb_points=10000
-        )
-        assert result.data[-1]["y"].shape[0] + result.data[-2]["y"].shape[
-            0
-        ] == pytest.approx(
-            total_points, abs=1
-        ), "All points are not plotted for 2d plot"
+        # Assert
+        assert (
+            len(self.result.data) > 1
+        ), "Median is still showing even after it is turned off"
 
-    def test_data_all_information_plotted_for_2d(
-        self,
-    ):
+
+class TestPlotlyVDFRangeCurve(VDFRangeCurve):
+    """
+    Testing different attributes of range curve plot on a vDataFrame
+    """
+
+    def test_data_x_axis(self, dummy_date_vd):
         """
-        Test if all four elements plotted
+        Test data for x-axis
         """
         # Arrange
-        total_elements = 4
+        test_set = set(dummy_date_vd.to_numpy()[:, 0])
         # Act
-        assert (
-            len(self.result.data) == total_elements
-        ), "The total number of elements plotted is not correct"
+        assert set(self.result.data[0]["x"]).issubset(
+            test_set
+        ), "There is descripancy between x axis values for the bounds"
```

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_pie.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_pie.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/plotting/plotly/test_plotly_scatter.py` & `verticapy-1.0.0b2/verticapy/tests_new/plotting/plotly/test_plotly_scatter.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/sdk/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/sql/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/sql/functions/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/sql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/sql/geo/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/sql/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/tests_new/utils/__init__.py` & `verticapy-1.0.0b2/verticapy/tests_new/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/udf/__init__.py` & `verticapy-1.0.0b2/verticapy/udf/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/utilities/__init__.py` & `verticapy-1.0.0b2/verticapy/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy/vdataframe/__init__.py` & `verticapy-1.0.0b2/verticapy/vdataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `verticapy-1.0.0b1/verticapy.egg-info/PKG-INFO` & `verticapy-1.0.0b2/verticapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verticapy
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: VerticaPy simplifies data exploration, data cleaning, and machine learning in Vertica.
 Home-page: https://github.com/vertica/VerticaPy
 Author: Badr Ouali
 Author-email: badr.ouali@vertica.com
 Keywords: vertica python ml data science machine learning statistics database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `verticapy-1.0.0b1/verticapy.egg-info/SOURCES.txt` & `verticapy-1.0.0b2/verticapy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,16 @@
 verticapy/tests_new/machine_learning/__init__.py
 verticapy/tests_new/machine_learning/memmodel/__init__.py
 verticapy/tests_new/machine_learning/metrics/__init__.py
 verticapy/tests_new/machine_learning/metrics/test_classification_metrics.py
 verticapy/tests_new/machine_learning/metrics/test_regression_metrics.py
 verticapy/tests_new/machine_learning/model_selection/__init__.py
 verticapy/tests_new/machine_learning/vertica/__init__.py
+verticapy/tests_new/machine_learning/vertica/linear_model/__init__.py
+verticapy/tests_new/machine_learning/vertica/linear_model/test_linear_regression.py
 verticapy/tests_new/plotting/__init__.py
 verticapy/tests_new/plotting/base_test_files.py
 verticapy/tests_new/plotting/conftest.py
 verticapy/tests_new/plotting/highcharts/__init__.py
 verticapy/tests_new/plotting/highcharts/conftest.py
 verticapy/tests_new/plotting/highcharts/test_highcharts_acf.py
 verticapy/tests_new/plotting/highcharts/test_highcharts_bar.py
```

