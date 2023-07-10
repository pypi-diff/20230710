# Comparing `tmp/epson_connect-0.1.0.tar.gz` & `tmp/epson_connect-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epson_connect-0.1.0.tar", max compression
+gzip compressed data, was "epson_connect-0.2.0.tar", max compression
```

## Comparing `epson_connect-0.1.0.tar` & `epson_connect-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      699 2023-07-09 05:46:25.682511 epson_connect-0.1.0/README.md
--rw-r--r--   0        0        0     1064 2023-07-08 22:35:34.100611 epson_connect-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-08 22:57:50.154790 epson_connect-0.1.0/src/epson_connect/__init__.py
--rw-r--r--   0        0        0     3210 2023-07-09 05:45:15.077764 epson_connect-0.1.0/src/epson_connect/authenticate.py
--rw-r--r--   0        0        0     1154 2023-07-09 05:46:28.548782 epson_connect-0.1.0/src/epson_connect/client.py
--rw-r--r--   0        0        0     3488 2023-07-09 05:46:32.089241 epson_connect-0.1.0/src/epson_connect/printer.py
--rw-r--r--   0        0        0     5149 2023-07-09 05:14:27.444060 epson_connect-0.1.0/src/epson_connect/printer_settings.py
--rw-r--r--   0        0        0      637 2023-07-09 05:46:33.820550 epson_connect-0.1.0/src/epson_connect/scanner.py
--rw-r--r--   0        0        0     1622 1970-01-01 00:00:00.000000 epson_connect-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-07-09 20:45:17.736792 epson_connect-0.2.0/LICENSE
+-rw-r--r--   0        0        0      704 2023-07-10 05:14:45.827382 epson_connect-0.2.0/README.md
+-rw-r--r--   0        0        0     1340 2023-07-10 17:07:54.467052 epson_connect-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-07-10 04:04:57.289077 epson_connect-0.2.0/src/epson_connect/__init__.py
+-rw-r--r--   0        0        0     3560 2023-07-10 04:07:20.223607 epson_connect-0.2.0/src/epson_connect/authenticate.py
+-rw-r--r--   0        0        0     1154 2023-07-09 05:46:28.548782 epson_connect-0.2.0/src/epson_connect/client.py
+-rw-r--r--   0        0        0     4349 2023-07-10 04:46:00.519043 epson_connect-0.2.0/src/epson_connect/printer.py
+-rw-r--r--   0        0        0     4924 2023-07-10 04:09:53.041881 epson_connect-0.2.0/src/epson_connect/printer_settings.py
+-rw-r--r--   0        0        0     2435 2023-07-10 04:19:47.452482 epson_connect-0.2.0/src/epson_connect/scanner.py
+-rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 epson_connect-0.2.0/PKG-INFO
```

### Comparing `epson_connect-0.1.0/README.md` & `epson_connect-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ## Usage
 
 ```python
 import epson_connect
 
 ec = espon_connect.Client(
-    username='...',
+    printer_email='...',
     client_id='...',
     client_secret='...',
 )
 
 # Or with these enviornment variables defined...
 # export ESPON_CONNECT_API_PRINTER_EMAIL=<an email address for the device>
 # export ESPON_CONNECT_API_CLIENT_ID=<client id>
```

### Comparing `epson_connect-0.1.0/pyproject.toml` & `epson_connect-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 [tool.poetry]
 name = "epson-connect"
-version = "0.1.0"
+version = "0.2.0"
 description = "Bindings for the Espon Connect API"
