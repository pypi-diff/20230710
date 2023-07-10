# Comparing `tmp/dbt-cratedb-1.0.3.0.tar.gz` & `tmp/dbt-cratedb-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-cratedb-1.0.3.0.tar", last modified: Thu Feb 24 20:41:25 2022, max compression
+gzip compressed data, was "dbt-cratedb-1.5.2.tar", last modified: Mon Jul 10 21:03:18 2023, max compression
```

## Comparing `dbt-cratedb-1.0.3.0.tar` & `dbt-cratedb-1.5.2.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/
--rw-rw-r--   0 julio     (1000) julio     (1000)       46 2021-07-29 22:38:16.000000 dbt-cratedb-1.0.3.0/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)      796 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      289 2021-10-05 19:04:03.000000 dbt-cratedb-1.0.3.0/README.md
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt/
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt/adapters/
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt/adapters/cratedbadapter/
--rw-rw-r--   0 julio     (1000) julio     (1000)      731 2021-09-28 17:09:24.000000 dbt-cratedb-1.0.3.0/dbt/adapters/cratedbadapter/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)        8 2021-07-29 22:38:16.000000 dbt-cratedb-1.0.3.0/dbt/adapters/cratedbadapter/__version__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     5816 2022-02-24 20:09:33.000000 dbt-cratedb-1.0.3.0/dbt/adapters/cratedbadapter/connections.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1977 2021-10-13 21:48:17.000000 dbt-cratedb-1.0.3.0/dbt/adapters/cratedbadapter/impl.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      934 2021-10-07 21:00:45.000000 dbt-cratedb-1.0.3.0/dbt/adapters/cratedbadapter/relation.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt/include/
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/
--rw-rw-r--   0 julio     (1000) julio     (1000)       51 2021-07-29 22:38:16.000000 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)       82 2021-10-11 21:57:45.000000 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/dbt_project.yml
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/
--rw-rw-r--   0 julio     (1000) julio     (1000)     3061 2021-10-14 22:39:21.000000 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/adapters.sql
--rw-rw-r--   0 julio     (1000) julio     (1000)     2394 2021-11-01 22:42:45.000000 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/catalog.sql
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/materializations/
--rw-rw-r--   0 julio     (1000) julio     (1000)      159 2021-10-14 19:33:32.000000 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/materializations/snapshot_merge.sql
--rw-rw-r--   0 julio     (1000) julio     (1000)       98 2021-09-28 19:23:45.000000 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/relations.sql
--rw-rw-r--   0 julio     (1000) julio     (1000)      185 2021-10-07 21:00:45.000000 dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/sample_profiles.yml
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/dbt_cratedb.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)      796 2022-02-24 20:41:25.000000 dbt-cratedb-1.0.3.0/dbt_cratedb.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      780 2022-02-24 20:41:25.000000 dbt-cratedb-1.0.3.0/dbt_cratedb.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2022-02-24 20:41:25.000000 dbt-cratedb-1.0.3.0/dbt_cratedb.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2021-10-05 17:23:10.000000 dbt-cratedb-1.0.3.0/dbt_cratedb.egg-info/not-zip-safe
--rw-rw-r--   0 julio     (1000) julio     (1000)       37 2022-02-24 20:41:25.000000 dbt-cratedb-1.0.3.0/dbt_cratedb.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        4 2022-02-24 20:41:25.000000 dbt-cratedb-1.0.3.0/dbt_cratedb.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       38 2022-02-24 20:41:25.005046 dbt-cratedb-1.0.3.0/setup.cfg
--rw-rw-r--   0 julio     (1000) julio     (1000)     2774 2022-02-24 20:30:57.000000 dbt-cratedb-1.0.3.0/setup.py
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       46 2023-07-03 22:05:42.000000 dbt-cratedb-1.5.2/MANIFEST.in
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     1243 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/PKG-INFO
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      539 2023-07-03 23:13:55.000000 dbt-cratedb-1.5.2/README.md
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/adapters/
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/adapters/cratedb/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      639 2023-07-10 20:50:03.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/__init__.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       17 2023-07-03 22:53:10.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/__version__.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       77 2023-07-04 19:23:08.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/column.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     6025 2023-07-10 20:01:04.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/connections.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2971 2023-07-10 20:22:35.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/impl.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      259 2023-07-05 15:57:50.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/relation.py
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/include/
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/include/cratedb/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       52 2023-07-04 19:34:23.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/__init__.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       77 2023-07-04 19:51:16.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/dbt_project.yml
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/include/cratedb/macros/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     3996 2023-07-10 19:57:54.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/macros/adapters.sql
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2814 2023-07-06 18:53:30.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/macros/catalog.sql
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      203 2023-07-03 22:53:10.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/sample_profiles.yml
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     1243 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/PKG-INFO
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      623 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/SOURCES.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        1 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/dependency_links.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        1 2023-07-04 19:58:52.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/not-zip-safe
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       30 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/requires.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        4 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/top_level.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       38 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/setup.cfg
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2436 2023-07-10 20:50:52.000000 dbt-cratedb-1.5.2/setup.py
```

### Comparing `dbt-cratedb-1.0.3.0/dbt/adapters/cratedbadapter/connections.py` & `dbt-cratedb-1.5.2/dbt/adapters/cratedb/connections.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,184 +1,193 @@
 from contextlib import contextmanager
 
