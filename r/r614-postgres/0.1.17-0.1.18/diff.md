# Comparing `tmp/r614_postgres-0.1.17.tar.gz` & `tmp/r614_postgres-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r614_postgres-0.1.17.tar", max compression
+gzip compressed data, was "r614_postgres-0.1.18.tar", max compression
```

## Comparing `r614_postgres-0.1.17.tar` & `r614_postgres-0.1.18.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7052 2023-07-09 21:20:39.559901 r614_postgres-0.1.17/LICENSE
--rw-r--r--   0        0        0       18 2023-07-09 21:20:39.562698 r614_postgres-0.1.17/README.md
--rw-r--r--   0        0        0      972 2023-07-09 21:38:56.407215 r614_postgres-0.1.17/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 21:20:39.563581 r614_postgres-0.1.17/r614_postgres/__init__.py
--rw-r--r--   0        0        0    24583 2023-07-09 21:26:05.358408 r614_postgres-0.1.17/r614_postgres/postgres.py
--rw-r--r--   0        0        0        0 2023-07-09 21:20:39.564011 r614_postgres-0.1.17/r614_postgres/py.typed
--rw-r--r--   0        0        0     1308 2023-07-09 21:20:39.563477 r614_postgres-0.1.17/r614_postgres/retries.py
--rw-r--r--   0        0        0    12591 2023-07-09 21:25:30.709343 r614_postgres-0.1.17/r614_postgres/validation.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 r614_postgres-0.1.17/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-07-09 21:20:39.559901 r614_postgres-0.1.18/LICENSE
+-rw-r--r--   0        0        0       18 2023-07-09 21:20:39.562698 r614_postgres-0.1.18/README.md
+-rw-r--r--   0        0        0      971 2023-07-09 22:05:49.823697 r614_postgres-0.1.18/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 21:20:39.563581 r614_postgres-0.1.18/r614_postgres/__init__.py
+-rw-r--r--   0        0        0    24136 2023-07-09 22:04:56.674240 r614_postgres-0.1.18/r614_postgres/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:20:39.564011 r614_postgres-0.1.18/r614_postgres/py.typed
+-rw-r--r--   0        0        0     1308 2023-07-09 21:20:39.563477 r614_postgres-0.1.18/r614_postgres/retries.py
+-rw-r--r--   0        0        0    12591 2023-07-09 21:25:30.709343 r614_postgres-0.1.18/r614_postgres/validation.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 r614_postgres-0.1.18/PKG-INFO
```

### Comparing `r614_postgres-0.1.17/LICENSE` & `r614_postgres-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `r614_postgres-0.1.17/pyproject.toml` & `r614_postgres-0.1.18/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "r614-postgres"
-version = "0.1.17"
+version = "0.1.18"
 description = "Postgres wrapper for python"
 authors = ["Roshan Pawar <steradian614@gmail.com>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "r614_postgres"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typing-extensions = "^4.4.0"
 psycopg = { extras = ["pool", "binary"], version = "^3.1.8" }
-r614-config = "^0.1.6"
-latch-o11y = "^0.1.4"
+r614-config = "^0.1.7"
+r614-o11y = "^0.1.5"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 rich = "^13.2.0"
```

### Comparing `r614_postgres-0.1.17/r614_postgres/postgres.py` & `r614_postgres-0.1.18/r614_postgres/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     ParamSpec,
     TypeVar,
     cast,
 )
 
 import psycopg.sql as sql
 from r614_config.config import PostgresConnectionConfig
-from validation import JsonObject, validate
-from latch_o11y.o11y import dict_to_attrs, trace_function
+from r614_postgres.validation import JsonObject, validate
+from r614_o11y.o11y import dict_to_attrs, trace_function
 from opentelemetry.sdk.resources import Attributes
 from opentelemetry.trace import SpanKind, get_tracer
 from psycopg import AsyncConnection, AsyncCursor, IsolationLevel
 from psycopg.abc import AdaptContext, Params, Query
 from psycopg.conninfo import conninfo_to_dict, make_conninfo
 from psycopg.errors import (
     AdminShutdown,
@@ -57,35 +57,25 @@
 )
 from psycopg.rows import AsyncRowFactory, Row, dict_row, kwargs_row
 from psycopg.types.composite import CompositeInfo, register_composite
 from psycopg.types.enum import EnumInfo, register_enum
 from psycopg_pool import AsyncConnectionPool
 from typing_extensions import Self
 
-from latch_postgres.retries import CABackoff
+from r614_postgres.retries import CABackoff
 
 T = TypeVar("T")
 
 tracer = get_tracer(__name__)
 
 
