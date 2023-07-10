# Comparing `tmp/arcane_pinterest-2.0.0.tar.gz` & `tmp/arcane_pinterest-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane_pinterest-2.0.0.tar", max compression
+gzip compressed data, was "arcane_pinterest-2.1.0.tar", max compression
```

## Comparing `arcane_pinterest-2.0.0.tar` & `arcane_pinterest-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      112 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/__init__.py
--rw-r--r--   0        0        0       51 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/const.py
--rw-r--r--   0        0        0      241 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/exceptions.py
--rw-r--r--   0        0        0     2394 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/lib.py
--rw-r--r--   0        0        0     6882 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/pinterest.py
--rw-r--r--   0        0        0      123 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/types.py
--rw-r--r--   0        0        0      408 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 arcane_pinterest-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-07-10 07:44:41.562000 arcane_pinterest-2.1.0/arcane/pinterest/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-10 07:44:41.562000 arcane_pinterest-2.1.0/arcane/pinterest/const.py
+-rw-r--r--   0        0        0      241 2023-07-10 07:44:41.562000 arcane_pinterest-2.1.0/arcane/pinterest/exceptions.py
+-rw-r--r--   0        0        0     2394 2023-07-10 07:44:41.562000 arcane_pinterest-2.1.0/arcane/pinterest/lib.py
+-rw-r--r--   0        0        0     8082 2023-07-10 07:44:41.562000 arcane_pinterest-2.1.0/arcane/pinterest/pinterest.py
+-rw-r--r--   0        0        0      123 2023-07-10 07:44:41.562000 arcane_pinterest-2.1.0/arcane/pinterest/types.py
+-rw-r--r--   0        0        0      408 2023-07-10 07:44:41.562000 arcane_pinterest-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 arcane_pinterest-2.1.0/PKG-INFO
```

### Comparing `arcane_pinterest-2.0.0/arcane/pinterest/lib.py` & `arcane_pinterest-2.1.0/arcane/pinterest/lib.py`

 * *Files identical despite different names*

### Comparing `arcane_pinterest-2.0.0/arcane/pinterest/pinterest.py` & `arcane_pinterest-2.1.0/arcane/pinterest/pinterest.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 API_VERSION = 'v5'
 
 class PinterestClient:
     def __init__(self, pinterest_credentials_path: str, _adscale_log: Optional[Callable] = None) -> None:
         with open(pinterest_credentials_path) as credentials:
             pinterest_credentials = json.load(credentials)
             pinterest_credentials = cast(dict[str, str], pinterest_credentials)
-        self._app_id = pinterest_credentials.get('app_id'),
-        self._app_secret = pinterest_credentials.get('app_secret'),
-        self._token = pinterest_credentials.get('access_token')
+        self._app_id = pinterest_credentials['app_id']
+        self._app_secret = pinterest_credentials['app_secret']
+        self._token = pinterest_credentials['access_token']
+        self._refresh_token = pinterest_credentials['refresh_token']
+
         # To get owner user id, you should go to Pinterest > Business Access > Select Arcane - The Feed Agency > Employee > Select the employee (ie: reporting@arcane.run (production) or pierre@arcane.run(staging))
         # > Get the last id in url: pinterest.fr/business/business-access/{business_id}/employees/{owner_user_id}/details/
         self._owner_user_id = pinterest_credentials.get('owner_user_id')
         if _adscale_log:
             self.log = _adscale_log
         else:
             self.log = print
@@ -45,14 +47,48 @@
             response_temp = requests.request(method=method, url=f"{PINTEREST_SERVER_URL}{endpoint}", headers=headers, params=params, **kwargs)
             response_temp.raise_for_status()
             response_temp = response_temp.json()
             response['items'] += response_temp['items']
 
         return response
 
+    def refresh_token(self) -> str:
+
+        def _hash_token(token: str) -> str:
+            import hashlib
+            return hashlib.sha256(token.encode()).hexdigest()
+
+        previous_hased_token = _hash_token(self._token)
+
+        json_params = {
+            'grant_type': 'refresh_token',
+            'refresh_token': self._refresh_token,
+            'scope': 'ads:read'
+        }
+
+        auth = self._app_id + ":" + self._app_secret
+        import base64
+        b64auth = base64.b64encode(auth.encode("ascii")).decode("ascii")
+        auth_headers = {"Authorization": "Basic " + b64auth}
+        response = requests.request(
+            method='POST',
+            url=f"{PINTEREST_SERVER_URL}/v5/oauth/token",
+            data=json_params,
+            headers={
+                'ContentType': 'application/x-www-form-urlencoded',
+                **auth_headers
+            }
+        )
+        response.raise_for_status()
+        response = response.json()
+        new_token = response['access_token']
+        assert _hash_token(new_token) != previous_hased_token, "New token is the same as the previous one"
+
+        return new_token
+
     def get_account_campaigns(self, ad_account_id: str) -> List[dict[str, str]]:
         """Get account campaigns given its ID."""
         try:
             response = self._make_request(
                 f'/{API_VERSION}/ad_accounts/{ad_account_id}/campaigns/',
                 'GET'
                 )
```

### Comparing `arcane_pinterest-2.0.0/PKG-INFO` & `arcane_pinterest-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcane-pinterest
-Version: 2.0.0
+Version: 2.1.0
 Summary: Helpers to request Pinterest API 
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

