# Comparing `tmp/cr8-0.9.2.tar.gz` & `tmp/cr8-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cr8-0.9.2.tar", last modified: Sat Feb 11 18:34:37 2017, max compression
+gzip compressed data, was "dist/cr8-0.9.3.tar", last modified: Sun May 14 19:01:14 2017, max compression
```

## Comparing `cr8-0.9.2.tar` & `cr8-0.9.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/
--rw-r--r--   0 jordi     (1000) jordi     (1000)       38 2017-02-11 18:34:37.000000 cr8-0.9.2/setup.cfg
--rw-r--r--   0 jordi     (1000) jordi     (1000)     6415 2016-12-08 18:49:13.000000 cr8-0.9.2/README.rst
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8/
--rw-r--r--   0 jordi     (1000) jordi     (1000)     8572 2017-01-03 16:49:14.000000 cr8-0.9.2/cr8/insert_fake_data.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)       76 2016-11-03 20:11:04.000000 cr8-0.9.2/cr8/__init__.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     4762 2017-02-09 19:30:47.000000 cr8-0.9.2/cr8/clients.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     2704 2016-12-16 09:05:09.000000 cr8-0.9.2/cr8/misc.py
--rwxr-xr-x   0 jordi     (1000) jordi     (1000)      876 2017-02-09 19:30:47.000000 cr8-0.9.2/cr8/__main__.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)    13471 2017-02-09 19:30:56.000000 cr8-0.9.2/cr8/run_crate.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1968 2017-02-09 19:30:47.000000 cr8-0.9.2/cr8/engine.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)      906 2016-11-13 16:29:34.000000 cr8-0.9.2/cr8/insert_blob.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     2389 2016-10-05 18:12:54.000000 cr8-0.9.2/cr8/bench_spec.py
--rwxr-xr-x   0 jordi     (1000) jordi     (1000)     2682 2016-12-08 18:49:13.000000 cr8-0.9.2/cr8/insert_json.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1920 2016-12-08 18:49:13.000000 cr8-0.9.2/cr8/log.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     9128 2016-12-13 20:51:28.000000 cr8-0.9.2/cr8/run_spec.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     4072 2016-12-08 18:49:13.000000 cr8-0.9.2/cr8/run_track.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     3628 2016-12-08 13:52:51.000000 cr8-0.9.2/cr8/metrics.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1597 2016-12-10 18:46:58.000000 cr8-0.9.2/cr8/cli.py
--rwxr-xr-x   0 jordi     (1000) jordi     (1000)     1544 2016-12-16 09:05:09.000000 cr8-0.9.2/cr8/timeit.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     2467 2017-02-01 21:48:04.000000 cr8-0.9.2/cr8/aio.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1736 2016-10-05 18:12:54.000000 cr8-0.9.2/cr8/fake_providers.py
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8.egg-info/
--rw-r--r--   0 jordi     (1000) jordi     (1000)        1 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8.egg-info/dependency_links.txt
--rw-r--r--   0 jordi     (1000) jordi     (1000)       43 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8.egg-info/entry_points.txt
--rw-r--r--   0 jordi     (1000) jordi     (1000)      964 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8.egg-info/SOURCES.txt
--rw-r--r--   0 jordi     (1000) jordi     (1000)     8980 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8.egg-info/PKG-INFO
--rw-r--r--   0 jordi     (1000) jordi     (1000)        4 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8.egg-info/top_level.txt
--rw-r--r--   0 jordi     (1000) jordi     (1000)       66 2017-02-11 18:34:37.000000 cr8-0.9.2/cr8.egg-info/requires.txt
--rw-r--r--   0 jordi     (1000) jordi     (1000)      388 2017-01-03 16:27:02.000000 cr8-0.9.2/.travis.yml
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1092 2017-01-06 21:09:01.000000 cr8-0.9.2/setup.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     7872 2017-02-11 18:28:53.000000 cr8-0.9.2/CHANGES.rst
--rw-r--r--   0 jordi     (1000) jordi     (1000)      815 2016-06-16 18:00:19.000000 cr8-0.9.2/.gitignore
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1086 2016-02-29 21:21:04.000000 cr8-0.9.2/LICENSE
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/tests/
--rw-r--r--   0 jordi     (1000) jordi     (1000)      637 2016-05-29 14:52:19.000000 cr8-0.9.2/tests/test_misc.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     2447 2016-07-12 21:13:31.000000 cr8-0.9.2/tests/test_cli.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)        0 2016-02-29 21:21:04.000000 cr8-0.9.2/tests/__init__.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     3230 2017-01-03 17:29:41.000000 cr8-0.9.2/tests/test_insert_fake_data.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)      311 2016-06-22 07:08:55.000000 cr8-0.9.2/tests/test_fake_providers.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1108 2016-06-09 20:58:47.000000 cr8-0.9.2/tests/demo.json
--rw-r--r--   0 jordi     (1000) jordi     (1000)      890 2017-02-09 19:30:47.000000 cr8-0.9.2/tests/test_clients.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)      966 2016-11-23 21:07:57.000000 cr8-0.9.2/tests/test_log.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)      231 2016-06-22 07:08:55.000000 cr8-0.9.2/tests/test_insert_json.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     3447 2017-02-09 19:30:56.000000 cr8-0.9.2/tests/test_run_crate.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     2019 2016-12-09 20:03:05.000000 cr8-0.9.2/tests/test_integration.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     1872 2016-06-16 18:04:39.000000 cr8-0.9.2/tests/test_metrics.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)     8980 2017-02-11 18:34:37.000000 cr8-0.9.2/PKG-INFO
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/tracks/
--rw-r--r--   0 jordi     (1000) jordi     (1000)       96 2016-06-16 18:39:41.000000 cr8-0.9.2/tracks/default.toml
--rw-r--r--   0 jordi     (1000) jordi     (1000)      576 2017-02-01 21:47:42.000000 cr8-0.9.2/tracks/sample.toml
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/specs/
--rw-r--r--   0 jordi     (1000) jordi     (1000)      455 2016-06-20 23:14:18.000000 cr8-0.9.2/specs/count_countries.json
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/specs/sql/
--rw-r--r--   0 jordi     (1000) jordi     (1000)      414 2016-05-29 16:53:33.000000 cr8-0.9.2/specs/sql/create_countries.sql
--rw-r--r--   0 jordi     (1000) jordi     (1000)      542 2016-12-13 20:51:28.000000 cr8-0.9.2/specs/sample.py
--rw-r--r--   0 jordi     (1000) jordi     (1000)      409 2016-06-09 20:58:47.000000 cr8-0.9.2/specs/sample_insert.toml
-drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-02-11 18:34:37.000000 cr8-0.9.2/specs/data/
--rw-r--r--   0 jordi     (1000) jordi     (1000)     7898 2016-05-29 16:53:33.000000 cr8-0.9.2/specs/data/countries.json
--rw-r--r--   0 jordi     (1000) jordi     (1000)      681 2016-12-12 21:04:38.000000 cr8-0.9.2/specs/sample.toml
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)       38 2017-05-14 19:01:14.000000 cr8-0.9.3/setup.cfg
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     6419 2017-05-08 22:29:13.000000 cr8-0.9.3/README.rst
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     8719 2017-05-08 22:29:13.000000 cr8-0.9.3/cr8/insert_fake_data.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)       76 2016-11-03 20:11:04.000000 cr8-0.9.3/cr8/__init__.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     4755 2017-04-20 19:53:57.000000 cr8-0.9.3/cr8/clients.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     2704 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/misc.py
+-rwxr-xr-x   0 jordi     (1000) jordi     (1000)      876 2017-03-21 18:02:11.000000 cr8-0.9.3/cr8/__main__.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)    13471 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/run_crate.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1968 2017-03-21 18:02:11.000000 cr8-0.9.3/cr8/engine.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      906 2016-11-13 16:29:34.000000 cr8-0.9.3/cr8/insert_blob.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     2389 2016-10-05 18:12:54.000000 cr8-0.9.3/cr8/bench_spec.py
+-rwxr-xr-x   0 jordi     (1000) jordi     (1000)     2682 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/insert_json.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1920 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/log.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     9128 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/run_spec.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     4072 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/run_track.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     3628 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/metrics.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1597 2016-12-10 18:46:58.000000 cr8-0.9.3/cr8/cli.py
+-rwxr-xr-x   0 jordi     (1000) jordi     (1000)     1544 2017-03-03 17:31:46.000000 cr8-0.9.3/cr8/timeit.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     2467 2017-04-20 20:27:45.000000 cr8-0.9.3/cr8/aio.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1736 2016-10-05 18:12:54.000000 cr8-0.9.3/cr8/fake_providers.py
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8.egg-info/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)        1 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8.egg-info/dependency_links.txt
+-rw-r--r--   0 jordi     (1000) jordi     (1000)       43 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8.egg-info/entry_points.txt
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      964 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8.egg-info/SOURCES.txt
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     9007 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8.egg-info/PKG-INFO
+-rw-r--r--   0 jordi     (1000) jordi     (1000)        4 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8.egg-info/top_level.txt
+-rw-r--r--   0 jordi     (1000) jordi     (1000)       66 2017-05-14 19:01:14.000000 cr8-0.9.3/cr8.egg-info/requires.txt
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      388 2017-03-03 17:31:46.000000 cr8-0.9.3/.travis.yml
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1121 2017-04-20 19:53:57.000000 cr8-0.9.3/setup.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     8173 2017-05-14 18:59:05.000000 cr8-0.9.3/CHANGES.rst
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      815 2016-06-16 18:00:19.000000 cr8-0.9.3/.gitignore
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1086 2016-02-29 21:21:04.000000 cr8-0.9.3/LICENSE
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/tests/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      637 2016-05-29 14:52:19.000000 cr8-0.9.3/tests/test_misc.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     2447 2016-07-12 21:13:31.000000 cr8-0.9.3/tests/test_cli.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)        0 2016-02-29 21:21:04.000000 cr8-0.9.3/tests/__init__.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     3235 2017-03-03 17:31:46.000000 cr8-0.9.3/tests/test_insert_fake_data.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      311 2016-06-22 07:08:55.000000 cr8-0.9.3/tests/test_fake_providers.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1108 2016-06-09 20:58:47.000000 cr8-0.9.3/tests/demo.json
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      890 2017-03-03 17:31:46.000000 cr8-0.9.3/tests/test_clients.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      966 2017-03-03 17:31:46.000000 cr8-0.9.3/tests/test_log.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      231 2016-06-22 07:08:55.000000 cr8-0.9.3/tests/test_insert_json.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     3447 2017-03-03 17:31:46.000000 cr8-0.9.3/tests/test_run_crate.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     2019 2016-12-09 20:03:05.000000 cr8-0.9.3/tests/test_integration.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     1872 2016-06-16 18:04:39.000000 cr8-0.9.3/tests/test_metrics.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     9007 2017-05-14 19:01:14.000000 cr8-0.9.3/PKG-INFO
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/tracks/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)       96 2016-06-16 18:39:41.000000 cr8-0.9.3/tracks/default.toml
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      576 2017-03-03 17:31:46.000000 cr8-0.9.3/tracks/sample.toml
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/specs/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      455 2016-06-20 23:14:18.000000 cr8-0.9.3/specs/count_countries.json
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/specs/sql/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      414 2016-05-29 16:53:33.000000 cr8-0.9.3/specs/sql/create_countries.sql
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      542 2017-03-03 17:31:46.000000 cr8-0.9.3/specs/sample.py
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      409 2016-06-09 20:58:47.000000 cr8-0.9.3/specs/sample_insert.toml
+drwxr-xr-x   0 jordi     (1000) jordi     (1000)        0 2017-05-14 19:01:14.000000 cr8-0.9.3/specs/data/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     7898 2016-05-29 16:53:33.000000 cr8-0.9.3/specs/data/countries.json
+-rw-r--r--   0 jordi     (1000) jordi     (1000)      681 2017-03-03 17:31:46.000000 cr8-0.9.3/specs/sample.toml
```

### Comparing `cr8-0.9.2/README.rst` & `cr8-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     Found schema: 
     {
         "country": "string",
         "id": "integer",
         "name": "string"
     }
     Using insert statement: 
