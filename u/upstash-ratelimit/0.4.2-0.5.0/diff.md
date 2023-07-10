# Comparing `tmp/upstash_ratelimit-0.4.2.tar.gz` & `tmp/upstash_ratelimit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.4.2.tar", max compression
+gzip compressed data, was "upstash_ratelimit-0.5.0.tar", max compression
```

## Comparing `upstash_ratelimit-0.4.2.tar` & `upstash_ratelimit-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-07-04 08:45:40.697860 upstash_ratelimit-0.4.2/LICENSE
--rw-r--r--   0        0        0     7542 2023-07-04 08:45:40.697860 upstash_ratelimit-0.4.2/README.md
--rw-r--r--   0        0        0      475 2023-07-04 08:45:40.697860 upstash_ratelimit-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       73 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0     1780 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/algorithm.py
--rw-r--r--   0        0        0     3242 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/fixed_window_core.py
--rw-r--r--   0        0        0     5790 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/sliding_window_core.py
--rw-r--r--   0        0        0     5232 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/token_bucket_core.py
--rw-r--r--   0        0        0       81 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/async_blocker.py
--rw-r--r--   0        0        0     3012 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/fixed_window.py
--rw-r--r--   0        0        0     3427 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/limiter.py
--rw-r--r--   0        0        0     3935 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/sliding_window.py
--rw-r--r--   0        0        0     3440 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/token_bucket.py
--rw-r--r--   0        0        0      265 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3411 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0     2840 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/fixed_window.py
--rw-r--r--   0        0        0     3541 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/sliding_window.py
--rw-r--r--   0        0        0     1067 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/sync_blocker.py
--rw-r--r--   0        0        0     3196 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/token_bucket.py
--rw-r--r--   0        0        0      392 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0     8163 1970-01-01 00:00:00.000000 upstash_ratelimit-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8060 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/README.md
+-rw-r--r--   0        0        0     1331 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     4481 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/asyncio/ratelimit.py
+-rw-r--r--   0        0        0    14777 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0     4244 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/ratelimit.py
+-rw-r--r--   0        0        0      138 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/typing.py
+-rw-r--r--   0        0        0     1123 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/utils.py
+-rw-r--r--   0        0        0     9253 1970-01-01 00:00:00.000000 upstash_ratelimit-0.5.0/PKG-INFO
```

### Comparing `upstash_ratelimit-0.4.2/LICENSE` & `upstash_ratelimit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/sliding_window.py` & `upstash_ratelimit-0.5.0/upstash_ratelimit/ratelimit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,134 @@
-from typing import ClassVar, Literal
-from upstash_redis.asyncio import Redis
-from upstash_ratelimit.algorithms.sliding_window_core import SlidingWindowCore
-from upstash_ratelimit.asyncio.async_blocker import AsyncBlocker
-from upstash_ratelimit.utils.time import to_milliseconds
-from upstash_ratelimit.config import PREFIX, SDK
-from upstash_ratelimit.schema.response import RateLimitResponse
-from time import time_ns
-from math import floor
+import time
+from typing import Optional
 
+from upstash_redis import Redis
 