-# todo(maximsmol): switch all the tracing attributes to otel spec
-# del span.type
-# in event names postgres -> postgresql (or to psycopg)?
-# out.host -> net.peer.name
-# out.port -> net.peer.port
-# sql.query -> db.statement
-# del resource.name
 def conninfo_attributes(x: str) -> Attributes:
     data = conninfo_to_dict(x)
 
     res: Attributes = {
-        # todo(maximsmol): is this service name override a datadog idiosyncrasy?
-        # todo(maximsmol): allow for multiple databases
-        "service.name": "vacuole",
         "db.system": "postgresql",
         "span.type": "sql",
         "db.connection_string": make_conninfo(x, password="[REDACTED]"),
     }
     if data["host"] is not None:
         res["out.host"] = data["host"]
     if data["port"] is not None:
@@ -106,15 +96,14 @@
 
     if isinstance(x, bytes):
         return x
 
     return x.as_string(ctx)
 
 
-# todo(maximsmol): switch tracing to use decorators from o11y
 class TracedAsyncCursor(AsyncCursor[Row]):
     trace_attributes: Attributes
 
     async def execute(
         self,
         query: Query,
         params: Params | None = None,
@@ -150,15 +139,15 @@
         ) as span:
             try:
                 return await super().executemany(query, params_seq)
             finally:
                 span.set_attributes({"db.rowcount": self.rowcount})
 
 
-class LatchAsyncConnection(AsyncConnection[Row]):
+class PostgresAsyncConnection(AsyncConnection[Row]):
     trace_attributes: Attributes
 
     def cursor(
         self,
         row_factory: AsyncRowFactory[Any],
         *,
         binary: bool = True,
@@ -270,15 +259,15 @@
             configure=self._configure_wrapper,
             reset=reset,
             **kwargs,
         )
 
     async def _configure_wrapper(self, conn: AsyncConnection[object]):
         with tracer.start_as_current_span("configure connection"):
-            assert isinstance(conn, LatchAsyncConnection)
+            assert isinstance(conn, PostgresAsyncConnection)
 
             conn.cursor_factory = TracedAsyncCursor
             conn.trace_attributes = self._trace_attributes
 
             if (
                 len(self.setup_commands) > 0
                 or len(self.enum_map) > 0
@@ -482,29 +471,29 @@
         "sqlstate": x.sqlstate,
         "diagnostic": diagnostic_obj,
         "type": type(x).__name__,
     }
 
 
 def with_conn_retry(
-    f: Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]],
+    f: Callable[Concatenate[PostgresAsyncConnection[Any], P], Awaitable[T]],
     pool: AsyncConnectionPool,
     db_config: PostgresConnectionConfig,
 ) -> Callable[P, Awaitable[T]]:
     @functools.wraps(f)
     async def inner(*args: P.args, **kwargs: P.kwargs):
         with tracer.start_as_current_span("database session") as s:
             try:
                 retries = 0
                 accum_retry_time = 0
 
                 while True:
                     try:
                         async with pool.connection() as conn:
-                            assert isinstance(conn, LatchAsyncConnection)
+                            assert isinstance(conn, PostgresAsyncConnection)
 
                             backoff = CABackoff(
                                 db_config.tx_retries.delay_quant,
                                 db_config.tx_retries.max_wait_time,
                             )
                             while True:
                                 try:
@@ -611,15 +600,15 @@
 
     return inner
 
 
 def get_with_conn_retry(
     pool: AsyncConnectionPool, db_config: PostgresConnectionConfig
 ) -> Callable[
-    [Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]]],
+    [Callable[Concatenate[PostgresAsyncConnection[Any], P], Awaitable[T]]],
     Callable[P, Awaitable[T]],
 ]:
     return functools.partial(with_conn_retry, pool=pool, db_config=db_config)
 
 
 def sqlq(x: str):
     return sql.SQL(dedent(x))
@@ -664,9 +653,9 @@
         open=False,
         configure=functools.partial(
             reset_conn, read_only=read_only, isolation_level=isolation_level
         ),
         reset=functools.partial(
             reset_conn, read_only=read_only, isolation_level=isolation_level
         ),
-        connection_class=LatchAsyncConnection,
+        connection_class=PostgresAsyncConnection,
     )
```

### Comparing `r614_postgres-0.1.17/r614_postgres/retries.py` & `r614_postgres-0.1.18/r614_postgres/retries.py`

 * *Files identical despite different names*

### Comparing `r614_postgres-0.1.17/r614_postgres/validation.py` & `r614_postgres-0.1.18/r614_postgres/validation.py`

 * *Files identical despite different names*

### Comparing `r614_postgres-0.1.17/PKG-INFO` & `r614_postgres-0.1.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: r614-postgres
-Version: 0.1.17
+Version: 0.1.18
 Summary: Postgres wrapper for python
 License: CC0 1.0
 Author: Roshan Pawar
 Author-email: steradian614@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: latch-o11y (>=0.1.4,<0.2.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.8,<4.0.0)
-Requires-Dist: r614-config (>=0.1.6,<0.2.0)
+Requires-Dist: r614-config (>=0.1.7,<0.2.0)
+Requires-Dist: r614-o11y (>=0.1.5,<0.2.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # python-postgres
```