-    insert into x.demo ("country", "id", "name") values (?, ?, ?)
+    insert into "x"."demo" ("country", "id", "name") values (?, ?, ?)
     Will make 1 requests with a bulk size of 200
     Generating fake data and executing inserts
     <BLANKLINE>
 
 
 It will automatically read the schema from the table and map the columns to
 faker `providers
```

### Comparing `cr8-0.9.2/cr8/insert_fake_data.py` & `cr8-0.9.3/cr8/insert_fake_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,18 @@
     _mapping = {
         ('id', 'string'): operator.attrgetter('uuid4'),
         ('id', 'integer'): auto_inc,
         ('id', 'long'): auto_inc,
     }
 
     _type_default = {
-        'integer': operator.attrgetter('random_int'),
-        'long': operator.attrgetter('random_int'),
+        'integer': lambda f: partial(
+            f.random_int, min=-2147483648, max=2147483647),
+        'long': lambda f: partial(
+            f.random_int, min=-9223372036854775808, max=9223372036854775807),
         'float': operator.attrgetter('pyfloat'),
         'double': operator.attrgetter('pydecimal'),
         'ip': operator.attrgetter('ipv4'),
         'timestamp': timestamp,
         'string': operator.attrgetter('word'),
         'boolean': operator.attrgetter('boolean'),
         'geo_point': operator.attrgetter('geo_point'),
@@ -225,15 +227,15 @@
         mapping = json.load(mapping_file)
 
     bulk_size = min(num_records, bulk_size)
     num_inserts = int(math.ceil(num_records / bulk_size))
 
     gen_row = create_row_generator(columns, mapping)
 
-    stmt = to_insert(table, columns)[0]
+    stmt = to_insert('"{schema}"."{table_name}"'.format(**locals()), columns)[0]
     print('Using insert statement: ')
     print(stmt)
 
     print('Will make {} requests with a bulk size of {}'.format(
         num_inserts, bulk_size))
 
     print('Generating fake data and executing inserts')
```

### Comparing `cr8-0.9.2/cr8/clients.py` & `cr8-0.9.3/cr8/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def __init__(self, message):
         self.message = message
 
 
 client_errors = [
     SqlException,
-    aiohttp.errors.ClientError
+    aiohttp.ClientError
 ]
 
 
 def _to_http_uri(s: str) -> str:
     """Prefix the string with 'http://' if there is no schema."""
     if not s.startswith(('http://', 'https://')):
         return 'http://' + s
```

### Comparing `cr8-0.9.2/cr8/misc.py` & `cr8-0.9.3/cr8/misc.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/__main__.py` & `cr8-0.9.3/cr8/__main__.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/run_crate.py` & `cr8-0.9.3/cr8/run_crate.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/engine.py` & `cr8-0.9.3/cr8/engine.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/insert_blob.py` & `cr8-0.9.3/cr8/insert_blob.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/bench_spec.py` & `cr8-0.9.3/cr8/bench_spec.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/insert_json.py` & `cr8-0.9.3/cr8/insert_json.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/log.py` & `cr8-0.9.3/cr8/log.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/run_spec.py` & `cr8-0.9.3/cr8/run_spec.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/run_track.py` & `cr8-0.9.3/cr8/run_track.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/metrics.py` & `cr8-0.9.3/cr8/metrics.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/cli.py` & `cr8-0.9.3/cr8/cli.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/timeit.py` & `cr8-0.9.3/cr8/timeit.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/aio.py` & `cr8-0.9.3/cr8/aio.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8/fake_providers.py` & `cr8-0.9.3/cr8/fake_providers.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8.egg-info/SOURCES.txt` & `cr8-0.9.3/cr8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/cr8.egg-info/PKG-INFO` & `cr8-0.9.3/cr8.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: cr8
-Version: 0.9.2
+Version: 0.9.3
 Summary: A collection of command line tools for crate devs
 Home-page: https://github.com/mfussenegger/cr8
 Author: Mathias Fußenegger
 Author-email: pip@zignar.net
 License: UNKNOWN
 Description: ===
         cr8
@@ -131,15 +131,15 @@
             Found schema: 
             {
                 "country": "string",
                 "id": "integer",
                 "name": "string"
             }
             Using insert statement: 
-            insert into x.demo ("country", "id", "name") values (?, ?, ?)
+            insert into "x"."demo" ("country", "id", "name") values (?, ?, ?)
             Will make 1 requests with a bulk size of 200
             Generating fake data and executing inserts
             <BLANKLINE>
         
         
         It will automatically read the schema from the table and map the columns to
         faker `providers
@@ -267,7 +267,8 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Requires-Python: >=3.5
```

### Comparing `cr8-0.9.2/setup.py` & `cr8-0.9.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,20 +24,21 @@
     },
     packages=['cr8'],
     install_requires=[
         'crate>=0.16',
         'argh',
         'tqdm',
         'Faker',
-        'aiohttp>=1.1,<2',
+        'aiohttp>=2.0,<3',
         'toml'
     ],
     extras_require={
         'uvloop': ['uvloop'],
     },
