# Comparing `tmp/nextcore-2.0.0.tar.gz` & `tmp/nextcore-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcore-2.0.0.tar", max compression
+gzip compressed data, was "nextcore-2.0.1.tar", max compression
```

## Comparing `nextcore-2.0.0.tar` & `nextcore-2.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1076 2023-07-05 17:53:36.135146 nextcore-2.0.0/LICENSE
--rw-r--r--   0        0        0     2873 2023-07-05 17:53:36.135146 nextcore-2.0.0/README.md
--rw-r--r--   0        0        0     1334 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/__init__.py
--rw-r--r--   0        0        0     1550 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/__init__.py
--rw-r--r--   0        0        0    19861 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/dispatcher.py
--rw-r--r--   0        0        0     1453 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/errors.py
--rw-r--r--   0        0        0     2432 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/json.py
--rw-r--r--   0        0        0     2444 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/maybe_coro.py
--rw-r--r--   0        0        0     1371 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/times_per/__init__.py
--rw-r--r--   0        0        0     2140 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/times_per/priority_queue_container.py
--rw-r--r--   0        0        0     6559 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/times_per/times_per.py
--rw-r--r--   0        0        0     1797 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/undefined.py
--rw-r--r--   0        0        0     1855 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/__init__.py
--rw-r--r--   0        0        0     2540 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/close_code.py
--rw-r--r--   0        0        0     3227 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/decompressor.py
--rw-r--r--   0        0        0     3571 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/errors.py
--rw-r--r--   0        0        0     2854 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/exponential_backoff.py
--rw-r--r--   0        0        0     1935 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/op_code.py
--rw-r--r--   0        0        0    34036 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/shard.py
--rw-r--r--   0        0        0    13422 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/shard_manager.py
--rw-r--r--   0        0        0     1548 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/__init__.py
--rw-r--r--   0        0        0     1465 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/__init__.py
--rw-r--r--   0        0        0     2765 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/base.py
--rw-r--r--   0        0        0     2633 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/bearer.py
--rw-r--r--   0        0        0     2918 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/bot.py
--rw-r--r--   0        0        0    10011 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/bucket.py
--rw-r--r--   0        0        0     2558 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/bucket_metadata.py
--rw-r--r--   0        0        0     1153 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/client/__init__.py
--rw-r--r--   0        0        0     1978 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/client/base_client.py
--rw-r--r--   0        0        0    19632 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/client/client.py
--rw-r--r--   0        0        0     5627 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/errors.py
--rw-r--r--   0        0        0     1504 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/__init__.py
--rw-r--r--   0        0        0     3183 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/base.py
--rw-r--r--   0        0        0     2044 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/limited.py
--rw-r--r--   0        0        0     5929 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/unlimited.py
--rw-r--r--   0        0        0     6274 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/rate_limit_storage.py
--rw-r--r--   0        0        0     2481 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/request_session.py
--rw-r--r--   0        0        0     4133 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/route.py
--rw-r--r--   0        0        0       85 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/py.typed
--rw-r--r--   0        0        0     2476 2023-07-05 17:53:36.143146 nextcore-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 nextcore-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-09 22:42:23.167802 nextcore-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1323 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/__init__.py
+-rw-r--r--   0        0        0    19850 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/dispatcher.py
+-rw-r--r--   0        0        0     1442 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/errors.py
+-rw-r--r--   0        0        0     2421 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/json.py
+-rw-r--r--   0        0        0     2433 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/maybe_coro.py
+-rw-r--r--   0        0        0     1360 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/times_per/__init__.py
+-rw-r--r--   0        0        0     2129 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/times_per/priority_queue_container.py
+-rw-r--r--   0        0        0     6548 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/times_per/times_per.py
+-rw-r--r--   0        0        0     1786 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/common/undefined.py
+-rw-r--r--   0        0        0     1844 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/gateway/__init__.py
+-rw-r--r--   0        0        0     2529 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/gateway/close_code.py
+-rw-r--r--   0        0        0     3216 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/gateway/decompressor.py
+-rw-r--r--   0        0        0     3560 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/gateway/errors.py
+-rw-r--r--   0        0        0     2843 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/gateway/exponential_backoff.py
+-rw-r--r--   0        0        0     1924 2023-07-09 22:42:23.171802 nextcore-2.0.1/nextcore/gateway/op_code.py
+-rw-r--r--   0        0        0    34379 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/gateway/shard.py
+-rw-r--r--   0        0        0    13411 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/gateway/shard_manager.py
+-rw-r--r--   0        0        0     1537 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/__init__.py
+-rw-r--r--   0        0        0     1454 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/authentication/__init__.py
+-rw-r--r--   0        0        0     2754 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/authentication/base.py
+-rw-r--r--   0        0        0     2622 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/authentication/bearer.py
+-rw-r--r--   0        0        0     2907 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/authentication/bot.py
+-rw-r--r--   0        0        0    10000 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/bucket.py
+-rw-r--r--   0        0        0     2547 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/bucket_metadata.py
+-rw-r--r--   0        0        0     1142 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/client/__init__.py
+-rw-r--r--   0        0        0     1967 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/client/base_client.py
+-rw-r--r--   0        0        0    19621 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/client/client.py
+-rw-r--r--   0        0        0     5616 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/errors.py
+-rw-r--r--   0        0        0     1493 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/global_rate_limiter/__init__.py
+-rw-r--r--   0        0        0     3172 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/global_rate_limiter/base.py
+-rw-r--r--   0        0        0     2033 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/global_rate_limiter/limited.py
+-rw-r--r--   0        0        0     5918 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/global_rate_limiter/unlimited.py
+-rw-r--r--   0        0        0     6263 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/rate_limit_storage.py
+-rw-r--r--   0        0        0     2470 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/request_session.py
+-rw-r--r--   0        0        0     4122 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/http/route.py
+-rw-r--r--   0        0        0       85 2023-07-09 22:42:23.175802 nextcore-2.0.1/nextcore/py.typed
+-rw-r--r--   0        0        0     2752 2023-07-09 22:42:23.175802 nextcore-2.0.1/pypi-README.md
+-rw-r--r--   0        0        0     2565 2023-07-09 22:42:23.175802 nextcore-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 nextcore-2.0.1/PKG-INFO
```

### Comparing `nextcore-2.0.0/LICENSE` & `nextcore-2.0.1/nextcore/common/errors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-MIT License
+# The MIT License (MIT)
+# Copyright (c) 2021-present tag-epic
+#
+# Permission is hereby granted, free of charge, to any person obtaining a
+# copy of this software and associated documentation files (the "Software"),
+# to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense,
+# and/or sell copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+# OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+# DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2021 nextcore developers
+from __future__ import annotations
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Final
+
+__all__: Final[tuple[str, ...]] = ("RateLimitedError",)
+
+
+class RateLimitedError(Exception):
+    """A error for when a :class:`~nextcore.common.TimesPer` is rate limited and ``wait`` was :data:`False`"""
```

### Comparing `nextcore-2.0.0/README.md` & `nextcore-2.0.1/pypi-README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 ### ✨ Features
 
 - #### Speed
 
   We try to make the library as fast as possible, without compromising on readability of the code or features.
   