-import psycopg2
-import time
+from crate import client
+from crate.client.exceptions import Error, DatabaseError, InterfaceError
+from crate.client.converter import DataType
+
 from typing import List, Optional, Tuple, Any, Iterable, Dict, Union
-from dbt.contracts.connection import (
-    Connection, ConnectionState, AdapterResponse
-)
+
 import dbt.exceptions
 from dbt.adapters.base import Credentials
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse
-from dbt.logger import GLOBAL_LOGGER as logger
+from dbt.events import AdapterLogger
 
-from dbt.helper_types import Port
 from dataclasses import dataclass
-from typing import Optional
+
+logger = AdapterLogger("Cratedb")
 
 
 @dataclass
-class CratedbAdapterCredentials(Credentials):
-    host: str
-    user: str
-    port: Port
-    password: str  # on postgres the password is mandatory
+class CrateDBAdapterCredentials(Credentials):
+    database: str = "crate"
+    host: Optional[str | List[str]] = "http://localhost:4200/"
+    username: Optional[str] = "crate"
+    password: Optional[str] = None
+    ca_cert: Optional[str] = None
+    verify_ssl_cert: Optional[bool] = False
+    cert_file: Optional[str] = None
+    key_file: Optional[str] = None
+    timeout: Optional[int] = 60  # Timeout in Seconds
+    error_trace: Optional[bool] = False
+    backoff_factor: Optional[float] = 0.1
+    socket_keepalive: Optional[bool] = False
+    socket_tcp_keepidle: Optional[int] = None
+    socket_tcp_keepintvl: Optional[int] = None
+    socket_tcp_keepcnt: Optional[int] = None
+    schema: Optional[str] = "doc"
+    retries: int = 1
 
     _ALIASES = {
-        'dbname': 'database',
         'pass': 'password'
     }
 
     @property
     def type(self):
-        return 'cratedbadapter'
+        return 'cratedb'
+
+    @property
+    def unique_field(self):
+        return self.host
 
     def _connection_keys(self):
-        # return an iterator of keys to pretty-print in 'dbt debug'.
-        # Omit fields like 'password'!
-        return ('host', 'port', 'user', 'schema')
-
-
-class CratedbAdapterConnectionManager(SQLConnectionManager):
-    TYPE = 'cratedbadapter'
-
-    def add_query(
-        self,
-        sql: str,
-        auto_begin: bool = False,
-        bindings: Optional[Any] = None,
-        abridge_sql_log: bool = False
-    ) -> Tuple[Connection, Any]:
-        connection = self.get_thread_connection()
-        sql=sql.replace('"".','')
-        sql = sql.replace(' cascade', '')
-        sql = sql.replace(' limit 100;', '')
-        #print("...")
-        #print(sql)
-        #print("...")
-        if auto_begin and connection.transaction_open is False:
-            self.begin()
-
-        logger.debug('Using {} connection "{}".'
-                     .format(self.TYPE, connection.name))
-
-        with self.exception_handler(sql):
-            if abridge_sql_log:
-                log_sql = '{}...'.format(sql[:512])
-            else:
-                log_sql = sql
-
-            logger.debug(
-                'On {connection_name}: {sql}',
-                connection_name=connection.name,
-                sql=log_sql,
-            )
-            pre = time.time()
+        return (
+            'host',
+            'user',
+            'schema'
+        )
 