+    python_requires='>=3.5',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
     ],
```

### Comparing `cr8-0.9.2/CHANGES.rst` & `cr8-0.9.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+2017-05-14 0.9.3
+================
+
+- ``insert-fake-data``: Increased the default value range for columns of type
+  ``integer`` or ``long``.
+
+- Updated ``aiohttp`` to version 2
+
+- ``insert-fake-data``: The schema and table name is now quoted to allow using
+  reserved keywords as schema or table name.
 
-2016-02-11 0.9.2
+2017-02-11 0.9.2
 ================
 
 - Values of type ``Decimal`` or ``datetime`` can now be serialized.
   This fixes an issue that could cause ``insert-fake-data`` to not work with
   schemas that contained columns of type ``double``.
   It also allows track files written in python to use ``Decimal`` or
   ``datetime`` objects as arguments.
@@ -12,15 +22,15 @@
   up to enable tab-completion in bash.
 
 - Fixed an issue that caused warnings with newer ``aiohttp`` versions.
 
 - Adapted ``run-crate`` to handle upcoming breaking changes. It's now able to
   launch tarballs of CrateDB ``1.1`` and ``1.2.`` snapshots.
 
-2016-01-03 0.9.1
+2017-01-03 0.9.1
 ================
 
 - Fixed an issue that caused failures on Windows
 
 - ``timeit`` can now receive multi-line statements via stdin
 
 2016-12-13 0.9.0