-  <video src="https://user-images.githubusercontent.com/35035079/172221406-b8d618e6-75fd-45d4-a470-62aeeab5bc0a.mp4" />
-
 - #### Modularity
 
   All the components can easily be swapped out with your own.
 
 - #### Control
 
   Nextcore offers fine-grained control over things most libraries don't support.
```

### Comparing `nextcore-2.0.0/nextcore/__init__.py` & `nextcore-2.0.1/nextcore/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -22,9 +22,9 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Final
 
-__version__: Final[str] = "2.0.0"
+__version__: Final[str] = "2.0.1"
 __all__: Final[tuple[str, ...]] = ("__version__",)
```

### Comparing `nextcore-2.0.0/nextcore/common/__init__.py` & `nextcore-2.0.1/nextcore/common/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/common/dispatcher.py` & `nextcore-2.0.1/nextcore/common/dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/common/errors.py` & `nextcore-2.0.1/nextcore/http/global_rate_limiter/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -19,15 +19,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from .base import BaseGlobalRateLimiter
+from .limited import LimitedGlobalRateLimiter
+from .unlimited import UnlimitedGlobalRateLimiter
+
 if TYPE_CHECKING:
     from typing import Final
 
-__all__: Final[tuple[str, ...]] = ("RateLimitedError",)
-
-
-class RateLimitedError(Exception):
-    """A error for when a :class:`~nextcore.common.TimesPer` is rate limited and ``wait`` was :data:`False`"""
+__all__: Final[tuple[str, ...]] = ("BaseGlobalRateLimiter", "UnlimitedGlobalRateLimiter", "LimitedGlobalRateLimiter")
```

### Comparing `nextcore-2.0.0/nextcore/common/json.py` & `nextcore-2.0.1/nextcore/common/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/common/maybe_coro.py` & `nextcore-2.0.1/nextcore/common/maybe_coro.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/common/times_per/__init__.py` & `nextcore-2.0.1/nextcore/common/times_per/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/common/times_per/priority_queue_container.py` & `nextcore-2.0.1/nextcore/common/times_per/priority_queue_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/common/times_per/times_per.py` & `nextcore-2.0.1/nextcore/common/times_per/times_per.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/common/undefined.py` & `nextcore-2.0.1/nextcore/common/undefined.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/gateway/__init__.py` & `nextcore-2.0.1/nextcore/gateway/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/gateway/close_code.py` & `nextcore-2.0.1/nextcore/gateway/close_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/gateway/decompressor.py` & `nextcore-2.0.1/nextcore/gateway/decompressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/gateway/errors.py` & `nextcore-2.0.1/nextcore/gateway/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/gateway/exponential_backoff.py` & `nextcore-2.0.1/nextcore/gateway/exponential_backoff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/gateway/op_code.py` & `nextcore-2.0.1/nextcore/gateway/op_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/gateway/shard.py` & `nextcore-2.0.1/nextcore/gateway/shard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -129,14 +129,18 @@
         The bot's token to connect with. If this is changed, the session will be invalidated.
     presence:
         The initial presence info to send when connecting.
     large_threshold:
         A value between 50 and 250 that determines how many members a guild needs for the gateway to stop sending offline members in the guild member list.
     library_name:
         The name of the library that is using this gateway. This should be set if you are making your own library on top of nextcore.
