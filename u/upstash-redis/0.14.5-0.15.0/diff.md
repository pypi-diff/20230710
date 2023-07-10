# Comparing `tmp/upstash_redis-0.14.5.tar.gz` & `tmp/upstash_redis-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.14.5.tar", max compression
+gzip compressed data, was "upstash_redis-0.15.0.tar", max compression
```

## Comparing `upstash_redis-0.14.5.tar` & `upstash_redis-0.15.0.tar`

### file list

```diff
@@ -1,23 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-07-04 06:35:23.850037 upstash_redis-0.14.5/LICENSE
--rw-r--r--   0        0        0     5266 2023-07-04 06:35:23.850037 upstash_redis-0.14.5/README.md
--rw-r--r--   0        0        0      500 2023-07-04 06:35:23.850037 upstash_redis-0.14.5/pyproject.toml
--rw-r--r--   0        0        0      146 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4638 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     4768 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/client.py
--rw-r--r--   0        0        0       77 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0       79 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    21043 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    71958 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    20072 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0      283 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/exception.py
--rw-r--r--   0        0        0     4563 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/http.py
--rw-r--r--   0        0        0      431 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0      752 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      174 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     8861 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 upstash_redis-0.14.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-10 09:39:40.872329 upstash_redis-0.15.0/LICENSE
+-rw-r--r--   0        0        0     4441 2023-07-10 09:39:40.872329 upstash_redis-0.15.0/README.md
+-rw-r--r--   0        0        0     1400 2023-07-10 09:39:40.872329 upstash_redis-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     5029 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     3427 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/client.py
+-rw-r--r--   0        0        0    61076 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/commands.py
+-rw-r--r--   0        0        0    37029 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/commands.pyi
+-rw-r--r--   0        0        0       40 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/errors.py
+-rw-r--r--   0        0        0     8723 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/format.py
+-rw-r--r--   0        0        0     4665 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/http.py
+-rw-r--r--   0        0        0        0 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/py.typed
+-rw-r--r--   0        0        0      552 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/typing.py
+-rw-r--r--   0        0        0     3449 2023-07-10 09:39:40.880329 upstash_redis-0.15.0/upstash_redis/utils.py
+-rw-r--r--   0        0        0     5707 1970-01-01 00:00:00.000000 upstash_redis-0.15.0/PKG-INFO
```

### Comparing `upstash_redis-0.14.5/LICENSE` & `upstash_redis-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.5/README.md` & `upstash_redis-0.15.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-# Upstash Redis - python edition
+# Upstash Redis Python SDK
 