-license = "BSD-3"
+license = "MIT"
 authors = ["Paul Logston <paul.logston@gmail.com>"]
 maintainers = ["Paul Logston <paul.logston@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/epson-connect/"
 repository = "https://github.com/logston/epson-connect"
 keywords = ["epson", "connect", "api"]
 classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
+    "Topic :: Internet",
+    "Topic :: Printing",
+    "Topic :: Software Development :: Libraries",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "epson_connect", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 requests = "^2.31.0"
 
-
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 tox = ">=3.16.1"
-flake8 = ">=3.8.3"
+flake8 = ">=6.0.0"
 toml = ">=0.10.1"
-flake8-isort = ">=3.0.0"
+flake8-isort = ">=6.0.0"
 pytest = ">=5.4.0"
 coverage = ">=6.4.2"
 pytest-cov = ">=3.0.0"
+pytest-mock = "^3.11.1"
+sphinx = "^7.0.1"
+myst-parser = "^2.0.0"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
-
 pythonpath = "src"
+python_files = "tests/test_*.py"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `epson_connect-0.1.0/src/epson_connect/authenticate.py` & `epson_connect-0.2.0/src/epson_connect/authenticate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from datetime import datetime, timedelta
 import os
+from datetime import datetime, timedelta
 
 import requests
 from requests.auth import HTTPBasicAuth
 
 
 class AuthCtx:
     def __init__(
@@ -29,15 +29,15 @@
         method = 'POST'
         path = '/api/1/printing/oauth2/auth/token?subject=printer'
 
         if self._expires_at > datetime.now():
             return
 
         headers = {
-            'Content-Type':'application/x-www-form-urlencoded'
+            'Content-Type': 'application/x-www-form-urlencoded'
         }
         auth = HTTPBasicAuth(self._client_id, self._client_secret)
 
         if self._access_token == '':
             data = {
                 'grant_type': 'password',
                 'username': self._printer_email,
@@ -45,15 +45,18 @@
             }
         else:
             data = {
                 'grant_type': 'refresh_token',
                 'refresh_token': self._refresh_token,
             }
 
-        body = self.send(method, path, data, headers=headers, auth=auth)
+        try:
+            body = self.send(method, path, data, headers=headers, auth=auth)
+        except ApiError as e:
+            raise AuthenticationError(e)
 
         error = body.get('error')
         if error:
             raise AuthenticationError(error)
 
         # First time authenticating, set refresh_token.
         if self._access_token == '':
@@ -68,35 +71,42 @@
         Cancel authentication.
         """
         method = 'DELETE'
         path = f'/api/1/printing/printers/{self._subject_id}'
         self.send(method, path)
 
     def send(self, method, path, data=None, headers=None, auth=None) -> dict:
-        if not headers:
-            headers = {
-                'Authorization': f'Bearer {self._access_token}',
-                'Content-Type': f'application/json',
-            }
+        # auth is only set when we are authenticating with Client ID and Client Secret.
+        # In this scenario, we do not want to call self._auth again as that
+        # would cause a recursion exception.
+        if not auth:
+            self._auth()
 
         resp = requests.request(
-                method=method,
-                url=self._base_url + path,
-                headers=headers,
-                data=data,
-                auth=auth,
+            method=method,
+            url=self._base_url + path,
+            headers=headers or self.default_headers,
+            data=data,
+            auth=auth,
         ).json()
 
         error = resp.get('code')
         if error:
             raise ApiError(error)
 
         return resp
 
     @property
+    def default_headers(self):
+        return {
+            'Authorization': f'Bearer {self._access_token}',
+            'Content-Type': 'application/json',
+        }
+
+    @property
     def device_id(self):
         return self._subject_id
 
 
 class AuthenticationError(RuntimeError):
     """
     Error for authentication specific exceptions.
```

### Comparing `epson_connect-0.1.0/src/epson_connect/client.py` & `epson_connect-0.2.0/src/epson_connect/client.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.1.0/src/epson_connect/printer.py` & `epson_connect-0.2.0/src/epson_connect/printer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import pathlib
 from urllib.parse import parse_qs, urlencode, urlparse
 
 from .authenticate import AuthCtx
-from .print_settings import (
-    PrintSettingError,
-    merge_with_default_settings,
-    validate_settings,
-)
+from .printer_settings import merge_with_default_settings, validate_settings
 
 
 class Printer:
-
     VALID_EXTENSIONS = {
         'doc',
         'docx',
         'xls',
         'xlsx',
         'ppt',
         'pptx',
@@ -22,14 +17,19 @@
         'jpeg',
         'bmp',
         'gif',
         'png',
         'tiff',
     }
 
+    VALID_OPERATORS = {
+        'user',
+        'operator',
+    }
+
     def __init__(self, auth_ctx: AuthCtx) -> None:
         self._auth_ctx = auth_ctx
 
     @property
     def device_id(self):
         return self._auth_ctx.device_id
 
@@ -54,15 +54,15 @@
     def _upload_file(self, upload_uri: str, file_path: str, print_mode: str) -> None:
         """
         Upload file to be printed.
         """
         # Get extension from file path.
         extension = pathlib.Path(file_path).suffix.lower()
         if extension[1:] not in self.VALID_EXTENSIONS:
-            raise PrintSettingError(f'{extension} is not a valid printing extension.')
+            raise PrinterError(f'{extension} is not a valid printing extension.')
 
         o = urlparse(upload_uri)
         q_dict = parse_qs(o.query)
         q_dict['File'] = [f'1{extension}']
         path = o._replace(query=urlencode(q_dict)).geturl()
 
         content_type = 'application/octet-stream'
@@ -98,35 +98,60 @@
         validate_settings(settings)
 
         job_data = self._print_setting(settings)
         self._upload_file(job_data['upload_uri'], file_path, settings['print_mode'])
         self._execute_print(job_data['id'])
         return job_data['id']
 
-    def cancel_print(self, job_id):
+    def cancel_print(self, job_id, operated_by='user'):
         """
         Cancel print.
         """
         method = 'POST'
         path = f'/api/1/printing/printers/{self.device_id}/jobs/{job_id}/cancel'
 
+        if operated_by not in self.VALID_OPERATORS:
+            raise PrinterError(f'Invalid "operated_by" value {operated_by}')
+
+        job_status = self.job_info(job_id).get('status')
+        if job_status not in ('pending', 'pending_held'):
+            raise PrinterError(f'Can not cancel job with status {job_status}')
+
+        data = {
+            'operated_by': operated_by,
+        }
+
+        self._auth_ctx.send(method, path, data)
+
     def job_info(self, job_id):
         """
         Get print job information.
         """
         method = 'GET'
         path = f'/api/1/printing/printers/{self.device_id}/jobs/{job_id}'
+        return self._auth_ctx.send(method, path)
 
     def info(self):
         """
         Get device information.
         """
         method = 'GET'
         path = f'/api/1/printing/printers/{self.device_id}'
+        return self._auth_ctx.send(method, path)
 
-
-    def notifications(self):
+    def notification(self, callback_uri, enabled=True):
         """
-        Set notifications.
+        Set whether or not to notify of the print job status change.
         """
         method = 'POST'
         path = f'/api/1/printing/printers/{self.device_id}/settings/notifications'
+
+        data = {
+            'notification': enabled,
+            'callback_uri': callback_uri,
+        }
+
+        return self._auth_ctx.send(method, path, data)
+
+
+class PrinterError(ValueError):
+    pass
```

### Comparing `epson_connect-0.1.0/src/epson_connect/printer_settings.py` & `epson_connect-0.2.0/src/epson_connect/printer_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
 import string
 
-
 VALID_PRINT_MODES = {
     'document',
     'photo',
 }
 
 VALID_MEDIA_SIZES = {
     'ms_a3',
@@ -64,90 +63,58 @@
 
 def merge_with_default_settings(settings=None):
     settings = settings or {}
 
     job_name = settings.get('job_name') or ''
     if not job_name:
         # Generate random name if one is not given.
-        job_name = ''.join(random.choice(string.ascii_letters) for _ in range(25))
+        job_name = 'job-' + ''.join(random.choice(string.ascii_letters) for _ in range(8))
 
     settings['job_name'] = job_name
 
     settings['print_mode'] = settings.get('print_mode') or 'document'
 
     print_setting = settings.get('print_setting') or {}
 
     # print_setting is optional so we can exit early if its not present.
     if not print_setting:
         return settings
 
-    # Media Size
-    print_setting['media_size'] = print_setting.get('media_size') or 'ms_a4'
-
-    # media_type
-    print_setting['media_type'] = print_setting.get('media_type') or 'mt_plainpaper'
-
-    # borderless
-    print_setting['borderless'] = print_setting.get('borderless') or False
-
-    # print_quality
-    print_setting['print_quality'] = print_setting.get('print_quality') or 'normal'
-
-    # print_quality
-    print_setting['source'] = print_setting.get('source') or 'auto'
-
-    # color_mode
-    print_setting['color_mode'] = print_setting.get('color_mode') or 'color'
-
-    # two_sided
-    print_setting['2_sided'] = print_setting.get('2_sided') or 'none'
-
-    # reverse_order
-    reverse_order = print_setting.get('reverse_order')
-    if not reverse_order:
-        reverse_order = False
-
-    if print_setting['2_sided'] in ('long', 'short'):
-        reverse_order = False
-
-    print_setting['reverse_order'] = reverse_order
-
-    # copies
-    print_setting['copies'] = print_setting.get('copies') or 1
-
-    # collate
     collate = print_setting.get('collate')
-    if not collate:
-        collate = True
-
-    if print_setting['2_sided'] in ('long', 'short'):
-        collate = True
-
-    print_setting['collate'] = collate
-
-    settings['print_setting'] = print_setting
+    settings['print_setting'] = {
+        'media_size': print_setting.get('media_size') or 'ms_a4',
+        'media_type': print_setting.get('media_type') or 'mt_plainpaper',
+        'borderless': print_setting.get('borderless') or False,
+        'print_quality': print_setting.get('print_quality') or 'normal',
+        'source': print_setting.get('source') or 'auto',
+        'color_mode': print_setting.get('color_mode') or 'color',
+        '2_sided': print_setting.get('2_sided') or 'none',
+        'reverse_order': print_setting.get('reverse_order') or False,
+        'copies': print_setting.get('copies') or 1,
+        'collate': collate if collate is not None else True,
+    }
 
     return settings
 
 
-def validate_settings(settings: dict):
+def validate_settings(settings: dict):  # noqa: C901
     """
     Validate all parts of a settings object.
     """
     extra_keys = set(settings.keys()) - {'job_name', 'print_mode', 'print_setting'}
     if extra_keys:
         raise PrintSettingError(f'Invalid settings keys {extra_keys}.')
 
     job_name = settings['job_name']
     if len(job_name) > 256:
         raise PrintSettingError(f'Job name is greater than 256 chars: {job_name}')
 
     print_mode = settings['print_mode']
     if print_mode not in VALID_PRINT_MODES:
-        raise PrintSettingError(f'Not a valid print mode {print_mode}')
+        raise PrintSettingError(f'Invalid print mode {print_mode}')
 
     # print_setting is optional so we can exit early if its not present.
     print_setting = settings.get('print_setting')
     if not print_setting:
         return
 
     # Media Size
@@ -159,22 +126,22 @@
     media_type = print_setting['media_type']
     if media_type not in VALID_MEDIA_TYPES:
         raise PrintSettingError(f'Invalid media type {media_size}')
 
     # borderless
     borderless = print_setting['borderless']
     if not isinstance(borderless, bool):
-        raise PrintSettingError(f'borderless must be a bool')
+        raise PrintSettingError('borderless must be a bool')
 
     # print_quality
     print_quality = print_setting['print_quality']
     if print_quality not in VALID_PRINT_QUALITIES:
         raise PrintSettingError(f'Invalid print quality {print_quality}')
 
-    # print_quality
+    # Paper source
     source = print_setting['source']
     if source not in VALID_PAPER_SOURCES:
         raise PrintSettingError(f'Invalid source {source}')
 
     # color_mode
     color_mode = print_setting['color_mode']
     if color_mode not in VALID_COLOR_MODES:
@@ -184,22 +151,28 @@
     two_sided = print_setting['2_sided']
     if two_sided not in VALID_TWO_SIDE:
         raise PrintSettingError(f'Invalid 2-sided value {two_sided}')
 
     # reverse_order
     reverse_order = print_setting['reverse_order']
     if not isinstance(reverse_order, bool):
-        raise PrintSettingError(f'Reverse order must be a bool')
+        raise PrintSettingError('Reverse order must be a bool')
+
+    if print_setting['2_sided'] in ('long', 'short') and reverse_order:
+        raise PrintSettingError('Can not use reverse order when using two-sided printing.')
 
     # copies
     copies = print_setting['copies']
     if copies < 1 or copies > 99:
         raise PrintSettingError(f'Invalid number of copies {copies}')
 
     # collate
     collate = print_setting['collate']
     if not isinstance(collate, bool):
-        raise PrintSettingError(f'Collate must be a bool')
+        raise PrintSettingError('Collate must be a bool')
+
+    if print_setting['2_sided'] in ('long', 'short') and not collate:
+        raise PrintSettingError('Must collate when using two-sided printing.')
 
 
 class PrintSettingError(ValueError):
     pass
```

