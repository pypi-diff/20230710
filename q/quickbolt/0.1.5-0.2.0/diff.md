# Comparing `tmp/quickbolt-0.1.5.tar.gz` & `tmp/quickbolt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbolt-0.1.5.tar", max compression
+gzip compressed data, was "quickbolt-0.2.0.tar", max compression
```

## Comparing `quickbolt-0.1.5.tar` & `quickbolt-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.5/LICENSE
--rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.1.5/README.md
--rw-r--r--   0        0        0     1238 2023-07-08 00:26:07.761170 quickbolt-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.5/quickbolt/__init__.py
--rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.5/quickbolt/batch_generation/__init__.py
--rw-r--r--   0        0        0    11377 2023-07-07 23:59:06.071578 quickbolt-0.1.5/quickbolt/batch_generation/batch_generation.py
--rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.5/quickbolt/clients/__init__.py
--rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.5/quickbolt/clients/aio_requests.py
--rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.5/quickbolt/clients/httpx_requests.py
--rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.5/quickbolt/logging/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.5/quickbolt/logging/async_logger.py
--rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.5/quickbolt/pytest/__init__.py
--rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.5/quickbolt/pytest/core_pytest_base.py
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.5/quickbolt/reporting/__init__.py
--rw-r--r--   0        0        0     7522 2023-07-05 05:48:43.803436 quickbolt-0.1.5/quickbolt/reporting/response_csv.py
--rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.5/quickbolt/utils/__init__.py
--rw-r--r--   0        0        0     4529 2023-07-05 05:48:43.803703 quickbolt-0.1.5/quickbolt/utils/dictionary.py
--rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.5/quickbolt/utils/directory.py
--rw-r--r--   0        0        0     2802 2023-07-07 23:59:06.071757 quickbolt-0.1.5/quickbolt/utils/json.py
--rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.5/quickbolt/utils/sync_async.py
--rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.5/quickbolt/validations/__init__.py
--rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.5/quickbolt/validations/validations.py
--rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.2.0/README.md
+-rw-r--r--   0        0        0     1238 2023-07-10 03:58:55.439034 quickbolt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.2.0/quickbolt/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.2.0/quickbolt/batch_generation/__init__.py
+-rw-r--r--   0        0        0    11377 2023-07-07 23:59:06.071578 quickbolt-0.2.0/quickbolt/batch_generation/batch_generation.py
+-rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.2.0/quickbolt/clients/__init__.py
+-rw-r--r--   0        0        0    10215 2023-07-10 03:29:24.475286 quickbolt-0.2.0/quickbolt/clients/aio_requests.py
+-rw-r--r--   0        0        0    10430 2023-07-10 03:29:24.475556 quickbolt-0.2.0/quickbolt/clients/httpx_requests.py
+-rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.2.0/quickbolt/logging/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.2.0/quickbolt/logging/async_logger.py
+-rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.2.0/quickbolt/pytest/__init__.py
+-rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.2.0/quickbolt/pytest/core_pytest_base.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.2.0/quickbolt/reporting/__init__.py
+-rw-r--r--   0        0        0     8518 2023-07-10 03:29:24.475798 quickbolt-0.2.0/quickbolt/reporting/response_csv.py
+-rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.2.0/quickbolt/utils/__init__.py
+-rw-r--r--   0        0        0     4529 2023-07-05 05:48:43.803703 quickbolt-0.2.0/quickbolt/utils/dictionary.py
+-rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.2.0/quickbolt/utils/directory.py
+-rw-r--r--   0        0        0     2802 2023-07-07 23:59:06.071757 quickbolt-0.2.0/quickbolt/utils/json.py
+-rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.2.0/quickbolt/utils/sync_async.py
+-rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.2.0/quickbolt/validations/__init__.py
+-rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.2.0/quickbolt/validations/validations.py
+-rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.2.0/PKG-INFO
```

### Comparing `quickbolt-0.1.5/LICENSE` & `quickbolt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/README.md` & `quickbolt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/pyproject.toml` & `quickbolt-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbolt"
-version = "0.1.5"
+version = "0.2.0"
 description = "Asynchronously make and validate requests!"
 authors = ["Ashton Szabo <aszabo00@gmail.com>"]
 repository = "https://github.com/aszabo00/quickbolt"
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `quickbolt-0.1.5/quickbolt/batch_generation/batch_generation.py` & `quickbolt-0.2.0/quickbolt/batch_generation/batch_generation.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/quickbolt/clients/aio_requests.py` & `quickbolt-0.2.0/quickbolt/clients/aio_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,45 +221,55 @@
 
     @sa.force_sync
     async def request(
         self,
         data: list[dict] | dict,
         delay: int | float = 0,
         report: bool = True,
+        full_scrub_fields: None | list = None,
         **kwargs: Any,
     ) -> dict:
         """
         The batch executor for the requests batch.
 
         Args:
             data: The list of info needed to make the request eg [{'url': ..., 'method': 'get'}].
             delay: How long to delay between requests.
             report: Whether to create or update a report with the current responses.
+            full_scrub_fields: The fields to do a full char scrub on.
             **kwargs: The additional params eg headers or data etc. See
                 https://docs.aiohttp.org/en/stable/client_reference.html for more details.
 
         Returns:
             responses: The global response object eg {'duration': ..., 'responses': ...}.
         """
-        return await self.async_request(data=data, delay=delay, report=report, **kwargs)
+        return await self.async_request(
+            data=data,
+            delay=delay,
+            report=report,
+            full_scrub_fields=full_scrub_fields,
+            **kwargs,
+        )
 
     async def async_request(
         self,
         data: list[dict] | dict,
         delay: int | float = 0,
         report: bool = True,
+        full_scrub_fields: None | list = None,
         **kwargs: Any,
     ) -> dict:
         """
         The batch executor for the async requests batch.
 
         Args:
             data: The list of info needed to make the request eg [{'url': ..., 'method': 'get'}].
             delay: How long to delay between requests.
             report: Whether to create or update a report with the current responses.
+            full_scrub_fields: The fields to do a full char scrub on.
             **kwargs: The additional params eg headers or data etc. See
                 https://docs.aiohttp.org/en/stable/client_reference.html for more details.
 
         Returns:
             responses: The global response object eg {'duration': ..., 'responses': ...}.
         """
         self.batch_number += 1
@@ -273,9 +283,11 @@
             "duration": round(t1 - t0, 2),
             "responses": sorted(responses, key=itemgetter("index")),
         }
         self._return_history.append(_return)
         await self.logger.info(f'The batch duration was {_return["duration"]} seconds.')
 
         if _return["responses"]:
-            not report or await rc.create_csv_report(self.csv_path, _return, scrub=True)
+            not report or await rc.create_csv_report(
+                self.csv_path, _return, scrub=True, full_scrub_fields=full_scrub_fields
+            )
         return _return
```