-upstash-redis is a connectionless, HTTP-based Redis client for python, designed to be used in serverless and serverful environments such as:
+upstash-redis is a connectionless, HTTP-based Redis client for Python, designed to be used in serverless and serverful environments such as:
 - AWS Lambda
 - Vercel Serverless
 - Google Cloud Functions
 - and other environments where HTTP is preferred over TCP.
 
 Inspired by other Redis clients like [@upstash/redis](https://github.com/upstash/upstash-redis) and [redis-py](https://github.com/redis/redis-py),
-the goal of this SDK is to provide a simple way to use Redis in HTTP-based environments.
+the goal of this SDK is to provide a simple way to use Redis over the [Upstash REST API](https://docs.upstash.com/redis/features/restapi).
 
-The SDK is currently compatible with python 3.8 and above.
+The SDK is currently compatible with Python 3.8 and above.
 
 <!-- toc -->
 
-- [Upstash Redis - python edition](#upstash-redis---python-edition)
+- [Upstash Redis Python SDK](#upstash-redis-python-sdk)
 - [Quick Start](#quick-start)
   - [Install](#install)
-    - [PyPi](#pypi)
+    - [PyPI](#pypi)
   - [Usage](#usage)
     - [BITFIELD and BITFIELD\_RO](#bitfield-and-bitfield_ro)
     - [Custom commands](#custom-commands)
 - [Encoding](#encoding)
 - [Retry mechanism](#retry-mechanism)
-- [Formatting returns](#formatting-returns)
 - [Contributing](#contributing)
   - [Preparing the environment](#preparing-the-environment)
   - [Running tests](#running-tests)
 
 <!-- tocstop -->
 
 # Quick Start
 
 ## Install
 
-### PyPi
+### PyPI
 ```bash
 pip install upstash-redis
 ```
 
-
 ## Usage
 To be able to use upstash-redis, you need to create a database on [Upstash](https://console.upstash.com/)
 and grab `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` from the console.
 
 ```python
-# In this method, you can also give specific parameters for the Redis instance instance, such as rest_retries and so on
-
 # for sync client
 from upstash_redis import Redis
+
 redis = Redis(url="UPSTASH_REDIS_REST_URL", token="UPSTASH_REDIS_REST_TOKEN")
 
 # for async client
 from upstash_redis.asyncio import Redis
 
 redis = Redis(url="UPSTASH_REDIS_REST_URL", token="UPSTASH_REDIS_REST_TOKEN")
 ```
@@ -64,100 +61,76 @@
 redis = Redis.from_env()
 
 # for async use
 from upstash_redis.asyncio import Redis
 redis = Redis.from_env()
 ```
 
-
 If you are in a serverless environment that allows it, it's recommended to initialise the client outside the request handler
 to be reused while your function is still hot.
 
 Running commands might look like this:
 
 ```python
 from upstash_redis import Redis
+
 redis = Redis.from_env()
 
 def main():
   redis.set("a", "b")
   print(redis.get("a"))
 
 # or for async context:
 
 from upstash_redis.asyncio import Redis
+
 redis = Redis.from_env()
 
-async def main():
-  async with redis:
-    await redis.set("a", "b")
-    print(await redis.get("a"))
+async def main():  
+  await redis.set("a", "b")
+  print(await redis.get("a"))
 ```
 
 ### BITFIELD and BITFIELD_RO
 One particular case is represented by these two chained commands, which are available as functions that return an instance of 
 the `BITFIELD` and, respectively, `BITFIELD_RO` classes. Use the `execute` function to run the commands.
 
 ```python
-    redis.bitfield("test_key")
-    .incrby(encoding="i8", offset=100, increment=100)
-    .overflow("SAT")
-    .incrby(encoding="i8", offset=100, increment=100)
-    .execute()
-
-    redis.bitfield_ro("test_key_2")
-    .get(encoding="u8", offset=0)
-    .get(encoding="u8", offset="#1")
-    .execute()
+redis.bitfield("test_key") \
+  .incrby(encoding="i8", offset=100, increment=100) \
+  .overflow("SAT") \
+  .incrby(encoding="i8", offset=100, increment=100) \
+  .execute()
+
+redis.bitfield_ro("test_key_2") \
+  .get(encoding="u8", offset=0) \
+  .get(encoding="u8", offset="#1") \
+  .execute()
 ```
 
-
 ### Custom commands
-If you want to run a command that hasn't been implemented, you can use the `run` function of your client instance
-and pass the command as `list`
+If you want to run a command that hasn't been implemented, you can use the `execute` function of your client instance
+and pass the command as a `list`.
 
 ```python
-redis.run(command=["XLEN", "test_stream"])
+redis.execute(command=["XLEN", "test_stream"])
 ```
 
-If you want to have more control over your session management or need to use multiple custom values, use
-the [sync_execute](./upstash_redis/http/execute.py) function directly.
-
-
-
 # Encoding
 Although Redis can store invalid JSON data, there might be problems with the deserialization.
 To avoid this, the Upstash REST proxy is capable of encoding the data as base64 on the server and then sending it to the client to be
 decoded. 
 
 For very large data, this can add a few milliseconds in latency. So, if you're sure that your data is valid JSON, you can set
-`rest_encoding` to `False`.
-
+`rest_encoding` to `None`.
 
 # Retry mechanism
 upstash-redis has a fallback mechanism in case of network or API issues. By default, if a request fails it'll retry once, 3 seconds 
 after the error. If you want to customize that, set `rest_retries` and `rest_retry_interval` (in seconds).
 
-
-# Formatting returns
-The SDK relies on the Upstash REST proxy, which returns the `RESP2` responses of the given commands.
-By default, we apply formatting to some of them to provide a better developer experience.
-If you want the commands to output the raw return, set `format_return` to `False`.
-
-You can also opt out of individual commands:
-
-```python
-redis.format_return = False
-
-print(redis.copy(source="source_string", destination="destination_string"))
-
-redis.format_return = True
-```
-
-
 # Contributing
 
 ## Preparing the environment
 This project uses [Poetry](https://python-poetry.org) for packaging and dependency management. Make sure you are able to create the poetry shell with relevant dependencies.
 
 You will also need a database on [Upstash](https://console.upstash.com/).
```

### Comparing `upstash_redis-0.14.5/upstash_redis/asyncio/client.py` & `upstash_redis-0.15.0/upstash_redis/asyncio/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,152 @@
 from os import environ
-from typing import Any, List, Type, Union
+from typing import Any, List, Literal, Optional, Type, Union
 
 from aiohttp import ClientSession
 
-from upstash_redis.commands.async_commands import AsyncCommands
-from upstash_redis.config import (
-    ALLOW_TELEMETRY,
-    FORMAT_RETURN,
-    REST_ENCODING,
-    REST_RETRIES,
-    REST_RETRY_INTERVAL,
-)
+from upstash_redis.commands import AsyncCommands
+from upstash_redis.format import FORMATTERS
 from upstash_redis.http import async_execute, make_headers
-from upstash_redis.schema.http import RESTEncoding, RESTResult
-from upstash_redis.utils.format import FormattedResponse
+from upstash_redis.typing import RESTResultT
 
 
-class Redis(FormattedResponse, AsyncCommands):
+class Redis(AsyncCommands):
     def __init__(
         self,
         url: str,
         token: str,
-        rest_encoding: RESTEncoding = REST_ENCODING,
-        rest_retries: int = REST_RETRIES,
-        rest_retry_interval: int = REST_RETRY_INTERVAL,  # Seconds.
-        format_return: bool = FORMAT_RETURN,
-        allow_telemetry: bool = ALLOW_TELEMETRY,
+        rest_encoding: Union[Literal["base64"], None] = "base64",
+        rest_retries: int = 1,
+        rest_retry_interval: float = 3,  # Seconds.
+        allow_telemetry: bool = True,
     ):
         """
         :param url: UPSTASH_REDIS_REST_URL in the console
         :param token: UPSTASH_REDIS_REST_TOKEN in the console
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
-        :param format_return: whether the raw, RESP2 result or a formatted response will be returned
         :param allow_telemetry: whether anonymous telemetry can be collected
         """
 
-        self.url = url
-        self.token = token
+        self._url = url
+        self._token = token
 
-        self.allow_telemetry = allow_telemetry
+        self._allow_telemetry = allow_telemetry
 
-        self.format_return = format_return
-
-        self.rest_encoding = rest_encoding
-        self.rest_retries = rest_retries
-        self.rest_retry_interval = rest_retry_interval
-
-        self.FORMATTERS = self.__class__.FORMATTERS
+        self._rest_encoding = rest_encoding
+        self._rest_retries = rest_retries
+        self._rest_retry_interval = rest_retry_interval
 
         self._headers = make_headers(token, rest_encoding, allow_telemetry)
+        self._context_manager: Optional[_SessionContextManager] = None
 
     @classmethod
     def from_env(
         cls,
-        rest_encoding: RESTEncoding = REST_ENCODING,
-        rest_retries: int = REST_RETRIES,
-        rest_retry_interval: int = REST_RETRY_INTERVAL,
-        format_return: bool = FORMAT_RETURN,
-        allow_telemetry: bool = ALLOW_TELEMETRY,
+        rest_encoding: Union[Literal["base64"], None] = "base64",
+        rest_retries: int = 1,
+        rest_retry_interval: float = 3,
+        allow_telemetry: bool = True,
     ):
         """
         Load the credentials from environment.
 
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
-        :param format_return: whether the raw, RESP2 result or a formatted response will be returned
         :param allow_telemetry: whether anonymous telemetry can be collected
         """
 
         return cls(
             environ["UPSTASH_REDIS_REST_URL"],
             environ["UPSTASH_REDIS_REST_TOKEN"],
             rest_encoding,
             rest_retries,
             rest_retry_interval,
-            format_return,
             allow_telemetry,
         )
 
-    async def __aenter__(self) -> ClientSession:
-        """
-        Enter the async context.
-        """
-
-        self._session: ClientSession = ClientSession()
-        # It needs to return the session object because it will be used in "async with" statements.
-        return self._session
+    async def __aenter__(self) -> "Redis":
+        self._context_manager = _SessionContextManager(
+            ClientSession(), close_session=False
+        )
+        return self
 
     async def __aexit__(
         self,
         exc_type: Union[Type[BaseException], None],
         exc_val: Union[BaseException, None],
         exc_tb: Any,
     ) -> None:
-        """
-        Exit the async context.
-        """
+        await self.close()
 
-        await self._session.close()
-
-    async def run(self, command: List) -> RESTResult:
+    async def close(self) -> None:
         """
-        Specify the http options and execute the command.
+        Closes the resources associated with the client.
         """
-
-        res = await async_execute(
-            session=self._session,
-            url=self.url,
-            headers=self._headers,
-            encoding=self.rest_encoding,
-            retries=self.rest_retries,
-            retry_interval=self.rest_retry_interval,
-            command=command,
-        )
+        if self._context_manager:
+            await self._context_manager.close_session()
+            self._context_manager = None
+
+    async def execute(self, command: List) -> RESTResultT:
+        """
+        Executes the given command.
+        """
+        context_manager = self._context_manager
+        if not context_manager:
+            context_manager = _SessionContextManager(
+                ClientSession(), close_session=True
+            )
+
+        async with context_manager:
+            res = await async_execute(
+                session=context_manager.session,
+                url=self._url,
+                headers=self._headers,
+                encoding=self._rest_encoding,
+                retries=self._rest_retries,
+                retry_interval=self._rest_retry_interval,
+                command=command,
+            )
 
         main_command = command[0]
-        if len(command) > 1 and (main_command == "PUBSUB" or main_command == "SCRIPT"):
+        if len(command) > 1 and main_command == "SCRIPT":
             main_command = f"{main_command} {command[1]}"
 
-        if (
-            self.format_return
-            or main_command == "HSCAN"
-            or main_command == "SMEMBERS"
-            or main_command == "SDIFF"
-            or main_command == "SINTER"
-            or main_command == "SSCAN"
-            or main_command == "SUNION"
-            or main_command == "ZSCAN"
-        ) and (main_command in self.FORMATTERS):
-            return self.FORMATTERS[main_command](res, command)
+        if main_command in FORMATTERS:
+            return FORMATTERS[main_command](res, command)
 
         return res
+
+
+class _SessionContextManager:
+    """
+    Allows a session to be re-used in multiple async with
+    blocks when the `close_session` is False.
+
+    Main use case is to re-use sessions in multiple HTTP
+    requests when the client is used in an async with block.
+
+    The logic around the places in which we use this class is
+    required so that the same client can be re-used even in
+    different event loops, one after another.
+    """
+
+    def __init__(self, session: ClientSession, close_session: bool) -> None:
+        self.session = session
+        self._close_session = close_session
+
+    async def close_session(self) -> None:
+        await self.session.close()
+
+    async def __aenter__(self) -> ClientSession:
+        return self.session
+
+    async def __aexit__(
+        self,
+        exc_type: Union[Type[BaseException], None],
+        exc_val: Union[BaseException, None],
+        exc_tb: Any,
+    ) -> None:
+        if self._close_session:
+            await self.close_session()
```

### Comparing `upstash_redis-0.14.5/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.15.0/upstash_redis/commands.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,271 +1,692 @@
-from upstash_redis.schema.commands.parameters import (
-    BitFieldOffset,
-    GeoMember,
-    FloatMinMax,
-)
+from typing import Any, Dict, List, Literal, Optional, Set, Tuple, Union
 
-from typing import Any, Iterable, Optional, Set, Tuple, Union, List, Literal, Dict
+from upstash_redis.typing import FloatMinMaxT, GeoSearchResult
+
+class Commands:
+    def bitcount(
+        self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
+    ) -> int: ...
+    def bitfield(self, key: str) -> "BitFieldCommands": ...
+    def bitfield_ro(self, key: str) -> "BitFieldROCommands": ...
+    def bitop(
+        self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *keys: str
+    ) -> int: ...
+    def bitpos(
+        self,
+        key: str,
+        bit: Literal[0, 1],
+        start: Union[int, None] = None,
+        end: Union[int, None] = None,
+    ) -> int: ...
+    def getbit(self, key: str, offset: int) -> Literal[0, 1]: ...
+    def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int: ...
+    def ping(self, message: Union[str, None] = None) -> str: ...
+    def echo(self, message: str) -> str: ...
+    def copy(self, source: str, destination: str, replace: bool = False) -> bool: ...
+    def delete(self, *keys: str) -> int: ...
+    def exists(self, *keys: str) -> int: ...
+    def expire(self, key: str, seconds: int) -> bool: ...
+    def expireat(self, key: str, unix_time_seconds: int) -> bool: ...
+    def keys(self, pattern: str) -> List[str]: ...
+    def persist(self, key: str) -> bool: ...
+    def pexpire(self, key: str, milliseconds: int) -> bool: ...
+    def pexpireat(self, key: str, unix_time_milliseconds: int) -> bool: ...
+    def pttl(self, key: str) -> int: ...
+    def randomkey(self) -> Union[str, None]: ...
+    def rename(self, key: str, newkey: str) -> bool: ...
+    def renamenx(self, key: str, newkey: str) -> bool: ...
+    def scan(
+        self,
+        cursor: int,
+        match: Union[str, None] = None,
+        count: Union[int, None] = None,
+        type: Union[str, None] = None,
+    ) -> Tuple[int, List[str]]: ...
+    def touch(self, *keys: str) -> int: ...
+    def ttl(self, key: str) -> int: ...
+    def type(self, key: str) -> Union[str, None]: ...
+    def unlink(self, *keys: str) -> int: ...
+    def geoadd(
+        self,
+        key: str,
+        *members: Tuple[float, float, str],
+        nx: bool = False,
+        xx: bool = False,
+        ch: bool = False,
+    ) -> int: ...
+    def geodist(
+        self,
+        key: str,
+        member1: str,
+        member2: str,
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+    ) -> Union[float, None]: ...
+    def geohash(self, key: str, *members: str) -> List[Union[str, None]]: ...
+    def geopos(
+        self, key: str, *members: str
+    ) -> List[Union[Tuple[float, float], None]]: ...
+    def georadius(
+        self,
+        key: str,
+        longitude: float,
+        latitude: float,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+        store: Union[str, None] = None,
+        storedist: Union[str, None] = None,
+    ) -> Union[List[Union[str, GeoSearchResult]], int]: ...
+    def georadius_ro(
+        self,
+        key: str,
+        longitude: float,
+        latitude: float,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> List[Union[str, GeoSearchResult]]: ...
+    def georadiusbymember(
+        self,
+        key: str,
+        member: str,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+        store: Union[str, None] = None,
+        storedist: Union[str, None] = None,
+    ) -> Union[List[Union[str, GeoSearchResult]], int]: ...
+    def georadiusbymember_ro(
+        self,
+        key: str,
+        member: str,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> List[Union[str, GeoSearchResult]]: ...
+    def geosearch(
+        self,
+        key: str,
+        unit: Literal["M", "KM", "FT", "MI"],
+        member: Union[str, None] = None,
+        longitude: Union[float, None] = None,
+        latitude: Union[float, None] = None,
+        radius: Union[float, None] = None,
+        width: Union[float, None] = None,
+        height: Union[float, None] = None,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+        count: Union[int, None] = None,
+        any: bool = False,
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+    ) -> List[Union[str, GeoSearchResult]]: ...
+    def geosearchstore(
+        self,
+        destination: str,
+        source: str,
+        member: Union[str, None] = None,
+        longitude: Union[float, None] = None,
+        latitude: Union[float, None] = None,
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+        radius: Union[float, None] = None,
+        width: Union[float, None] = None,
+        height: Union[float, None] = None,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+        count: Union[int, None] = None,
+        any: bool = False,
+        storedist: bool = False,
+    ) -> int: ...
+    def hdel(self, key: str, *fields: str) -> int: ...
+    def hexists(self, key: str, field: str) -> bool: ...
+    def hget(self, key: str, field: str) -> Union[str, None]: ...
+    def hgetall(self, key: str) -> Dict[str, str]: ...
+    def hincrby(self, key: str, field: str, increment: int) -> int: ...
+    def hincrbyfloat(self, key: str, field: str, increment: float) -> float: ...
+    def hkeys(self, key: str) -> List[str]: ...
+    def hlen(self, key: str) -> int: ...
+    def hmget(self, key: str, *fields: str) -> List[Union[str, None]]: ...
+    def hmset(self, key: str, values: Dict[str, str]) -> bool: ...
+    def hrandfield(
+        self, key: str, count: Union[int, None] = None, withvalues: bool = False
+    ) -> Union[str, None, List[str], Dict[str, str]]: ...
+    def hscan(
+        self,
+        key: str,
+        cursor: int,
+        match: Union[str, None] = None,
+        count: Union[int, None] = None,
+    ) -> Tuple[int, Dict[str, str]]: ...
+    def hset(
+        self,
+        key: str,
+        field: Optional[str] = None,
+        value: Optional[str] = None,
+        values: Optional[Dict[str, str]] = None,
+    ) -> int: ...
+    def hsetnx(self, key: str, field: str, value: str) -> bool: ...
+    def hstrlen(self, key: str, field: str) -> int: ...
+    def hvals(self, key: str) -> List[str]: ...
+    def pfadd(self, key: str, *elements: Any) -> bool: ...
+    def pfcount(self, *keys: str) -> int: ...
+    def pfmerge(self, destkey: str, *sourcekeys: str) -> bool: ...
+    def lindex(self, key: str, index: int) -> Union[str, None]: ...
+    def linsert(
+        self,
+        key: str,
+        where: Literal["BEFORE", "AFTER"],
+        pivot: str,
+        element: str,
+    ) -> int: ...
+    def llen(self, key: str) -> int: ...
+    def lmove(
+        self,
+        source: str,
+        destination: str,
+        wherefrom: Literal["LEFT", "RIGHT"] = "LEFT",
+        whereto: Literal["LEFT", "RIGHT"] = "RIGHT",
+    ) -> Union[str, None]: ...
+    def lpop(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[str, List[str], None]: ...
+    def lpos(
+        self,
+        key: str,
+        element: str,
+        rank: Union[int, None] = None,
+        count: Union[int, None] = None,
+        maxlen: Union[int, None] = None,
+    ) -> Union[(Union[int, None]), List[int]]: ...
+    def lpush(self, key: str, *elements: str) -> int: ...
+    def lpushx(self, key: str, *elements: str) -> int: ...
+    def lrange(self, key: str, start: int, stop: int) -> List[str]: ...
+    def lrem(self, key: str, count: int, element: str) -> int: ...
+    def lset(self, key: str, index: int, element: str) -> bool: ...
+    def ltrim(self, key: str, start: int, stop: int) -> str: ...
+    def rpop(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[str, List[str], None]: ...
+    def rpoplpush(self, source: str, destination: str) -> Union[str, None]: ...
+    def rpush(self, key: str, *elements: str) -> int: ...
+    def rpushx(self, key: str, *elements: str) -> int: ...
+    def publish(self, channel: str, message: str) -> int: ...
+    def eval(
+        self,
+        script: str,
+        keys: Union[List[str], None] = None,
+        args: Union[List, None] = None,
+    ) -> Any: ...
+    def evalsha(
+        self,
+        sha1: str,
+        keys: Union[List[str], None] = None,
+        args: Union[List, None] = None,
+    ) -> Any: ...
+    def dbsize(self) -> int: ...
+    def flushall(
+        self, flush_type: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> bool: ...
+    def flushdb(
+        self, flush_type: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> bool: ...
+    def time(self) -> Tuple[int, int]: ...
+    def sadd(self, key: str, *members: str) -> int: ...
+    def scard(self, key: str) -> int: ...
+    def sdiff(self, *keys: str) -> Set[str]: ...
+    def sdiffstore(self, destination: str, *keys: str) -> int: ...
+    def sinter(self, *keys: str) -> Set[str]: ...
+    def sinterstore(self, destination: str, *keys: str) -> int: ...
+    def sismember(self, key: str, member: str) -> bool: ...
+    def smismember(self, key: str, *members: str) -> List[bool]: ...
+    def smembers(self, key: str) -> Set[str]: ...
+    def smove(self, source: str, destination: str, member: str) -> bool: ...
+    def spop(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[str, List[str], None]: ...
+    def srandmember(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[str, List[str], None]: ...
+    def srem(self, key: str, *members: str) -> int: ...
+    def sscan(
+        self,
+        key: str,
+        cursor: int = 0,
+        match: Union[str, None] = None,
+        count: Union[int, None] = None,
+    ) -> Tuple[int, List[str]]: ...
+    def sunion(self, *keys: str) -> Set[str]: ...
+    def sunionstore(self, destination: str, *keys: str) -> int: ...
+    def zadd(
+        self,
+        key: str,
+        scores: Dict[str, float],
+        nx: bool = False,
+        xx: bool = False,
+        gt: bool = False,
+        lt: bool = False,
+        ch: bool = False,
+        incr: bool = False,
+    ) -> Union[int, float, None]: ...
+    def zcard(self, key: str) -> int: ...
+    def zcount(self, key: str, min: FloatMinMaxT, max: FloatMinMaxT) -> int: ...
+    def zdiff(
+        self, keys: List[str], withscores: bool = False
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zdiffstore(self, destination: str, keys: List[str]) -> int: ...
+    def zincrby(self, key: str, increment: float, member: str) -> float: ...
+    def zinter(
+        self,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
+        withscores: bool = False,
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zinterstore(
+        self,
+        destination: str,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
+    ) -> int: ...
+    def zlexcount(self, key: str, min: str, max: str) -> int: ...
+    def zmscore(self, key: str, members: List[str]) -> List[Union[float, None]]: ...
+    def zpopmax(
+        self, key: str, count: Union[int, None] = None
+    ) -> List[Tuple[str, float]]: ...
+    def zpopmin(
+        self, key: str, count: Union[int, None] = None
+    ) -> List[Tuple[str, float]]: ...
+    def zrandmember(
+        self, key: str, count: Union[int, None] = None, withscores: bool = False
+    ) -> Union[str, None, List[str], List[Tuple[str, float]]]: ...
+    def zrange(
+        self,
+        key: str,
+        start: FloatMinMaxT,
+        stop: FloatMinMaxT,
+        sortby: Union[Literal["BYSCORE", "BYLEX"], None] = None,
+        rev: bool = False,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+        withscores: bool = False,
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zrangebylex(
+        self,
+        key: str,
+        min: str,
+        max: str,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> List[str]: ...
+    def zrangebyscore(
+        self,
+        key: str,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
+        withscores: bool = False,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zrangestore(
+        self,
+        dst: str,
+        src: str,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
+        sortby: Union[Literal["BYSCORE", "BYLEX"], None] = None,
+        rev: bool = False,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> int: ...
+    def zrank(self, key: str, member: str) -> Union[int, None]: ...
+    def zrem(self, key: str, *members: str) -> int: ...
+    def zremrangebylex(self, key: str, min: str, max: str) -> int: ...
+    def zremrangebyrank(self, key: str, start: int, stop: int) -> int: ...
+    def zremrangebyscore(
+        self, key: str, min: FloatMinMaxT, max: FloatMinMaxT
+    ) -> int: ...
+    def zrevrange(
+        self, key: str, start: int, stop: int, withscores: bool = False
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zrevrangebylex(
+        self,
+        key: str,
+        max: str,
+        min: str,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> List[str]: ...
+    def zrevrangebyscore(
+        self,
+        key: str,
+        max: FloatMinMaxT,
+        min: FloatMinMaxT,
+        withscores: bool = False,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zrevrank(self, key: str, member: str) -> Union[int, None]: ...
+    def zscan(
+        self,
+        key: str,
+        cursor: int,
+        match: Union[str, None] = None,
+        count: Union[int, None] = None,
+    ) -> Tuple[int, List[Tuple[str, float]]]: ...
+    def zscore(self, key: str, member: str) -> Union[float, None]: ...
+    def zunion(
+        self,
+        keys: List[str],
+        weights: Union[List[float], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
+        withscores: bool = False,
+    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    def zunionstore(
+        self,
+        destination: str,
+        keys: List[str],
+        weights: Union[List[float], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
+    ) -> int: ...
+    def append(self, key: str, value: str) -> int: ...
+    def decr(self, key: str) -> int: ...
+    def decrby(self, key: str, decrement: int) -> int: ...
+    def get(self, key: str) -> Union[str, None]: ...
+    def getdel(self, key: str) -> Union[str, None]: ...
+    def getex(
+        self,
+        key: str,
+        ex: Union[int, None] = None,
+        px: Union[int, None] = None,
+        exat: Union[int, None] = None,
+        pxat: Union[int, None] = None,
+        persist: Union[bool, None] = None,
+    ) -> Union[str, None]: ...
+    def getrange(self, key: str, start: int, end: int) -> str: ...
+    def getset(self, key: str, value: str) -> Union[str, None]: ...
+    def incr(self, key: str) -> int: ...
+    def incrby(self, key: str, increment: int) -> int: ...
+    def incrbyfloat(self, key: str, increment: float) -> float: ...
+    def mget(self, *keys: str) -> List[Union[str, None]]: ...
+    def mset(self, values: Dict[str, str]) -> Literal[True]: ...
+    def msetnx(self, values: Dict[str, str]) -> bool: ...
+    def psetex(self, key: str, milliseconds: int, value: str) -> Literal[True]: ...
+    def set(
+        self,
+        key: str,
+        value: Any,
+        nx: bool = False,
+        xx: bool = False,
+        get: bool = False,
+        ex: Union[int, None] = None,
+        px: Union[int, None] = None,
+        exat: Union[int, None] = None,
+        pxat: Union[int, None] = None,
+        keepttl: bool = False,
+    ) -> Union[str, None]: ...
+    def setex(self, key: str, seconds: int, value: str) -> Literal[True]: ...
+    def setnx(self, key: str, value: str) -> bool: ...
+    def setrange(self, key: str, offset: int, value: str) -> int: ...
+    def strlen(self, key: str) -> int: ...
+    def substr(self, key: str, start: int, end: int) -> str: ...
+    def script_exists(self, *sha1: str) -> List[bool]: ...
+    def script_flush(
+        self, flush_type: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> bool: ...
+    def script_load(self, script: str) -> str: ...
 
 class AsyncCommands:
     def __init__(self): ...
     async def bitcount(
         self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
     ) -> int: ...
-    def bitfield(self, key: str) -> "BitFieldCommands": ...
-    def bitfield_ro(self, key: str) -> "BitFieldRO": ...
+    def bitfield(self, key: str) -> "AsyncBitFieldCommands": ...
+    def bitfield_ro(self, key: str) -> "AsyncBitFieldROCommands": ...
     async def bitop(
-        self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *srckeys: str
+        self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *keys: str
     ) -> int: ...
     async def bitpos(
         self,
         key: str,
         bit: Literal[0, 1],
         start: Union[int, None] = None,
         end: Union[int, None] = None,
     ) -> int: ...
-    async def getbit(self, key: str, offset: int) -> int: ...
+    async def getbit(self, key: str, offset: int) -> Literal[0, 1]: ...
     async def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int: ...
     async def ping(self, message: Union[str, None] = None) -> str: ...
     async def echo(self, message: str) -> str: ...
     async def copy(
         self, source: str, destination: str, replace: bool = False
-    ) -> Union[Literal[1, 0], bool]: ...
+    ) -> bool: ...
     async def delete(self, *keys: str) -> int: ...
     async def exists(self, *keys: str) -> int: ...
-    async def expire(self, key: str, seconds: int) -> Union[Literal[1, 0], bool]: ...
-    async def expireat(
-        self, key: str, unix_time_seconds: int
-    ) -> Union[Literal[1, 0], bool]: ...
+    async def expire(self, key: str, seconds: int) -> bool: ...
+    async def expireat(self, key: str, unix_time_seconds: int) -> bool: ...
     async def keys(self, pattern: str) -> List[str]: ...
-    async def persist(self, key: str) -> Union[Literal[1, 0], bool]: ...
-    async def pexpire(
-        self, key: str, milliseconds: int
-    ) -> Union[Literal[1, 0], bool]: ...
-    async def pexpireat(
-        self, key: str, unix_time_milliseconds: int
-    ) -> Union[Literal[1, 0], bool]: ...
+    async def persist(self, key: str) -> bool: ...
+    async def pexpire(self, key: str, milliseconds: int) -> bool: ...
+    async def pexpireat(self, key: str, unix_time_milliseconds: int) -> bool: ...
     async def pttl(self, key: str) -> int: ...
     async def randomkey(self) -> Union[str, None]: ...
-    async def rename(self, key: str, newkey: str) -> str: ...
-    async def renamenx(self, key: str, newkey: str) -> Union[Literal[1, 0], bool]: ...
+    async def rename(self, key: str, newkey: str) -> bool: ...
+    async def renamenx(self, key: str, newkey: str) -> bool: ...
     async def scan(
         self,
         cursor: int,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
-        scan_type: Union[str, None] = None,
-    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]: ...
+        type: Union[str, None] = None,
+    ) -> Tuple[int, List[str]]: ...
     async def touch(self, *keys: str) -> int: ...
     async def ttl(self, key: str) -> int: ...
     async def type(self, key: str) -> Union[str, None]: ...
     async def unlink(self, *keys: str) -> int: ...
     async def geoadd(
         self,
         key: str,
-        *members: GeoMember,
+        *members: Tuple[float, float, str],
         nx: bool = False,
         xx: bool = False,
         ch: bool = False,
     ) -> int: ...
     async def geodist(
         self,
         key: str,
         member1: str,
         member2: str,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M",
-    ) -> Union[str, float, None]: ...
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+    ) -> Union[float, None]: ...
     async def geohash(self, key: str, *members: str) -> List[Union[str, None]]: ...
     async def geopos(
         self, key: str, *members: str
-    ) -> Union[List[Union[List[str], None]], List[Union[Dict[str, float], None]]]: ...
+    ) -> List[Union[Tuple[float, float], None]]: ...
     async def georadius(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> Union[
-        List[Union[str, List[Union[str, List[str]]]]],
-        List[Dict[str, Union[str, float, int]]],
-        int,
-    ]: ...
+    ) -> Union[List[Union[str, GeoSearchResult]], int]: ...
     async def georadius_ro(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> Union[
-        List[Union[str, List[Union[str, List[str]]]]],
-        List[Dict[str, Union[str, float, int]]],
-    ]: ...
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> List[Union[str, GeoSearchResult]]: ...
     async def georadiusbymember(
         self,
         key: str,
         member: str,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> Union[
-        List[Union[str, List[Union[str, List[str]]]]],
-        List[Dict[str, Union[str, float, int]]],
-        int,
-    ]: ...
+    ) -> Union[List[Union[str, GeoSearchResult]], int]: ...
     async def georadiusbymember_ro(
         self,
         key: str,
         member: str,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> Union[
-        List[Union[str, List[Union[str, List[str]]]]],
-        List[Dict[str, Union[str, float, int]]],
-    ]: ...
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> List[Union[str, GeoSearchResult]]: ...
     async def geosearch(
         self,
         key: str,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        frommember: Union[str, None] = None,
-        fromlonlat_longitude: Union[float, None] = None,
-        fromlonlat_latitude: Union[float, None] = None,
-        byradius: Union[float, None] = None,
-        bybox_width: Union[float, None] = None,
-        bybox_height: Union[float, None] = None,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        unit: Literal["M", "KM", "FT", "MI"],
+        member: Union[str, None] = None,
+        longitude: Union[float, None] = None,
+        latitude: Union[float, None] = None,
+        radius: Union[float, None] = None,
+        width: Union[float, None] = None,
+        height: Union[float, None] = None,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
-        count_any: bool = False,
+        any: bool = False,
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
-    ) -> Union[
-        List[Union[str, List[Union[str, List[str]]]]],
-        List[Dict[str, Union[str, float, int]]],
-    ]: ...
+    ) -> List[Union[str, GeoSearchResult]]: ...
     async def geosearchstore(
         self,
         destination: str,
         source: str,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        frommember: Union[str, None] = None,
-        fromlonlat_longitude: Union[float, None] = None,
-        fromlonlat_latitude: Union[float, None] = None,
-        byradius: Union[float, None] = None,
-        bybox_width: Union[float, None] = None,
-        bybox_height: Union[float, None] = None,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        member: Union[str, None] = None,
+        longitude: Union[float, None] = None,
+        latitude: Union[float, None] = None,
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+        radius: Union[float, None] = None,
+        width: Union[float, None] = None,
+        height: Union[float, None] = None,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
-        count_any: bool = False,
+        any: bool = False,
         storedist: bool = False,
     ) -> int: ...
     async def hdel(self, key: str, *fields: str) -> int: ...
-    async def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]: ...
+    async def hexists(self, key: str, field: str) -> bool: ...
     async def hget(self, key: str, field: str) -> Union[str, None]: ...
-    async def hgetall(self, key: str) -> Union[List[str], Dict[str, str]]: ...
+    async def hgetall(self, key: str) -> Dict[str, str]: ...
     async def hincrby(self, key: str, field: str, increment: int) -> int: ...
-    async def hincrbyfloat(
-        self, key: str, field: str, increment: float
-    ) -> Union[str, float]: ...
+    async def hincrbyfloat(self, key: str, field: str, increment: float) -> float: ...
     async def hkeys(self, key: str) -> List[str]: ...
     async def hlen(self, key: str) -> int: ...
     async def hmget(self, key: str, *fields: str) -> List[Union[str, None]]: ...
-    async def hmset(self, key: str, field_value_pairs: Dict) -> str: ...
+    async def hmset(self, key: str, values: Dict[str, str]) -> bool: ...
     async def hrandfield(
         self, key: str, count: Union[int, None] = None, withvalues: bool = False
-    ): ...
+    ) -> Union[str, None, List[str], Dict[str, str]]: ...
     async def hscan(
         self,
-        name: str,
+        key: str,
         cursor: int,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
     ) -> Tuple[int, Dict[str, str]]: ...
     async def hset(
         self,
-        name: str,
-        key: Optional[str] = None,
-        val: Optional[str] = None,
-        field_value_pairs: Optional[Dict] = None,
-    ) -> int: ...
-    async def hsetnx(
-        self, key: str, field: str, value: Any
-    ) -> Union[Literal[1, 0], bool]: ...
+        key: str,
+        field: Optional[str] = None,
+        value: Optional[str] = None,
+        values: Optional[Dict[str, str]] = None,
+    ) -> int: ...
+    async def hsetnx(self, key: str, field: str, value: str) -> bool: ...
     async def hstrlen(self, key: str, field: str) -> int: ...
     async def hvals(self, key: str) -> List[str]: ...
-    async def pfadd(self, key: str, *elements: Any) -> Union[Literal[1, 0], bool]: ...
+    async def pfadd(self, key: str, *elements: Any) -> bool: ...
     async def pfcount(self, *keys: str) -> int: ...
-    async def pfmerge(self, destkey: str, *sourcekeys: str) -> str: ...
+    async def pfmerge(self, destkey: str, *sourcekeys: str) -> bool: ...
     async def lindex(self, key: str, index: int) -> Union[str, None]: ...
     async def linsert(
         self,
         key: str,
-        position: Literal["BEFORE", "AFTER", "before", "after"],
-        pivot: Any,
-        element: Any,
+        where: Literal["BEFORE", "AFTER"],
+        pivot: str,
+        element: str,
     ) -> int: ...
     async def llen(self, key: str) -> int: ...
     async def lmove(
         self,
         source: str,
         destination: str,
-        source_position: Literal["LEFT", "RIGHT"] = "LEFT",
-        destination_position: Literal["LEFT", "RIGHT"] = "RIGHT",
+        wherefrom: Literal["LEFT", "RIGHT"] = "LEFT",
+        whereto: Literal["LEFT", "RIGHT"] = "RIGHT",
     ) -> Union[str, None]: ...
     async def lpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]: ...
+    ) -> Union[str, List[str], None]: ...
     async def lpos(
         self,
         key: str,
-        element: Any,
+        element: str,
         rank: Union[int, None] = None,
         count: Union[int, None] = None,
         maxlen: Union[int, None] = None,
     ) -> Union[(Union[int, None]), List[int]]: ...
-    async def lpush(self, key: str, *elements: Any) -> int: ...
-    async def lpushx(self, key: str, *elements: Any) -> int: ...
+    async def lpush(self, key: str, *elements: str) -> int: ...
+    async def lpushx(self, key: str, *elements: str) -> int: ...
     async def lrange(self, key: str, start: int, stop: int) -> List[str]: ...
-    async def lrem(self, key: str, count: int, element: Any) -> int: ...
-    async def lset(self, key: str, index: int, element: Any) -> str: ...
+    async def lrem(self, key: str, count: int, element: str) -> int: ...
+    async def lset(self, key: str, index: int, element: str) -> bool: ...
     async def ltrim(self, key: str, start: int, stop: int) -> str: ...
     async def rpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]: ...
+    ) -> Union[str, List[str], None]: ...
     async def rpoplpush(self, source: str, destination: str) -> Union[str, None]: ...
-    async def rpush(self, key: str, *elements: Any) -> int: ...
-    async def rpushx(self, key: str, *elements: Any) -> int: ...
+    async def rpush(self, key: str, *elements: str) -> int: ...
+    async def rpushx(self, key: str, *elements: str) -> int: ...
     async def publish(self, channel: str, message: str) -> int: ...
     async def eval(
         self,
         script: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
     ) -> Any: ...
@@ -273,258 +694,263 @@
         self,
         sha1: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
     ) -> Any: ...
     async def dbsize(self) -> int: ...
     async def flushall(
-        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
-    ) -> Union[str, bool]: ...
+        self, flush_type: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> bool: ...
     async def flushdb(
-        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
-    ) -> Union[str, bool]: ...
-    async def time(self) -> Union[List[str], Dict[str, int]]: ...
-    async def sadd(self, key: str, *members: Any) -> int: ...
+        self, flush_type: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> bool: ...
+    async def time(self) -> Tuple[int, int]: ...
+    async def sadd(self, key: str, *members: str) -> int: ...
     async def scard(self, key: str) -> int: ...
     async def sdiff(self, *keys: str) -> Set[str]: ...
     async def sdiffstore(self, destination: str, *keys: str) -> int: ...
     async def sinter(self, *keys: str) -> Set[str]: ...
     async def sinterstore(self, destination: str, *keys: str) -> int: ...
-    async def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]: ...
-    async def smismember(
-        self, key: str, *members: Any
-    ) -> Union[List[Literal[1, 0]], List[bool]]: ...
+    async def sismember(self, key: str, member: str) -> bool: ...
+    async def smismember(self, key: str, *members: str) -> List[bool]: ...
     async def smembers(self, key: str) -> Set[str]: ...
-    async def smove(
-        self, source: str, destination: str, member: Any
-    ) -> Union[Literal[1, 0], bool]: ...
+    async def smove(self, source: str, destination: str, member: str) -> bool: ...
     async def spop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]: ...
+    ) -> Union[str, List[str], None]: ...
     async def srandmember(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), List[str]]: ...
-    async def srem(self, key: str, *members: Any) -> int: ...
+    ) -> Union[str, List[str], None]: ...
+    async def srem(self, key: str, *members: str) -> int: ...
     async def sscan(
         self,
         key: str,
         cursor: int = 0,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
     ) -> Tuple[int, List[str]]: ...
     async def sunion(self, *keys: str) -> Set[str]: ...
     async def sunionstore(self, destination: str, *keys: str) -> int: ...
     async def zadd(
         self,
         key: str,
-        score_member_pairs: Dict,
+        scores: Dict[str, float],
         nx: bool = False,
         xx: bool = False,
         gt: bool = False,
         lt: bool = False,
         ch: bool = False,
         incr: bool = False,
-    ) -> Union[int, (Union[str, None, float])]: ...
+    ) -> Union[int, float, None]: ...
     async def zcard(self, key: str) -> int: ...
-    async def zcount(
-        self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
-    ) -> int: ...
-    def zdiff(
+    async def zcount(self, key: str, min: FloatMinMaxT, max: FloatMinMaxT) -> int: ...
+    async def zdiff(
         self, keys: List[str], withscores: bool = False
     ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zdiffstore(self, destination: str, keys: List[str]) -> int: ...
-    async def zincrby(
-        self, key: str, increment: float, member: str
-    ) -> Union[str, float]: ...
+    async def zincrby(self, key: str, increment: float, member: str) -> float: ...
     async def zinter(
         self,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
     ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zinterstore(
         self,
         destination: str,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int: ...
-    async def zlexcount(self, key: str, min_score: str, max_score: str) -> int: ...
+    async def zlexcount(self, key: str, min: str, max: str) -> int: ...
     async def zmscore(
         self, key: str, members: List[str]
-    ) -> Union[List[Union[str, None]], List[Union[float, None]]]: ...
+    ) -> List[Union[float, None]]: ...
     async def zpopmax(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    ) -> List[Tuple[str, float]]: ...
     async def zpopmin(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[List[str], List[Tuple[str, float]]]: ...
+    ) -> List[Tuple[str, float]]: ...
     async def zrandmember(
         self, key: str, count: Union[int, None] = None, withscores: bool = False
-    ) -> Union[(Union[str, None]), (Union[List[str], List[Tuple[str, float]]])]: ...
+    ) -> Union[str, None, List[str], List[Tuple[str, float]]]: ...
     async def zrange(
         self,
         key: str,
-        start: FloatMinMax,
-        stop: FloatMinMax,
-        range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
+        start: FloatMinMaxT,
+        stop: FloatMinMaxT,
+        sortby: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
         withscores: bool = False,
     ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrangebylex(
         self,
         key: str,
-        min_score: str,
-        max_score: str,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
-    ) -> List[Union[str, None]]: ...
+        min: str,
+        max: str,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> List[str]: ...
     async def zrangebyscore(
         self,
         key: str,
-        min_score: FloatMinMax,
-        max_score: FloatMinMax,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
         withscores: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
     ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrangestore(
         self,
         dst: str,
         src: str,
-        start: FloatMinMax,
-        stop: FloatMinMax,
-        range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
+        sortby: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
     ) -> int: ...
     async def zrank(self, key: str, member: str) -> Union[int, None]: ...
     async def zrem(self, key: str, *members: str) -> int: ...
-    async def zremrangebylex(self, key: str, min_score: str, max_score: str) -> int: ...
+    async def zremrangebylex(self, key: str, min: str, max: str) -> int: ...
     async def zremrangebyrank(self, key: str, start: int, stop: int) -> int: ...
     async def zremrangebyscore(
-        self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
+        self, key: str, min: FloatMinMaxT, max: FloatMinMaxT
     ) -> int: ...
     async def zrevrange(
         self, key: str, start: int, stop: int, withscores: bool = False
     ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrevrangebylex(
         self,
         key: str,
-        max_score: str,
-        min_score: str,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
+        max: str,
+        min: str,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
     ) -> List[str]: ...
     async def zrevrangebyscore(
         self,
         key: str,
-        max_score: FloatMinMax,
-        min_score: FloatMinMax,
+        max: FloatMinMaxT,
+        min: FloatMinMaxT,
         withscores: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
     ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zrevrank(self, key: str, member: str) -> Union[int, None]: ...
     async def zscan(
         self,
         key: str,
         cursor: int,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
     ) -> Tuple[int, List[Tuple[str, float]]]: ...
-    async def zscore(self, key: str, member: str) -> Union[str, None, float]: ...
-    def zunion(
+    async def zscore(self, key: str, member: str) -> Union[float, None]: ...
+    async def zunion(
         self,
         keys: List[str],
-        weights: Union[List[float], List[int], None] = None,
+        weights: Union[List[float], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
     ) -> Union[List[str], List[Tuple[str, float]]]: ...
     async def zunionstore(
         self,
         destination: str,
         keys: List[str],
-        weights: Union[List[float], List[int], None] = None,
+        weights: Union[List[float], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int: ...
-    async def append(self, key: str, value: Any) -> int: ...
+    async def append(self, key: str, value: str) -> int: ...
     async def decr(self, key: str) -> int: ...
     async def decrby(self, key: str, decrement: int) -> int: ...
     async def get(self, key: str) -> Union[str, None]: ...
     async def getdel(self, key: str) -> Union[str, None]: ...
     async def getex(
         self,
         key: str,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         persist: Union[bool, None] = None,
     ) -> Union[str, None]: ...
     async def getrange(self, key: str, start: int, end: int) -> str: ...
-    async def getset(self, key: str, value: Any) -> Union[str, None]: ...
+    async def getset(self, key: str, value: str) -> Union[str, None]: ...
     async def incr(self, key: str) -> int: ...
     async def incrby(self, key: str, increment: int) -> int: ...
-    async def incrbyfloat(self, key: str, increment: float) -> Union[str, float]: ...
+    async def incrbyfloat(self, key: str, increment: float) -> float: ...
     async def mget(self, *keys: str) -> List[Union[str, None]]: ...
-    async def mset(self, key_value_pairs: Dict) -> Literal["OK"]: ...
-    async def msetnx(self, key_value_pairs: Dict) -> Literal[1, 0]: ...
-    async def psetex(self, key: str, milliseconds: int, value: Any) -> str: ...
+    async def mset(self, values: Dict[str, str]) -> Literal[True]: ...
+    async def msetnx(self, values: Dict[str, str]) -> bool: ...
+    async def psetex(
+        self, key: str, milliseconds: int, value: str
+    ) -> Literal[True]: ...
     async def set(
         self,
         key: str,
         value: Any,
         nx: bool = False,
         xx: bool = False,
         get: bool = False,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         keepttl: bool = False,
     ) -> Union[str, None]: ...
-    async def setex(self, key: str, seconds: int, value: Any) -> str: ...
-    async def setnx(self, key: str, value: Any) -> Literal[1, 0]: ...
-    async def setrange(self, key: str, offset: int, value: Any) -> int: ...
+    async def setex(self, key: str, seconds: int, value: str) -> Literal[True]: ...
+    async def setnx(self, key: str, value: str) -> bool: ...
+    async def setrange(self, key: str, offset: int, value: str) -> int: ...
     async def strlen(self, key: str) -> int: ...
     async def substr(self, key: str, start: int, end: int) -> str: ...
-    async def script_exists(self, *sha1: str) -> Union[List[int], List[bool]]: ...
+    async def script_exists(self, *sha1: str) -> List[bool]: ...
     async def script_flush(
-        self, mode: Optional[Literal["ASYNC", "SYNC"]] = None
-    ) -> Union[str, bool]: ...
+        self, flush_type: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> bool: ...
     async def script_load(self, script: str) -> str: ...
 
-    # async def pubsub_channels(self, pattern: Union[str, None] = None) -> List[str]:
-    #     ...
-
-    # async def pubsub_numpat(self) -> int:
-    #     ...
-
-    # async def pubsub_numsub(
-    #     self, *channels: str
-    # ) -> Union[List[Union[str, int]], Dict[str, int]]:
-    #     ...
-
-# It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
-    def __init__(self, client: AsyncCommands, key: str): ...
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands": ...
+    def __init__(self, client: Commands, key: str): ...
+    def get(self, encoding: str, offset: Union[int, str]) -> "BitFieldCommands": ...
     def set(
-        self, encoding: str, offset: BitFieldOffset, value: int
+        self, encoding: str, offset: Union[int, str], value: int
     ) -> "BitFieldCommands": ...
     def incrby(
-        self, encoding: str, offset: BitFieldOffset, increment: int
+        self, encoding: str, offset: Union[int, str], increment: int
     ) -> "BitFieldCommands": ...
     def overflow(
         self, overflow: Literal["WRAP", "SAT", "FAIL"]
     ) -> "BitFieldCommands": ...
+    def execute(self) -> List: ...
+
+class BitFieldROCommands:
+    def __init__(self, client: Commands, key: str): ...
+    def get(self, encoding: str, offset: Union[int, str]) -> "BitFieldROCommands": ...
+    def execute(self) -> List: ...
+
+class AsyncBitFieldCommands:
+    def __init__(self, client: AsyncCommands, key: str): ...
+    def get(
+        self, encoding: str, offset: Union[int, str]
+    ) -> "AsyncBitFieldCommands": ...
+    def set(
+        self, encoding: str, offset: Union[int, str], value: int
+    ) -> "AsyncBitFieldCommands": ...
+    def incrby(
+        self, encoding: str, offset: Union[int, str], increment: int
+    ) -> "AsyncBitFieldCommands": ...
+    def overflow(
+        self, overflow: Literal["WRAP", "SAT", "FAIL"]
+    ) -> "AsyncBitFieldCommands": ...
     async def execute(self) -> List: ...
 
-class BitFieldRO:
+class AsyncBitFieldROCommands:
     def __init__(self, client: AsyncCommands, key: str): ...
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO": ...
+    def get(
+        self, encoding: str, offset: Union[int, str]
+    ) -> "AsyncBitFieldROCommands": ...
     async def execute(self) -> List: ...
```

### Comparing `upstash_redis-0.14.5/upstash_redis/commands/commands.py` & `upstash_redis-0.15.0/upstash_redis/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,82 @@
-from upstash_redis.typing import CommandsProtocol, ResponseType
+from typing import Any, Awaitable, Dict, List, Literal, Optional, Tuple, Union
 
-from upstash_redis.utils.exception import (
+from upstash_redis.typing import FloatMinMaxT
+from upstash_redis.utils import (
+    handle_georadius_write_exceptions,
     handle_geosearch_exceptions,
     handle_non_deprecated_zrange_exceptions,
     handle_zrangebylex_exceptions,
-    handle_georadius_write_exceptions,
-)
-from upstash_redis.utils.comparison import number_are_not_none
-from upstash_redis.schema.commands.parameters import (
-    BitFieldOffset,
-    GeoMember,
-    FloatMinMax,
+    number_are_not_none,
 )
 
-from typing import Any, Iterable, Literal, Optional, Union, List, Dict
+ResponseT = Union[Awaitable, Any]
 
 
-class Commands(CommandsProtocol):
-    def run(self, command):
-        ...
+class Commands:
+    def execute(self, command: List) -> ResponseT:
+        raise NotImplementedError("execute")
 
     def bitcount(
         self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/bitcount
         """
 
         if number_are_not_none(start, end, number=1):
             raise Exception('Both "start" and "end" must be specified.')
 
         command: List = ["BITCOUNT", key]
 
         if start is not None:
             command.extend([start, end])
 
-        return self.run(command)
+        return self.execute(command)
 
     def bitfield(self, key: str) -> "BitFieldCommands":
         """
         See https://redis.io/commands/bitfield
         """
 
         return BitFieldCommands(key=key, client=self)
 
-    def bitfield_ro(self, key: str) -> "BitFieldRO":
+    def bitfield_ro(self, key: str) -> "BitFieldROCommands":
         """
         See https://redis.io/commands/bitfield_ro
         """
 
-        return BitFieldRO(key=key, client=self)
+        return BitFieldROCommands(key=key, client=self)
 
     def bitop(
-        self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *srckeys: str
-    ) -> ResponseType:
+        self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *keys: str
+    ) -> ResponseT:
         """
         See https://redis.io/commands/bitop
         """
 
-        if len(srckeys) == 0:
+        if len(keys) == 0:
             raise Exception("At least one source key must be specified.")
 
-        if operation == "NOT" and len(srckeys) > 1:
+        if operation == "NOT" and len(keys) > 1:
             raise Exception(
                 'The "NOT " operation takes only one source key as argument.'
             )
 
-        command: List = ["BITOP", operation, destkey, *srckeys]
+        command: List = ["BITOP", operation, destkey, *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
     def bitpos(
         self,
         key: str,
         bit: Literal[0, 1],
         start: Union[int, None] = None,
         end: Union[int, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/bitpos
         """
 
         if start is None and end is not None:
             raise Exception('"end" is specified, but "start" is missing.')
 
@@ -88,281 +84,260 @@
 
         if start is not None:
             command.append(start)
 
         if end is not None:
             command.append(end)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def getbit(self, key: str, offset: int) -> ResponseType:
+    def getbit(self, key: str, offset: int) -> ResponseT:
         """
         See https://redis.io/commands/getbit
         """
 
         command: List = ["GETBIT", key, offset]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> ResponseType:
+    def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> ResponseT:
         """
         See https://redis.io/commands/setbit
         """
 
         command: List = ["SETBIT", key, offset, value]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def ping(self, message: Union[str, None] = None) -> ResponseType:
+    def ping(self, message: Union[str, None] = None) -> ResponseT:
         """
         See https://redis.io/commands/ping
         """
 
         command: List = ["PING"]
 
         if message is not None:
             command.append(message)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def echo(self, message: str) -> ResponseType:
+    def echo(self, message: str) -> ResponseT:
         """
         See https://redis.io/commands/echo
         """
 
         command: List = ["ECHO", message]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def copy(
-        self, source: str, destination: str, replace: bool = False
-    ) -> ResponseType:
+    def copy(self, source: str, destination: str, replace: bool = False) -> ResponseT:
         """
         See https://redis.io/commands/copy
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["COPY", source, destination]
 
         if replace:
             command.append("REPLACE")
 
-        return self.run(command)
+        return self.execute(command)
 
-    def delete(self, *keys: str) -> ResponseType:
+    def delete(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/del
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be deleted.")
 
         command: List = ["DEL", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def exists(self, *keys: str) -> ResponseType:
+    def exists(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/exists
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be checked.")
 
         command: List = ["EXISTS", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def expire(self, key: str, seconds: int) -> ResponseType:
+    def expire(self, key: str, seconds: int) -> ResponseT:
         """
         See https://redis.io/commands/expire
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["EXPIRE", key, seconds]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def expireat(self, key: str, unix_time_seconds: int) -> ResponseType:
+    def expireat(self, key: str, unix_time_seconds: int) -> ResponseT:
         """
         See https://redis.io/commands/expireat
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["EXPIREAT", key, unix_time_seconds]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def keys(self, pattern: str) -> ResponseType:
+    def keys(self, pattern: str) -> ResponseT:
         """
         See https://redis.io/commands/keys
         """
 
         command: List = ["KEYS", pattern]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def persist(self, key: str) -> ResponseType:
+    def persist(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/persist
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["PERSIST", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def pexpire(self, key: str, milliseconds: int) -> ResponseType:
+    def pexpire(self, key: str, milliseconds: int) -> ResponseT:
         """
         See https://redis.io/commands/pexpire
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["PEXPIRE", key, milliseconds]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def pexpireat(self, key: str, unix_time_milliseconds: int) -> ResponseType:
+    def pexpireat(self, key: str, unix_time_milliseconds: int) -> ResponseT:
         """
         See https://redis.io/commands/pexpireat
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["PEXPIREAT", key, unix_time_milliseconds]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def pttl(self, key: str) -> ResponseType:
+    def pttl(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/pttl
         """
 
         command: List = ["PTTL", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def randomkey(self) -> ResponseType:
+    def randomkey(self) -> ResponseT:
         """
         See https://redis.io/commands/randomkey
         """
 
         command: List = ["RANDOMKEY"]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def rename(self, key: str, newkey: str) -> ResponseType:
+    def rename(self, key: str, newkey: str) -> ResponseT:
         """
         See https://redis.io/commands/rename
         """
 
         command: List = ["RENAME", key, newkey]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def renamenx(self, key: str, newkey: str) -> ResponseType:
+    def renamenx(self, key: str, newkey: str) -> ResponseT:
         """
         See https://redis.io/commands/renamenx
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["RENAMENX", key, newkey]
 
-        return self.run(command)
+        return self.execute(command)
 
     def scan(
         self,
         cursor: int,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
-        scan_type: Union[str, None] = None,
-    ) -> ResponseType:
+        type: Union[str, None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/scan
-
-        :param scan_type: replacement for "TYPE"
-        :param match_pattern: replacement for "MATCH"
-
-        :return: The cursor will be an integer if "format_return" is True.
         """
 
         command: List = ["SCAN", cursor]
 
-        if match_pattern is not None:
-            command.extend(["MATCH", match_pattern])
+        if match is not None:
+            command.extend(["MATCH", match])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        if scan_type is not None:
-            command.extend(["TYPE", scan_type])
+        if type is not None:
+            command.extend(["TYPE", type])
 
         # The raw result is composed of the new cursor and the List of elements.
-        return self.run(command)
+        return self.execute(command)
 
-    def touch(self, *keys: str) -> ResponseType:
+    def touch(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/touch
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["TOUCH", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def ttl(self, key: str) -> ResponseType:
+    def ttl(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/ttl
         """
 
         command: List = ["TTL", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def type(self, key: str) -> ResponseType:
+    def type(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/type
         """
 
         command: List = ["TYPE", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def unlink(self, *keys: str) -> ResponseType:
+    def unlink(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/unlink
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["UNLINK", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
     def geoadd(
         self,
         key: str,
-        *members: GeoMember,
+        *members: Tuple[float, float, str],
         nx: bool = False,
         xx: bool = False,
         ch: bool = False,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/geoadd
 
-        :param members: a sequence of GeoMember Dict types (longitude, latitude, name).
+        :param members: a sequence of (longitude, latitude, name).
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be added.")
 
         if nx and xx:
             raise Exception('"nx" and "xx" are mutually exclusive.')
@@ -375,81 +350,73 @@
         if xx:
             command.append("XX")
 
         if ch:
             command.append("CH")
 
         for member in members:
-            command.extend([member["longitude"], member["latitude"], member["member"]])
+            command.extend(member)
 
-        return self.run(command)
+        return self.execute(command)
 
     def geodist(
         self,
         key: str,
         member1: str,
         member2: str,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M",
-    ) -> ResponseType:
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+    ) -> ResponseT:
         """
         See https://redis.io/commands/geodist
-
-        :return: A float value if "format_return" is True.
         """
 
         command: List = ["GEODIST", key, member1, member2, unit]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def geohash(self, key: str, *members: str) -> ResponseType:
+    def geohash(self, key: str, *members: str) -> ResponseT:
         """
         See https://redis.io/commands/geohash
         """
 
         command: List = ["GEOHASH", key, *members]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def geopos(self, key: str, *members: str) -> ResponseType:
+    def geopos(self, key: str, *members: str) -> ResponseT:
         """
         See https://redis.io/commands/geopos
-
-        :return: A List of Dicts with either None or the longitude and latitude if "format_return" is True.
         """
 
         command: List = ["GEOPOS", key, *members]
 
-        return self.run(command)
+        return self.execute(command)
 
     def georadius(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/georadius
-
-        :param count_any: replacement for "ANY"
-
-        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         handle_georadius_write_exceptions(
-            withdist, withhash, withcoord, count, count_any, store, storedist
+            withdist, withhash, withcoord, count, any, store, storedist
         )
 
         command: List = ["GEORADIUS", key, longitude, latitude, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
@@ -457,101 +424,93 @@
             command.append("WITHHASH")
 
         if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
-            if count_any:
+            if any:
                 command.append("ANY")
 
-        if sort:
-            command.append(sort)
+        if order:
+            command.append(order)
 
         if store:
             command.extend(["STORE", store])
 
         if storedist:
             command.extend(["STOREDIST", storedist])
 
         # If none of the additional properties are requested, the result will be "List[str]".
-        return self.run(command)
+        return self.execute(command)
 
     def georadius_ro(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> ResponseType:
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/georadius_ro
-
-        :param count_any: replacement for "ANY"
-
-        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
-        if count_any and count is None:
-            raise Exception('"count_any" can only be used together with "count".')
+        if any and count is None:
+            raise Exception('"any" can only be used together with "count".')
 
         command: List = ["GEORADIUS_RO", key, longitude, latitude, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
         if withhash:
             command.append("WITHHASH")
 
         if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
-            if count_any:
+            if any:
                 command.append("ANY")
 
-        if sort:
-            command.append(sort)
+        if order:
+            command.append(order)
 
         # If none of the additional properties are requested, the result will be "List[str]".
-        return self.run(command)
+        return self.execute(command)
 
     def georadiusbymember(
         self,
         key: str,
         member: str,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         store: Union[str, None] = None,
         storedist: Union[str, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/georadiusbymember
-
-        :param count_any: replacement for "ANY"
-
-        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         handle_georadius_write_exceptions(
-            withdist, withhash, withcoord, count, count_any, store, storedist
+            withdist, withhash, withcoord, count, any, store, storedist
         )
 
         command: List = ["GEORADIUSBYMEMBER", key, member, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
@@ -559,521 +518,495 @@
             command.append("WITHHASH")
 
         if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
-            if count_any:
+            if any:
                 command.append("ANY")
 
-        if sort:
-            command.append(sort)
+        if order:
+            command.append(order)
 
         if store:
             command.extend(["STORE", store])
 
         if storedist:
             command.extend(["STOREDIST", storedist])
 
         # If none of the additional properties are requested, the result will be "List[str]".
-        return self.run(command)
+        return self.execute(command)
 
     def georadiusbymember_ro(
         self,
         key: str,
         member: str,
         radius: float,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
+        unit: Literal["M", "KM", "FT", "MI"],
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
         count: Union[int, None] = None,
-        count_any: bool = False,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
-    ) -> ResponseType:
+        any: bool = False,
+        order: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/georadiusbymember_ro
-
-        :param count_any: replacement for "ANY"
-
-        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
-        if count_any and count is None:
-            raise Exception('"count_any" can only be used together with "count".')
+        if any and count is None:
+            raise Exception('"any" can only be used together with "count".')
 
         command: List = ["GEORADIUSBYMEMBER_RO", key, member, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
         if withhash:
             command.append("WITHHASH")
 
         if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
-            if count_any:
+            if any:
                 command.append("ANY")
 
-        if sort:
-            command.append(sort)
+        if order:
+            command.append(order)
 
         # If none of the additional properties are requested, the result will be "List[str]".
-        return self.run(command)
+        return self.execute(command)
 
     def geosearch(
         self,
         key: str,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        frommember: Union[str, None] = None,
-        fromlonlat_longitude: Union[float, None] = None,
-        fromlonlat_latitude: Union[float, None] = None,
-        byradius: Union[float, None] = None,
-        bybox_width: Union[float, None] = None,
-        bybox_height: Union[float, None] = None,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        member: Union[str, None] = None,
+        longitude: Union[float, None] = None,
+        latitude: Union[float, None] = None,
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+        radius: Union[float, None] = None,
+        width: Union[float, None] = None,
+        height: Union[float, None] = None,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
-        count_any: bool = False,
+        any: bool = False,
         withdist: bool = False,
         withhash: bool = False,
         withcoord: bool = False,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/geosearch
-
-        :param count_any: replacement for "ANY"
-
-        :return: A List of Dicts with the requested properties if "format_return" is True and any of the `with` parameters is used.
         """
 
         handle_geosearch_exceptions(
-            frommember,
-            fromlonlat_longitude,
-            fromlonlat_latitude,
-            byradius,
-            bybox_width,
-            bybox_height,
+            member,
+            longitude,
+            latitude,
+            radius,
+            width,
+            height,
             count,
-            count_any,
+            any,
         )
 
         command: List = ["GEOSEARCH", key]
 
-        if frommember is not None:
-            command.extend(["FROMMEMBER", frommember])
+        if member is not None:
+            command.extend(["FROMMEMBER", member])
 
-        if fromlonlat_longitude is not None:
-            command.extend(["FROMLONLAT", fromlonlat_longitude, fromlonlat_latitude])
+        if longitude is not None:
+            command.extend(["FROMLONLAT", longitude, latitude])
 
-        if byradius is not None:
-            command.extend(["BYRADIUS", byradius])
+        if radius is not None:
+            command.extend(["BYRADIUS", radius])
 
-        if bybox_width is not None:
-            command.extend(["BYBOX", bybox_width, bybox_height])
+        if width is not None:
+            command.extend(["BYBOX", width, height])
 
         command.append(unit)
 
-        if sort:
-            command.append(sort)
+        if order:
+            command.append(order)
 
         if count is not None:
             command.extend(["COUNT", count])
-            if count_any:
+            if any:
                 command.append("ANY")
 
         if withdist:
             command.append("WITHDIST")
 
         if withhash:
             command.append("WITHHASH")
 
         if withcoord:
             command.append("WITHCOORD")
 
         # If none of the additional properties are requested, the result will be "List[str]".
-        return self.run(command)
+        return self.execute(command)
 
     def geosearchstore(
         self,
         destination: str,
         source: str,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        frommember: Union[str, None] = None,
-        fromlonlat_longitude: Union[float, None] = None,
-        fromlonlat_latitude: Union[float, None] = None,
-        byradius: Union[float, None] = None,
-        bybox_width: Union[float, None] = None,
-        bybox_height: Union[float, None] = None,
-        sort: Union[Literal["ASC", "DESC"], None] = None,
+        member: Union[str, None] = None,
+        longitude: Union[float, None] = None,
+        latitude: Union[float, None] = None,
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+        radius: Union[float, None] = None,
+        width: Union[float, None] = None,
+        height: Union[float, None] = None,
+        order: Union[Literal["ASC", "DESC"], None] = None,
         count: Union[int, None] = None,
-        count_any: bool = False,
+        any: bool = False,
         storedist: bool = False,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/geosearchstore
-
-        :param count_any: replacement for "ANY"
         """
 
         handle_geosearch_exceptions(
-            frommember,
-            fromlonlat_longitude,
-            fromlonlat_latitude,
-            byradius,
-            bybox_width,
-            bybox_height,
+            member,
+            longitude,
+            latitude,
+            radius,
+            width,
+            height,
             count,
-            count_any,
+            any,
         )
 
         command: List = ["GEOSEARCHSTORE", destination, source]
 
-        if frommember is not None:
-            command.extend(["FROMMEMBER", frommember])
+        if member is not None:
+            command.extend(["FROMMEMBER", member])
 
-        if fromlonlat_longitude is not None:
-            command.extend(["FROMLONLAT", fromlonlat_longitude, fromlonlat_latitude])
+        if longitude is not None:
+            command.extend(["FROMLONLAT", longitude, latitude])
 
-        if byradius is not None:
-            command.extend(["BYRADIUS", byradius])
+        if radius is not None:
+            command.extend(["BYRADIUS", radius])
 
-        if bybox_width is not None:
-            command.extend(["BYBOX", bybox_width, bybox_height])
+        if width is not None:
+            command.extend(["BYBOX", width, height])
 
         command.append(unit)
 
-        if sort:
-            command.append(sort)
+        if order:
+            command.append(order)
 
         if count is not None:
             command.extend(["COUNT", count])
-            if count_any:
+            if any:
                 command.append("ANY")
 
         if storedist:
             command.append("STOREDIST")
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hdel(self, key: str, *fields: str) -> ResponseType:
+    def hdel(self, key: str, *fields: str) -> ResponseT:
         """
         See https://redis.io/commands/hdel
         """
 
         if len(fields) == 0:
             raise Exception("At least one field must be deleted.")
 
         command: List = ["HDEL", key, *fields]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hexists(self, key: str, field: str) -> ResponseType:
+    def hexists(self, key: str, field: str) -> ResponseT:
         """
         See https://redis.io/commands/hexists
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["HEXISTS", key, field]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hget(self, key: str, field: str) -> ResponseType:
+    def hget(self, key: str, field: str) -> ResponseT:
         """
         See https://redis.io/commands/hget
         """
 
         command: List = ["HGET", key, field]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hgetall(self, key: str) -> ResponseType:
+    def hgetall(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/hgetall
-
-        :return: A Dict of field-value pairs if "format_return" is True.
         """
 
         command: List = ["HGETALL", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hincrby(self, key: str, field: str, increment: int) -> ResponseType:
+    def hincrby(self, key: str, field: str, increment: int) -> ResponseT:
         """
         See https://redis.io/commands/hincrby
         """
 
         command: List = ["HINCRBY", key, field, increment]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hincrbyfloat(self, key: str, field: str, increment: float) -> ResponseType:
+    def hincrbyfloat(self, key: str, field: str, increment: float) -> ResponseT:
         """
         See https://redis.io/commands/hincrbyfloat
-
-        :return: A float if "format_return" is True.
         """
 
         command: List = ["HINCRBYFLOAT", key, field, increment]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hkeys(self, key: str) -> ResponseType:
+    def hkeys(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/hkeys
         """
 
         command: List = ["HKEYS", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hlen(self, key: str) -> ResponseType:
+    def hlen(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/hlen
         """
 
         command: List = ["HLEN", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hmget(self, key: str, *fields: str) -> ResponseType:
+    def hmget(self, key: str, *fields: str) -> ResponseT:
         """
         See https://redis.io/commands/hmget
         """
 
         if len(fields) == 0:
             raise Exception("At least one field must be specified.")
 
         command: List = ["HMGET", key, *fields]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hmset(self, key: str, field_value_pairs: Dict) -> ResponseType:
+    def hmset(self, key: str, values: Dict[str, str]) -> ResponseT:
         """
         See https://redis.io/commands/hmset
         """
 
         command: List = ["HMSET", key]
 
-        for field, value in field_value_pairs.items():
+        for field, value in values.items():
             command.extend([field, value])
 
-        return self.run(command)
+        return self.execute(command)
 
     def hrandfield(
         self, key: str, count: Union[int, None] = None, withvalues: bool = False
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/hrandfield
-
-        :return: A Dict of field-value pairs if "count" and "withvalues" are specified and "format_return" is True.
         """
 
         if count is None and withvalues:
             raise Exception('"withvalues" can only be used together with "count"')
 
         command: List = ["HRANDFIELD", key]
 
         if count is not None:
             command.extend([count])
 
             if withvalues:
                 command.append("WITHVALUES")
 
-        return self.run(command)
+        return self.execute(command)
 
     def hscan(
         self,
-        name: str,
+        key: str,
         cursor: int,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/hscan
-
-        :param match_pattern: replacement for "MATCH"
         """
 
-        command: List = ["HSCAN", name, cursor]
+        command: List = ["HSCAN", key, cursor]
 
-        if match_pattern is not None:
-            command.extend(["MATCH", match_pattern])
+        if match is not None:
+            command.extend(["MATCH", match])
 
         if count is not None:
             command.extend(["COUNT", count])
 
         # The raw result is composed of the new cursor and the List of elements.
-        return self.run(command)
+        return self.execute(command)
 
     def hset(
         self,
-        name: str,
-        key: Optional[str] = None,
-        val: Optional[str] = None,
-        field_value_pairs: Optional[Dict] = None,
-    ) -> ResponseType:
+        key: str,
+        field: Optional[str] = None,
+        value: Optional[str] = None,
+        values: Optional[Dict[str, str]] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/hset
         """
-        command: List = ["HSET", name]
+        command: List = ["HSET", key]
 
-        if key is None and field_value_pairs is None:
+        if field is None and values is None:
             raise Exception("'hset' with no key value pairs")
 
-        if key and val:
-            command.extend([key, val])
+        if field and value:
+            command.extend([field, value])
 
-        if field_value_pairs is not None:
-            for field, value in field_value_pairs.items():
+        if values is not None:
+            for field, value in values.items():
                 command.extend([field, value])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hsetnx(self, key: str, field: str, value: Any) -> ResponseType:
+    def hsetnx(self, key: str, field: str, value: str) -> ResponseT:
         """
         See https://redis.io/commands/hsetnx
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["HSETNX", key, field, value]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hstrlen(self, key: str, field: str) -> ResponseType:
+    def hstrlen(self, key: str, field: str) -> ResponseT:
         """
         See https://redis.io/commands/hstrlen
         """
 
         command: List = ["HSTRLEN", key, field]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def hvals(self, key: str) -> ResponseType:
+    def hvals(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/hvals
         """
 
         command: List = ["HVALS", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def pfadd(self, key: str, *elements: Any) -> ResponseType:
+    def pfadd(self, key: str, *elements: Any) -> ResponseT:
         """
         See https://redis.io/commands/pfadd
-
-        :return: A bool if "format_return" is True.
         """
 
         command: List = ["PFADD", key, *elements]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def pfcount(self, *keys: str) -> ResponseType:
+    def pfcount(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/pfcount
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["PFCOUNT", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def pfmerge(self, destkey: str, *sourcekeys: str) -> ResponseType:
+    def pfmerge(self, destkey: str, *sourcekeys: str) -> ResponseT:
         """
         See https://redis.io/commands/pfmerge
         """
 
         command: List = ["PFMERGE", destkey, *sourcekeys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def lindex(self, key: str, index: int) -> ResponseType:
+    def lindex(self, key: str, index: int) -> ResponseT:
         """
         See https://redis.io/commands/lindex
         """
 
         command: List = ["LINDEX", key, index]
 
-        return self.run(command)
+        return self.execute(command)
 
     def linsert(
         self,
         key: str,
-        position: Literal["BEFORE", "AFTER", "before", "after"],
-        pivot: Any,
-        element: Any,
-    ) -> ResponseType:
+        where: Literal["BEFORE", "AFTER"],
+        pivot: str,
+        element: str,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/linsert
         """
 
-        command: List = ["LINSERT", key, position, pivot, element]
+        command: List = ["LINSERT", key, where, pivot, element]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def llen(self, key: str) -> ResponseType:
+    def llen(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/llen
         """
 
         command: List = ["LLEN", key]
 
-        return self.run(command)
+        return self.execute(command)
 
     def lmove(
         self,
         source: str,
         destination: str,
-        source_position: Literal["LEFT", "RIGHT"] = "LEFT",
-        destination_position: Literal["LEFT", "RIGHT"] = "RIGHT",
-    ) -> ResponseType:
+        wherefrom: Literal["LEFT", "RIGHT"] = "LEFT",
+        whereto: Literal["LEFT", "RIGHT"] = "RIGHT",
+    ) -> ResponseT:
         """
         See https://redis.io/commands/lmove
         """
 
         command: List = [
             "LMOVE",
             source,
             destination,
-            source_position,
-            destination_position,
+            wherefrom,
+            whereto,
         ]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def lpop(self, key: str, count: Union[int, None] = None) -> ResponseType:
+    def lpop(self, key: str, count: Union[int, None] = None) -> ResponseT:
         """
         See https://redis.io/commands/lpop
-
-        :param count: defaults to 1 on the server side
         """
 
         command: List = ["LPOP", key]
 
         if count is not None:
             command.append(count)
 
-        return self.run(command)
+        return self.execute(command)
 
     def lpos(
         self,
         key: str,
-        element: Any,
+        element: str,
         rank: Union[int, None] = None,
         count: Union[int, None] = None,
         maxlen: Union[int, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/lpos
         """
 
         command: List = ["LPOS", key, element]
 
         if rank is not None:
@@ -1081,138 +1014,136 @@
 
         if count is not None:
             command.extend(["COUNT", count])
 
         if maxlen is not None:
             command.extend(["MAXLEN", maxlen])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def lpush(self, key: str, *elements: Any) -> ResponseType:
+    def lpush(self, key: str, *elements: str) -> ResponseT:
         """
         See https://redis.io/commands/lpush
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
         command: List = ["LPUSH", key, *elements]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def lpushx(self, key: str, *elements: Any) -> ResponseType:
+    def lpushx(self, key: str, *elements: str) -> ResponseT:
         """
         See https://redis.io/commands/lpushx
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
         command: List = ["LPUSHX", key, *elements]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def lrange(self, key: str, start: int, stop: int) -> ResponseType:
+    def lrange(self, key: str, start: int, stop: int) -> ResponseT:
         """
         See https://redis.io/commands/lrange
         """
 
         command: List = ["LRANGE", key, start, stop]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def lrem(self, key: str, count: int, element: Any) -> ResponseType:
+    def lrem(self, key: str, count: int, element: str) -> ResponseT:
         """
         See https://redis.io/commands/lrem
         """
 
         command: List = ["LREM", key, count, element]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def lset(self, key: str, index: int, element: Any) -> ResponseType:
+    def lset(self, key: str, index: int, element: str) -> ResponseT:
         """
         See https://redis.io/commands/lset
         """
 
         command: List = ["LSET", key, index, element]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def ltrim(self, key: str, start: int, stop: int) -> ResponseType:
+    def ltrim(self, key: str, start: int, stop: int) -> ResponseT:
         """
         See https://redis.io/commands/ltrim
         """
 
         command: List = ["LTRIM", key, start, stop]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def rpop(self, key: str, count: Union[int, None] = None) -> ResponseType:
+    def rpop(self, key: str, count: Union[int, None] = None) -> ResponseT:
         """
         See https://redis.io/commands/rpop
-
-        :param count: defaults to 1 on the server side
         """
 
         command: List = ["RPOP", key]
 
         if count is not None:
             command.append(count)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def rpoplpush(self, source: str, destination: str) -> ResponseType:
+    def rpoplpush(self, source: str, destination: str) -> ResponseT:
         """
         See https://redis.io/commands/rpoplpush
         """
 
         command: List = ["RPOPLPUSH", source, destination]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def rpush(self, key: str, *elements: Any) -> ResponseType:
+    def rpush(self, key: str, *elements: str) -> ResponseT:
         """
         See https://redis.io/commands/rpush
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
         command: List = ["RPUSH", key, *elements]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def rpushx(self, key: str, *elements: Any) -> ResponseType:
+    def rpushx(self, key: str, *elements: Any) -> ResponseT:
         """
         See https://redis.io/commands/rpushx
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
         command: List = ["RPUSHX", key, *elements]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def publish(self, channel: str, message: str) -> ResponseType:
+    def publish(self, channel: str, message: str) -> ResponseT:
         """
         See https://redis.io/commands/publish
         """
 
         command: List = ["PUBLISH", channel, message]
 
-        return self.run(command)
+        return self.execute(command)
 
     def eval(
         self,
         script: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/eval
 
         The number of keys is calculated automatically.
         """
 
         command: List = ["EVAL", script]
@@ -1221,22 +1152,22 @@
             command.extend([len(keys), *keys])
         else:
             command.append(0)
 
         if args:
             command.extend(args)
 
-        return self.run(command)
+        return self.execute(command)
 
     def evalsha(
         self,
         sha1: str,
         keys: Union[List[str], None] = None,
         args: Union[List, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/evalsha
 
         The number of keys is calculated automatically.
         """
 
         command: List = ["EVALSHA", sha1]
@@ -1245,286 +1176,265 @@
             command.extend([len(keys), *keys])
         else:
             command.append(0)
 
         if args:
             command.extend(args)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def dbsize(self) -> ResponseType:
+    def dbsize(self) -> ResponseT:
         """
         See https://redis.io/commands/dbsize
         """
 
         command: List = ["DBSIZE"]
 
-        return self.run(command)
+        return self.execute(command)
 
     def flushall(
-        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
-    ) -> ResponseType:
+        self, flush_type: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> ResponseT:
         """
         See https://redis.io/commands/flushall
         """
 
         command: List = ["FLUSHALL"]
 
-        if mode:
-            command.append(mode)
+        if flush_type:
+            command.append(flush_type)
 
-        return self.run(command)
+        return self.execute(command)
 
     def flushdb(
-        self, mode: Union[Literal["ASYNC", "SYNC"], None] = None
-    ) -> ResponseType:
+        self, flush_type: Union[Literal["ASYNC", "SYNC"], None] = None
+    ) -> ResponseT:
         """
         See https://redis.io/commands/flushdb
         """
 
         command: List = ["FLUSHDB"]
 
-        if mode:
-            command.append(mode)
+        if flush_type:
+            command.append(flush_type)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def time(self) -> ResponseType:
+    def time(self) -> ResponseT:
         """
         See https://redis.io/commands/time
-
-        :return: A Dict with the keys "seconds" and "microseconds" if self.format_return is True.
         """
 
         command: List = ["TIME"]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def sadd(self, key: str, *members: Any) -> ResponseType:
+    def sadd(self, key: str, *members: str) -> ResponseT:
         """
         See https://redis.io/commands/sadd
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be added.")
 
         command: List = ["SADD", key, *members]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def scard(self, key: str) -> ResponseType:
+    def scard(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/scard
         """
 
         command: List = ["SCARD", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def sdiff(self, *keys: str) -> ResponseType:
+    def sdiff(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/sdiff
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["SDIFF", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def sdiffstore(self, destination: str, *keys: str) -> ResponseType:
+    def sdiffstore(self, destination: str, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/sdiffstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["SDIFFSTORE", destination, *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def sinter(self, *keys: str) -> ResponseType:
+    def sinter(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/sinter
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["SINTER", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def sinterstore(self, destination: str, *keys: str) -> ResponseType:
+    def sinterstore(self, destination: str, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/sinterstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["SINTERSTORE", destination, *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def sismember(self, key: str, member: Any) -> ResponseType:
+    def sismember(self, key: str, member: str) -> ResponseT:
         """
         See https://redis.io/commands/sismember
-
-        :return: A bool if self.format_return is True.
         """
 
         command: List = ["SISMEMBER", key, member]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def smembers(self, key: str) -> ResponseType:
+    def smembers(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/smembers
         """
 
         command: List = ["SMEMBERS", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def smismember(self, key: str, *members: Any) -> ResponseType:
+    def smismember(self, key: str, *members: str) -> ResponseT:
         """
         See https://redis.io/commands/smismember
-
-        :return: A bool list if self.format_return is True.
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be removed.")
 
         command: List = ["SMISMEMBER", key, *members]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def smove(self, source: str, destination: str, member: Any) -> ResponseType:
+    def smove(self, source: str, destination: str, member: str) -> ResponseT:
         """
         See https://redis.io/commands/smove
-
-        :return: A bool if self.format_return is True.
         """
 
         command: List = ["SMOVE", source, destination, member]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def spop(self, key: str, count: Union[int, None] = None) -> ResponseType:
+    def spop(self, key: str, count: Union[int, None] = None) -> ResponseT:
         """
         See https://redis.io/commands/spop
-
-        :param count: defaults to 1 on the server side
         """
 
         command: List = ["SPOP", key]
 
         if count is not None:
             command.append(count)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def srandmember(self, key: str, count: Union[int, None] = None) -> ResponseType:
+    def srandmember(self, key: str, count: Union[int, None] = None) -> ResponseT:
         """
         See https://redis.io/commands/srandmember
-
-        :param count: defaults to 1 on the server side
         """
 
         command: List = ["SRANDMEMBER", key]
 
         if count is not None:
             command.append(count)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def srem(self, key: str, *members: Any) -> ResponseType:
+    def srem(self, key: str, *members: str) -> ResponseT:
         """
         See https://redis.io/commands/srem
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be removed.")
 
         command: List = ["SREM", key, *members]
 
-        return self.run(command)
+        return self.execute(command)
 
     def sscan(
         self,
         key: str,
         cursor: int = 0,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/sscan
-
-        :param match_pattern: replacement for "MATCH"
-
-        :return: The cursor will be an integer if "format_return" is True.
         """
 
         command: List = ["SSCAN", key, cursor]
 
-        if match_pattern is not None:
-            command.extend(["MATCH", match_pattern])
+        if match is not None:
+            command.extend(["MATCH", match])
 
         if count is not None:
             command.extend(["COUNT", count])
 
         # The raw result is composed of the new cursor and the List of elements.
-        return self.run(command)
+        return self.execute(command)
 
-    def sunion(self, *keys: str) -> ResponseType:
+    def sunion(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/sunion
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["SUNION", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def sunionstore(self, destination: str, *keys: str) -> ResponseType:
+    def sunionstore(self, destination: str, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/sunionstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["SUNIONSTORE", destination, *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
     def zadd(
         self,
         key: str,
-        score_member_pairs: Dict,
+        scores: Dict[str, float],
         nx: bool = False,
         xx: bool = False,
         gt: bool = False,
         lt: bool = False,
         ch: bool = False,
         incr: bool = False,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zadd
-
-        :param score_member_pairs: a Dict containing members and their scores.
-
-        :return: A float representing the number of elements added or None if "incr" is False
-        and "format_return" is True.
         """
 
         if nx and xx:
             raise Exception('"nx" and "xx" are mutually exclusive.')
 
         if gt and lt:
             raise Exception('"gt" and "lt" are mutually exclusive.')
@@ -1548,111 +1458,90 @@
 
         if ch:
             command.append("CH")
 
         if incr:
             command.append("INCR")
 
-        for name, score in score_member_pairs.items():
+        for name, score in scores.items():
             command.extend([score, name])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zcard(self, key: str) -> ResponseType:
+    def zcard(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/zcard
         """
 
         command: List = ["ZCARD", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zcount(
-        self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
-    ) -> ResponseType:
+    def zcount(self, key: str, min: FloatMinMaxT, max: FloatMinMaxT) -> ResponseT:
         """
         See https://redis.io/commands/zcount
 
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
-
         If you need to use "-inf" and "+inf", please write them as strings.
         """
 
-        command: List = ["ZCOUNT", key, min_score, max_score]
+        command: List = ["ZCOUNT", key, min, max]
 
-        return self.run(command)
+        return self.execute(command)
 
-    """
-    This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be List[str].
-    """
-
-    def zdiff(self, keys: List[str], withscores: bool = False) -> ResponseType:
+    def zdiff(self, keys: List[str], withscores: bool = False) -> ResponseT:
         """
         See https://redis.io/commands/zdiff
 
         The number of keys is calculated automatically.
-
-        :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["ZDIFF", len(keys), *keys]
 
         if withscores:
             command.append("WITHSCORES")
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zdiffstore(self, destination: str, keys: List[str]) -> ResponseType:
+    def zdiffstore(self, destination: str, keys: List[str]) -> ResponseT:
         """
         See https://redis.io/commands/zdiffstore
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["ZDIFFSTORE", destination, len(keys), *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zincrby(self, key: str, increment: float, member: str) -> ResponseType:
+    def zincrby(self, key: str, increment: float, member: str) -> ResponseT:
         """
         See https://redis.io/commands/zincrby
-
-        :return: A float if "format_return" is True.
         """
 
         command: List = ["ZINCRBY", key, increment, member]
 
-        return self.run(command)
-
-    """
-    This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be List[str].
-    """
+        return self.execute(command)
 
     def zinter(
         self,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zinter
 
         The number of keys is calculated automatically.
-
-        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["ZINTER", len(keys), *keys]
 
@@ -1661,23 +1550,23 @@
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
         if withscores:
             command.append("WITHSCORES")
 
-        return self.run(command)
+        return self.execute(command)
 
     def zinterstore(
         self,
         destination: str,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zinterstore
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
@@ -1687,456 +1576,375 @@
 
         if weights:
             command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zlexcount(self, key: str, min_score: str, max_score: str) -> ResponseType:
+    def zlexcount(self, key: str, min: str, max: str) -> ResponseT:
         """
         See https://redis.io/commands/zlexcount
-
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
         """
 
-        if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
+        if not min.startswith(("(", "[", "+", "-")) or not max.startswith(
             ("(", "[", "+", "-")
         ):
             raise Exception(
-                "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
+                "\"min\" and \"max\" must either start with '(' or '[' or be '+' or '-'."
             )
 
-        command: List = ["ZLEXCOUNT", key, min_score, max_score]
+        command: List = ["ZLEXCOUNT", key, min, max]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zmscore(self, key: str, members: List[str]) -> ResponseType:
+    def zmscore(self, key: str, members: List[str]) -> ResponseT:
         """
         See https://redis.io/commands/zmscore
-
-        :return: A List of float or None values if "format_return" is True.
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be specified.")
 
         command: List = ["ZMSCORE", key, *members]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zpopmax(self, key: str, count: Union[int, None] = None) -> ResponseType:
+    def zpopmax(self, key: str, count: Union[int, None] = None) -> ResponseT:
         """
         See https://redis.io/commands/zpopmax
-
-        :param count: defaults to 1 on the server side
-
-        :return: A Dict of member-score pairs if "format_return" is True.
         """
 
         command: List = ["ZPOPMAX", key]
 
         if count is not None:
             command.append(count)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zpopmin(self, key: str, count: Union[int, None] = None) -> ResponseType:
+    def zpopmin(self, key: str, count: Union[int, None] = None) -> ResponseT:
         """
         See https://redis.io/commands/zpopmin
-
-        :param count: defaults to 1 on the server side
-
-        :return: A Dict of member-score pairs if "format_return" is True.
         """
 
         command: List = ["ZPOPMIN", key]
 
         if count is not None:
             command.append(count)
 
-        return self.run(command)
+        return self.execute(command)
 
     def zrandmember(
         self, key: str, count: Union[int, None] = None, withscores: bool = False
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrandmember
-
-        :param count: defaults to 1 on the server side
-
-        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if count is None and withscores:
             raise Exception('"withscores" can only be used with "count".')
 
         command: List = ["ZRANDMEMBER", key]
 
         if count is not None:
             command.append(count)
 
             if withscores:
                 command.append("WITHSCORES")
 
-        return self.run(command)
-
-    """
-    This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be List[str].
-    """
+        return self.execute(command)
 
     def zrange(
         self,
         key: str,
-        start: FloatMinMax,
-        stop: FloatMinMax,
-        range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
+        start: FloatMinMaxT,
+        stop: FloatMinMaxT,
+        sortby: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
         withscores: bool = False,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrange
 
         If you need to use "-inf" and "+inf", please write them as strings.
-
-        :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
-        handle_non_deprecated_zrange_exceptions(
-            range_method, start, stop, limit_offset, limit_count
-        )
+        handle_non_deprecated_zrange_exceptions(sortby, start, stop, offset, count)
 
         command: List = ["ZRANGE", key, start, stop]
 
-        if range_method:
-            command.append(range_method)
+        if sortby:
+            command.append(sortby)
 
         if rev:
             command.append("REV")
 
-        if limit_offset is not None:
-            command.extend(["LIMIT", limit_offset, limit_count])
+        if offset is not None:
+            command.extend(["LIMIT", offset, count])
 
         if withscores:
             command.append("WITHSCORES")
 
-        return self.run(command)
+        return self.execute(command)
 
     def zrangebylex(
         self,
         key: str,
-        min_score: str,
-        max_score: str,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
-    ) -> ResponseType:
+        min: str,
+        max: str,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrangebylex
-
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
         """
 
-        handle_zrangebylex_exceptions(min_score, max_score, limit_offset, limit_count)
+        handle_zrangebylex_exceptions(min, max, offset, count)
 
-        command: List = ["ZRANGEBYLEX", key, min_score, max_score]
+        command: List = ["ZRANGEBYLEX", key, min, max]
 
-        if limit_offset is not None:
-            command.extend(["LIMIT", limit_offset, limit_count])
+        if offset is not None:
+            command.extend(["LIMIT", offset, count])
 
-        return self.run(command)
-
-    """
-    This has actually 3 return scenarios, but, 
-    whether "withscores" is True or not, its raw return type will be List[str].
-    """
+        return self.execute(command)
 
     def zrangebyscore(
         self,
         key: str,
-        min_score: FloatMinMax,
-        max_score: FloatMinMax,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
         withscores: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
-    ) -> ResponseType:
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
-
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
-
-        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
-        if number_are_not_none(limit_offset, limit_count, number=1):
+        if number_are_not_none(offset, count, number=1):
             raise Exception('Both "offset" and "count" must be specified.')
 
-        command: List = ["ZRANGEBYSCORE", key, min_score, max_score]
+        command: List = ["ZRANGEBYSCORE", key, min, max]
 
-        if limit_offset is not None:
-            command.extend(["LIMIT", limit_offset, limit_count])
+        if offset is not None:
+            command.extend(["LIMIT", offset, count])
 
         if withscores:
             command.append("WITHSCORES")
 
-        return self.run(command)
+        return self.execute(command)
 
     def zrangestore(
         self,
         dst: str,
         src: str,
-        start: FloatMinMax,
-        stop: FloatMinMax,
-        range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
+        sortby: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
-    ) -> ResponseType:
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrangestore
-
-        :param start: replacement for "MIN"
-        :param stop: replacement for "MAX"
         """
 
-        handle_non_deprecated_zrange_exceptions(
-            range_method, start, stop, limit_offset, limit_count
-        )
+        handle_non_deprecated_zrange_exceptions(sortby, min, max, offset, count)
 
-        command: List = ["ZRANGESTORE", dst, src, start, stop]
+        command: List = ["ZRANGESTORE", dst, src, min, max]
 
-        if range_method:
-            command.append(range_method)
+        if sortby:
+            command.append(sortby)
 
         if rev:
             command.append("REV")
 
-        if limit_offset is not None:
-            command.extend(["LIMIT", limit_offset, limit_count])
+        if offset is not None:
+            command.extend(["LIMIT", offset, count])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zrank(self, key: str, member: str) -> ResponseType:
+    def zrank(self, key: str, member: str) -> ResponseT:
         """
         See https://redis.io/commands/zrank
         """
 
         command: List = ["ZRANK", key, member]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zrem(self, key: str, *members: str) -> ResponseType:
+    def zrem(self, key: str, *members: str) -> ResponseT:
         """
         See https://redis.io/commands/zrem
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be removed.")
 
         command: List = ["ZREM", key, *members]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zremrangebylex(self, key: str, min_score: str, max_score: str) -> ResponseType:
+    def zremrangebylex(self, key: str, min: str, max: str) -> ResponseT:
         """
         See https://redis.io/commands/zremrangebylex
-
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
         """
 
-        if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
+        if not min.startswith(("(", "[", "+", "-")) or not max.startswith(
             ("(", "[", "+", "-")
         ):
             raise Exception(
-                "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
+                "\"min\" and \"max\" must either start with '(' or '[' or be '+' or '-'."
             )
 
-        command: List = ["ZREMRANGEBYLEX", key, min_score, max_score]
+        command: List = ["ZREMRANGEBYLEX", key, min, max]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zremrangebyrank(self, key: str, start: int, stop: int) -> ResponseType:
+    def zremrangebyrank(self, key: str, start: int, stop: int) -> ResponseT:
         """
         See https://redis.io/commands/zremrangebyrank
         """
 
         command: List = ["ZREMRANGEBYRANK", key, start, stop]
 
-        return self.run(command)
+        return self.execute(command)
 
     def zremrangebyscore(
-        self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
-    ) -> ResponseType:
+        self, key: str, min: FloatMinMaxT, max: FloatMinMaxT
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zremrangebyscore\
-        
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
 
         If you need to use "-inf" and "+inf", please write them as strings.
         """
 
-        command: List = ["ZREMRANGEBYSCORE", key, min_score, max_score]
-
-        return self.run(command)
+        command: List = ["ZREMRANGEBYSCORE", key, min, max]
 
-    """
-    This has actually 3 return scenarios, but,
-    whether "with_scores" is True or not, its raw return type will be List[str].
-    """
+        return self.execute(command)
 
     def zrevrange(
         self, key: str, start: int, stop: int, withscores: bool = False
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrevrange
-
-        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         command: List = ["ZREVRANGE", key, start, stop]
 
         if withscores:
             command.append("WITHSCORES")
 
-        return self.run(command)
+        return self.execute(command)
 
     def zrevrangebylex(
         self,
         key: str,
-        max_score: str,
-        min_score: str,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
-    ) -> ResponseType:
+        max: str,
+        min: str,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrevrangebylex
-
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
         """
 
-        handle_zrangebylex_exceptions(min_score, max_score, limit_offset, limit_count)
-
-        command: List = ["ZREVRANGEBYLEX", key, max_score, min_score]
+        handle_zrangebylex_exceptions(min, max, offset, count)
 
-        if limit_offset is not None:
-            command.extend(["LIMIT", limit_offset, limit_count])
+        command: List = ["ZREVRANGEBYLEX", key, max, min]
 
-        return self.run(command)
+        if offset is not None:
+            command.extend(["LIMIT", offset, count])
 
-    """
-    This has actually 3 return scenarios, but,
-    whether "withscores" is True or not, its raw return type will be List[str].
-    """
+        return self.execute(command)
 
     def zrevrangebyscore(
         self,
         key: str,
-        max_score: FloatMinMax,
-        min_score: FloatMinMax,
+        max: FloatMinMaxT,
+        min: FloatMinMaxT,
         withscores: bool = False,
-        limit_offset: Union[int, None] = None,
-        limit_count: Union[int, None] = None,
-    ) -> ResponseType:
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zrevrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
-
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
-
-        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
-        if number_are_not_none(limit_offset, limit_count, number=1):
-            raise Exception('Both "limit_offset" and "limit_count" must be specified.')
+        if number_are_not_none(offset, count, number=1):
+            raise Exception('Both "offset" and "count" must be specified.')
 
-        command: List = ["ZREVRANGEBYSCORE", key, max_score, min_score]
+        command: List = ["ZREVRANGEBYSCORE", key, max, min]
 
-        if limit_offset is not None:
-            command.extend(["LIMIT", limit_offset, limit_count])
+        if offset is not None:
+            command.extend(["LIMIT", offset, count])
 
         if withscores:
             command.append("WITHSCORES")
 
-        return self.run(command)
+        return self.execute(command)
 
-    def zrevrank(self, key: str, member: str) -> ResponseType:
+    def zrevrank(self, key: str, member: str) -> ResponseT:
         """
         See https://redis.io/commands/zrevrank
         """
 
         command: List = ["ZREVRANK", key, member]
 
-        return self.run(command)
+        return self.execute(command)
 
     def zscan(
         self,
         key: str,
         cursor: int,
-        match_pattern: Union[str, None] = None,
+        match: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zscan
-
-        :param match_pattern: replacement for "MATCH"
         """
 
         command: List = ["ZSCAN", key, cursor]
 
-        if match_pattern is not None:
-            command.extend(["MATCH", match_pattern])
+        if match is not None:
+            command.extend(["MATCH", match])
 
         if count is not None:
             command.extend(["COUNT", count])
 
         # The raw result is composed of the new cursor and the List of elements.
-        return self.run(command)
+        return self.execute(command)
 
-    def zscore(self, key: str, member: str) -> ResponseType:
+    def zscore(self, key: str, member: str) -> ResponseT:
         """
         See https://redis.io/commands/zscore
-
-        :return: A float or None if "format_return" is True.
         """
 
         command: List = ["ZSCORE", key, member]
 
-        return self.run(command)
-
-    """
-    This has actually 3 return scenarios, but,
-    whether "withscores" is True or not, its raw return type will be List[str].
-    """
+        return self.execute(command)
 
     def zunion(
         self,
         keys: List[str],
-        weights: Union[List[float], List[int], None] = None,
+        weights: Union[List[float], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zunion
 
         The number of keys is calculated automatically.
-
-        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["ZUNION", len(keys), *keys]
 
@@ -2145,23 +1953,23 @@
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
         if withscores:
             command.append("WITHSCORES")
 
-        return self.run(command)
+        return self.execute(command)
 
     def zunionstore(
         self,
         destination: str,
         keys: List[str],
         weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/zunionstore
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
@@ -2171,70 +1979,70 @@
 
         if weights:
             command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def append(self, key: str, value: Any) -> ResponseType:
+    def append(self, key: str, value: str) -> ResponseT:
         """
         See https://redis.io/commands/append
         """
 
         command: List = ["APPEND", key, value]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def decr(self, key: str) -> ResponseType:
+    def decr(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/decr
         """
 
         command: List = ["DECR", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def decrby(self, key: str, decrement: int) -> ResponseType:
+    def decrby(self, key: str, decrement: int) -> ResponseT:
         """
         See https://redis.io/commands/decrby
         """
 
         command: List = ["DECRBY", key, decrement]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def get(self, key: str) -> ResponseType:
+    def get(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/get
         """
 
         command: List = ["GET", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def getdel(self, key: str) -> ResponseType:
+    def getdel(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/getdel
         """
 
         command: List = ["GETDEL", key]
 
-        return self.run(command)
+        return self.execute(command)
 
     def getex(
         self,
         key: str,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         persist: Union[bool, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/getex
         """
 
         if (ex or px or exat or pxat or persist) and not number_are_not_none(
             ex, px, exat, pxat, persist, number=1
         ):
@@ -2253,121 +2061,119 @@
 
         if pxat is not None:
             command.extend(["PXAT", pxat])
 
         if persist is not None:
             command.append("PERSIST")
 
-        return self.run(command)
+        return self.execute(command)
 
-    def getrange(self, key: str, start: int, end: int) -> ResponseType:
+    def getrange(self, key: str, start: int, end: int) -> ResponseT:
         """
         See https://redis.io/commands/getrange
         """
 
         command: List = ["GETRANGE", key, start, end]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def getset(self, key: str, value: Any) -> ResponseType:
+    def getset(self, key: str, value: str) -> ResponseT:
         """
         See https://redis.io/commands/getset
         """
 
         command: List = ["GETSET", key, value]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def incr(self, key: str) -> ResponseType:
+    def incr(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/incr
         """
 
         command: List = ["INCR", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def incrby(self, key: str, increment: int) -> ResponseType:
+    def incrby(self, key: str, increment: int) -> ResponseT:
         """
         See https://redis.io/commands/incrby
         """
 
         command: List = ["INCRBY", key, increment]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def incrbyfloat(self, key: str, increment: float) -> ResponseType:
+    def incrbyfloat(self, key: str, increment: float) -> ResponseT:
         """
         See https://redis.io/commands/incrbyfloat
-
-        :return: A float if "format_return" is True.
         """
 
         command: List = ["INCRBYFLOAT", key, increment]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def mget(self, *keys: str) -> ResponseType:
+    def mget(self, *keys: str) -> ResponseT:
         """
         See https://redis.io/commands/mget
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: List = ["MGET", *keys]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def mset(self, key_value_pairs: Dict) -> ResponseType:
+    def mset(self, values: Dict[str, str]) -> ResponseT:
         """
         See https://redis.io/commands/mset
         """
 
         command: List = ["MSET"]
 
-        for key, value in key_value_pairs.items():
+        for key, value in values.items():
             command.extend([key, value])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def msetnx(self, key_value_pairs: Dict) -> ResponseType:
+    def msetnx(self, values: Dict[str, str]) -> ResponseT:
         """
         See https://redis.io/commands/msetnx
         """
 
         command: List = ["MSETNX"]
 
-        for key, value in key_value_pairs.items():
+        for key, value in values.items():
             command.extend([key, value])
 
-        return self.run(command)
+        return self.execute(command)
 
-    def psetex(self, key: str, milliseconds: int, value: Any) -> ResponseType:
+    def psetex(self, key: str, milliseconds: int, value: str) -> ResponseT:
         """
         See https://redis.io/commands/psetex
         """
 
         command: List = ["PSETEX", key, milliseconds, value]
 
-        return self.run(command)
+        return self.execute(command)
 
     def set(
         self,
         key: str,
         value: Any,
         nx: Union[bool, None] = None,
         xx: Union[bool, None] = None,
         get: Union[bool, None] = None,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
         keepttl: Union[bool, None] = None,
-    ) -> ResponseType:
+    ) -> ResponseT:
         """
         See https://redis.io/commands/set
         """
 
         if nx and xx:
             raise Exception('"nx" and "xx" are mutually exclusive.')
 
@@ -2401,167 +2207,131 @@
 
         if pxat is not None:
             command.extend(["PXAT", pxat])
 
         if keepttl:
             command.append("KEEPTTL")
 
-        return self.run(command)
+        return self.execute(command)
 
-    def setex(self, key: str, seconds: int, value: Any) -> ResponseType:
+    def setex(self, key: str, seconds: int, value: str) -> ResponseT:
         """
         See https://redis.io/commands/setex
         """
 
         command: List = ["SETEX", key, seconds, value]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def setnx(self, key: str, value: Any) -> ResponseType:
+    def setnx(self, key: str, value: str) -> ResponseT:
         """
         See https://redis.io/commands/setnx
         """
 
         command: List = ["SETNX", key, value]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def setrange(self, key: str, offset: int, value: Any) -> ResponseType:
+    def setrange(self, key: str, offset: int, value: str) -> ResponseT:
         """
         See https://redis.io/commands/setrange
         """
 
         command: List = ["SETRANGE", key, offset, value]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def strlen(self, key: str) -> ResponseType:
+    def strlen(self, key: str) -> ResponseT:
         """
         See https://redis.io/commands/strlen
         """
 
         command: List = ["STRLEN", key]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def substr(self, key: str, start: int, end: int) -> ResponseType:
+    def substr(self, key: str, start: int, end: int) -> ResponseT:
         """
         See https://redis.io/commands/substr
         """
 
         command: List = ["SUBSTR", key, start, end]
 
-        return self.run(command)
+        return self.execute(command)
 
-    def script_exists(self, *sha1: str) -> ResponseType:
+    def script_exists(self, *sha1: str) -> ResponseT:
         """
         See https://redis.io/commands/script-exists
-
-        :return: A List of bools if "format_return" is True.
         """
 
         if len(sha1) == 0:
             raise Exception("At least one sha1 digests must be provided.")
 
         command: List = ["SCRIPT", "EXISTS", *sha1]
 
-        return self.run(command)
+        return self.execute(command)
 
     def script_flush(
-        self, mode: Optional[Literal["ASYNC", "SYNC"]] = None
-    ) -> ResponseType:
+        self, flush_type: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> ResponseT:
         """
         See https://redis.io/commands/script-flush
         """
 
         command: List = ["SCRIPT", "FLUSH"]
 
-        if mode:
-            command.append(mode)
+        if flush_type:
+            command.append(flush_type)
 
-        return self.run(command)
+        return self.execute(command)
 
-    def script_load(self, script: str) -> ResponseType:
+    def script_load(self, script: str) -> ResponseT:
         """
         See https://redis.io/commands/script-load
         """
 
         command: List = ["SCRIPT", "LOAD", script]
 
-        return self.run(command)
-
-    # def pubsub_channels(self, pattern: Union[str, None] = None) -> ResponseType:
-    #     """
-    #     See https://redis.io/commands/pubsub-channels
-    #     """
-
-    #     command: List = ["PUBSUB", "CHANNELS"]
-
-    #     if pattern is not None:
-    #         command.append(pattern)
-
-    #     return self.run(command)
-
-    # def pubsub_numpat(self) -> ResponseType:
-    #     """
-    #     See https://redis.io/commands/pubsub-numpat
-    #     """
-
-    #     command: List = ["PUBSUB", "NUMPAT"]
-
-    #     return self.run(command)
-
-    # def pubsub_numsub(
-    #     self, *channels: str
-    # ) -> ResponseType:
-    #     """
-    #     See https://redis.io/commands/pubsub-numsub
-
-    #     :return: A Dict with channel-number_of_subscribers pairs if "format_return" is True.
-    #     """
-
-    #     command: List = ["PUBSUB", "NUMSUB", *channels]
-
-    #     return self.run(command)
+        return self.execute(command)
 
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
     def __init__(self, client: Commands, key: str):
         self.client = client
         self.command: List = ["BITFIELD", key]
 
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands":
+    def get(self, encoding: str, offset: Union[int, str]) -> "BitFieldCommands":
         """
         Returns the specified bit field.
 
         Source: https://redis.io/commands/bitfield
         """
 
         _command = ["GET", encoding, offset]
         self.command.extend(_command)
 
         return self
 
     def set(
-        self, encoding: str, offset: BitFieldOffset, value: int
+        self, encoding: str, offset: Union[int, str], value: int
     ) -> "BitFieldCommands":
         """
         Set the specified bit field and returns its old value.
 
         Source: https://redis.io/commands/bitfield
         """
 
         _command = ["SET", encoding, offset, value]
         self.command.extend(_command)
 
         return self
 
     def incrby(
-        self, encoding: str, offset: BitFieldOffset, increment: int
+        self, encoding: str, offset: Union[int, str], increment: int
     ) -> "BitFieldCommands":
         """
         Increments or decrements (if a negative increment is given) the specified bit field and returns the new value.
 
         Source: https://redis.io/commands/bitfield
         """
 
@@ -2583,123 +2353,35 @@
         """
 
         _command = ["OVERFLOW", overflow]
         self.command.extend(_command)
 
         return self
 
-    def execute(self) -> ResponseType:
-        return self.client.run(command=self.command)
+    def execute(self) -> ResponseT:
+        return self.client.execute(command=self.command)
 
 
-class BitFieldRO:
+class BitFieldROCommands:
     def __init__(self, client: Commands, key: str):
         self.client = client
         self.command: List = ["BITFIELD_RO", key]
 
-    def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO":
+    def get(self, encoding: str, offset: Union[int, str]) -> "BitFieldROCommands":
         """
         Returns the specified bit field.
 
         Source: https://redis.io/commands/bitfield_ro
         """
 
         _command = ["GET", encoding, offset]
         self.command.extend(_command)
 
         return self
 
-    def execute(self) -> ResponseType:
-        return self.client.run(command=self.command)
-
-
-"""
-class ACL:
-    def __init__(self, client: Commands):
-        self.client = client
-
-    async def cat(self, category: Union[str, None] = None) -> List[str]:
-        # See https://redis.io/commands/acl-cat
-
-        command: List = ["ACL", "CAT"]
-
-        if category is not None:
-            command.append(category)
-
-        return await self.client.run(command=command)
-
-    async def deluser(self, *usernames: str) -> int:
-        # See https://redis.io/commands/acl-deluser
-        
-        if len(usernames) == 0:
-            raise Exception("At least one username must be provided.")
-
-        command: List = ["ACL", "DELUSER", *usernames]
-
-        return await self.client.run(command=command)
-
-    async def genpass(self, bits: Union[int, None] = None) -> str:
-        # See https://redis.io/commands/acl-genpass
-
-        command: List = ["ACL", "GENPASS"]
-
-        if bits is not None:
-            command.append(bits)
-
-        return await self.client.run(command=command)
-
-    # Is it possible to format this output?
-    async def getuser(self, username: str) -> Union[List[str], None]:
-        # See https://redis.io/commands/acl-getuser
-
-        command: List = ["ACL", "GETUSER", username]
-
-        return await self.client.run(command=command)
-
-    async def List_rules(self) -> List[str]:
-        # See https://redis.io/commands/acl-List
-
-        command = ["ACL", "LIST"]
-
-        return await self.client.run(command=command)
-
-    async def load(self) -> str:
-        # See https://redis.io/commands/acl-load
-
-        command = ["ACL", "LOAD"]
-
-        return await self.client.run(command=command)
-
-    async def log(self, count: Union[int, None] = None, reset: bool = False) -> List[str]:
-        # See https://redis.io/commands/acl-log
-
-        if count is not None and reset:
-            raise Exception("Cannot specify both "count" and "reset".")
-
-        command: List = ["ACL", "LOG"]
-
-        if count is not None:
-            command.append(count)
-
-        if reset:
-            command.append("RESET")
-
-        return await self.client.run(command=command)
-
-    async def save(self, count: Union[int, None] = None, reset: bool = False) -> List[str]:
-        # See https://redis.io/commands/acl-save
-
-        command: List = ["ACL", "SAVE"]
-
-        return await self.client.run(command=command)
-
-    async def setuser():
-        ...
-    
-    async def users():
-        ...
-
-    async def whoami():
-        ...
+    def execute(self) -> ResponseT:
+        return self.client.execute(command=self.command)
 
 
-"""
+AsyncCommands = Commands
+AsyncBitFieldCommands = BitFieldCommands
+AsyncBitFieldROCommands = BitFieldROCommands
```

### Comparing `upstash_redis-0.14.5/upstash_redis/utils/exception.py` & `upstash_redis-0.15.0/upstash_redis/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,88 @@
-from upstash_redis.schema.commands.parameters import FloatMinMax
-from upstash_redis.utils.comparison import number_are_not_none
-from typing import Literal, Union
+from typing import Any, Literal, Union
+
+from upstash_redis.typing import FloatMinMaxT
+
+
+def number_are_not_none(*parameters: Any, number: int) -> bool:
+    """
+    Check if "number" of the given parameters are not None.
+    """
+
+    return sum(parameter is not None for parameter in parameters) == number
 
 
 def handle_georadius_write_exceptions(
     withdist: bool = False,
     withhash: bool = False,
     withcoord: bool = False,
     count: Union[int, None] = None,
-    count_any: bool = False,
+    any: bool = False,
     store: Union[str, None] = None,
     storedist: Union[str, None] = None,
 ) -> None:
     """
     Handle exceptions for "GEORADIUS*" write commands.
     """
 
-    if count_any and count is None:
-        raise Exception('"count_any" can only be used together with "count".')
+    if any and count is None:
+        raise Exception('"any" can only be used together with "count".')
 
     if (withdist or withhash or withcoord) and (store or storedist):
         raise Exception(
             'Cannot use "store" or "storedist" when requesting additional properties.'
         )
 
 
 def handle_geosearch_exceptions(
     member: Union[str, None],
-    fromlonlat_longitude: Union[float, None],
-    fromlonlat_latitude: Union[float, None],
-    byradius: Union[float, None],
-    bybox_width: Union[float, None],
-    bybox_height: Union[float, None],
+    longitude: Union[float, None],
+    latitude: Union[float, None],
+    radius: Union[float, None],
+    width: Union[float, None],
+    height: Union[float, None],
     count: Union[int, None],
-    count_any: bool,
+    any: bool,
 ) -> None:
     """
     Handle exceptions for "GEOSEARCH*" commands.
     """
 
-    if number_are_not_none(fromlonlat_longitude, fromlonlat_latitude, number=1):
-        raise Exception(
-            'Both "fromlonlat_longitude" and "fromlonlat_latitude" must be specified.'
-        )
+    if number_are_not_none(longitude, latitude, number=1):
+        raise Exception('Both "longitude" and "latitude" must be specified.')
 
-    if number_are_not_none(bybox_width, bybox_height, number=1):
-        raise Exception('Both "bybox_width" and "bybox_height" must be specified.')
+    if number_are_not_none(width, height, number=1):
+        raise Exception('Both "width" and "height" must be specified.')
 
-    if not number_are_not_none(member, fromlonlat_longitude, number=1):
+    if not number_are_not_none(member, longitude, number=1):
         raise Exception(
-            """Specify either the member's name with "member",
-or the fromlonlat_longitude and fromlonlat_latitude with "fromlonlat_longitude" and "fromlonlat_latitude", but not both."""
+            """Specify either the member's name with "member", or the "longitude" and "latitude", but not both."""
         )
 
-    if not number_are_not_none(byradius, bybox_width, number=1):
+    if not number_are_not_none(radius, width, number=1):
         raise Exception(
-            """Specify either the byradius with "byradius",
-or the bybox_width and bybox_height with "bybox_width" and "bybox_height", but not both."""
+            """Specify either the "radius", or the "width" and "height", but not both."""
         )
 
-    if count_any and count is None:
-        raise Exception('"count_any" can only be used together with "count".')
+    if any and count is None:
+        raise Exception('"any" can only be used together with "count".')
 
 
 def handle_non_deprecated_zrange_exceptions(
-    range_method: Union[Literal["BYLEX", "BYSCORE"], None],
-    start: FloatMinMax,
-    stop: FloatMinMax,
+    sortby: Union[Literal["BYLEX", "BYSCORE"], None],
+    start: FloatMinMaxT,
+    stop: FloatMinMaxT,
     offset: Union[int, None],
     count: Union[int, None],
 ) -> None:
     """
     Handle exceptions for non-deprecated "ZRANGE*" commands.
     """
 
-    if range_method == "BYLEX" and (
+    if sortby == "BYLEX" and (
         not (isinstance(start, str) and isinstance(stop, str))
         or not (
             start.startswith(("(", "[", "+", "-"))
             and stop.startswith(("(", "[", "+", "-"))
         )
     ):
         raise Exception(
@@ -87,28 +91,25 @@
         )
 
     if number_are_not_none(offset, count, number=1):
         raise Exception('Both "offset" and "count" must be specified.')
 
 
 def handle_zrangebylex_exceptions(
-    min_score: str,
-    max_score: str,
+    min: str,
+    max: str,
     offset: Union[int, None],
     count: Union[int, None],
 ) -> None:
     """
     Handle exceptions for "ZRANGEBYLEX" and "ZREVRANGEBYLEX" commands.
-
-    :param min_score: replacement for "MIN"
-    :param max_score: replacement for "MAX"
     """
 
-    if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
+    if not min.startswith(("(", "[", "+", "-")) or not max.startswith(
         ("(", "[", "+", "-")
     ):
         raise Exception(
-            "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
+            "\"min\" and \"max\" must either start with '(' or '[' or be '+' or '-'."
         )
 
     if number_are_not_none(offset, count, number=1):
         raise Exception('Both "offset" and "count" must be specified.')
```

### Comparing `upstash_redis-0.14.5/upstash_redis/utils/format.py` & `upstash_redis-0.15.0/upstash_redis/format.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,117 @@
-from typing import Literal, Tuple, Union, List, Dict
+from typing import Callable, Dict, List, Literal, Tuple, Union
 
+from upstash_redis.typing import GeoSearchResult
 
-def _list_to_dict(raw: List, command=None) -> Dict:
+
+def list_to_dict(raw: List, command=None) -> Dict:
     """
     Convert a list that contains ungrouped pairs as consecutive elements (usually field-value or similar) into a dict.
     """
 
     return {raw[iterator]: raw[iterator + 1] for iterator in range(0, len(raw), 2)}
 
 
-def format_geo_positions_return(
+def format_geopos(
     raw: List[Union[List[str], None]], command=None
-) -> List[Union[Dict[str, float], None]]:
-    """
-    Format the raw output returned by "GEOPOS".
-    """
-
+) -> List[Union[Tuple[float, float], None]]:
     return [
-        {"longitude": float(member[0]), "latitude": float(member[1])}
-        if isinstance(member, List)
-        else None
+        (float(member[0]), float(member[1])) if isinstance(member, List) else None
         for member in raw
     ]
 
 
-def format_geo_members_return(
-    raw: List[Union[str, List[Union[str, List[str]]]]],
-    with_distance: Union[bool, None],
-    with_hash: Union[bool, None],
-    with_coordinates: Union[bool, None],
-) -> List[Dict[str, Union[str, float, int]]]:
+def format_geo_search_result(
+    raw: List[List[Union[str, List[str]]]],
+    with_distance: bool,
+    with_hash: bool,
+    with_coordinates: bool,
+) -> List[GeoSearchResult]:
     """
     Format the raw output given by some Geo commands, usually the ones that return properties of members,
     when additional properties are requested.
 
-    Note that the output's type might differ from the "GeoMember" type that represents the initial properties of
-    a geo member.
-
     They generally return, if requested, in order:
      - the distance (float)
      - the hash (int)
      - the coordinates as:
         - the longitude
         - the latitude
 
     All represented as strings
     """
 
-    result: List[Dict[str, Union[str, float, int]]] = []
+    result: List[GeoSearchResult] = []
+
+    # (metin): mypy has trouble narrowing down the types in this function.
+    # We can use typing.cast(str, xxx) to force it manually narrow
+    # down the types, but I don't like the idea of calling a function
+    # that has a runtime cost to just please the type checker. Until
+    # there is a better way of doing it, I wil just ignore the errors.
 
     for member in raw:
-        formatted_member: Dict[str, Union[str, float, int]] = {"member": member[0]}
+        formatted: GeoSearchResult = {"member": member[0]}  # type: ignore[typeddict-item]
 
         if with_distance:
-            formatted_member["distance"] = float(member[1])
+            formatted["distance"] = float(member[1])  # type: ignore[arg-type]
 
             if with_hash:
-                formatted_member["hash"] = int(member[2])
+                formatted["hash"] = int(member[2])  # type: ignore[arg-type]
 
                 if with_coordinates:
-                    formatted_member["longitude"] = float(member[3][0])
-                    formatted_member["latitude"] = float(member[3][1])
+                    formatted["longitude"] = float(member[3][0])  # type: ignore[arg-type]
+                    formatted["latitude"] = float(member[3][1])  # type: ignore[arg-type]
 
             elif with_coordinates:
-                formatted_member["longitude"] = float(member[2][0])
-                formatted_member["latitude"] = float(member[2][1])
+                formatted["longitude"] = float(member[2][0])  # type: ignore[arg-type]
+                formatted["latitude"] = float(member[2][1])  # type: ignore[arg-type]
 
         elif with_hash:
-            formatted_member["hash"] = int(member[1])
+            formatted["hash"] = int(member[1])  # type: ignore[arg-type]
 
             if with_coordinates:
-                formatted_member["longitude"] = float(member[2][0])
-                formatted_member["latitude"] = float(member[2][1])
+                formatted["longitude"] = float(member[2][0])  # type: ignore[arg-type]
+                formatted["latitude"] = float(member[2][1])  # type: ignore[arg-type]
 
         elif with_coordinates:
-            formatted_member["longitude"] = float(member[1][0])
-            formatted_member["latitude"] = float(member[1][1])
+            formatted["longitude"] = float(member[1][0])  # type: ignore[arg-type]
+            formatted["latitude"] = float(member[1][1])  # type: ignore[arg-type]
 
-        result.append(formatted_member)
+        result.append(formatted)
 
     return result
 
 
 def format_hash_return(raw: List[str], command=None) -> Dict[str, str]:
     """
     Format the raw output given by Hash commands, usually the ones that return the field-value
     pairs of Hashes.
     """
 
-    return _list_to_dict(raw=raw)
+    return list_to_dict(raw=raw)
 
 
 def format_pubsub_numsub_return(raw: List[Union[str, int]]) -> Dict[str, int]:
     """
     Format the raw output returned by "PUBSUB NUMSUB".
     """
 
-    return _list_to_dict(raw=raw)
+    return list_to_dict(raw=raw)
 
 
 def format_bool_list(raw: List[Literal[0, 1]]) -> List[bool]:
     """
     Format a list of boolean integers.
     """
 
     return [bool(value) for value in raw]
 
 
-def format_server_time_return(raw: List[str], command=None) -> Dict[str, int]:
-    """
-    Format the raw output returned by "TIME".
-    """
-
-    return {"seconds": int(raw[0]), "microseconds": int(raw[1])}
+def format_time(raw: List[str], command=None) -> Tuple[int, int]:
+    return (int(raw[0]), int(raw[1]))
 
 
 def format_sorted_set_return(raw: List[str], command=None) -> List[Tuple[str, float]]:
     """
     Format the raw output given by Sorted Set commands, usually the ones that return the member-score
     pairs of Sorted Sets.
     """
@@ -146,20 +141,27 @@
     return bool(res)
 
 
 def list_to_bool_list(res, command):
     return list(map(bool, res))
 
 
+def float_or_none(res, command):
+    if res is None:
+        return None
+
+    return float(res)
+
+
 def to_float(res, command):
     return float(res)
 
 
-def scan_formatter(res, command):
-    return [int(res[0]), res[1]]
+def format_scan(res, command):
+    return (int(res[0]), res[1])
 
 
 def hscan_formatter(res, command):
     return [int(res[0]), format_hash_return(res[1])]
 
 
 def sscan_formatter(res, command):  ## same with scan_formatter
@@ -170,25 +172,25 @@
     return [int(res[0]), format_sorted_set_return(res[1])]
 
 
 def zscore_formatter(res, command):
     return float(res) if res is not None else res
 
 
-def georadius_formatter(res, command):
+def format_search(res, command):
     withdist = "WITHDIST" in command
     withhash = "WITHHASH" in command
     withcoord = "WITHCOORD" in command
     if withdist or withhash or withcoord:
-        return format_geo_members_return(res, withdist, withhash, withcoord)
+        return format_geo_search_result(res, withdist, withhash, withcoord)
 
     return res
 
 
-def hrandfield_formatter(res, command):
+def format_hrandfield(res, command):
     withvalues = "WITHVALUES" in command
     if withvalues:
         return format_hash_return(res)
 
     return res
 
 
@@ -196,15 +198,15 @@
     incr = "INCR" in command
     if incr:
         return float(res) if res is not None else res
 
     return res
 
 
-def zdiff_formatter(res, command):
+def format_zdiff(res, command):
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
 
     return res
 
 
@@ -260,72 +262,71 @@
     withscores = "WITHSCORES" in command
     if withscores:
         return format_sorted_set_return(res)
 
     return res
 
 
-class FormattedResponse:
-    FORMATTERS = {
-        "COPY": to_bool,
-        "EXPIRE": to_bool,
-        "EXPIREAT": to_bool,
-        "PERSIST": to_bool,
-        "PEXPIRE": to_bool,
-        "PEXPIREAT": to_bool,
-        "RENAMENX": to_bool,
-        "SCAN": scan_formatter,
-        "GEODIST": to_float,
-        "GEOPOS": format_geo_positions_return,
-        "GEORADIUS": georadius_formatter,
-        "GEORADIUS_RO": georadius_formatter,
-        "GEORADIUSBYMEMBER": georadius_formatter,
-        "GEORADIUSBYMEMBER_RO": georadius_formatter,
-        "GEOSEARCH": georadius_formatter,
-        "HEXISTS": to_bool,
-        "HGETALL": format_hash_return,
-        "HINCRBYFLOAT": to_float,
-        "HRANDFIELD": hrandfield_formatter,
-        "HSCAN": hscan_formatter,
-        "HSETNX": to_bool,
-        "PFADD": to_bool,
-        "TIME": format_server_time_return,
-        "SISMEMBER": to_bool,
-        "SMISMEMBER": list_to_bool_list,
-        "SMOVE": to_bool,
-        "SSCAN": sscan_formatter,
-        "ZADD": zadd_formatter,
-        "ZDIFF": zdiff_formatter,
-        "ZINCRBY": to_float,
-        "ZINTER": zinter_formatter,
-        "ZMSCORE": format_float_list,
-        "ZPOPMAX": format_sorted_set_return,
-        "ZPOPMIN": format_sorted_set_return,
-        "ZRANDMEMBER": zrandmember_formatter,
-        "ZRANGE": zrange_formatter,
-        "ZRANGEBYSCORE": zrangebyscore_formatter,
-        "ZREVRANGE": zrevrange_formatter,
-        "ZREVRANGEBYSCORE": zrevrangebyscore_formatter,
-        "ZSCAN": zscan_formatter,
-        "ZSCORE": zscore_formatter,
-        "ZUNION": zunion_formatter,
-        "INCRBYFLOAT": to_float,
-        "PUBSUB NUMSUB": _list_to_dict,
-        "SCRIPT EXISTS": format_bool_list,
-        "FLUSHALL": ok_to_bool,
-        "FLUSHDB": ok_to_bool,
-        "MSETNX": to_bool,
-        "PSETEX": ok_to_bool,
-        "SET": ok_to_bool,
-        "SETEX": ok_to_bool,
-        "SETNX": to_bool,
-        "HMSET": ok_to_bool,
-        "SMEMBERS": to_set,
-        "SDIFF": to_set,
-        "SINTER": to_set,
-        "SUNION": to_set,
-        "SCRIPT FLUSH": ok_to_bool,
-        "SCRIPT EXISTS": list_to_bool_list,
-    }
-
-    # TODO: lots of duplicate formatters. unite them, especially format_sorted_set_return
-    # TODO: all formatters should take `command` parameter
+FORMATTERS: Dict[str, Callable] = {
+    "COPY": to_bool,
+    "EXPIRE": to_bool,
+    "EXPIREAT": to_bool,
+    "PERSIST": to_bool,
+    "PEXPIRE": to_bool,
+    "PEXPIREAT": to_bool,
+    "RENAME": ok_to_bool,
+    "RENAMENX": to_bool,
+    "SCAN": format_scan,
+    "GEODIST": float_or_none,
+    "GEOPOS": format_geopos,
+    "GEORADIUS": format_search,
+    "GEORADIUS_RO": format_search,
+    "GEORADIUSBYMEMBER": format_search,
+    "GEORADIUSBYMEMBER_RO": format_search,
+    "GEOSEARCH": format_search,
+    "HEXISTS": to_bool,
+    "HGETALL": format_hash_return,
+    "HINCRBYFLOAT": to_float,
+    "HRANDFIELD": format_hrandfield,
+    "HSCAN": hscan_formatter,
+    "HSETNX": to_bool,
+    "PFADD": to_bool,
+    "PFMERGE": ok_to_bool,
+    "TIME": format_time,
+    "SISMEMBER": to_bool,
+    "SMISMEMBER": list_to_bool_list,
+    "SMOVE": to_bool,
+    "SSCAN": sscan_formatter,
+    "ZADD": zadd_formatter,
+    "ZDIFF": format_zdiff,
+    "ZINCRBY": to_float,
+    "ZINTER": zinter_formatter,
+    "ZMSCORE": format_float_list,
+    "ZPOPMAX": format_sorted_set_return,
+    "ZPOPMIN": format_sorted_set_return,
+    "ZRANDMEMBER": zrandmember_formatter,
+    "ZRANGE": zrange_formatter,
+    "ZRANGEBYSCORE": zrangebyscore_formatter,
+    "ZREVRANGE": zrevrange_formatter,
+    "ZREVRANGEBYSCORE": zrevrangebyscore_formatter,
+    "ZSCAN": zscan_formatter,
+    "ZSCORE": zscore_formatter,
+    "ZUNION": zunion_formatter,
+    "INCRBYFLOAT": to_float,
+    "PUBSUB NUMSUB": list_to_dict,
+    "FLUSHALL": ok_to_bool,
+    "FLUSHDB": ok_to_bool,
+    "PSETEX": ok_to_bool,
+    "SET": ok_to_bool,
+    "SETEX": ok_to_bool,
+    "SETNX": to_bool,
+    "MSET": ok_to_bool,
+    "MSETNX": to_bool,
+    "HMSET": ok_to_bool,
+    "LSET": ok_to_bool,
+    "SMEMBERS": to_set,
+    "SDIFF": to_set,
+    "SINTER": to_set,
+    "SUNION": to_set,
+    "SCRIPT FLUSH": ok_to_bool,
+    "SCRIPT EXISTS": list_to_bool_list,
+}
```

### Comparing `upstash_redis-0.14.5/PKG-INFO` & `upstash_redis-0.15.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,86 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.14.5
-Summary: Serverless Redis Sdk from Upstash
+Version: 0.15.0
+Summary: Serverless Redis SDK from Upstash
+Home-page: https://github.com/upstash/redis-python
+License: MIT
+Keywords: Upstash Redis,Serverless Redis
 Author: Upstash
 Author-email: support@upstash.com
+Maintainer: Upstash
+Maintainer-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pytest (>=7.3.0,<8.0.0)
-Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.6,<2.0)
+Project-URL: Repository, https://github.com/upstash/redis-python
 Description-Content-Type: text/markdown
 
-# Upstash Redis - python edition
+# Upstash Redis Python SDK
 
-upstash-redis is a connectionless, HTTP-based Redis client for python, designed to be used in serverless and serverful environments such as:
+upstash-redis is a connectionless, HTTP-based Redis client for Python, designed to be used in serverless and serverful environments such as:
 - AWS Lambda
 - Vercel Serverless
 - Google Cloud Functions
 - and other environments where HTTP is preferred over TCP.
 
 Inspired by other Redis clients like [@upstash/redis](https://github.com/upstash/upstash-redis) and [redis-py](https://github.com/redis/redis-py),
-the goal of this SDK is to provide a simple way to use Redis in HTTP-based environments.
+the goal of this SDK is to provide a simple way to use Redis over the [Upstash REST API](https://docs.upstash.com/redis/features/restapi).
 
-The SDK is currently compatible with python 3.8 and above.
+The SDK is currently compatible with Python 3.8 and above.
 
 <!-- toc -->
 
-- [Upstash Redis - python edition](#upstash-redis---python-edition)
+- [Upstash Redis Python SDK](#upstash-redis-python-sdk)
 - [Quick Start](#quick-start)
   - [Install](#install)
-    - [PyPi](#pypi)
+    - [PyPI](#pypi)
   - [Usage](#usage)
     - [BITFIELD and BITFIELD\_RO](#bitfield-and-bitfield_ro)
     - [Custom commands](#custom-commands)
 - [Encoding](#encoding)
 - [Retry mechanism](#retry-mechanism)
-- [Formatting returns](#formatting-returns)
 - [Contributing](#contributing)
   - [Preparing the environment](#preparing-the-environment)
   - [Running tests](#running-tests)
 
 <!-- tocstop -->
 
 # Quick Start
 
 ## Install
 
-### PyPi
+### PyPI
 ```bash
 pip install upstash-redis
 ```
 
-
 ## Usage
 To be able to use upstash-redis, you need to create a database on [Upstash](https://console.upstash.com/)
 and grab `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` from the console.
 
 ```python
-# In this method, you can also give specific parameters for the Redis instance instance, such as rest_retries and so on
-
 # for sync client
 from upstash_redis import Redis
+
 redis = Redis(url="UPSTASH_REDIS_REST_URL", token="UPSTASH_REDIS_REST_TOKEN")
 
 # for async client
 from upstash_redis.asyncio import Redis
 
 redis = Redis(url="UPSTASH_REDIS_REST_URL", token="UPSTASH_REDIS_REST_TOKEN")
 ```
@@ -83,100 +93,76 @@
 redis = Redis.from_env()
 
 # for async use
 from upstash_redis.asyncio import Redis
 redis = Redis.from_env()
 ```
 
-
 If you are in a serverless environment that allows it, it's recommended to initialise the client outside the request handler
 to be reused while your function is still hot.
 
 Running commands might look like this:
 
 ```python
 from upstash_redis import Redis
+
 redis = Redis.from_env()
 
 def main():
   redis.set("a", "b")
   print(redis.get("a"))
 
 # or for async context:
 
 from upstash_redis.asyncio import Redis
+
 redis = Redis.from_env()
 
-async def main():
-  async with redis:
-    await redis.set("a", "b")
-    print(await redis.get("a"))
+async def main():  
+  await redis.set("a", "b")
+  print(await redis.get("a"))
 ```
 
 ### BITFIELD and BITFIELD_RO
 One particular case is represented by these two chained commands, which are available as functions that return an instance of 
 the `BITFIELD` and, respectively, `BITFIELD_RO` classes. Use the `execute` function to run the commands.
 
 ```python
-    redis.bitfield("test_key")
-    .incrby(encoding="i8", offset=100, increment=100)
-    .overflow("SAT")
-    .incrby(encoding="i8", offset=100, increment=100)
-    .execute()
-
-    redis.bitfield_ro("test_key_2")
-    .get(encoding="u8", offset=0)
-    .get(encoding="u8", offset="#1")
-    .execute()
+redis.bitfield("test_key") \
+  .incrby(encoding="i8", offset=100, increment=100) \
+  .overflow("SAT") \
+  .incrby(encoding="i8", offset=100, increment=100) \
+  .execute()
+
+redis.bitfield_ro("test_key_2") \
+  .get(encoding="u8", offset=0) \
+  .get(encoding="u8", offset="#1") \
+  .execute()
 ```
 
-
 ### Custom commands
-If you want to run a command that hasn't been implemented, you can use the `run` function of your client instance
-and pass the command as `list`
+If you want to run a command that hasn't been implemented, you can use the `execute` function of your client instance
+and pass the command as a `list`.
 
 ```python
-redis.run(command=["XLEN", "test_stream"])
+redis.execute(command=["XLEN", "test_stream"])
 ```
 
-If you want to have more control over your session management or need to use multiple custom values, use
-the [sync_execute](./upstash_redis/http/execute.py) function directly.
-
-
-
 # Encoding
 Although Redis can store invalid JSON data, there might be problems with the deserialization.
 To avoid this, the Upstash REST proxy is capable of encoding the data as base64 on the server and then sending it to the client to be
 decoded. 
 
 For very large data, this can add a few milliseconds in latency. So, if you're sure that your data is valid JSON, you can set
-`rest_encoding` to `False`.
-
+`rest_encoding` to `None`.
 
 # Retry mechanism
 upstash-redis has a fallback mechanism in case of network or API issues. By default, if a request fails it'll retry once, 3 seconds 
 after the error. If you want to customize that, set `rest_retries` and `rest_retry_interval` (in seconds).
 
-
-# Formatting returns
-The SDK relies on the Upstash REST proxy, which returns the `RESP2` responses of the given commands.
-By default, we apply formatting to some of them to provide a better developer experience.
-If you want the commands to output the raw return, set `format_return` to `False`.
-
-You can also opt out of individual commands:
-
-```python
-redis.format_return = False
-
-print(redis.copy(source="source_string", destination="destination_string"))
-
-redis.format_return = True
-```
-
-
 # Contributing
 
 ## Preparing the environment
 This project uses [Poetry](https://python-poetry.org) for packaging and dependency management. Make sure you are able to create the poetry shell with relevant dependencies.
 
 You will also need a database on [Upstash](https://console.upstash.com/).
```