+    connected:
+        When this shard is connected to the gateway, but not identified yet.
+
+        This also requires the gateway to send the `HELLO <https://discord.dev/topics/gateway-events#hello>` event, as rate-limiters are not setup yet.
     ready:
         Fires when the gateway has connected and received the READY event.
     raw_dispatcher:
         A dispatcher with raw payloads sent by discord. The event name is the opcode, and the value is the raw data.
     event_dispatcher:
         A dispatcher for DISPATCH events sent by discord. The event name is the event name, and the value is the inner payload.
     dispatcher:
@@ -153,14 +157,15 @@
         "shard_id",
         "shard_count",
         "intents",
         "token",
         "presence",
         "large_threshold",
         "library_name",
+        "connected",
         "ready",
         "raw_dispatcher",
         "event_dispatcher",
         "dispatcher",
         "session_id",
         "session_sequence_number",
         "should_reconnect",
@@ -196,14 +201,15 @@
         self.intents: int = intents
         self.token: str = token
         self.presence: UpdatePresenceData | None = presence
         self.large_threshold: int | None = large_threshold
         self.library_name: str = library_name
 
         # Publics
+        self.connected: Event = Event()
         self.ready: Event = Event()
         self.raw_dispatcher: Dispatcher[int] = Dispatcher()
         self.event_dispatcher: Dispatcher[str] = Dispatcher()
         self.dispatcher: Dispatcher[Literal["disconnect", "sent", "critical", "client_disconnect"]] = Dispatcher()
 
         # Session related
         self.session_id: str | None = None