### Comparing `quickbolt-0.1.5/quickbolt/clients/httpx_requests.py` & `quickbolt-0.2.0/quickbolt/clients/httpx_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,46 +225,56 @@
 
     @sa.force_sync
     async def request(
         self,
         data: list[dict] | dict,
         delay: int | float = 0,
         report: bool = True,
+        full_scrub_fields: None | list = None,
         **kwargs: Any,
     ) -> dict:
         """
         The batch executor for the requests batch.
 
         Args:
             data: The list of info needed to make the request eg [{'url': ..., 'method': 'get'}].
             delay: How long to delay between requests.
             report: Whether to create or update a report with the current responses.
+            full_scrub_fields: The fields to do a full char scrub on.
             **kwargs: The additional params eg headers or data etc. See
                 https://github.com/encode/httpx/blob/5b06aea1d64f0815af6fe71da3ac725bed3ec09f/httpx/_client.py#L1481
                 for more details.
 
         Returns:
             responses: The global response object eg {'duration': ..., 'responses': ...}.
         """
-        return await self.async_request(data=data, delay=delay, report=report, **kwargs)
+        return await self.async_request(
+            data=data,
+            delay=delay,
+            report=report,
+            full_scrub_fields=full_scrub_fields,
+            **kwargs,
+        )
 
     async def async_request(
         self,
         data: list[dict] | dict,
         delay: int | float = 0,
         report: bool = True,
+        full_scrub_fields: None | list = None,
         **kwargs: Any,
     ) -> dict:
         """
         The batch executor for the async requests batch.
 
         Args:
             data: The list of info needed to make the request eg [{'url': ..., 'method': 'get'}].
             delay: How long to delay between requests.
             report: Whether to create or update a report with the current responses.
+            full_scrub_fields: The fields to do a full char scrub on.
             **kwargs: The additional params eg headers or data etc. See
                 https://github.com/encode/httpx/blob/5b06aea1d64f0815af6fe71da3ac725bed3ec09f/httpx/_client.py#L1481
                 for more details.
 
         Returns:
             responses: The global response object eg {'duration': ..., 'responses': ...}.
         """