-            cursor = connection.handle.cursor()
-            cursor.execute(sql, bindings)
-            logger.debug(
-                "SQL status: {status} in {elapsed:0.2f} seconds",
-                status=self.get_response(cursor),
-                elapsed=(time.time() - pre)
-            )
+    def auth_args(self):
+        result = {}
+
+        if self.ca_cert:
+            result['ca_cert'] = self.ca_cert
+        if self.verify_ssl_cert is not None:
+            result['verify_ssl_cert'] = self.verify_ssl_cert
+        if self.cert_file:
+            result['cert_file'] = self.cert_file
+        if self.key_file:
+            result['key_file'] = self.key_file
+        if self.timeout:
+            result['timeout'] = self.timeout
+        if self.error_trace is not None:
+            result['error_trace'] = self.error_trace
+        if self.backoff_factor:
+            result['backoff_factor'] = self.backoff_factor
+        if self.socket_keepalive:
+            if self.socket_tcp_keepidle:
+                result['socket_tcp_keepidle'] = self.socket_tcp_keepidle
+            if self.socket_tcp_keepintvl:
+                result['socket_tcp_keepintvl'] = self.socket_tcp_keepintvl
+            if self.socket_tcp_keepcnt:
+                result['socket_tcp_keepcnt'] = self.socket_tcp_keepcnt
+
+        return result
+
+
+class CrateDBAdapterConnectionManager(SQLConnectionManager):
+    TYPE = 'cratedb'
+
+    @contextmanager
+    def exception_handler(self, sql):
+        try:
+            yield
+
+        except DatabaseError as e:
+            logger.debug('CrateDB error: {}'.format(str(e)))
+            try:
+                self.rollback_if_open()
+            except Error:
+                logger.debug("Failed to release connection!")
+                pass
+
+            raise dbt.exceptions.DbtDatabaseError(str(e).strip()) from e
+
+        except Exception as e:
+            logger.debug("Error running SQL: {}", sql)
+            logger.debug("Rolling back transaction.")
+            self.rollback_if_open()
+            if isinstance(e, dbt.exceptions.DbtRuntimeError):
+                # during a sql query, an internal to dbt exception was raised.
+                # this sounds a lot like a signal handler and probably has
+                # useful information, so raise it without modification.
+                raise
 
-            return connection, cursor
+            raise dbt.exceptions.DbtRuntimeError(e) from e
 
     @classmethod
     def open(cls, connection):
         if connection.state == 'open':
             logger.debug('Connection is already open, skipping open.')
             return connection
 
-        credentials = cls.get_credentials(connection.credentials)
+        creds = connection.credentials
 
-        try:
-            handle = psycopg2.connect(
-                dbname="",
-                user=credentials.user,
-                host=credentials.host,
-                password=credentials.password,
-                port=credentials.port,
-                connect_timeout=10)
-            connection.handle = handle
-        except psycopg2.Error as e:
-            logger.debug("Got an error when attempting to open a cratedb "
-                         "connection: '{}'"
-                         .format(e))
-            connection.handle = None
-            connection.state = 'fail'
-            raise dbt.exceptions.FailedToConnectException(str(e))
-        return connection
+        def connect():
+            handle = client.connect(
+                creds.host,
+                username=creds.username,
+                password=creds.password,
+                schema=creds.schema,
+                **creds.auth_args()
+            )
+            return handle
+
+        retryable_exceptions = [
+            client.exceptions.OperationalError,
+            client.exceptions.InternalError,
+            client.exceptions.DatabaseError
+        ]
+
+        def exponential_backoff(attempt: int):
+            return attempt * attempt
+
+        return cls.retry_connection(
+            connection,
+            connect=connect,
+            logger=logger,
+            retry_limit=creds.retries,
+            retry_timeout=exponential_backoff,
+            retryable_exceptions=retryable_exceptions
+        )
 
     def cancel(self, connection):
         connection_name = connection.name
         try:
-            pid = connection.handle.get_backend_pid()
-        except psycopg2.InterfaceError as exc:
+            pid = connection.handle.get_backend_pid()  # TODO: Investigate if this is the right way to get the pid in crate
+        except InterfaceError as exc:
             # if the connection is already closed, not much to cancel!
             if 'already closed' in str(exc):
                 logger.debug(
                     f'Connection {connection_name} was already closed'
                 )
                 return
-            # probably bad, re-raise it
             raise
 
-        sql = "select pg_terminate_backend({})".format(pid)
+        sql = "KILL {})".format(pid)
 
         logger.debug("Cancelling query '{}' ({})".format(connection_name, pid))
 
         _, cursor = self.add_query(sql)
         res = cursor.fetchone()
 
         logger.debug("Cancel query '{}': {}".format(connection_name, res))
 
     @classmethod
-    def get_credentials(cls, credentials):
-        return credentials
-
-    @classmethod
     def get_response(cls, cursor) -> AdapterResponse:
-        message = str(cursor.statusmessage)
         rows = cursor.rowcount
-        status_message_parts = message.split() if message is not None else []
-        status_messsage_strings = [
-            part
-            for part in status_message_parts
-            if not part.isdigit()
-        ]
-        code = ' '.join(status_messsage_strings)
+
         return AdapterResponse(
-            _message=message,
-            code=code,
+            _message="{} {}".format(rows, "row" if rows == 1 else "rows"),
             rows_affected=rows
         )
 
-    @contextmanager
-    def exception_handler(self, sql):
-        try:
-            yield
-
-        except psycopg2.DatabaseError as e:
-            logger.debug('Postgres error: {}'.format(str(e)))
-
-            try:
-                self.rollback_if_open()
-            except psycopg2.Error:
-                logger.debug("Failed to release connection!")
-                pass
-
-            raise dbt.exceptions.DatabaseException(str(e).strip()) from e
+    @classmethod
+    def data_type_code_to_name(cls, type_code: Union[int, str]) -> str:
+        type_name = "UNKNOWN"
 
-        except Exception as e:
-            logger.debug("Error running SQL: {}", sql)
-            logger.debug("Rolling back transaction.")
-            self.rollback_if_open()
-            if isinstance(e, dbt.exceptions.RuntimeException):
-                # during a sql query, an internal to dbt exception was raised.
-                # this sounds a lot like a signal handler and probably has
-                # useful information, so raise it without modification.
-                raise
+        for t in list(DataType):
+            if t.value == type_code:
+                type_name = t.name
+                break
 