-class SlidingWindow(SlidingWindowCore, AsyncBlocker):
+from upstash_ratelimit.limiter import Limiter, Response
+from upstash_ratelimit.utils import merge_telemetry, now_s
+
+
+class Ratelimit:
     """
-    Combined approach of sliding logs and fixed window with lower storage
-    costs than sliding logs and improved boundary behavior by calculating a
-    weighted score between two windows.
+    Provides means of ratelimitting over the HTTP-based
+    Upstash Redis client.
     """
 
     def __init__(
-        self,
-        redis: Redis,
-        max_number_of_requests: int,
-        window: int,
-        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
-        prefix: str = PREFIX,
-    ):
-        """
-        :param redis: the Redis client that will be used to execute the algorithm's commands. If not given, will read from env variables `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN`
-        :param prefix: a prefix to distinguish between the keys used for rate limiting and others
-
-        :param max_number_of_requests: the number of requests allowed within the window
-        :param window: the number of time units in which requests are limited
-        :param unit: the shorthand version of the time measuring unit
-        """
-
-        if redis is None:
-            redis = Redis.from_env()
-
-        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
-        self.redis = redis
-
-        super().__init__(
-            max_number_of_requests=max_number_of_requests,
-            window=window,
-            unit=unit,
-            prefix=prefix,
-        )
-
-    async def limit(self, identifier: str) -> RateLimitResponse:
-        """
-        Increment identifier's request counter, determine whether it should pass
-        and return additional metadata.
-
-        Although we return the unix time when the next window begins (via "reset"), the limit is still enforced
-        between the two intervals.
-        """
-        async with self.redis:
-            remaining_requests: int = await self.redis.eval(
-                script=SlidingWindowCore.script,
-                keys=[
-                    self.get_current_key(identifier),
-                    self.get_previous_key(identifier),
-                ],
-                args=[
-                    self.max_number_of_requests,
-                    self.current_time_in_milliseconds,
-                    self.window,
-                ],
+        self, redis: Redis, limiter: Limiter, prefix: str = "upstash-ratelimit"
+    ) -> None:
+        """
+        :param redis: Upstash Redis instance to use.
+        :param limiter: Ratelimiter to use. Available limiters are \
+            `FixedWindow`, `SlidingWindow`, and `TokenBucket` which are provided \
+            in the `limiter` module. 
+        :param prefix: Prefix to distinguish the keys used in the ratelimit \
+            logic from others, in case the same Redis instance is reused between \
+            different applications. 
+        """
+
+        self._redis = redis
+        merge_telemetry(redis)
+
+        self._limiter = limiter
+        self._prefix = prefix
+
+    def limit(self, identifier: str) -> Response:
+        """
+        Determines if a request should pass or be rejected based on the identifier 
+        and previously chosen ratelimit.
+
+        Use this if you want to reject all requests that you can not handle 
+        right now.
+
+        .. code-block:: python
+
+            from upstash_redis import Redis
+            from upstash_ratelimit import Ratelimit, SlidingWindow
+
+            ratelimit = Ratelimit(
+                redis=Redis.from_env(),
+                limiter=SlidingWindow(max_requests=10, window=10, unit="s"),
             )
 
-        return super().limit(remaining_requests)
+            response = ratelimit.limit("some-id")
+            if not response.allowed:
+                print("Ratelimitted!")
 
-    async def remaining(self, identifier: str) -> int:
+            print("Good to go!")
+        
+        :param identifier: Identifier to ratelimit. Use a constant string to \
+            limit all requests, or user ids, API keys, or IP addresses for \
+            individual limits.
         """
-        Determine the number of identifier's remaining requests.
+
+        key = f"{self._prefix}:{identifier}"
+        return self._limiter.limit(self._redis, key)
+
+    def block_until_ready(self, identifier: str, timeout: float) -> Response:
         """
-        async with self.redis:
-            stored_requests_in_current_window = await self.redis.get(
-                self.get_current_key(identifier)
-            )
-            stored_requests_in_previous_window = await self.redis.get(
-                self.get_previous_key(identifier)
+        Blocks until the request may pass or timeout is reached.
+        
+        This method blocks until the request may be processed or the timeout 
+        has been reached.
+
+        Use this if you want to delay the request until it is ready to get 
+        processed.
+
+        .. code-block:: python
+
+            from upstash_redis import Redis
+            from upstash_ratelimit import Ratelimit, SlidingWindow
+
+            ratelimit = Ratelimit(
+                redis=Redis.from_env(),
+                limiter=SlidingWindow(max_requests=10, window=10, unit="s"),
             )
 
-        return super().remaining(
-            stored_requests_in_current_window, stored_requests_in_previous_window
-        )
+            response = ratelimit.block_until_ready("some-id", 60)
+            if not response.allowed:
+                print("Ratelimitted!")
 
-    async def reset(self, identifier: str) -> int:
+            print("Good to go!")
+        
+        :param identifier: Identifier to ratelimit. Use a constant string to \
+            limit all requests, or user ids, API keys, or IP addresses for \
+            individual limits.
+        :param timeout: Maximum time in seconds to wait until the request \
+            may pass.
         """
-        Determine the unix time in milliseconds when the next window begins.
 
-        If the identifier is not rate-limited, the returned value will be -1.
+        if timeout <= 0:
+            raise ValueError("Timeout must be positive")
+
+        response: Optional[Response] = None
+        deadline = now_s() + timeout
+
+        while True:
+            response = self.limit(identifier)
+            if response.allowed:
+                break
+
+            wait = max(0, min(response.reset, deadline) - now_s())
+            time.sleep(wait)
+
+            if now_s() > deadline:
+                break
+
+        return response
+
+    def get_remaining(self, identifier: str) -> int:
+        """
+        Returns the number of requests left for the given identifier.
         """
-        async with self.redis:
-            exists = await self.redis.exists(
-                self.get_previous_key(identifier), self.get_current_key(identifier)
-            )
 
-        return super().reset(exists)
+        key = f"{self._prefix}:{identifier}"
+        return self._limiter.get_remaining(self._redis, key)
 
-    def get_previous_key(self, identifier):
-        return f"{self.prefix}:{identifier}:{self.previous_window}"
+    def get_reset(self, identifier: str) -> float:
+        """
+        Returns the UNIX timestamp in seconds when the remaining
+        requests will be reset or replenished.
+        """
 
-    def get_current_key(self, identifier):
-        return f"{self.prefix}:{identifier}:{self.current_window}"
+        key = f"{self._prefix}:{identifier}"
+        return self._limiter.get_reset(self._redis, key)
```

