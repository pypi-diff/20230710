# Comparing `tmp/oidc_drf-1.3.1.tar.gz` & `tmp/oidc_drf-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.3.1.tar", last modified: Mon Jul 10 10:53:10 2023, max compression
+gzip compressed data, was "oidc_drf-1.3.2.tar", last modified: Mon Jul 10 11:51:39 2023, max compression
```

## Comparing `oidc_drf-1.3.1.tar` & `oidc_drf-1.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.521790 oidc_drf-1.3.1/
--rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 10:53:10.521657 oidc_drf-1.3.1/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     6480 2023-07-06 10:57:47.000000 oidc_drf-1.3.1/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.520199 oidc_drf-1.3.1/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.3.1/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      797 2023-07-10 10:52:57.000000 oidc_drf-1.3.1/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    16022 2023-07-06 10:55:49.000000 oidc_drf-1.3.1/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4767 2023-07-06 08:46:10.000000 oidc_drf-1.3.1/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.521493 oidc_drf-1.3.1/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)      737 2023-07-10 09:25:40.000000 oidc_drf-1.3.1/oidc_drf/migrations/0001_initial.py
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.3.1/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      277 2023-07-06 10:54:59.000000 oidc_drf-1.3.1/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.3.1/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2759 2023-07-06 05:52:37.000000 oidc_drf-1.3.1/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     8348 2023-07-06 10:55:47.000000 oidc_drf-1.3.1/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.521053 oidc_drf-1.3.1/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      393 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-10 10:53:10.521834 oidc_drf-1.3.1/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1197 2023-07-10 10:53:05.000000 oidc_drf-1.3.1/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 11:51:39.871916 oidc_drf-1.3.2/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7498 2023-07-10 11:51:39.871762 oidc_drf-1.3.2/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     6679 2023-07-10 11:51:04.000000 oidc_drf-1.3.2/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 11:51:39.870375 oidc_drf-1.3.2/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.3.2/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      797 2023-07-10 10:52:57.000000 oidc_drf-1.3.2/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    16422 2023-07-10 11:47:58.000000 oidc_drf-1.3.2/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4767 2023-07-06 08:46:10.000000 oidc_drf-1.3.2/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 11:51:39.871585 oidc_drf-1.3.2/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      737 2023-07-10 09:25:40.000000 oidc_drf-1.3.2/oidc_drf/migrations/0001_initial.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.3.2/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      277 2023-07-06 10:54:59.000000 oidc_drf-1.3.2/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.3.2/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2759 2023-07-06 05:52:37.000000 oidc_drf-1.3.2/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     8324 2023-07-10 11:42:55.000000 oidc_drf-1.3.2/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 11:51:39.871170 oidc_drf-1.3.2/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7498 2023-07-10 11:51:39.000000 oidc_drf-1.3.2/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      393 2023-07-10 11:51:39.000000 oidc_drf-1.3.2/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-10 11:51:39.000000 oidc_drf-1.3.2/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-10 11:51:39.000000 oidc_drf-1.3.2/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-10 11:51:39.000000 oidc_drf-1.3.2/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-10 11:51:39.871953 oidc_drf-1.3.2/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1197 2023-07-10 11:48:16.000000 oidc_drf-1.3.2/setup.py
```

### Comparing `oidc_drf-1.3.1/PKG-INFO` & `oidc_drf-1.3.2/oidc_drf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oidc_drf
-Version: 1.3.1
+Name: oidc-drf
+Version: 1.3.2
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -116,14 +116,16 @@
 OIDC_USERNAME_ALGO = None # defalut None
 OIDC_USE_ENCODED_USERNAME = None # defalut None
 OIDC_CREATE_USER = True # defalut True, Enables or disables automatic user creation during authentication
 OIDC_CHECK_USER_MODEL = True # defalut True, if it is set to false it can authenticated based on oidc without User
 OIDC_VERIFY_KID = True # defalut True 
 OIDC_ALLOW_UNSECURED_JWT = False # defalut False
 OIDC_TOKEN_USE_BASIC_AUTH = False # defalut False
