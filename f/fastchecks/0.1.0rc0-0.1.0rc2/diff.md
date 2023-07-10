# Comparing `tmp/fastchecks-0.1.0rc0.tar.gz` & `tmp/fastchecks-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.1.0rc0.tar", max compression
+gzip compressed data, was "fastchecks-0.1.0rc2.tar", max compression
```

## Comparing `fastchecks-0.1.0rc0.tar` & `fastchecks-0.1.0rc2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      457 2023-07-09 17:17:25.642629 fastchecks-0.1.0rc0/README.md
--rw-r--r--   0        0        0      707 2023-07-09 17:17:25.642969 fastchecks-0.1.0rc0/fastchecks/__init__.py
--rw-r--r--   0        0        0     4681 2023-07-09 17:17:25.643240 fastchecks-0.1.0rc0/fastchecks/check.py
--rw-r--r--   0        0        0     2067 2023-07-09 17:17:25.643588 fastchecks-0.1.0rc0/fastchecks/cli.py
--rw-r--r--   0        0        0     2754 2023-07-09 17:17:25.643960 fastchecks-0.1.0rc0/fastchecks/conf.py
--rw-r--r--   0        0        0     5228 2023-07-09 17:17:25.644201 fastchecks-0.1.0rc0/fastchecks/runner.py
--rw-r--r--   0        0        0     2048 2023-07-09 17:17:25.644600 fastchecks-0.1.0rc0/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     4584 2023-07-09 17:17:25.644821 fastchecks-0.1.0rc0/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      526 2023-07-09 17:17:25.645153 fastchecks-0.1.0rc0/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc0/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     5820 2023-07-09 17:17:25.645626 fastchecks-0.1.0rc0/fastchecks/types.py
--rw-r--r--   0        0        0     4261 2023-07-09 17:17:25.645812 fastchecks-0.1.0rc0/fastchecks/util.py
--rw-r--r--   0        0        0     1463 2023-07-09 17:17:25.702192 fastchecks-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1675 2023-07-10 18:11:32.675864 fastchecks-0.1.0rc2/README.md
+-rw-r--r--   0        0        0      707 2023-07-09 17:17:25.642969 fastchecks-0.1.0rc2/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4683 2023-07-10 18:11:32.676130 fastchecks-0.1.0rc2/fastchecks/check.py
+-rw-r--r--   0        0        0     9302 2023-07-10 18:11:32.676380 fastchecks-0.1.0rc2/fastchecks/cli.py
+-rw-r--r--   0        0        0     3075 2023-07-10 18:11:32.676609 fastchecks-0.1.0rc2/fastchecks/conf.py
+-rw-r--r--   0        0        0      311 2023-07-10 18:11:32.676793 fastchecks-0.1.0rc2/fastchecks/meta.py
+-rw-r--r--   0        0        0     5661 2023-07-10 18:11:32.677045 fastchecks-0.1.0rc2/fastchecks/runner.py
+-rw-r--r--   0        0        0     2328 2023-07-10 18:11:32.677294 fastchecks-0.1.0rc2/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     5114 2023-07-10 18:11:32.677569 fastchecks-0.1.0rc2/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      526 2023-07-09 17:17:25.645153 fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-10 18:11:32.677815 fastchecks-0.1.0rc2/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc2/fastchecks/util.py
+-rw-r--r--   0        0        0     3530 2023-07-10 18:11:32.678274 fastchecks-0.1.0rc2/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1860 2023-07-10 18:11:32.724497 fastchecks-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc2/PKG-INFO
```

### Comparing `fastchecks-0.1.0rc0/fastchecks/__init__.py` & `fastchecks-0.1.0rc2/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc0/fastchecks/check.py` & `fastchecks-0.1.0rc2/fastchecks/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-import re
+import re2
 import aiohttp
 
 from fastchecks import conf
 from fastchecks.types import CheckResult, WebsiteCheck
 from fastchecks.util import (
     get_utcnow,
     get_utcnow_time_difference_seconds,
@@ -108,15 +108,15 @@
     * If regex search can limited to a line, we could use use response.content.readline() instead of response.text().
     * The text body searched is raw HTML (in most cases), not the HTML's text. If we want to search the text of the HTML (or other text-based format) only, we would need a corresponding parser.
     """
     if is_likely_text_based_body(response) and is_content_length_less_than(
         response, length=conf.TOO_BIG_CONTENT_LENGTH_KB, allow_none_content_length=True
     ):
         content = await response.text()
-        match_opt = re.search(regex, content)
+        match_opt = re2.search(regex, content)
 
         if match_opt:
             return match_opt[0]
         else:
             return False
     else:
         logging.warning(
```

### Comparing `fastchecks-0.1.0rc0/fastchecks/conf.py` & `fastchecks-0.1.0rc2/fastchecks/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 from typing import Callable, TypeVar
-from fastchecks import require
-
+from fastchecks import vutil
 
 _CONVERSION_OUTPUT = TypeVar("_CONVERSION_OUTPUT")
 
 
 def get_typed_envar(
     envar_name: str, default: _CONVERSION_OUTPUT, conversion: Callable[[str], _CONVERSION_OUTPUT]
 ) -> _CONVERSION_OUTPUT:
@@ -36,45 +35,51 @@
     "FC_DEFAULT_REQ_TIMEOUT_SECONDS", default=10.0, conversion=lambda x: float(x)
 )
 
 MIN_INTERVAL_SECONDS: int = get_typed_envar("FC_MIN_INTERVAL_SECONDS", default=5, conversion=lambda x: int(x))
 
 MAX_INTERVAL_SECONDS: int = get_typed_envar("FC_MAX_INTERVAL_SECONDS", default=300, conversion=lambda x: int(x))
 
-DEFAULT_CHECK_INTERVAL_SECONDS: int = get_typed_envar(
-    "FC_DEFAULT_CHECK_INTERVAL_SECONDS", default=180, conversion=lambda x: int(x)
-)
 
+def validated_parsed_interval(interval_seconds: str) -> int:
+    return validated_interval(int(interval_seconds))
 
-def validate_interval(interval_seconds: int) -> int:
-    """
-    Validate the given interval, and return it if it is valid, otherwise raise ValueError.
-    """
-    require(
-        MIN_INTERVAL_SECONDS <= interval_seconds <= MAX_INTERVAL_SECONDS,
-        f"Interval {interval_seconds} must be between min ({MIN_INTERVAL_SECONDS}) and max ({MAX_INTERVAL_SECONDS})",
-    )
-    return interval_seconds
+
+def validated_interval(interval_seconds: int, name: str = "interval") -> int:
+    return vutil.validated_in_range(name, interval_seconds, MIN_INTERVAL_SECONDS, MAX_INTERVAL_SECONDS)
 
 
-validate_interval(DEFAULT_CHECK_INTERVAL_SECONDS)
+def validated_interval_accepting_none(interval_seconds: int | None, name: str = "interval") -> int | None:
+    if interval_seconds is None:
+        return None
+    else:
+        return vutil.validated_in_range(name, interval_seconds, MIN_INTERVAL_SECONDS, MAX_INTERVAL_SECONDS)
+
+
+DEFAULT_CHECK_INTERVAL_SECONDS: int = validated_interval(
+    get_typed_envar("FC_DEFAULT_CHECK_INTERVAL_SECONDS", default=180, conversion=lambda x: int(x)),
+    name="FC_DEFAULT_CHECK_INTERVAL_SECONDS",
+)
 
 
 # -----------------------------------------------------------------------------
 
 TOO_BIG_CONTENT_LENGTH_KB = get_typed_envar("FC_TOO_BIG_CONTENT_LENGTH_KB", default=100000, conversion=lambda x: int(x))
 """
 Limit value (in _kilo_ bytes, not kibi bytes) to consider a response's content length as too big to be read in memory.
 
 For reference, the size of https://python.org is, as of 2023-07-06, 49943 bytes.
 """
 
 # -----------------------------------------------------------------------------
 
-_POSTGRES_CONNINFO: str | None = os.environ.get("FC_POSTGRES_CONNINFO")
+_POSTGRES_CONNINFO_ENVAR_NAME = "FC_POSTGRES_CONNINFO"
+
+_POSTGRES_CONNINFO: str | None = os.environ.get(_POSTGRES_CONNINFO_ENVAR_NAME)
 
 
 def get_postgres_conninfo() -> str:
     """
-    Return the Postgres local connection string, or raise ValueError if the environment variable is not set.
+    Return the Postgres conninfo envar value, or raise ValueError if the environment variable is not set or invalid.
     """
-    return read_envar_value("_POSTGRES_CONNINFO", _POSTGRES_CONNINFO)
+    ret = read_envar_value(_POSTGRES_CONNINFO_ENVAR_NAME, _POSTGRES_CONNINFO)
+    return vutil.validated_postgres_conninfo(ret)
```

### Comparing `fastchecks-0.1.0rc0/fastchecks/runner.py` & `fastchecks-0.1.0rc2/fastchecks/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from typing import AsyncIterator
 
 import aiohttp
 from apscheduler.schedulers.async_ import AsyncScheduler
 from apscheduler.triggers.interval import IntervalTrigger
 
-from fastchecks import conf, require, util
+from fastchecks import conf, require, util, vutil
 from fastchecks.check import check_website
 from fastchecks.sockets import CheckResultSocket, WebsiteCheckSocket
 from fastchecks.sockets.postgres import CheckResultSocketPostgres, WebsiteCheckSocketPostgres
 from fastchecks.types import CheckResult, WebsiteCheck, WebsiteCheckScheduled
 
 # -----------------------------------------------------------------------------
 
@@ -35,37 +35,46 @@
 
         self._aiohttp_session = session
         self.checks = checks
         self.results = results
         self.default_interval_seconds = (
             conf.DEFAULT_CHECK_INTERVAL_SECONDS
             if default_interval_seconds is None
-            else conf.validate_interval(default_interval_seconds)
+            else conf.validated_interval(default_interval_seconds)
         )
         """Default interval for website checks that don't specify it"""
 
+    # -----------------------------------------------------------------------------
+
+    @classmethod
+    def init_with_postgres(cls, postgres_conninfo: str, **kwargs) -> "ChecksRunnerContext":
+        vutil.validated_postgres_conninfo(postgres_conninfo)
+
+        return cls(
+            session=aiohttp.ClientSession(),
+            checks=WebsiteCheckSocketPostgres(postgres_conninfo),
+            results=CheckResultSocketPostgres(postgres_conninfo),
+            **kwargs,
+        )
+
+    # -----------------------------------------------------------------------------
+
     async def __aenter__(self) -> "ChecksRunnerContext":
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await asyncio.gather(self._aiohttp_session.close(), self.checks.close(), self.results.close())
 
     async def close(self) -> None:
         await self.__aexit__(None, None, None)
 
     # -----------------------------------------------------------------------------
 
-    @classmethod
-    def init_with_postgres(cls, postgres_conninfo: str, **kwargs) -> "ChecksRunnerContext":
-        return cls(
-            session=aiohttp.ClientSession(),
-            checks=WebsiteCheckSocketPostgres(postgres_conninfo),
-            results=CheckResultSocketPostgres(postgres_conninfo),
-            **kwargs,
-        )
+    def get_interval_seconds(self, check: WebsiteCheckScheduled) -> int:
+        return self.default_interval_seconds if check.interval_seconds is None else check.interval_seconds
 
     # -----------------------------------------------------------------------------
 
     async def check_only(self, check: WebsiteCheck) -> CheckResult:
         """Check website without saving into results data storage."""
         ret = await check_website(self._aiohttp_session, check)
         logging.debug(ret)
@@ -73,32 +82,29 @@
 
     async def check_n_write(self, check: WebsiteCheck) -> CheckResult:
         """Check website and save into results data storage."""
         ret = await self.check_only(check)
         await self.results.write(ret)
         return ret
 
-    async def check_once_all_websites_n_write(self) -> AsyncIterator[CheckResult]:
+    async def check_all_once_n_write(self) -> AsyncIterator[CheckResult]:
         async for check in self.checks.read_n(util.PRACTICAL_MAX_INT):
             result = await self.check_only(check)
             await self.results.write(result)
             yield result
 
     # -----------------------------------------------------------------------------
 
-    def _get_interval_seconds(self, check: WebsiteCheckScheduled) -> int:
-        return self.default_interval_seconds if check.interval_seconds is None else check.interval_seconds
-
     async def _add_check_to_scheduler(self, scheduler: AsyncScheduler, check: WebsiteCheckScheduled) -> AsyncScheduler:
         fun = self.check_n_write
 
         # Note: we can later retrieve scheduled checks by their url (with `AsyncScheduler.get_schedule``)
         # MAYBE (2023-07-09; future idea): tag the check with the url's domain, so later we can filter on them
         await scheduler.add_schedule(
-            fun, trigger=IntervalTrigger(seconds=self._get_interval_seconds(check)), id=check.url, args=[check]
+            fun, trigger=IntervalTrigger(seconds=self.get_interval_seconds(check)), id=check.url, args=[check]
         )
 
         return scheduler
 
     async def _add_checks_to_scheduler(
         self, scheduler: AsyncScheduler, checks: AsyncIterator[WebsiteCheckScheduled]
     ) -> AsyncScheduler:
@@ -112,17 +118,20 @@
         Run all saved checks until stopped (e.g. with Ctrl+C) in the foreground.
         The interval for each check is taken from the check itself, or the default interval if not specified.
 
         If there are no checks yet, an error is raised.
         """
         try:
             async with AsyncScheduler() as scheduler:
+                default_interval_msg = f" -- with default interval: {self.default_interval_seconds}s"
+
                 async for check in await self.checks.read_all():
-                    logging.info(f"Adding check to scheduler: {check}")
                     await self._add_check_to_scheduler(scheduler, check)
+                    print(f"Adding check to scheduler: {check}{'' if check.interval_seconds else default_interval_msg}")
 
                 require(len(await scheduler.get_schedules()) != 0, "No checks to run. Add some checks first.")
 
+                print("\nRunning until stopped...")
                 await scheduler.run_until_stopped()
 
         except (KeyboardInterrupt, SystemExit):
             pass
```

### Comparing `fastchecks-0.1.0rc0/fastchecks/sockets/__init__.py` & `fastchecks-0.1.0rc2/fastchecks/sockets/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,15 +30,21 @@
 
         This is a sugar method that calls `read_n` with a practically infinite large number.
         Careful: Use this method only if the underlying storage can handle reading all checks (e.g., there not many written checks, which it's common).
         """
         return self.read_n(PRACTICAL_MAX_INT)
 
     @abstractmethod
-    async def delete(self, url: str) -> None:
+    async def delete(self, url: str) -> int:
+        """Return number of deleted checks, 0 (no actual deletion) or 1 (did delete)"""
+        ...
+
+    @abstractmethod
+    async def delete_all(self, confirm: bool) -> int:
+        """Return number of deleted checks. If the number is unknown, return a negative number like -1"""
         ...
 
     @abstractmethod
     async def close(self) -> None:
         ...
 
     async def __aenter__(self) -> "WebsiteCheckSocket":
```

### Comparing `fastchecks-0.1.0rc0/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.1.0rc2/fastchecks/sockets/postgres/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import AsyncIterator
 from pydantic import PositiveInt
 from fastchecks.types import CheckResult, WebsiteCheckScheduled, WebsiteCheck
 from fastchecks.sockets import CheckResultSocket, WebsiteCheckSocket
 from psycopg_pool import AsyncConnectionPool
 from psycopg.rows import namedtuple_row
 from psycopg import sql
@@ -18,15 +19,16 @@
         async with self.__pool.connection() as aconn:
             await aconn.execute(
                 """
             INSERT INTO WebsiteCheck
             (url, regex, interval_seconds)
             VALUES (%s, %s, %s)
             ON CONFLICT (url) DO UPDATE
-                SET regex = EXCLUDED.regex;
+                SET regex = EXCLUDED.regex,
+                    interval_seconds = EXCLUDED.interval_seconds;
             """,
                 (check.url, check.regex, check.interval_seconds),
             )
 
     async def read_n(self, n: PositiveInt) -> AsyncIterator[WebsiteCheckScheduled]:
         async with self.__pool.connection() as aconn:
             # We format the safe query in 2 steps (also below) to avoid false positives from bandit (B608:hardcoded_sql_expressions)
@@ -41,22 +43,35 @@
             acur.row_factory = namedtuple_row
             async for row in acur:
                 # without validation, because we trust the database -- its value were validated before
                 yield WebsiteCheckScheduled.with_check(
                     WebsiteCheck.without_validation(row.url, row.regex), row.interval_seconds
                 )
 
-    async def delete(self, url: str) -> None:
+    async def delete(self, url: str) -> int:
         async with self.__pool.connection() as aconn:
-            await aconn.execute(
+            cur = await aconn.execute(
                 """
             DELETE FROM WebsiteCheck
             WHERE url = %s;""",
                 (url,),
             )
+            return cur.rowcount
+
+    async def delete_all(self, confirm: bool) -> int:
+        if confirm:
+            async with self.__pool.connection() as aconn:
+                cur = await aconn.execute(
+                    """
+                TRUNCATE WebsiteCheck;"""
+                )
+                return cur.rowcount
+        else:
+            logging.warning("Not deleting all checks because confirm is False.")
+            return 0
 
     async def close(self) -> None:
         return await self.__pool.close()
 
 
 class CheckResultSocketPostgres(CheckResultSocket):
     def __init__(self, conninfo: str) -> None:
```

### Comparing `fastchecks-0.1.0rc0/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc0/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.1.0rc2/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc0/fastchecks/types.py` & `fastchecks-0.1.0rc2/fastchecks/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import datetime
 from pydantic import BaseModel
 
-from fastchecks.util import validate_regex, validate_url
+from fastchecks import util, vutil
 from fastchecks import conf, require
 
 
 # We use Pydantic classes for type safety and because they could be handy in the future for de/serialization.
 # See benchmarks with other alternatives (e.g. NamedTuple): https://janhendrikewers.uk/pydantic_vs_protobuf_vs_namedtuple_vs_dataclasses.html
 # Note that Pydantic V2 (released in 2023 June) promises a 5-50x speedup over V1: https://docs.pydantic.dev/2.0/blog/pydantic-v2-alpha/#headlines
 
+_MAX_REPR_LEN: int = 500
+
 
 class WebsiteCheck(BaseModel):
     url: str
     regex: str | None = None
 
     @classmethod
     def with_validation(cls, url: str, regex: str | None = None) -> "WebsiteCheck":
         """
         Validate the given URL and regex (if any), and return a WebsiteCheck instance.
 
         If the URL or regex are invalid, raise ValueError.
         """
-        validate_url(url)
-        if regex is not None:
-            validate_regex(regex)
-        return cls(url=url, regex=regex)
+        return cls(url=vutil.validated_web_url(url), regex=vutil.validated_regex_accepting_none(regex))
 
     @classmethod
     def without_validation(cls, url: str, regex: str | None = None) -> "WebsiteCheck":
         """
         Return a WebsiteCheck instance without validating the given URL and regex (if any).
 
         Only use this method if you are sure that the URL and regex are valid (e.g., they were validated before).
         """
         return cls(url=url, regex=regex)
 
+    def __repr__(self) -> str:
+        return util.shorten_str(super().__repr__(), max=_MAX_REPR_LEN)
+
+    def __str__(self) -> str:
+        return util.shorten_str(super().__repr__(), max=_MAX_REPR_LEN)
+
 
 class WebsiteCheckScheduled(WebsiteCheck):
     """
     WebsiteCheck with an schedule.
     """
 
     # url: str
     # regex: str | None = None
     interval_seconds: int | None
     """If None, later a system's default value will be used."""
 
     @classmethod
     def with_check(cls, check: WebsiteCheck, interval_seconds: int | None) -> "WebsiteCheckScheduled":
-        if interval_seconds is not None:
-            conf.validate_interval(interval_seconds)
-
-        return cls(url=check.url, regex=check.regex, interval_seconds=interval_seconds)
+        return cls(
+            url=check.url, regex=check.regex, interval_seconds=conf.validated_interval_accepting_none(interval_seconds)
+        )
 
 
 class CheckResult(BaseModel):
     #
     check: WebsiteCheck
     """The check that generated this result"""
     #
@@ -86,14 +90,20 @@
         Validate the input data.
         """
         super().__init__(**data)
 
         if self.check.regex is None:
             require(self.regex_match is None, "If there is no regex, regex_match MUST be None.")
 
+    def __repr__(self) -> str:
+        return util.shorten_str(super().__repr__(), max=_MAX_REPR_LEN)
+
+    def __str__(self) -> str:
+        return util.shorten_str(super().__repr__(), max=_MAX_REPR_LEN)
+
     def is_success(self) -> bool:
         """
         Return True if the check was successful (i.e. no error, response is OK, and expected regex wax matched if any).
         """
         return self.is_response_ok() and self.is_regex_validated()
 
     def is_response_ok(self) -> bool:
```

### Comparing `fastchecks-0.1.0rc0/fastchecks/util.py` & `fastchecks-0.1.0rc2/fastchecks/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import re
 from typing import AsyncIterator, TypeVar
 from urllib.parse import urlparse, urlunparse
 import sys
 import ctypes
 
 import aiohttp
 
@@ -20,37 +19,22 @@
 See:
 https://docs.python.org/2/library/sys.html#sys.maxsize
 https://stackoverflow.com/questions/855191/how-big-can-a-python-list-get#comment112727918_15739630
 https://stackoverflow.com/a/1406210/341320
 """
 
 
-def validate_url(url: str, raise_error: bool = True) -> str | None:
-    """
-    Validate given string is a valid URL.
+def str_pad(c: int, size: int = 3) -> str:
+    return str(c).zfill(size)
 
-    If the URL is valid, return its netloc (e.g. "www.example.com").
-    Else if raise_error is True, raise ValueError.
-    """
-    # See: https://snyk.io/blog/secure-python-url-validation/
 
-    ret: str | None
-    try:
-        result = urlparse(url)
-        ret = result.scheme and result.netloc
-    except:
-        ret = None
-
-    if ret:
-        return ret
-    elif raise_error:
-        raise ValueError(f"Invalid URL: {url}")
-    else:
-        # ret could have been (without exception) the empty string (which is also falsy), but we return None to avoid confusions
-        return None
+def shorten_str(x: str, max=100) -> str:
+    if len(x) > max:
+        x = x[:max] + "..."
+    return x
 
 
 def replace_url_last_segment(url: str, new_segment: str) -> str:
     """
     Example behavior (new_segment = "fastchecks"), urls:
     * "postgresql://localhost/postgres" -> "postgresql://localhost/fastchecks"
     * "postgresql://localhost/postgres?sslmode=require" -> "postgresql://localhost/fastchecks?sslmode=require"
@@ -64,30 +48,14 @@
     modified_url = urlunparse(
         (parsed_url.scheme, parsed_url.netloc, modified_path, parsed_url.params, parsed_url.query, parsed_url.fragment)
     )
 
     return modified_url
 
 
-def validate_regex(regex: str, raise_error: bool = True) -> re.Pattern | None:
-    """
-    Validate regex string: the regex must be compilable.
-
-    If the regex is valid, return its re.Pattern.
-    Else if raise_error is True, raise ValueError.
-    """
-    try:
-        return re.compile(regex)
-    except re.error:
-        if raise_error:
-            raise ValueError(f"Invalid regex (cannot compile it): {regex}")
-        else:
-            return None
-
-
 def get_utcnow() -> datetime.datetime:
     """
     Return the current UTC timestamp in seconds.
 
     Use this method to make sure you are always using a timestamp with same timezone (UTC).
     """
     return datetime.datetime.utcnow()
```