@@ -279,9 +289,11 @@
             "duration": round(t1 - t0, 2),
             "responses": sorted(responses, key=itemgetter("index")),
         }
         self._return_history.append(_return)
         await self.logger.info(f'The batch duration was {_return["duration"]} seconds.')
 
         if _return["responses"]:
-            not report or await rc.create_csv_report(self.csv_path, _return, scrub=True)
+            not report or await rc.create_csv_report(
+                self.csv_path, _return, scrub=True, full_scrub_fields=full_scrub_fields
+            )
         return _return
```

### Comparing `quickbolt-0.1.5/quickbolt/logging/async_logger.py` & `quickbolt-0.2.0/quickbolt/logging/async_logger.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/quickbolt/pytest/core_pytest_base.py` & `quickbolt-0.2.0/quickbolt/pytest/core_pytest_base.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/quickbolt/reporting/response_csv.py` & `quickbolt-0.2.0/quickbolt/reporting/response_csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,104 +42,130 @@
             for item in row
         ]
         for row in data
         if row
     ]
 
 
-def scrub(text: str) -> str:
+def scrub(text: str, full: bool = False) -> str:
     """
     This scrubs text of alphanumerical information.
 
     Args:
         text: The text to scrub.
+        full: Full char conversion to 0's.
 
     Returns:
         scrubbed_text: The scrubbed text.
     """
     # need to do better here
     text_dict = jh.deserialize(text)
     flat_scrubbed_text = dh.flatten(text_dict)
 
+    targets = []
     for key, value in flat_scrubbed_text.items():
         if isinstance(value, (int, float)):
             val_type = type(value).__name__
             flat_scrubbed_text[key] = f"{value} <{val_type}>"
 
+        target_str = str(flat_scrubbed_text[key])
+        target = [target_str]
+        if not full:
+            target = re.findall(
+                r"([A-Za-z]+[\d@]+[\w@]*|[\d@]+[A-Za-z]+[\w@]*|\d+)",
+                target_str,
+            )
+        targets.extend(target)
+    targets.sort(key=len, reverse=True)
+
     unflat_scrubbed_text = dh.unflatten(flat_scrubbed_text)
     scrubbed_text = jh.serialize(unflat_scrubbed_text)
 
-    targets = re.findall(
-        r"([A-Za-z]+[\d@]+[\w@]*|[\d@]+[A-Za-z]+[\w@]*|\d+)", scrubbed_text
-    )
-    targets.sort(key=len, reverse=True)
-
     for t in targets:
         scrubbed_text = scrubbed_text.replace(t, "0" * len(t))
 
     return scrubbed_text
 
 
-def scrub_data(data: dict) -> dict:
+def scrub_data(data: dict, full_scrub_fields: None | list = None) -> dict:
     """
     This scrubs a dict against pre-defined fields.
 
     Args:
         data: A response report object.
+        full_scrub_fields: The fields to do a full char scrub on.
 
     Returns:
         scrubbed_data: A scrubbed response report object.
     """
