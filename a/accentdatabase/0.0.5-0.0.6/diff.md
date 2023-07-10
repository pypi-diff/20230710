# Comparing `tmp/accentdatabase-0.0.5.tar.gz` & `tmp/accentdatabase-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accentdatabase-0.0.5.tar", last modified: Fri Feb 24 15:59:10 2023, max compression
+gzip compressed data, was "accentdatabase-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `accentdatabase-0.0.5.tar` & `accentdatabase-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentdatabase-0.0.5/.flake8
--rw-r--r--   0        0        0      921 2022-10-05 15:56:51.000000 accentdatabase-0.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0       98 2022-10-05 13:05:19.000000 accentdatabase-0.0.5/.gitignore
--rw-r--r--   0        0        0     1090 2022-10-10 11:22:41.000000 accentdatabase-0.0.5/LICENSE
--rw-r--r--   0        0        0      319 2022-10-06 08:19:07.000000 accentdatabase-0.0.5/README.md
--rw-r--r--   0        0        0      132 2023-02-24 15:57:08.000000 accentdatabase-0.0.5/accentdatabase/__init__.py
--rw-r--r--   0        0        0      481 2023-02-24 15:19:48.000000 accentdatabase-0.0.5/accentdatabase/base.py
--rw-r--r--   0        0        0      345 2022-10-06 13:04:06.000000 accentdatabase-0.0.5/accentdatabase/config.py
--rw-r--r--   0        0        0      333 2022-10-07 08:58:02.000000 accentdatabase-0.0.5/accentdatabase/encoders.py
--rw-r--r--   0        0        0      238 2022-10-06 13:43:32.000000 accentdatabase-0.0.5/accentdatabase/engine.py
--rw-r--r--   0        0        0      658 2023-02-24 15:56:58.000000 accentdatabase-0.0.5/accentdatabase/mixins.py
--rw-r--r--   0        0        0     6675 2023-01-03 13:49:46.000000 accentdatabase-0.0.5/accentdatabase/operations.py
--rw-r--r--   0        0        0      782 2022-10-07 09:26:52.000000 accentdatabase-0.0.5/accentdatabase/session.py
--rw-r--r--   0        0        0      989 2023-02-24 15:19:48.000000 accentdatabase-0.0.5/accentdatabase/testing.py
--rw-r--r--   0        0        0     1251 2023-02-24 15:19:48.000000 accentdatabase-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 accentdatabase-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentdatabase-0.0.6/.flake8
+-rw-r--r--   0        0        0      929 2023-07-10 10:47:48.676086 accentdatabase-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0       98 2022-10-05 13:05:19.000000 accentdatabase-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1090 2022-10-10 11:22:41.000000 accentdatabase-0.0.6/LICENSE
+-rw-r--r--   0        0        0      319 2022-10-06 08:19:07.000000 accentdatabase-0.0.6/README.md
+-rw-r--r--   0        0        0      134 2023-07-10 10:53:16.119670 accentdatabase-0.0.6/accentdatabase/__init__.py
+-rw-r--r--   0        0        0      481 2023-03-30 07:48:07.000000 accentdatabase-0.0.6/accentdatabase/base.py
+-rw-r--r--   0        0        0      413 2023-07-10 10:42:42.375920 accentdatabase-0.0.6/accentdatabase/config.py
+-rw-r--r--   0        0        0      333 2022-10-07 08:58:02.000000 accentdatabase-0.0.6/accentdatabase/encoders.py
+-rw-r--r--   0        0        0      243 2023-07-10 10:09:15.252548 accentdatabase-0.0.6/accentdatabase/engine.py
+-rw-r--r--   0        0        0      658 2023-02-24 15:56:58.000000 accentdatabase-0.0.6/accentdatabase/mixins.py
+-rw-r--r--   0        0        0     6675 2023-01-03 13:49:46.000000 accentdatabase-0.0.6/accentdatabase/operations.py
+-rw-r--r--   0        0        0      852 2023-07-10 10:52:21.692037 accentdatabase-0.0.6/accentdatabase/session.py
+-rw-r--r--   0        0        0     1007 2023-07-10 10:09:51.012364 accentdatabase-0.0.6/accentdatabase/testing.py
+-rw-r--r--   0        0        0     1304 2023-07-10 10:45:05.999094 accentdatabase-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 accentdatabase-0.0.6/PKG-INFO
```

### Comparing `accentdatabase-0.0.5/.github/workflows/test.yml` & `accentdatabase-0.0.6/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     types: [opened, synchronize]
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
       fail-fast: false
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `accentdatabase-0.0.5/LICENSE` & `accentdatabase-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.5/accentdatabase/mixins.py` & `accentdatabase-0.0.6/accentdatabase/mixins.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.5/accentdatabase/operations.py` & `accentdatabase-0.0.6/accentdatabase/operations.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.5/accentdatabase/testing.py` & `accentdatabase-0.0.6/accentdatabase/testing.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 async def recreate_postgres_database(
     database_url: PostgresDsn,
     maintenance_db: str = "postgres",
 ):
     """Drop and recreate test database, requires min of postgres v13"""
 
     maintenance_url = deepcopy(database_url)
-    maintenance_url = maintenance_url.replace(
+    maintenance_url_str = str(maintenance_url).replace(
         maintenance_url.path,
         f"/{maintenance_db}",
     )
-    test_db = database_url.split("/")[-1]
+    test_db = str(database_url).split("/")[-1]
 
     engine = create_async_engine(
-        maintenance_url,
+        maintenance_url_str,
         isolation_level="AUTOCOMMIT",
     )
 
     async with engine.begin() as conn:
         # drop the test database
         drop = f"DROP DATABASE IF EXISTS {test_db} WITH (FORCE);"
         await conn.execute(text(drop))
```