-            raise dbt.exceptions.RuntimeException(e) from e
+        return type_name
```

### Comparing `dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/adapters.sql` & `dbt-cratedb-1.5.2/dbt/include/cratedb/macros/adapters.sql`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 
-{% macro cratedbadapter__create_table_as(temporary, relation, sql) -%}
-
+{% macro cratedb__create_table_as(temporary, relation, sql) -%}
   {%- call statement('check_relation_exists', fetch_result=True) -%}
     select count(*) from "information_schema"."tables" where table_name='{{ relation.identifier }}' and table_schema='{{ relation.schema }}';
   {% endcall %}
+
   {% set relation_exists = load_result('check_relation_exists') %}
+
   {% if relation_exists['data'][0][0] == 0 %}
     create table {{ relation }}
       as (
         {{ sql }}
       );
-  {% else %}
-    commit;
   {% endif %}
 
 {%- endmacro %}
 
-{% macro cratedbadapter__check_schema_exists(information_schema, schema) -%}
-  {#
-    On CrateDB, schemas are created implicitly according to the name used.
-    If a schema does not exist, CrateDB create it automatically.
-  #}
-  {% call statement('check_schema_exists', fetch_result=True, auto_begin=False) %}
-    select 1;
-  {% endcall %}
-  {{ return(load_result('check_schema_exists').table) }}
-{% endmacro %}
-
-{% macro cratedbadapter__get_columns_in_relation(relation) -%}
+{% macro cratedb__get_columns_in_relation(relation) -%}
   {% call statement('get_columns_in_relation', fetch_result=True) %}
       select
           column_name,
           data_type,
           character_maximum_length,
           numeric_precision,
           numeric_scale
@@ -44,15 +32,15 @@
       order by ordinal_position
 
   {% endcall %}
   {% set table = load_result('get_columns_in_relation').table %}
   {{ return(sql_convert_columns_in_relation(table)) }}
 {% endmacro %}
 
-{% macro cratedbadapter__list_relations_without_caching(schema_relation) %}
+{% macro cratedb__list_relations_without_caching(schema_relation) %}
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
     select
       '{{ schema_relation.database }}' as database,
       table_name as name,
       table_schema as schema,
       'table' as type
     from information_schema.tables
@@ -65,36 +53,72 @@
       'view' as type
     from information_schema.views
     where table_schema ilike '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
-{% macro cratedbadapter__current_timestamp() -%}
+{% macro cratedb__current_timestamp() -%}
   now()
 {%- endmacro %}
 
 
-{% macro cratedbadapter__create_view_as(relation, sql) -%}
-  create table {{ relation }} as
+{% macro cratedb__create_view_as(relation, sql) -%}
+  create view {{ relation }} as
     {{ sql }};
 {% endmacro %}
 
 
-{% macro cratedbadapter__rename_relation(from_relation, to_relation) -%}
+{% macro cratedb__rename_relation(from_relation, to_relation) -%}
   {% call statement('rename_relation') -%}
     alter table {{ from_relation }} rename to {{ to_relation.name }}
   {%- endcall %}
 {% endmacro %}
 
-{% macro cratedbadapter__create_schema(relation) -%}
+{% macro cratedb__create_schema(relation) -%}
   {%- call statement('create_schema') -%}
     commit;
   {%- endcall -%}
 {% endmacro %}
 
-{% macro dbt_macro__create_schema(relation) -%}
-  {%- call statement('create_schema') -%}
-    commit;
-  {%- endcall -%}
+{% macro cratedb__list_schemas(database) -%}
+    {% call statement('list_schemas', fetch_result=True, auto_begin=False) %}
+      show schemas;
+    {% endcall %}
+    {{ return(load_result('list_schemas').table) }}
+{% endmacro %}
+
+{% macro cratedb__drop_relation(relation) -%}
+  {% call statement('drop_relation', auto_begin=False) -%}
+    drop {{ relation.type }} if exists {{ relation }}
+  {%- endcall %}
+{% endmacro %}
+
+{% macro rename_view_relation(from_relation, to_relation) -%}
+  {{ return(adapter.dispatch('rename_view_relation', 'dbt')(from_relation, to_relation)) }}
 {% endmacro %}
 
+{% macro cratedb__rename_view_relation(from_relation, to_relation) -%}
+    {% call statement('get_view_definition', fetch_result=True, auto_begin=False) %}
+        SELECT view_definition
+        FROM information_schema.views
+        WHERE table_schema = '{{from_relation.schema}}'
+        AND table_name = '{{from_relation.name}}' limit 1;
+    {%- endcall %}
+    {% set result = load_result('get_view_definition') -%}
+
+    {% if result['data'] != [] %}
+        {% set view_definition = result["data"][0][0] -%}
+
+        {% call statement('drop_view') -%}
+            drop view if exists {{ from_relation }};
+        {% endcall %}
+
+        {% call statement('create_view', fetch_result=True, auto_begin=False) -%}
+            {{adapter.dispatch('create_view_as', 'dbt')(to_relation, view_definition)}}
+        {% endcall %}
+        {% set create_view_result = load_result('create_view') -%}
+        {{return(result)}}
+    {% endif %}
+
+    {{return("")}}
+{% endmacro %}
```

