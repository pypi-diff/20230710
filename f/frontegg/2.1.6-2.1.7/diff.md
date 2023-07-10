# Comparing `tmp/frontegg-2.1.6.tar.gz` & `tmp/frontegg-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontegg-2.1.6.tar", max compression
+gzip compressed data, was "frontegg-2.1.7.tar", max compression
```

## Comparing `frontegg-2.1.6.tar` & `frontegg-2.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2022-10-13 14:59:50.240636 frontegg-2.1.6/LICENSE
--rw-r--r--   0        0        0      406 2023-02-02 10:01:16.057919 frontegg-2.1.6/README-PYPI.rst
--rw-r--r--   0        0        0      213 2023-06-18 07:04:25.922682 frontegg-2.1.6/frontegg/__init__.py
--rw-r--r--   0        0        0      243 2023-06-18 07:04:25.923013 frontegg-2.1.6/frontegg/common/__init__.py
--rw-r--r--   0        0        0      489 2023-06-18 07:04:25.923620 frontegg-2.1.6/frontegg/common/cache/cache_manager.py
--rw-r--r--   0        0        0     1206 2023-06-18 07:04:25.924185 frontegg-2.1.6/frontegg/common/cache/local_cache_manager.py
--rw-r--r--   0        0        0     1147 2023-06-18 07:04:25.924616 frontegg-2.1.6/frontegg/common/cache/redis_cache_manager.py
--rw-r--r--   0        0        0      202 2023-06-18 07:04:25.925034 frontegg-2.1.6/frontegg/common/clients/__init__.py
--rw-r--r--   0        0        0     1738 2023-06-18 07:04:25.925303 frontegg-2.1.6/frontegg/common/clients/audits_client.py
--rw-r--r--   0        0        0     3506 2023-06-18 07:04:30.572278 frontegg-2.1.6/frontegg/common/clients/http_client.py
--rw-r--r--   0        0        0     4338 2023-06-18 07:04:25.925865 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_resolver.py
--rw-r--r--   0        0        0      702 2023-06-18 07:04:25.926270 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
--rw-r--r--   0        0        0     2658 2023-06-18 07:04:25.926655 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
--rw-r--r--   0        0        0      985 2023-06-18 07:04:25.926997 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
--rw-r--r--   0        0        0      989 2023-06-18 07:04:25.927373 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
--rw-r--r--   0        0        0     1801 2023-06-18 07:04:30.572728 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
--rw-r--r--   0        0        0     1328 2023-06-18 07:04:25.928029 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
--rw-r--r--   0        0        0     1238 2023-06-18 07:04:30.573137 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
--rw-r--r--   0        0        0      968 2023-06-18 07:04:25.928568 frontegg-2.1.6/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
--rw-r--r--   0        0        0     3563 2023-06-18 07:04:25.928882 frontegg-2.1.6/frontegg/common/clients/token_resolvers/token_resolver.py
--rw-r--r--   0        0        0     1382 2023-06-21 11:15:20.617134 frontegg-2.1.6/frontegg/common/clients/types.py
--rw-r--r--   0        0        0     1736 2023-06-21 11:15:20.617810 frontegg-2.1.6/frontegg/common/frontegg_authenticator.py
--rw-r--r--   0        0        0      351 2023-06-18 07:04:25.929610 frontegg-2.1.6/frontegg/common/frontegg_config.py
--rw-r--r--   0        0        0     1518 2023-06-18 07:04:25.929880 frontegg-2.1.6/frontegg/common/frontegg_context.py
--rw-r--r--   0        0        0     4236 2023-06-18 07:04:30.573772 frontegg-2.1.6/frontegg/common/identity_mixin.py
--rw-r--r--   0        0        0      250 2023-06-18 07:04:25.930276 frontegg-2.1.6/frontegg/common/package_utils.py
--rw-r--r--   0        0        0     4247 2023-06-18 07:04:25.930800 frontegg-2.1.6/frontegg/fastapi/README.md
--rw-r--r--   0        0        0       53 2022-10-13 14:59:50.242552 frontegg-2.1.6/frontegg/fastapi/__init__.py
--rw-r--r--   0        0        0     1620 2023-06-18 07:04:25.931185 frontegg-2.1.6/frontegg/fastapi/frontegg.py
--rw-r--r--   0        0        0      152 2023-06-18 07:04:25.931640 frontegg-2.1.6/frontegg/fastapi/secure_access/__init__.py
--rw-r--r--   0        0        0     4747 2023-06-21 11:15:20.618482 frontegg-2.1.6/frontegg/fastapi/secure_access/frontegg_security.py
--rw-r--r--   0        0        0     4164 2023-06-18 07:04:25.932334 frontegg-2.1.6/frontegg/flask/README.md
--rw-r--r--   0        0        0       53 2023-06-18 07:04:25.932620 frontegg-2.1.6/frontegg/flask/__init__.py
--rw-r--r--   0        0        0     1620 2023-06-18 07:04:25.932999 frontegg-2.1.6/frontegg/flask/frontegg.py
--rw-r--r--   0        0        0       86 2023-06-18 07:04:25.933554 frontegg-2.1.6/frontegg/flask/secure_access/__init__.py
--rw-r--r--   0        0        0     1820 2023-06-18 07:04:25.933948 frontegg-2.1.6/frontegg/flask/secure_access/with_authentication.py
--rw-r--r--   0        0        0      589 2023-06-18 07:04:25.934422 frontegg-2.1.6/frontegg/helpers/exceptions.py
--rw-r--r--   0        0        0     1669 2023-06-18 07:04:25.934917 frontegg-2.1.6/frontegg/helpers/frontegg_urls.py
--rw-r--r--   0        0        0      295 2022-10-13 14:59:50.243962 frontegg-2.1.6/frontegg/helpers/logger.py
--rw-r--r--   0        0        0      984 2023-06-18 07:04:25.935451 frontegg-2.1.6/frontegg/helpers/retry.py
--rw-r--r--   0        0        0     1582 2023-06-21 11:23:25.405797 frontegg-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 frontegg-2.1.6/setup.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 frontegg-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-13 14:59:50.240636 frontegg-2.1.7/LICENSE
+-rw-r--r--   0        0        0      406 2023-02-02 10:01:16.057919 frontegg-2.1.7/README-PYPI.rst
+-rw-r--r--   0        0        0      213 2023-06-18 07:04:25.922682 frontegg-2.1.7/frontegg/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-18 07:04:25.923013 frontegg-2.1.7/frontegg/common/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-18 07:04:25.923620 frontegg-2.1.7/frontegg/common/cache/cache_manager.py
+-rw-r--r--   0        0        0     1206 2023-06-18 07:04:25.924185 frontegg-2.1.7/frontegg/common/cache/local_cache_manager.py
+-rw-r--r--   0        0        0     1147 2023-06-18 07:04:25.924616 frontegg-2.1.7/frontegg/common/cache/redis_cache_manager.py
+-rw-r--r--   0        0        0      202 2023-06-18 07:04:25.925034 frontegg-2.1.7/frontegg/common/clients/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-18 07:04:25.925303 frontegg-2.1.7/frontegg/common/clients/audits_client.py
+-rw-r--r--   0        0        0     3506 2023-06-18 07:04:30.572278 frontegg-2.1.7/frontegg/common/clients/http_client.py
+-rw-r--r--   0        0        0     4338 2023-06-18 07:04:25.925865 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_resolver.py
+-rw-r--r--   0        0        0      702 2023-06-18 07:04:25.926270 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
+-rw-r--r--   0        0        0     2658 2023-06-18 07:04:25.926655 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
+-rw-r--r--   0        0        0      985 2023-06-18 07:04:25.926997 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
+-rw-r--r--   0        0        0      989 2023-06-18 07:04:25.927373 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
+-rw-r--r--   0        0        0     1801 2023-06-18 07:04:30.572728 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
+-rw-r--r--   0        0        0     1364 2023-07-10 07:27:38.016804 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
+-rw-r--r--   0        0        0     1274 2023-07-10 07:53:34.815375 frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
+-rw-r--r--   0        0        0      968 2023-06-18 07:04:25.928568 frontegg-2.1.7/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
+-rw-r--r--   0        0        0     3563 2023-06-18 07:04:25.928882 frontegg-2.1.7/frontegg/common/clients/token_resolvers/token_resolver.py
+-rw-r--r--   0        0        0     1382 2023-06-21 11:15:20.617134 frontegg-2.1.7/frontegg/common/clients/types.py
+-rw-r--r--   0        0        0     1736 2023-06-21 11:15:20.617810 frontegg-2.1.7/frontegg/common/frontegg_authenticator.py
+-rw-r--r--   0        0        0      351 2023-06-18 07:04:25.929610 frontegg-2.1.7/frontegg/common/frontegg_config.py
+-rw-r--r--   0        0        0     1518 2023-06-18 07:04:25.929880 frontegg-2.1.7/frontegg/common/frontegg_context.py
+-rw-r--r--   0        0        0     4236 2023-06-18 07:04:30.573772 frontegg-2.1.7/frontegg/common/identity_mixin.py
+-rw-r--r--   0        0        0      250 2023-06-18 07:04:25.930276 frontegg-2.1.7/frontegg/common/package_utils.py
+-rw-r--r--   0        0        0     4247 2023-06-18 07:04:25.930800 frontegg-2.1.7/frontegg/fastapi/README.md
+-rw-r--r--   0        0        0       53 2022-10-13 14:59:50.242552 frontegg-2.1.7/frontegg/fastapi/__init__.py
+-rw-r--r--   0        0        0     1620 2023-06-18 07:04:25.931185 frontegg-2.1.7/frontegg/fastapi/frontegg.py
+-rw-r--r--   0        0        0      152 2023-06-18 07:04:25.931640 frontegg-2.1.7/frontegg/fastapi/secure_access/__init__.py
+-rw-r--r--   0        0        0     4747 2023-06-21 11:15:20.618482 frontegg-2.1.7/frontegg/fastapi/secure_access/frontegg_security.py
+-rw-r--r--   0        0        0     4164 2023-06-18 07:04:25.932334 frontegg-2.1.7/frontegg/flask/README.md
+-rw-r--r--   0        0        0       53 2023-06-18 07:04:25.932620 frontegg-2.1.7/frontegg/flask/__init__.py
+-rw-r--r--   0        0        0     1620 2023-06-18 07:04:25.932999 frontegg-2.1.7/frontegg/flask/frontegg.py
+-rw-r--r--   0        0        0       86 2023-06-18 07:04:25.933554 frontegg-2.1.7/frontegg/flask/secure_access/__init__.py
+-rw-r--r--   0        0        0     1820 2023-06-18 07:04:25.933948 frontegg-2.1.7/frontegg/flask/secure_access/with_authentication.py
+-rw-r--r--   0        0        0      589 2023-06-18 07:04:25.934422 frontegg-2.1.7/frontegg/helpers/exceptions.py
+-rw-r--r--   0        0        0     1669 2023-06-18 07:04:25.934917 frontegg-2.1.7/frontegg/helpers/frontegg_urls.py
+-rw-r--r--   0        0        0      295 2022-10-13 14:59:50.243962 frontegg-2.1.7/frontegg/helpers/logger.py
+-rw-r--r--   0        0        0      984 2023-06-18 07:04:25.935451 frontegg-2.1.7/frontegg/helpers/retry.py
+-rw-r--r--   0        0        0     1582 2023-07-10 08:09:34.941230 frontegg-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 frontegg-2.1.7/setup.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 frontegg-2.1.7/PKG-INFO
```

### Comparing `frontegg-2.1.6/LICENSE` & `frontegg-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/cache/local_cache_manager.py` & `frontegg-2.1.7/frontegg/common/cache/local_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/cache/redis_cache_manager.py` & `frontegg-2.1.7/frontegg/common/cache/redis_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/audits_client.py` & `frontegg-2.1.7/frontegg/common/clients/audits_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/http_client.py` & `frontegg-2.1.7/frontegg/common/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_resolver.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,10 +19,11 @@
         data = response.json()
 
         return {**entity, 'roles': data.get('roles'), 'permissions': data.get('permissions')}
 
     def get_active_access_token_ids_from_identity(self) -> List[str]:
         response = self.client.get(
             urljoin(frontegg_urls.identity_service['base_url'], 'resources/vendor-only/tenants/access-tokens/v1/active'))