### Comparing `accentdatabase-0.0.5/pyproject.toml` & `accentdatabase-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
 ]
 dependencies = [
-    "pydantic",
+    "pydantic>=2.0.1,<2.1.0",
+    "pydantic-settings>=2.0.1,<2.1.0",
     "sqlalchemy>=2.0.0,<2.1.0",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Homepage = "https://github.com/accentdesign/accentdatabase"
```

### Comparing `accentdatabase-0.0.5/PKG-INFO` & `accentdatabase-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: accentdatabase
-Version: 0.0.5
-Summary: Handling sqlalchemy connection and test helpers including declarative base, session, engine and mixins
+Version: 0.0.6
+Summary: Handling sqlalchemy connection and test helpers including
 Author-email: Accent Design Group Ltd <support@accentdesign.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
-Requires-Dist: pydantic
+Requires-Dist: pydantic>=2.0.1,<2.1.0
+Requires-Dist: pydantic-settings>=2.0.1,<2.1.0
 Requires-Dist: sqlalchemy>=2.0.0,<2.1.0
 Requires-Dist: alembic ; extra == "alembic"
 Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: accentdatabase Version: 0.0.5 Summary: Handling
-sqlalchemy connection and test helpers including declarative base, session,
-engine and mixins Author-email: Accent Design Group Ltd
+Metadata-Version: 2.1 Name: accentdatabase Version: 0.0.6 Summary: Handling
+sqlalchemy connection and test helpers including Author-email: Accent Design
+Group Ltd
 accentdesign.co.uk> Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Requires-Dist: pydantic Requires-Dist: sqlalchemy>=2.0.0,<2.1.0 Requires-Dist:
+Requires-Dist: pydantic>=2.0.1,<2.1.0 Requires-Dist: pydantic-
+settings>=2.0.1,<2.1.0 Requires-Dist: sqlalchemy>=2.0.0,<2.1.0 Requires-Dist:
 alembic ; extra == "alembic" Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev" Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: mypy ; extra ==
 "test" Requires-Dist: flake8 ; extra == "test" Requires-Dist: black ; extra ==
 "test" Requires-Dist: isort ; extra == "test" Project-URL: Homepage, https://
 github.com/accentdesign/accentdatabase Provides-Extra: alembic Provides-Extra:
 dev Provides-Extra: test [![Test](https://github.com/accentdesign/
```