@@ -277,15 +283,15 @@
             self._ws = ws  # Use the new connection
 
             create_task(self._receive_loop())
 
             # Connection logic is continued in _handle_hello to account for that rate limits are defined there.
 
             try:
-                await asyncio.wait_for(self.raw_dispatcher.wait_for(lambda _: True, GatewayOpcode.HELLO), timeout=10)
+                await asyncio.wait_for(self.connected.wait(), timeout=10)
             except asyncio.TimeoutError:
                 self._logger.warning("Timeout waiting for HELLO. Reconnecting!")
 
                 # A task is used here because of the connect lock.
                 # TODO: This can probably be done in a cleaner way?
                 asyncio.create_task(self.connect())
 
@@ -324,14 +330,15 @@
                 await self.dispatcher.dispatch("client_disconnect", True)
                 await self._ws.close()  # Disconnecting with a 1000 close code deletes the session.
             else:
                 await self.dispatcher.dispatch("client_disconnect", False)
                 await self._ws.close(code=999)
         self._ws = None  # Clear it to save some ram
         self._send_rate_limit = None  # No longer applies
+        self.connected.clear()
 
     @property
     def latency(self) -> float:
         """Time in seconds between a heartbeat being sent and discord acknowledging it.
 
         Raises
         ------
@@ -506,28 +513,31 @@
         if opcode == GatewayOpcode.DISPATCH.value:
             # Received dispatch
             # We are just trusing discord to provide the correct data here.
             dispatch_data: DispatchEvent = frozen_data
             await self.event_dispatcher.dispatch(dispatch_data["t"], dispatch_data["d"])
 
     async def _on_disconnect(self, ws: ClientWebSocketResponse) -> None:
+        self.connected.clear()
         self.ready.clear()
 
         close_code = ws.close_code
         if ws.close_code is None:
             # This happens when we closed the websocket. Just ignore it as there is basically no info here.
             return
 
         self._logger.debug("Disconnected with code %s", close_code)
 
         await self.dispatcher.dispatch("disconnect", close_code)
 
     # Raw handlers
     # These should be prefixed by handle_ to avoid confusiuon with loop callbacks
     async def _handle_hello(self, data: HelloEvent) -> None:
+        self.connected.set()
+
         # Start heartbeating
         heartbeat_interval = data["d"]["heartbeat_interval"] / 1000  # Convert from ms to seconds
 
         loop = get_running_loop()
         loop.create_task(self._heartbeat_loop(heartbeat_interval))
 
         # Create a rate limiter
```

### Comparing `nextcore-2.0.0/nextcore/gateway/shard_manager.py` & `nextcore-2.0.1/nextcore/gateway/shard_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/__init__.py` & `nextcore-2.0.1/nextcore/http/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/authentication/__init__.py` & `nextcore-2.0.1/nextcore/http/authentication/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/authentication/base.py` & `nextcore-2.0.1/nextcore/http/authentication/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/authentication/bearer.py` & `nextcore-2.0.1/nextcore/http/authentication/bearer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/authentication/bot.py` & `nextcore-2.0.1/nextcore/http/authentication/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/bucket.py` & `nextcore-2.0.1/nextcore/http/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/bucket_metadata.py` & `nextcore-2.0.1/nextcore/http/bucket_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/client/__init__.py` & `nextcore-2.0.1/nextcore/http/client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/client/base_client.py` & `nextcore-2.0.1/nextcore/http/client/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/client/client.py` & `nextcore-2.0.1/nextcore/http/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/errors.py` & `nextcore-2.0.1/nextcore/http/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/global_rate_limiter/base.py` & `nextcore-2.0.1/nextcore/http/global_rate_limiter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/global_rate_limiter/limited.py` & `nextcore-2.0.1/nextcore/http/global_rate_limiter/limited.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/global_rate_limiter/unlimited.py` & `nextcore-2.0.1/nextcore/http/global_rate_limiter/unlimited.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/rate_limit_storage.py` & `nextcore-2.0.1/nextcore/http/rate_limit_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/request_session.py` & `nextcore-2.0.1/nextcore/http/request_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/nextcore/http/route.py` & `nextcore-2.0.1/nextcore/http/route.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021-present nextcore developers
+# Copyright (c) 2021-present tag-epic
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
```

### Comparing `nextcore-2.0.0/pyproject.toml` & `nextcore-2.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [tool.poetry]
 name = "nextcore"
-version = "2.0.0"
+version = "2.0.1"
 description = "A low level Discord API wrapper"
-authors = ["nextcore developers"]
+authors = ["tag-epic"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Framework :: aiohttp",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Cython",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Communications :: Chat",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed"
 ]
-readme = "README.md"
-homepage = "https://nextcord.dev" # TODO: Replace this?
+readme = "pypi-README.md"
+#homepage = "https://nextcord.dev" # TODO: Replace this?
 repository = "https://github.com/nextsnake/nextcore"
-documentation = "https://docs.nextcord.gay" # TODO: Replace this
+documentation = "https://nextcore.readthedocs.io"
 keywords = ["discord", "bot", "wrapper", "api"]
 packages = [
     { include = "nextcore" }
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/nextsnake/nextcore/issues"
+"Discord" = "https://discord.gg/3RFUm3eP5c"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = ">=3.6.0,<4.0.0"
 frozendict = "^2.3.0"
 types-frozendict = "^2.0.6" # Could we extend the version requirement
 typing-extensions = "^4.1.1" # Same as above
@@ -50,14 +51,15 @@
 pytest-asyncio = "^0.18.1"
 pytest-mock = "^3.7.0"
 pre-commit = "^2.18.1"
 sphinxext-opengraph = "^0.6.3"
 slotscheck = "^0.14.0"
 sphinx-inline-tabs = "*" # CalVer, the version does not make sense to lock.
 towncrier = "^22.12.0"
+style-guide = {git = "https://github.com/nextsnake/style-guide"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 speed = ["orjson", "types-orjson"]
```

### Comparing `nextcore-2.0.0/PKG-INFO` & `nextcore-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: nextcore
-Version: 2.0.0
+Version: 2.0.1
 Summary: A low level Discord API wrapper
-Home-page: https://nextcord.dev
+Home-page: https://github.com/nextsnake/nextcore
 License: MIT
 Keywords: discord,bot,wrapper,api
-Author: nextcore developers
+Author: tag-epic
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -29,15 +29,16 @@
 Requires-Dist: discord-typings (>=0.5.0,<0.6.0)
 Requires-Dist: frozendict (>=2.3.0,<3.0.0)
 Requires-Dist: orjson (>=3.6.8,<4.0.0) ; extra == "speed"
 Requires-Dist: types-frozendict (>=2.0.6,<3.0.0)
 Requires-Dist: types-orjson (>=3.6.2,<4.0.0) ; extra == "speed"
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/nextsnake/nextcore/issues
-Project-URL: Documentation, https://docs.nextcord.gay
+Project-URL: Documentation, https://nextcore.readthedocs.io
+Project-URL: Discord, https://discord.gg/3RFUm3eP5c
 Project-URL: Repository, https://github.com/nextsnake/nextcore
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   <img alt="" src="docs/_static/logo.svg" width="160px"/>
   
@@ -48,16 +49,14 @@
 
 ### ✨ Features
 
 - #### Speed
 
   We try to make the library as fast as possible, without compromising on readability of the code or features.
   
-  <video src="https://user-images.githubusercontent.com/35035079/172221406-b8d618e6-75fd-45d4-a470-62aeeab5bc0a.mp4" />
-
 - #### Modularity
 
   All the components can easily be swapped out with your own.
 
 - #### Control
 
   Nextcore offers fine-grained control over things most libraries don't support.
```