```

### Comparing `cr8-0.9.2/.gitignore` & `cr8-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/LICENSE` & `cr8-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_misc.py` & `cr8-0.9.3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_cli.py` & `cr8-0.9.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_insert_fake_data.py` & `cr8-0.9.3/tests/test_insert_fake_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def test_fake_provider_for_long_id_column(self):
         provider = self.f.provider_for_column('id', 'long')
         self.assertEqual(provider(), 1)
 
     def test_type_default_provider_for_unknown_int_column(self):
         provider = self.f.provider_for_column(
             'column_name_without_provider', 'integer')
-        self.assertEqual(provider(), 1824)  # got random_int provider
+        self.assertEqual(provider(), 598833565)  # got random_int provider
 
     def test_timestamp_column_default(self):
         provider = self.f.provider_for_column('timestamp', 'timestamp')
         self.assertEqual(provider(), 1373158606000)
 
     def test_timestamp_type_default(self):
         provider = self.f.provider_for_column('some_ts_column', 'timestamp')
```

### Comparing `cr8-0.9.2/tests/demo.json` & `cr8-0.9.3/tests/demo.json`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_clients.py` & `cr8-0.9.3/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_log.py` & `cr8-0.9.3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_run_crate.py` & `cr8-0.9.3/tests/test_run_crate.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_integration.py` & `cr8-0.9.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/tests/test_metrics.py` & `cr8-0.9.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/PKG-INFO` & `cr8-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: cr8
-Version: 0.9.2
+Version: 0.9.3
 Summary: A collection of command line tools for crate devs
 Home-page: https://github.com/mfussenegger/cr8
 Author: Mathias Fußenegger
 Author-email: pip@zignar.net
 License: UNKNOWN
 Description: ===
         cr8
@@ -131,15 +131,15 @@
             Found schema: 
             {
                 "country": "string",
                 "id": "integer",
                 "name": "string"
             }
             Using insert statement: 
-            insert into x.demo ("country", "id", "name") values (?, ?, ?)
+            insert into "x"."demo" ("country", "id", "name") values (?, ?, ?)
             Will make 1 requests with a bulk size of 200
             Generating fake data and executing inserts
             <BLANKLINE>
         
         
         It will automatically read the schema from the table and map the columns to
         faker `providers
@@ -267,7 +267,8 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Requires-Python: >=3.5
```

### Comparing `cr8-0.9.2/tracks/sample.toml` & `cr8-0.9.3/tracks/sample.toml`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/specs/sample.py` & `cr8-0.9.3/specs/sample.py`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/specs/data/countries.json` & `cr8-0.9.3/specs/data/countries.json`

 * *Files identical despite different names*

### Comparing `cr8-0.9.2/specs/sample.toml` & `cr8-0.9.3/specs/sample.toml`

 * *Files identical despite different names*