+OIDC_USER_CREATED_IS_ACTIVE= True # defalut True created user by oidc is set to is_active True
+OIDC_USER_CREATED_IS_SUPERUSER= False# defalut False  created user by oidc is set to is_superuser False
 
 # you can map the info comming back from the IDP to user model
 # defalut is {}
 OIDC_FIELD_MAPPING = {
     'field_in_my_user_model': 'field_in_in_oidc',
     'first_name': 'given_name',
     'last_name': 'family_name',
```

### Comparing `oidc_drf-1.3.1/README.md` & `oidc_drf-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 OIDC_USERNAME_ALGO = None # defalut None
 OIDC_USE_ENCODED_USERNAME = None # defalut None
 OIDC_CREATE_USER = True # defalut True, Enables or disables automatic user creation during authentication
 OIDC_CHECK_USER_MODEL = True # defalut True, if it is set to false it can authenticated based on oidc without User
 OIDC_VERIFY_KID = True # defalut True 
 OIDC_ALLOW_UNSECURED_JWT = False # defalut False
 OIDC_TOKEN_USE_BASIC_AUTH = False # defalut False
+OIDC_USER_CREATED_IS_ACTIVE= True # defalut True created user by oidc is set to is_active True
+OIDC_USER_CREATED_IS_SUPERUSER= False# defalut False  created user by oidc is set to is_superuser False
 
 # you can map the info comming back from the IDP to user model
 # defalut is {}
 OIDC_FIELD_MAPPING = {
     'field_in_my_user_model': 'field_in_in_oidc',
     'first_name': 'given_name',
     'last_name': 'family_name',
```

### Comparing `oidc_drf-1.3.1/oidc_drf/admin.py` & `oidc_drf-1.3.2/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.1/oidc_drf/backends.py` & `oidc_drf-1.3.2/oidc_drf/backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         self.OIDC_USERNAME_ALGO = import_from_settings("OIDC_USERNAME_ALGO", None)
         self.OIDC_VERIFY_KID = import_from_settings("OIDC_VERIFY_KID", True)
         self.OIDC_ALLOW_UNSECURED_JWT = import_from_settings("OIDC_ALLOW_UNSECURED_JWT", False)
         self.OIDC_USE_NONCE = import_from_settings("OIDC_USE_NONCE", True)
         self.OIDC_TOKEN_USE_BASIC_AUTH = import_from_settings("OIDC_TOKEN_USE_BASIC_AUTH", False)
         self.OIDC_CREATE_USER = import_from_settings("OIDC_CREATE_USER", True)
         self.OIDC_CHECK_USER_MODEL = import_from_settings("OIDC_CHECK_USER_MODEL", True)
+        self.OIDC_USER_CREATED_IS_ACTIVE = import_from_settings("OIDC_USER_CREATED_IS_ACTIVE", True)
+        self.OIDC_USER_CREATED_IS_SUPERUSER = import_from_settings("OIDC_USER_CREATED_IS_SUPERUSER", False)
+
         
         if self.OIDC_RP_SIGN_ALGO.startswith("RS") and (
             self.OIDC_RP_IDP_SIGN_KEY is None and self.OIDC_OP_JWKS_ENDPOINT is None
         ):
             msg = "{} alg requires OIDC_RP_IDP_SIGN_KEY or OIDC_OP_JWKS_ENDPOINT to be configured."
             raise ImproperlyConfigured(msg.format(self.OIDC_RP_SIGN_ALGO))
 
@@ -224,14 +227,17 @@
         return str(claims.get(self.OIDC_USERNAME_CLAIM))
 
     def get_user_obj(self, claims):
 
         """Return object for a newly created user account."""
         username = self.get_username(claims)        
         user_fields = self.mapper(claims)
+        # Set is_active and is_superuser fields
+        user_fields['is_active'] = self.OIDC_USER_CREATED_IS_ACTIVE
+        user_fields['is_superuser'] = self.OIDC_USER_CREATED_IS_SUPERUSER
         user = self.UserModel(username, **user_fields)
         return user
     
     def create_user(self, claims):
 
         """Return object for a newly created user account."""
         username = self.get_username(claims)
```

### Comparing `oidc_drf-1.3.1/oidc_drf/drf.py` & `oidc_drf-1.3.2/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.1/oidc_drf/migrations/0001_initial.py` & `oidc_drf-1.3.2/oidc_drf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.1/oidc_drf/utils.py` & `oidc_drf-1.3.2/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.1/oidc_drf/views.py` & `oidc_drf-1.3.2/oidc_drf/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             kwargs = {
                 "request": request,
                 "nonce": data.get("nonce",None),
                 "code_verifier": data.get("code_verifier",None),
             }
             self.user = auth.authenticate(**kwargs)
                         
-            if self.user and self.user.is_active:
+            if self.user:
                 return self.login_success()
         
         return self.login_failure("Login failed",status.HTTP_401_UNAUTHORIZED)
 
 class OIDCLogoutView(APIView):
     permission_classes = [AllowAny]    
     def login_failure(self,error_message,status):
```

### Comparing `oidc_drf-1.3.1/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oidc-drf
-Version: 1.3.1
+Name: oidc_drf
+Version: 1.3.2
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -116,14 +116,16 @@
 OIDC_USERNAME_ALGO = None # defalut None
 OIDC_USE_ENCODED_USERNAME = None # defalut None
 OIDC_CREATE_USER = True # defalut True, Enables or disables automatic user creation during authentication
 OIDC_CHECK_USER_MODEL = True # defalut True, if it is set to false it can authenticated based on oidc without User
 OIDC_VERIFY_KID = True # defalut True 
 OIDC_ALLOW_UNSECURED_JWT = False # defalut False
 OIDC_TOKEN_USE_BASIC_AUTH = False # defalut False
+OIDC_USER_CREATED_IS_ACTIVE= True # defalut True created user by oidc is set to is_active True
+OIDC_USER_CREATED_IS_SUPERUSER= False# defalut False  created user by oidc is set to is_superuser False
 
 # you can map the info comming back from the IDP to user model
 # defalut is {}
 OIDC_FIELD_MAPPING = {
     'field_in_my_user_model': 'field_in_in_oidc',
     'first_name': 'given_name',
     'last_name': 'family_name',
```

### Comparing `oidc_drf-1.3.1/setup.py` & `oidc_drf-1.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.3.1',
+    version='1.3.2',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