+        response.raise_for_status()
         data = response.json()
 
         return data
```

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def __init__(self, client: HttpClient):
         super().__init__(TokenTypes.UserAccessToken.value)
         self.client = client
 
     def get_entity_from_identity(self, entity: IUserAccessToken) -> IEntityWithRoles:
         endpoint = urljoin('resources/vendor-only/users/access-tokens/v1/', entity.get('sub'))
         response = self.client.get(urljoin(frontegg_urls.identity_service['base_url'], endpoint))
+        response.raise_for_status()
         data = response.json()
 
         return {**entity, 'roles': data.get('roles'), 'permissions': data.get('permissions')}
 
     def get_active_access_token_ids_from_identity(self) -> List[str]:
         response = self.client.get(
             urljoin(frontegg_urls.identity_service['base_url'], 'resources/vendor-only/users/access-tokens/v1/active'))
```

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/authorization_header_resolver.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/authorization_header_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/token_resolvers/token_resolver.py` & `frontegg-2.1.7/frontegg/common/clients/token_resolvers/token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/clients/types.py` & `frontegg-2.1.7/frontegg/common/clients/types.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/frontegg_authenticator.py` & `frontegg-2.1.7/frontegg/common/frontegg_authenticator.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/frontegg_context.py` & `frontegg-2.1.7/frontegg/common/frontegg_context.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/common/identity_mixin.py` & `frontegg-2.1.7/frontegg/common/identity_mixin.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/fastapi/README.md` & `frontegg-2.1.7/frontegg/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/fastapi/frontegg.py` & `frontegg-2.1.7/frontegg/fastapi/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/fastapi/secure_access/frontegg_security.py` & `frontegg-2.1.7/frontegg/fastapi/secure_access/frontegg_security.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/flask/README.md` & `frontegg-2.1.7/frontegg/flask/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/flask/frontegg.py` & `frontegg-2.1.7/frontegg/flask/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/flask/secure_access/with_authentication.py` & `frontegg-2.1.7/frontegg/flask/secure_access/with_authentication.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/helpers/exceptions.py` & `frontegg-2.1.7/frontegg/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/helpers/frontegg_urls.py` & `frontegg-2.1.7/frontegg/helpers/frontegg_urls.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/frontegg/helpers/retry.py` & `frontegg-2.1.7/frontegg/helpers/retry.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.6/pyproject.toml` & `frontegg-2.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frontegg"
-version = "2.1.6"
+version = "2.1.7"
 description = "Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code."
 homepage = "https://frontegg.com/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `frontegg-2.1.6/setup.py` & `frontegg-2.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'typing-extensions>=4.4.0,<5.0.0']
 
 extras_require = \
 {'fastapi': ['fastapi'], 'flask': ['flask>=1.0,<2.0']}
 
 setup_kwargs = {
     'name': 'frontegg',
-    'version': '2.1.6',
+    'version': '2.1.7',
     'description': 'Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.',
     'long_description': '.. image:: https://fronteggstuff.blob.core.windows.net/frongegg-logos/logo-transparent.png\n   :alt: Frontegg\n\nFrontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.\n\nFor more information and usage you can visit the `github repo <https://github.com/frontegg/python-sdk>`_.',
     'author': 'Frontegg LTD',
     'author_email': 'hello@frontegg.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://frontegg.com/',
```

### Comparing `frontegg-2.1.6/PKG-INFO` & `frontegg-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontegg
-Version: 2.1.6
+Version: 2.1.7
 Summary: Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.
 Home-page: https://frontegg.com/
 Author: Frontegg LTD
 Author-email: hello@frontegg.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