### Comparing `dbt-cratedb-1.0.3.0/dbt/include/cratedbadapter/macros/catalog.sql` & `dbt-cratedb-1.5.2/dbt/include/cratedb/macros/catalog.sql`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% macro cratedbadapter__alter_column_type(relation, column_name, new_column_type) -%}
+{% macro cratedb__alter_column_type(relation, column_name, new_column_type) -%}
   {#
     1. Create a new column (w/ temp name and correct type)
     2. Copy data over to it
     3. XXX Drop the existing column (cascade!) XXX
     4. Rename the new column to existing column
   #}
   {%- set tmp_column = column_name + "__dbt_alter" -%}
@@ -18,48 +18,55 @@
 
 {% macro default__drop_schema(relation) -%}
   {%- call statement('drop_schema') -%}
     commit;
   {% endcall %}
 {% endmacro %}
 
-{% macro cratedbadapter__get_catalog(information_schema, schemas) -%}
+{% macro cratedb__get_catalog(information_schema, schemas) -%}
 
   {%- call statement('catalog', fetch_result=True) -%}
+    {% set database = information_schema.database %}
+    {{ adapter.verify_database(database) }}
 
     select
-        sch.nspname as table_schema,
-        tbl.relname as table_name,
-        case tbl.relkind
-            when 'v' then 'VIEW'
-            else 'BASE TABLE'
-        end as table_type,
-        tbl_desc.description as table_comment,
-        col.attname as column_name,
-        col.attnum as column_index,
-        pg_catalog.format_type(col.atttypid, col.atttypmod) as column_type,
-        col_desc.description as column_comment,
-        pg_get_userbyid(tbl.relowner) as table_owner
+    '{{ database }}' as table_database
+    sch.nspname as table_schema,
+    tbl.relname as table_name,
+    case tbl.relkind
+        when 'v' then 'VIEW'
+        else 'BASE TABLE'
+    end as table_type,
+    tbl_desc.description as table_comment,
+    col.attname as column_name,
+    col.attnum as column_index,
+    pg_catalog.format_type(col.atttypid, col.atttypmod) as column_type,
+    col_desc.description as column_comment,
+    pg_get_userbyid(tbl.relowner) as table_owner
 
     from pg_catalog.pg_namespace sch
     join pg_catalog.pg_class tbl on tbl.relnamespace = sch.oid
     join pg_catalog.pg_attribute col on col.attrelid = tbl.oid
     left outer join pg_catalog.pg_description tbl_desc on (tbl_desc.objoid = tbl.oid and tbl_desc.objsubid = 0)
     left outer join pg_catalog.pg_description col_desc on (col_desc.objoid = tbl.oid and col_desc.objsubid = col.attnum)
 
     where (
         {%- for schema in schemas -%}
           upper(sch.nspname) = upper('{{ schema }}'){%- if not loop.last %} or {% endif -%}
         {%- endfor -%}
       )
-      and tbl.relpersistence = 'p'
-      and tbl.relkind in ('r', 'v', 'f', 'p')
-      and col.attnum > 0
-      and not col.attisdropped
-      order by sch.nspname, tbl.relname, col.attnum
+      and tbl.relpersistence = 'p' -- [p]ermanent table. Other values are [u]nlogged table, [t]emporary table
+      and tbl.relkind in ('r', 'v', 'f', 'p') -- o[r]dinary table, [v]iew, [f]oreign table, [p]artitioned table. Other values are [i]ndex, [S]equence, [c]omposite type, [t]OAST table, [m]aterialized view
+      and col.attnum > 0 -- negative numbers are used for system columns such as oid
+      and not col.attisdropped -- column as not been dropped
+
+    order by
+        sch.nspname,
+        tbl.relname,
+        col.attnum
 
   {%- endcall -%}
 
   {{ return(load_result('catalog').table) }}
 
 {%- endmacro %}
```