+    if not isinstance(full_scrub_fields, list):
+        full_scrub_fields = ["headers"]
+    full_scrub_fields = [f.lower() for f in full_scrub_fields]
+
     scrub_fields = ["message", "url", "server_headers", "headers", "kwargs", "body"]
 
     data_copy = deepcopy(data)
     for key, value in data_copy.items():
-        if key.lower() in scrub_fields:
+        key_lower = key.lower()
+        if key_lower in scrub_fields and value:
+            full = False
+            if key_lower in full_scrub_fields:
+                full = True
+
             data_ser = jh.serialize(value)
-            data_scr = scrub(data_ser)
+            data_scr = scrub(data_ser, full)
             data_copy[key] = jh.deserialize(data_scr)
 
     return data_copy
 
 
-async def csv_to_dict(csv_data: str | list, scrub: bool = False) -> list[dict]:
+async def csv_to_dict(
+    csv_data: str | list, scrub: bool = False, full_scrub_fields: None | list = None
+) -> list[dict]:
     """
 
     Args:
         csv_data: The path to the csv file to be read in or the data itself.
         scrub: Whether to remove sensitive info from the data.
+        full_scrub_fields: The fields to do a full char scrub on.
 
     Returns:
         data: The csv file represented as a dictionary.
     """
     if isinstance(csv_data, str):
         async with aopen(csv_data, encoding="ascii", newline="") as csv_file:
             data = [row async for row in AsyncDictReader(csv_file)]
     elif isinstance(csv_data, list):
         data = [dict(zip(csv_data[0], r)) for r in csv_data[1:] if r]
 
     if scrub:
-        data = [scrub_data(d) for d in data]
+        data = [scrub_data(d, full_scrub_fields=full_scrub_fields) for d in data]
 
     for row in data:
         for k, v in row.items():
             if v:
                 row[k] = jh.deserialize(v, safe=True)
 
     return data
 
 
-async def create_csv_report(csv_path: str, _return: dict, scrub: bool = False):
+async def create_csv_report(
+    csv_path: str,
+    _return: dict,
+    scrub: bool = False,
+    full_scrub_fields: None | list = None,
+):
     """
     This writes the results of each batch of requests to a csv report file.
 
     Args:
         csv_path: The path to store the csv report.
         _return: The _return from a batch request.
         scrub: Whether to remove sensitive info from the data.
+        full_scrub_fields: The fields to do a full char scrub on.
     """
     responses = _return["responses"]
 
     for r in responses:
         r["server_headers"] = {k: v for k, v in r["server_headers"].items()}
 
         kwargs = r.get("kwargs", {})
@@ -171,15 +197,18 @@
     if scrub:
         scrubbed_csv_path = csv_path.replace(".csv", "_scrubbed.csv")
 
         scrubbed_responses = [
             {k: v if k != "curl" else "" for k, v in r.copy().items()}
             for r in responses
         ]
-        scrubbed_responses = [scrub_data(r) for r in scrubbed_responses]
+        scrubbed_responses = [
+            scrub_data(r, full_scrub_fields=full_scrub_fields)
+            for r in scrubbed_responses
+        ]
 
         col_titles = [""]
         if not await aos.path.exists(scrubbed_csv_path):
             col_titles = [[key.upper() for key in responses[0].keys()]]
 
         csv_data = col_titles + [list(r.values()) for r in scrubbed_responses]
         await add_rows_to_csv_report(scrubbed_csv_path, csv_data)
```

### Comparing `quickbolt-0.1.5/quickbolt/utils/dictionary.py` & `quickbolt-0.2.0/quickbolt/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/quickbolt/utils/directory.py` & `quickbolt-0.2.0/quickbolt/utils/directory.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/quickbolt/utils/json.py` & `quickbolt-0.2.0/quickbolt/utils/json.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/quickbolt/validations/validations.py` & `quickbolt-0.2.0/quickbolt/validations/validations.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.5/PKG-INFO` & `quickbolt-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbolt
-Version: 0.1.5
+Version: 0.2.0
 Summary: Asynchronously make and validate requests!
 Home-page: https://github.com/aszabo00/quickbolt
 License: MIT
 Author: Ashton Szabo
 Author-email: aszabo00@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
```

