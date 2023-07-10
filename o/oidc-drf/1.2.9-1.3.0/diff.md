# Comparing `tmp/oidc_drf-1.2.9.tar.gz` & `tmp/oidc_drf-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.2.9.tar", last modified: Tue Jul  4 11:09:44 2023, max compression
+gzip compressed data, was "oidc_drf-1.3.0.tar", last modified: Mon Jul 10 09:32:16 2023, max compression
```

## Comparing `oidc_drf-1.2.9.tar` & `oidc_drf-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.923215 oidc_drf-1.2.9/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:09:44.923090 oidc_drf-1.2.9/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.9/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.922111 oidc_drf-1.2.9/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.9/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.9/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    16020 2023-07-04 11:05:08.000000 oidc_drf-1.2.9/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.9/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.922935 oidc_drf-1.2.9/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.9/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.9/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.9/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.9/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     8944 2023-07-04 11:09:32.000000 oidc_drf-1.2.9/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.922797 oidc_drf-1.2.9/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 11:09:44.923249 oidc_drf-1.2.9/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 11:09:41.000000 oidc_drf-1.2.9/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.661878 oidc_drf-1.3.0/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 09:32:16.661740 oidc_drf-1.3.0/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     6480 2023-07-06 10:57:47.000000 oidc_drf-1.3.0/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.660562 oidc_drf-1.3.0/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.3.0/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-05 17:40:53.000000 oidc_drf-1.3.0/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    16022 2023-07-06 10:55:49.000000 oidc_drf-1.3.0/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4767 2023-07-06 08:46:10.000000 oidc_drf-1.3.0/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.661546 oidc_drf-1.3.0/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      737 2023-07-10 09:25:40.000000 oidc_drf-1.3.0/oidc_drf/migrations/0001_initial.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.3.0/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      277 2023-07-06 10:54:59.000000 oidc_drf-1.3.0/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.3.0/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2759 2023-07-06 05:52:37.000000 oidc_drf-1.3.0/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     8348 2023-07-06 10:55:47.000000 oidc_drf-1.3.0/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.661191 oidc_drf-1.3.0/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      393 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-10 09:32:16.661915 oidc_drf-1.3.0/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1197 2023-07-10 09:27:55.000000 oidc_drf-1.3.0/setup.py
```

### Comparing `oidc_drf-1.2.9/PKG-INFO` & `oidc_drf-1.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: oidc_drf
-Version: 1.2.9
-Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
-Home-page: https://github.com/halmogbl/oidc_drf
-Author: Hamad Almogbl
-Author-email: hamad.almogbl@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-
 # Overview
 
 Django DRF OIDC Auth library Securely authenticate users using OIDC in Django DRF. 
 It Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 
 ----
 # Installation
@@ -40,22 +24,20 @@
 
 Configure the following settings in your Django project's settings module:
 
 ```python
 
 OIDC_RP_CLIENT_ID = '' # required
 OIDC_RP_CLIENT_SECRET = '' # optional if public client 
-OIDC_OP_JWKS_ENDPOINT = None # defalut None
 OIDC_OP_AUTHORIZATION_ENDPOINT = ''# required
 OIDC_OP_TOKEN_ENDPOINT = ''# required
 OIDC_OP_USER_ENDPOINT = '' # required
 OIDC_OP_LOGOUT_ENDPOINT ='' # required
 
 OIDC_AUTHENTICATION_SSO_CALLBACK_URL = '' # required - identity provider will redirect you to this url after login
-OIDC_LOGOUT_REDIRECT_URL = '' # required - identity provider will redirect you to this url after logout
 
 # Django Rest Framework settings
 REST_FRAMEWORK = {
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'oidc_drf.drf.OIDCAuthentication',  # This is important to be the first one 
     ],
 }
@@ -99,27 +81,30 @@
 those settings are optional and populated with default values.
 
 ```python
 
 OIDC_USE_NONCE = True # defalut true
 OIDC_USE_PKCE = True # defalut true
 
-OIDC_USERNAME_CLAIM = 'preferred_username' # defalut 'preferred_username'
-OIDC_RP_SIGN_ALGO = 'RS256' # defalut RS256
-OIDC_RP_SCOPES = 'openid email' # defalut openid email
+# For RS256 algorithm to work, you need to set either the OP signing key or the OP JWKS Endpoint.
 OIDC_RP_IDP_SIGN_KEY = None # defalut None
+OIDC_OP_JWKS_ENDPOINT = None # defalut None
+
+OIDC_USERNAME_CLAIM = 'preferred_username' # defalut 'preferred_username'
+OIDC_RP_SIGN_ALGO = 'HS256' # defalut HS256
+OIDC_RP_SCOPES = 'openid email profile' # defalut openid 
 OIDC_VERIFY_SSL = True # defalut True
 OIDC_TIMEOUT = None # defalut None
 OIDC_PROXY = None # defalut None
 OIDC_USERNAME_ALGO = None # defalut None
 OIDC_USE_ENCODED_USERNAME = None # defalut None
 OIDC_CREATE_USER = True # defalut True, Enables or disables automatic user creation during authentication
+OIDC_CHECK_USER_MODEL = True # defalut True, if it is set to false it can authenticated based on oidc without User
 OIDC_VERIFY_KID = True # defalut True 
 OIDC_ALLOW_UNSECURED_JWT = False # defalut False
-returning unsecured JWT tokens and RP wants to accept them.
 OIDC_TOKEN_USE_BASIC_AUTH = False # defalut False
 
 # you can map the info comming back from the IDP to user model
 # defalut is {}
 OIDC_FIELD_MAPPING = {
     'field_in_my_user_model': 'field_in_in_oidc',
     'first_name': 'given_name',
@@ -138,28 +123,62 @@
 ![Screenshot3][django_admin_3]
 ----
 # REST APIs
 The REST API to the OIDC DRF is described below.
 
 ## AUTH ENDPOINT
 
+**Note**
+
+If `OIDC_USE_PKCE` is set to `True`:
+
+- You should add `code_challenge` and `code_challenge_method` parameters to the authentication endpoint.
+- You should save the `code_verifier` in local storage because it will be needed in the callback and refresh endpoints.
+
+If `OIDC_USE_NONCE` is set to `True`:
+
+- You should add the `nonce` parameter to the authentication endpoint.
+- You should save the `nonce` in local storage because it will be needed in the callback endpoint.
+
+----
+***To generate the `code_challenge` and `nonce`, refer to this JavaScript library: [oidc_pkce](https://github.com/halmogbl/oidc_pkce).***
+
+----
+
+
+Example request with parameters:
 ### Request
 
 `GET /oidc/auth/`
 
     curl --location 'http://localhost:8000/oidc/auth?code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss&code_challenge_method=S256&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc'
 ### Response
 
     Status: 200 OK
     {
         "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc&code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss0&code_challenge_method=S256"
     }
     
 ## CALLBACK ENDPOINT
 
+**Note**
+
+If `OIDC_USE_PKCE` is set to `True`:
+
+- you should include the "code_verifier" parameter in the request body.
+
+If `OIDC_USE_NONCE` is set to `True`:
+
+- you should include the "nonce" parameter in the request body.
+
+Remember to pass all the parameters returned from the 'OIDC_AUTHENTICATION_SSO_CALLBACK_URL', such as `state`, `session_state`, and `code`, to the callback endpoint.
+
+Example request with parameters and request body:
+
+
 ### Request
 
 `POST /oidc/callback/`
 
     curl --location 'http://localhost:8000/oidc/callback/?state=alksdfjlka&session_state=alsdjflajsdk&code=alsdjflaksdflkjls' \
     --header 'Content-Type: application/json' \
     --data '{
@@ -168,55 +187,59 @@
     }'
 ### Response
 
     Status: 200 OK
     {
        "access":"jwt access token",
        "refresh":"jwt refresh token",
-       "oidc_id_token":"jwt id token",
     }
 
 
 
 ## REFRESH ENDPOINT
 
+**Note**
+
+If `OIDC_USE_PKCE` is set to `True`:
+- you should include the "code_verifier" parameter in the request body.
 ### Request
 
 `POST /oidc/refresh/`
 
+Example request with request body:
+
     curl --location 'http://localhost:8000/oidc/refresh/' \
     --header 'Content-Type: application/json' \
     --data '{
         "refresh": "jwt refresh token",
         "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
         }'
 ### Response
 
     Status: 200 OK
     {
        "access":"jwt access token",
        "refresh":"jwt refresh token",
-       "oidc_id_token":"jwt id token",
     }
 
 
 ## LOGOUT ENDPOINT
 
 ### Request
 
 `POST /oidc/logout/`
 
     curl --location 'http://localhost:8000/api/v1/oidc/logout' \
-    --data '{"oidc_id_token": "jwt id token"}'
+    --data '{"refresh": "jwt refresh token"}'
 
 ### Response
 
     Status: 200 OK
     {
-        "message": "Logout OIDC successful"
+        "message": "Logout OIDC Successful"
     }
 
 
 [django_admin_1]: https://i.ibb.co/855dw0N/django-admin-1.png
 [django_admin_2]: https://i.ibb.co/LdmfNky/django-admin-2.png
 [django_admin_3]: https://i.ibb.co/J2rDkXS/django-admin-3.png
```

### Comparing `oidc_drf-1.2.9/README.md` & `oidc_drf-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: oidc_drf
+Version: 1.3.0
+Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
+Home-page: https://github.com/halmogbl/oidc_drf
+Author: Hamad Almogbl
+Author-email: hamad.almogbl@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Security
+Description-Content-Type: text/markdown
+
 # Overview
 
 Django DRF OIDC Auth library Securely authenticate users using OIDC in Django DRF. 
 It Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 
 ----
 # Installation
@@ -24,22 +42,20 @@
 
 Configure the following settings in your Django project's settings module:
 
 ```python
 
 OIDC_RP_CLIENT_ID = '' # required
 OIDC_RP_CLIENT_SECRET = '' # optional if public client 
-OIDC_OP_JWKS_ENDPOINT = None # defalut None
 OIDC_OP_AUTHORIZATION_ENDPOINT = ''# required
 OIDC_OP_TOKEN_ENDPOINT = ''# required
 OIDC_OP_USER_ENDPOINT = '' # required
 OIDC_OP_LOGOUT_ENDPOINT ='' # required
 
 OIDC_AUTHENTICATION_SSO_CALLBACK_URL = '' # required - identity provider will redirect you to this url after login
-OIDC_LOGOUT_REDIRECT_URL = '' # required - identity provider will redirect you to this url after logout
 
 # Django Rest Framework settings
 REST_FRAMEWORK = {
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'oidc_drf.drf.OIDCAuthentication',  # This is important to be the first one 
     ],
 }
@@ -83,27 +99,30 @@
 those settings are optional and populated with default values.
 
 ```python
 
 OIDC_USE_NONCE = True # defalut true
 OIDC_USE_PKCE = True # defalut true
 
-OIDC_USERNAME_CLAIM = 'preferred_username' # defalut 'preferred_username'
-OIDC_RP_SIGN_ALGO = 'RS256' # defalut RS256
-OIDC_RP_SCOPES = 'openid email' # defalut openid email
+# For RS256 algorithm to work, you need to set either the OP signing key or the OP JWKS Endpoint.
 OIDC_RP_IDP_SIGN_KEY = None # defalut None
+OIDC_OP_JWKS_ENDPOINT = None # defalut None
+
+OIDC_USERNAME_CLAIM = 'preferred_username' # defalut 'preferred_username'
+OIDC_RP_SIGN_ALGO = 'HS256' # defalut HS256
+OIDC_RP_SCOPES = 'openid email profile' # defalut openid 
 OIDC_VERIFY_SSL = True # defalut True
 OIDC_TIMEOUT = None # defalut None
 OIDC_PROXY = None # defalut None
 OIDC_USERNAME_ALGO = None # defalut None
 OIDC_USE_ENCODED_USERNAME = None # defalut None
 OIDC_CREATE_USER = True # defalut True, Enables or disables automatic user creation during authentication
+OIDC_CHECK_USER_MODEL = True # defalut True, if it is set to false it can authenticated based on oidc without User
 OIDC_VERIFY_KID = True # defalut True 
 OIDC_ALLOW_UNSECURED_JWT = False # defalut False
-returning unsecured JWT tokens and RP wants to accept them.
 OIDC_TOKEN_USE_BASIC_AUTH = False # defalut False
 
 # you can map the info comming back from the IDP to user model
 # defalut is {}
 OIDC_FIELD_MAPPING = {
     'field_in_my_user_model': 'field_in_in_oidc',
     'first_name': 'given_name',
@@ -122,28 +141,62 @@
 ![Screenshot3][django_admin_3]
 ----
 # REST APIs
 The REST API to the OIDC DRF is described below.
 
 ## AUTH ENDPOINT
 
+**Note**
+
+If `OIDC_USE_PKCE` is set to `True`:
+
+- You should add `code_challenge` and `code_challenge_method` parameters to the authentication endpoint.
+- You should save the `code_verifier` in local storage because it will be needed in the callback and refresh endpoints.
+
+If `OIDC_USE_NONCE` is set to `True`:
+
+- You should add the `nonce` parameter to the authentication endpoint.
+- You should save the `nonce` in local storage because it will be needed in the callback endpoint.
+
+----
+***To generate the `code_challenge` and `nonce`, refer to this JavaScript library: [oidc_pkce](https://github.com/halmogbl/oidc_pkce).***
+
+----
+
+
+Example request with parameters:
 ### Request
 
 `GET /oidc/auth/`
 
     curl --location 'http://localhost:8000/oidc/auth?code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss&code_challenge_method=S256&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc'
 ### Response
 
     Status: 200 OK
     {
         "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc&code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss0&code_challenge_method=S256"
     }
     
 ## CALLBACK ENDPOINT
 
+**Note**
+
+If `OIDC_USE_PKCE` is set to `True`:
+
+- you should include the "code_verifier" parameter in the request body.
+
+If `OIDC_USE_NONCE` is set to `True`:
+
+- you should include the "nonce" parameter in the request body.
+
+Remember to pass all the parameters returned from the 'OIDC_AUTHENTICATION_SSO_CALLBACK_URL', such as `state`, `session_state`, and `code`, to the callback endpoint.
+
+Example request with parameters and request body:
+
+
 ### Request
 
 `POST /oidc/callback/`
 
     curl --location 'http://localhost:8000/oidc/callback/?state=alksdfjlka&session_state=alsdjflajsdk&code=alsdjflaksdflkjls' \
     --header 'Content-Type: application/json' \
     --data '{
@@ -152,55 +205,59 @@
     }'
 ### Response
 
     Status: 200 OK
     {
        "access":"jwt access token",
        "refresh":"jwt refresh token",
-       "oidc_id_token":"jwt id token",
     }
 
 
 
 ## REFRESH ENDPOINT
 
+**Note**
+
+If `OIDC_USE_PKCE` is set to `True`:
+- you should include the "code_verifier" parameter in the request body.
 ### Request
 
 `POST /oidc/refresh/`
 
+Example request with request body:
+
     curl --location 'http://localhost:8000/oidc/refresh/' \
     --header 'Content-Type: application/json' \
     --data '{
         "refresh": "jwt refresh token",
         "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
         }'
 ### Response
 
     Status: 200 OK
     {
        "access":"jwt access token",
        "refresh":"jwt refresh token",
-       "oidc_id_token":"jwt id token",
     }
 
 
 ## LOGOUT ENDPOINT
 
 ### Request
 
 `POST /oidc/logout/`
 
     curl --location 'http://localhost:8000/api/v1/oidc/logout' \
-    --data '{"oidc_id_token": "jwt id token"}'
+    --data '{"refresh": "jwt refresh token"}'
 
 ### Response
 
     Status: 200 OK
     {
-        "message": "Logout OIDC successful"
+        "message": "Logout OIDC Successful"
     }
 
 
 [django_admin_1]: https://i.ibb.co/855dw0N/django-admin-1.png
 [django_admin_2]: https://i.ibb.co/LdmfNky/django-admin-2.png
 [django_admin_3]: https://i.ibb.co/J2rDkXS/django-admin-3.png
```

### Comparing `oidc_drf-1.2.9/oidc_drf/admin.py` & `oidc_drf-1.3.0/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.9/oidc_drf/backends.py` & `oidc_drf-1.3.0/oidc_drf/backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import base64
-import hashlib
+
 import requests
 import logging
 import json
 import jwt
 
-from oidc_drf.utils import import_from_settings
+from oidc_drf.utils import import_from_settings, default_username_algo
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.backends import ModelBackend
 from django.contrib.auth.backends import ModelBackend
 from django.core.exceptions import ImproperlyConfigured, SuspiciousOperation
 from django.utils.module_loading import import_string
 from django.utils.encoding import force_bytes, smart_bytes, smart_str
@@ -20,88 +19,70 @@
 from josepy.jwk import JWK
 
 from oidc_drf.models import OIDCExtraData
 LOGGER = logging.getLogger(__name__)
 
 
 
-def default_username_algo(email):
-    """Generate username for the Django user.
-
-    :arg str/unicode email: the email address to use to generate a username
-
-    :returns: str/unicode
-
-    """
-    # bluntly stolen from django-browserid
-    # store the username as a base64 encoded sha224 of the email address
-    # this protects against data leakage because usernames are often
-    # treated as public identifiers (so we can't use the email address).
-    username = base64.urlsafe_b64encode(
-        hashlib.sha1(force_bytes(email)).digest()
-    ).rstrip(b"=")
 
-    return smart_str(username)
 
 class OIDCAuthenticationBackend(ModelBackend):
 
     def __init__(self, *args, **kwargs):
         """Initialize settings."""
+        self.UserModel = get_user_model()
         self.OIDC_OP_TOKEN_ENDPOINT = import_from_settings("OIDC_OP_TOKEN_ENDPOINT")
         self.OIDC_OP_USER_ENDPOINT = import_from_settings("OIDC_OP_USER_ENDPOINT")
         self.OIDC_OP_JWKS_ENDPOINT = import_from_settings("OIDC_OP_JWKS_ENDPOINT", None)
         self.OIDC_RP_CLIENT_ID = import_from_settings("OIDC_RP_CLIENT_ID")
         self.OIDC_RP_CLIENT_SECRET = import_from_settings("OIDC_RP_CLIENT_SECRET","")
-        self.OIDC_RP_SIGN_ALGO = import_from_settings("OIDC_RP_SIGN_ALGO", "RS256")
+        self.OIDC_RP_SIGN_ALGO = import_from_settings("OIDC_RP_SIGN_ALGO", "HS256")
         self.OIDC_RP_IDP_SIGN_KEY = import_from_settings("OIDC_RP_IDP_SIGN_KEY", None)
-
+        self.OIDC_AUTHENTICATION_SSO_CALLBACK_URL = import_from_settings("OIDC_AUTHENTICATION_SSO_CALLBACK_URL", "http://localhost:3000/callback")
+        self.OIDC_VERIFY_SSL = import_from_settings("OIDC_VERIFY_SSL", True)
+        self.OIDC_TIMEOUT = import_from_settings("OIDC_TIMEOUT", None)
+        self.OIDC_PROXY = import_from_settings("OIDC_PROXY", None)
+        self.OIDC_RP_SCOPES = import_from_settings("OIDC_RP_SCOPES", "openid email profile")
+        self.OIDC_USERNAME_CLAIM = import_from_settings("OIDC_USERNAME_CLAIM", "preferred_username")
+        self.OIDC_FIELD_MAPPING = import_from_settings("OIDC_FIELD_MAPPING",{} )
+        self.OIDC_USE_ENCODED_USERNAME = import_from_settings("OIDC_USE_ENCODED_USERNAME", None)
+        self.OIDC_USERNAME_ALGO = import_from_settings("OIDC_USERNAME_ALGO", None)
+        self.OIDC_VERIFY_KID = import_from_settings("OIDC_VERIFY_KID", True)
+        self.OIDC_ALLOW_UNSECURED_JWT = import_from_settings("OIDC_ALLOW_UNSECURED_JWT", False)
+        self.OIDC_USE_NONCE = import_from_settings("OIDC_USE_NONCE", True)
+        self.OIDC_TOKEN_USE_BASIC_AUTH = import_from_settings("OIDC_TOKEN_USE_BASIC_AUTH", False)
+        self.OIDC_CREATE_USER = import_from_settings("OIDC_CREATE_USER", True)
+        self.OIDC_CHECK_USER_MODEL = import_from_settings("OIDC_CHECK_USER_MODEL", True)
+        
         if self.OIDC_RP_SIGN_ALGO.startswith("RS") and (
             self.OIDC_RP_IDP_SIGN_KEY is None and self.OIDC_OP_JWKS_ENDPOINT is None
         ):
             msg = "{} alg requires OIDC_RP_IDP_SIGN_KEY or OIDC_OP_JWKS_ENDPOINT to be configured."
             raise ImproperlyConfigured(msg.format(self.OIDC_RP_SIGN_ALGO))
 
-        self.UserModel = get_user_model()
-
-    def authenticate(self,request, **kwargs):          
-        
-        print("authenticate")
+    def authenticate(self,request, **kwargs):
         self.request = request
         if not self.request:
-            print("1")
             return None
 
 
         state = self.request.GET.get("state")
         code = self.request.GET.get("code")
         nonce = kwargs.pop("nonce", None)
         code_verifier = kwargs.pop("code_verifier", None)
         
-
-        print("nonce")
-        print(nonce)
-        print("code_verifier")
-        print(code_verifier)
-
         if not code or not state:
-            print("2")
             return None
 
-        redirect_uri = import_from_settings(
-            "OIDC_AUTHENTICATION_SSO_CALLBACK_URL", "http://localhost:3000/callback"
-        )
-
-
-
         token_payload = {
             "client_id": self.OIDC_RP_CLIENT_ID,
             "client_secret": self.OIDC_RP_CLIENT_SECRET,
             "grant_type": "authorization_code",
             "code": code,
-            "redirect_uri":redirect_uri,
+            "redirect_uri":self.OIDC_AUTHENTICATION_SSO_CALLBACK_URL,
         }
 
 
         # Send code_verifier with token request if using PKCE
         if code_verifier is not None:
             token_payload.update({"code_verifier": code_verifier})
 
@@ -112,73 +93,108 @@
         access_token = token_info.get("access_token")
         
         
         # Validate the token
         payload = self.verify_token(id_token, nonce=nonce)
                 
         if payload:
-            self.store_tokens(access_token, id_token, refresh_token)
+            self.store_tokens(access_token, refresh_token)
             try:
                 return self.get_or_create_user(access_token, id_token, payload)
             except SuspiciousOperation as exc:
                 LOGGER.warning("failed to get or create user: %s", exc)
-                print("3")
                 return None
-        print("4")
-        return None
-        
+        return None       
+     
+    def get_or_create_user(self, access_token, id_token, payload):
+        """Returns a User instance if 1 user is found. Creates a user if not found
+        and configured to do so. Returns nothing if multiple users are matched."""
+
+        user_info = self.get_userinfo(access_token, id_token, payload)
         
+        if not self.OIDC_CHECK_USER_MODEL:
+            return self.get_user_obj(user_info)
+            
+        # username based filtering
+        users = self.filter_users_by_claims(user_info)
+
+        if len(users) == 1:
+            user = self.update_user(users[0], user_info)
+            
+            if user_info and access_token and id_token:
+                user_json = self.create_user_json(user_info, access_token, id_token)
+                self.save_user_data(user, user_json)
+            return user
+
+        elif len(users) > 1:
+            # In the rare case that two user accounts have the same email address,
+            # bail. Randomly selecting one seems really wrong.
+            msg = "Multiple users returned"
+            raise SuspiciousOperation(msg)
+        elif self.OIDC_CREATE_USER:
+            user = self.create_user(user_info)
+            if user_info and access_token and id_token:
+                user_json = self.create_user_json(user_info, access_token, id_token)
+                self.save_user_data(user, user_json)
+            return user
+        else:
+            LOGGER.debug(
+                "Login failed: No user with %s found, and " "OIDC_CREATE_USER is False",
+                self.describe_user_by_claims(user_info),
+            )
+            
+            return None
+           
     def get_userinfo(self, access_token, id_token, payload):
         """Return user details dictionary. The id_token and payload are not used in
         the default implementation, but may be used when overriding this method"""
 
         user_response = requests.get(
             self.OIDC_OP_USER_ENDPOINT,
             headers={"Authorization": "Bearer {0}".format(access_token)},
-            verify=import_from_settings("OIDC_VERIFY_SSL", True),
-            timeout=import_from_settings("OIDC_TIMEOUT", None),
-            proxies=import_from_settings("OIDC_PROXY", None),
+            verify=self.OIDC_VERIFY_SSL,
+            timeout=self.OIDC_TIMEOUT,
+            proxies=self.OIDC_PROXY,
         )
         
   
         user_response.raise_for_status()
         return user_response.json()
     
     def verify_claims(self, claims):
         """Verify the provided claims to decide if authentication should be allowed."""
 
         # Verify claims required by default configuration
-        scopes = import_from_settings("OIDC_RP_SCOPES", "openid email")
+        scopes = self.OIDC_RP_SCOPES
         if "email" in scopes.split():
             return "email" in claims
 
         LOGGER.warning(
             "Custom OIDC_RP_SCOPES defined. "
             "You need to override `verify_claims` for custom claims verification."
         )
 
         return True
 
     def describe_user_by_claims(self, claims):
-        username_claim = import_from_settings("OIDC_USERNAME_CLAIM", "preferred_username")
-        username = claims.get(str(username_claim))
+        username = claims.get(self.OIDC_USERNAME_CLAIM)
         return "username {}".format(username)
     
     def filter_users_by_claims(self, claims):
         """Return all users matching the specified username."""
 
         username = self.get_username(claims)
         
         if not username:
             return self.UserModel.objects.none()
         return self.UserModel.objects.filter(username__iexact=username)
     
     def mapper(self,claims):
         user_fields = {}
-        field_mapping = import_from_settings("OIDC_FIELD_MAPPING",{} )
+        field_mapping = self.OIDC_FIELD_MAPPING
         for field_name, claim_key in field_mapping.items():
             value = claims.get(claim_key)
             if field_name == "username":
                 continue
             if value is not None:
                 user_fields[field_name] = value
         return user_fields
@@ -193,38 +209,41 @@
         user.save()
 
         """Update existing user with new claims, if necessary save, and return user"""
         return user
 
     def get_username(self, claims):
         """Generate username based on claims."""
-        username_algo = import_from_settings("OIDC_USERNAME_ALGO", None)
-        username_claim = import_from_settings("OIDC_USERNAME_CLAIM", "preferred_username")
-        use_encoded_username = import_from_settings("OIDC_USE_ENCODED_USERNAME", None)
+        username_algo = self.OIDC_USERNAME_ALGO
 
-        if use_encoded_username:
+        if self.OIDC_USE_ENCODED_USERNAME:
             if username_algo:
                 if isinstance(username_algo, str):
                     username_algo = import_string(username_algo)
-                return username_algo(claims.get(str(username_claim)))
+                return username_algo(claims.get(self.OIDC_USERNAME_CLAIM))
+            return  default_username_algo(claims.get(self.OIDC_USERNAME_CLAIM))
+        return str(claims.get(self.OIDC_USERNAME_CLAIM))
+
+    def get_user_obj(self, claims):
 
-            default_username_algo =  default_username_algo(claims.get(str(username_claim)))
+        """Return object for a newly created user account."""
+        username = self.get_username(claims)        
+        user_fields = self.mapper(claims)
+        user = self.UserModel(username, **user_fields)
+        return user
     
-        return str(claims.get(str(username_claim)))
-        
     def create_user(self, claims):
 
         """Return object for a newly created user account."""
         username = self.get_username(claims)        
         user_fields = self.mapper(claims)
-        user = get_user_model().objects.create_user(username, **user_fields)
+        user = self.UserModel.objects.create_user(username, **user_fields)
 
         return user
     
-    
     def create_user_json(self,user_info_json, access_token, id_token):
         excluded_fields = [
             "exp", "iat", "auth_time", "jti", "iss", "aud", "sub", "typ",
             "azp", "nonce", "session_state", "at_hash", "acr","allowed-origins","realm_access","resource_access","scope","sid"
         ]
 
         decoded_access_token = jwt.decode(access_token, algorithms=[self.OIDC_RP_SIGN_ALGO], verify=False, options={"verify_signature": False})
@@ -248,76 +267,34 @@
         try:
             oidc_extra_data = user.oidcextradata
             oidc_extra_data.data = user_data
             oidc_extra_data.save()
         except OIDCExtraData.DoesNotExist:
             # Create a new OIDCExtraData object for the user
             oidc_extra_data = OIDCExtraData.objects.create(user=user, data=user_data)
-
-
     
-    def get_or_create_user(self, access_token, id_token, payload):
-        """Returns a User instance if 1 user is found. Creates a user if not found
-        and configured to do so. Returns nothing if multiple users are matched."""
-
-        user_info = self.get_userinfo(access_token, id_token, payload)
-        
-
-
-
-        # email based filtering
-        users = self.filter_users_by_claims(user_info)
-
-        if len(users) == 1:
-            user = self.update_user(users[0], user_info)
-            
-            if user_info and access_token and id_token:
-                user_json = self.create_user_json(user_info, access_token, id_token)
-                self.save_user_data(user, user_json)
-            return user
-
-        elif len(users) > 1:
-            # In the rare case that two user accounts have the same email address,
-            # bail. Randomly selecting one seems really wrong.
-            msg = "Multiple users returned"
-            raise SuspiciousOperation(msg)
-        elif import_from_settings("OIDC_CREATE_USER", True):
-            user = self.create_user(user_info)
-            if user_info and access_token and id_token:
-                user_json = self.create_user_json(user_info, access_token, id_token)
-                self.save_user_data(user, user_json)
-            return user
-        else:
-            LOGGER.debug(
-                "Login failed: No user with %s found, and " "OIDC_CREATE_USER is False",
-                self.describe_user_by_claims(user_info),
-            )
-            
-            print("5")
-            return None
-
     def retrieve_matching_jwk(self, token):
         """Get the signing key by exploring the JWKS endpoint of the OP."""
         response_jwks = requests.get(
             self.OIDC_OP_JWKS_ENDPOINT,
-            verify=import_from_settings("OIDC_VERIFY_SSL", True),
-            timeout=import_from_settings("OIDC_TIMEOUT", None),
-            proxies=import_from_settings("OIDC_PROXY", None),
+            verify=self.OIDC_VERIFY_SSL,
+            timeout=self.OIDC_TIMEOUT,
+            proxies=self.OIDC_PROXY,
         )
         response_jwks.raise_for_status()
         jwks = response_jwks.json()
 
         # Compute the current header from the given token to find a match
         jws = JWS.from_compact(token)
         json_header = jws.signature.protected
         header = Header.json_loads(json_header)
 
         key = None
         for jwk in jwks["keys"]:
-            if import_from_settings("OIDC_VERIFY_KID", True) and jwk[
+            if self.OIDC_VERIFY_KID and jwk[
                 "kid"
             ] != smart_str(header.kid):
                 continue
             if "alg" in jwk and jwk["alg"] != smart_str(header.alg):
                 continue
             key = jwk
         if key is None:
@@ -352,15 +329,15 @@
             msg = "JWS token verification failed."
             raise SuspiciousOperation(msg)
 
         return jws.payload
     
     def get_payload_data(self, token, key):
         """Helper method to get the payload of the JWT token."""
-        if import_from_settings("OIDC_ALLOW_UNSECURED_JWT", False):
+        if self.OIDC_ALLOW_UNSECURED_JWT:
             header, payload_data, signature = token.split(b".")
             header = json.loads(smart_str(b64decode(header)))
 
             # If config allows unsecured JWTs check the header and return the decoded payload
             if "alg" in header and header["alg"] == "none":
                 return b64decode(payload_data)
 
@@ -388,41 +365,42 @@
         # In Python 3 and 2, that's always a byte string.
         # In Python3.6, the json.loads() function can accept a byte string
         # as it will automagically decode it to a unicode string before
         # deserializing https://bugs.python.org/issue17909
         payload = json.loads(payload_data.decode("utf-8"))
         token_nonce = payload.get("nonce")
 
-        if import_from_settings("OIDC_USE_NONCE", True) and nonce != token_nonce:
+        if self.OIDC_USE_NONCE and nonce != token_nonce:
             msg = "JWT Nonce verification failed."
             raise SuspiciousOperation(msg)
         return payload
     
     def get_token(self, payload):
         """Return token object as a dictionary."""
 
         auth = None
-        if import_from_settings("OIDC_TOKEN_USE_BASIC_AUTH", False):
+        if self.OIDC_TOKEN_USE_BASIC_AUTH:
             # When Basic auth is defined, create the Auth Header and remove secret from payload.
             user = payload.get("client_id")
             pw = payload.get("client_secret")
 
             auth = HTTPBasicAuth(user, pw)
             del payload["client_secret"]
 
         response = requests.post(self.OIDC_OP_TOKEN_ENDPOINT,
             data=payload,
             auth=auth,
-            verify=import_from_settings("OIDC_VERIFY_SSL", True),
-            timeout=import_from_settings("OIDC_TIMEOUT", None),
-            proxies=import_from_settings("OIDC_PROXY", None),
+            verify=self.OIDC_VERIFY_SSL,
+            timeout=self.OIDC_TIMEOUT,
+            proxies=self.OIDC_PROXY,
         )
+
         response.raise_for_status()
+        
         return response.json()
     
-    def store_tokens(self, access_token, id_token, refresh_token):
-        """Store OIDC tokens."""
+    def store_tokens(self, access_token, refresh_token):
+        """Store access_token and refresh_token temperory."""
         session = self.request.session
         session["oidc_access_token"] = access_token
-        session["oidc_id_token"] = id_token
         session["oidc_refresh_token"] = refresh_token
```

### Comparing `oidc_drf-1.2.9/oidc_drf/drf.py` & `oidc_drf-1.3.0/oidc_drf/drf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
+from requests.exceptions import HTTPError
 from rest_framework import exceptions
+from rest_framework import authentication, exceptions
 from django.core.exceptions import  SuspiciousOperation
 from django.utils.module_loading import import_string
-from requests.exceptions import HTTPError
 from django.conf import settings
-from rest_framework import authentication, exceptions
 from django.core.exceptions import ImproperlyConfigured, SuspiciousOperation
+from django.contrib.auth import get_backends
 from oidc_drf.utils import import_from_settings,parse_www_authenticate_header
 from oidc_drf.backends import OIDCAuthenticationBackend
-from django.contrib.auth import get_backends
 
 LOGGER = logging.getLogger(__name__)
 
 def get_oidc_backend():
     """
     Get the Django auth backend that uses OIDC.
     """
@@ -52,23 +52,24 @@
         
 
     def authenticate(self, request):
         access_token = self.get_access_token(request)
         if not access_token:
             return None
         try:
+            """ try other DEFAULT_AUTHENTICATION_CLASSES first """
             for auth_class in settings.REST_FRAMEWORK['DEFAULT_AUTHENTICATION_CLASSES']:
                 auth_class_name = auth_class.split('.')[-1]
                 if auth_class_name != self.__class__.__name__:
                     auth = import_string(auth_class)()
                     user = auth.authenticate(request)
                     if user is not None:
                         return user
         except:
-
+            """ if did not authenticate try this (oidc_drf.drf.OIDCAuthentication) DEFAULT_AUTHENTICATION_CLASSES """
             try:
                 user = self.backend.get_or_create_user(access_token, None, None)
             except HTTPError as exc:
                 resp = exc.response
                 if resp.status_code == 401 and "www-authenticate" in resp.headers:
                     data = parse_www_authenticate_header(resp.headers["www-authenticate"])
                     raise exceptions.AuthenticationFailed(
```

### Comparing `oidc_drf-1.2.9/oidc_drf/utils.py` & `oidc_drf-1.3.0/oidc_drf/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from hashlib import sha256
 import josepy.b64
 from django.core.exceptions import ImproperlyConfigured
 from django.conf import settings
 from urllib.request import parse_http_list, parse_keqv_list
-
+import base64
+import hashlib
+from django.utils.encoding import force_bytes, smart_str
 
 def absolutify(request, path):
     """Return the absolute URL of a path."""
     return request.build_absolute_uri(path)
 
 def parse_www_authenticate_header(header):
     """
@@ -61,7 +63,25 @@
         return code_verifier
 
     elif method == "S256":
         return base64_url_encode(sha256(code_verifier.encode("ascii")).digest())
 
     else:
         raise ValueError("code challenge method must be 'plain' or 'S256'.")
+
+def default_username_algo(email):
+    """Generate username for the Django user.
+
+    :arg str/unicode email: the email address to use to generate a username
+
+    :returns: str/unicode
+
+    """
+    # bluntly stolen from django-browserid
+    # store the username as a base64 encoded sha224 of the email address
+    # this protects against data leakage because usernames are often
+    # treated as public identifiers (so we can't use the email address).
+    username = base64.urlsafe_b64encode(
+        hashlib.sha1(force_bytes(email)).digest()
+    ).rstrip(b"=")
+
+    return smart_str(username)
```

### Comparing `oidc_drf-1.2.9/oidc_drf/views.py` & `oidc_drf-1.3.0/oidc_drf/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,232 +1,202 @@
 from django.http import JsonResponse
 from django.contrib import auth
-from rest_framework.permissions import AllowAny,IsAuthenticated
+from rest_framework.permissions import AllowAny
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from rest_framework import status
 from urllib.parse import urlencode
 from django.utils.crypto import get_random_string
 from oidc_drf.utils import import_from_settings
 import requests
-LOGGER = logging.getLogger(__name__)
 
 
-from  oidc_drf.utils import generate_code_challenge
-
 class OIDCGenerateAuthenticationUrlView(APIView):
     permission_classes = [AllowAny]    
+    def login_failure(self,error_message,status):
+        return Response({"detail":error_message}, status=status)
+    
     def get(self, request):
-
         state = get_random_string(import_from_settings("OIDC_STATE_SIZE", 32))
         auth_url = import_from_settings("OIDC_OP_AUTHORIZATION_ENDPOINT")
-        # oidc_states = {}
 
         params ={
             "response_type":  'code',
             "client_id":  import_from_settings("OIDC_RP_CLIENT_ID"),
             "redirect_uri":  import_from_settings("OIDC_AUTHENTICATION_SSO_CALLBACK_URL"),
             "scope":  import_from_settings("OIDC_RP_SCOPES"),
             "state":  state,
         }
         
-
-        
         if import_from_settings("OIDC_USE_NONCE", True):
-            # nonce = get_random_string(import_from_settings("OIDC_NONCE_SIZE", 32))
             nonce = request.GET.get('nonce',None)
+            if nonce == None:
+                return self.login_failure("missing nonce",status.HTTP_400_BAD_REQUEST)
             params.update({"nonce": nonce})
-            # oidc_states.update({"nonce":nonce})
 
-
-
-        if import_from_settings("OIDC_USE_PKCE", True):
-            # code_verifier_length = import_from_settings("OIDC_PKCE_CODE_VERIFIER_SIZE", 64)
-            # Check that code_verifier_length is between the min and max length
-            # defined in https://datatracker.ietf.org/doc/html/rfc7636#section-4.1
-            # if not (43 <= code_verifier_length <= 128):
-            #     raise ValueError("code_verifier_length must be between 43 and 128")
-
-            # Generate code_verifier and code_challenge pair
-            # code_verifier = get_random_string(code_verifier_length)
-
-
-            # oidc_states.update({"code_verifier":code_verifier})
-            # code_challenge_method = import_from_settings(
-            #     "OIDC_PKCE_CODE_CHALLENGE_METHOD", "S256"
-            # )
-            # code_challenge = generate_code_challenge(
-            #     code_verifier, code_challenge_method
-            # )
-
-            # Append code_challenge to authentication request parameters
-            
+        if import_from_settings("OIDC_USE_PKCE", True):            
             code_challenge = request.GET.get('code_challenge',None)
             code_challenge_method = request.GET.get('code_challenge_method',None)
+            if code_challenge == None:
+                return self.login_failure("missing code_challenge",status.HTTP_400_BAD_REQUEST)
+            if code_challenge_method == None:
+                return self.login_failure("missing code_challenge_method",status.HTTP_400_BAD_REQUEST)
             params.update(
                 {
                     "code_challenge": code_challenge,
                     "code_challenge_method": code_challenge_method,
                 })
             
-
-
         query = urlencode(params)
         redirect_url = "{url}?{query}".format(url=auth_url, query=query)
 
-
         return Response({
             "redirect_url":redirect_url
             } )
 
 class OIDCAuthenticationCallbackView(APIView):
     """OIDC client authentication callback HTTP endpoint"""
     permission_classes = [AllowAny]    
 
-    def login_failure(self,error_message):
-        return Response({"detail":error_message}, status=status.HTTP_401_UNAUTHORIZED)
+    def login_failure(self,error_message,status):
+        return Response({"detail":error_message}, status=status)
 
     def login_success(self):   
-        print("login_success")
         try:     
             oidc_access_token = self.request.session["oidc_access_token"]
-            oidc_id_token = self.request.session["oidc_id_token"]
             oidc_refresh_token = self.request.session["oidc_refresh_token"]
             
             data = {
                 'access': str(oidc_access_token),
                 'refresh': str(oidc_refresh_token),
-                'oidc_id_token': str(oidc_id_token),
             } 
             
             del self.request.session["oidc_access_token"]
-            del self.request.session["oidc_id_token"]
             del self.request.session["oidc_refresh_token"]
             self.request.session.save()
 
             
             return JsonResponse(data)
     
         except:
-            return self.login_failure("Login failed")
-
+            return self.login_failure("Login failed",status.HTTP_401_UNAUTHORIZED)
 
     def post(self, request):
-        LOGGER.debug("=================== LOGGER.debug===================")
-        print("=======================================")
-        print("=======================================")
-        print("in post request")
         """Callback handler for OIDC authorization code flow"""
         data = request.data
         
-        if "error" in request.GET:
-            return self.login_failure(request.GET.get("error_description"))
-        
-        elif import_from_settings("OIDC_USE_PKCE", True):
+        if import_from_settings("OIDC_USE_PKCE", True):
             code_verifier = data.get("code_verifier",None)
             if code_verifier == None:
-                return self.login_failure("missing code_verifier")
+                return self.login_failure("missing code_verifier",status.HTTP_400_BAD_REQUEST)
             
-        elif import_from_settings("OIDC_USE_NONCE", True):
+        if import_from_settings("OIDC_USE_NONCE", True):
             nonce = data.get("nonce",None)
             if nonce == None:
-                return self.login_failure("missing nonce")
-            
-
-        elif "code" in request.GET and "state" in request.GET:
-
+                return self.login_failure("missing nonce",status.HTTP_400_BAD_REQUEST)
             
+        if "error" in request.GET:
+            return self.login_failure(request.GET.get("error_description"),status.HTTP_400_BAD_REQUEST)
+        
+        elif "code" in request.GET and "state" in request.GET:            
             kwargs = {
                 "request": request,
                 "nonce": data.get("nonce",None),
                 "code_verifier": data.get("code_verifier",None),
             }
-
             self.user = auth.authenticate(**kwargs)
-            print(self.user)
+                        
             if self.user and self.user.is_active:
                 return self.login_success()
         
-        return self.login_failure("Login failed")
+        return self.login_failure("Login failed",status.HTTP_401_UNAUTHORIZED)
 
 class OIDCLogoutView(APIView):
     permission_classes = [AllowAny]    
-
+    def login_failure(self,error_message,status):
+        return Response({"detail":error_message}, status=status)
+    
     def post(self, request):     
-        oidc_id_token = request.data.get('oidc_id_token', '')
-        if oidc_id_token:
+        client_id = import_from_settings("OIDC_RP_CLIENT_ID", "")
+        client_secret = import_from_settings("OIDC_RP_CLIENT_SECRET", "")
+        refresh = request.data.get('refresh', None)
+        
+        if refresh == None:
+            return self.login_failure("missing refresh field",status.HTTP_400_BAD_REQUEST)
+        else:
 
-            logout_endpoint = import_from_settings("OIDC_OP_LOGOUT_ENDPOINT", "")
-            post_logout_redirect_uri = import_from_settings("OIDC_LOGOUT_REDIRECT_URL", "http://localhost:3000")
-            
+            logout_endpoint = import_from_settings("OIDC_OP_LOGOUT_ENDPOINT", "")            
             headers = {
                 'Content-Type': 'application/x-www-form-urlencoded',
             }
 
             data = {
-                'post_logout_redirect_uri': post_logout_redirect_uri,
-                'id_token_hint': oidc_id_token,
+                'client_id': client_id,
+                'client_secret': client_secret,
+                'refresh_token': refresh,
             }
+            
             response = requests.post(logout_endpoint, data=data, headers=headers)
             
-            if response.status_code != 200:
+            if response.status_code == 204:
+                return JsonResponse({'message': 'Logout OIDC Successful'}, status=status.HTTP_200_OK)
+            else:
                 error_message = response.json().get('error', 'Logout Request failed with status code: {}'.format(response.status_code))
                 error_data = {
                     'error': error_message
                 }
                 return JsonResponse(error_data, status=response.status_code)
 
-        
-            if response.status_code == 204 or response.status_code == 200:
-                return JsonResponse({'message': 'Logout OIDC successful'}, status=response.status_code)
-            
-        return Response({"error":"user has not id token !!"}, status=status.HTTP_400_BAD_REQUEST)    
-
 class OIDCRefreshTokenView(APIView):
     permission_classes = [AllowAny]    
-
+    def login_failure(self,error_message,status):
+        return Response({"detail":error_message}, status=status)
+    
     def post(self, request):     
         url = import_from_settings("OIDC_OP_TOKEN_ENDPOINT", "")
-        refresh_token = request.data.get("refresh",'')
-        code_verifier = request.data.get("code_verifier",'')
+        refresh_token = request.data.get("refresh",None)
+        code_verifier = request.data.get("code_verifier",None)
         client_secret = import_from_settings("OIDC_RP_CLIENT_SECRET", "")
         client_id = import_from_settings("OIDC_RP_CLIENT_ID", "")
 
+        if import_from_settings("OIDC_USE_PKCE", True) and code_verifier == None:
+            return self.login_failure("missing code_verifier",status.HTTP_400_BAD_REQUEST)
+            
+        if refresh_token == None:
+            return self.login_failure("missing code_verifier",status.HTTP_400_BAD_REQUEST)
+
         data = {
             "grant_type": "refresh_token",
             "refresh_token": refresh_token,
             "client_id": client_id,
             "code_verifier": code_verifier,
             "client_secret": client_secret
         }
         
         headers = {
             "Content-Type": "application/x-www-form-urlencoded"
         }
         
         try:
-
             response = requests.post(url, data=urlencode(data), headers=headers)
             json_data = response.json()
             
             if response.status_code != 200:
                 error_message = json_data.get('error', 'Request failed with status code: {}'.format(response.status_code))
                 error_data = {
                     'error': error_message
                 }
                 return JsonResponse(error_data, status=response.status_code)
             
             oidc_access_token = json_data.get("access_token")
-            oidc_id_token = json_data.get("id_token")
             oidc_refresh_token = json_data.get("refresh_token")
             
             data = {
                 'access': str(oidc_access_token),
                 'refresh': str(oidc_refresh_token),
-                'oidc_id_token': str(oidc_id_token),
             }       
     
             return JsonResponse(data)
         except requests.exceptions.RequestException as e:
             # Handle any request exceptions here
             error_message = str(e)
             error_data = {
```

### Comparing `oidc_drf-1.2.9/setup.py` & `oidc_drf-1.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.2.9',
+    version='1.3.0',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Software Development :: Libraries :: Application Frameworks',
+        'Topic :: Internet :: WWW/HTTP',
+        'Topic :: Security',
+
     ],
     install_requires=[
         "Django >= 3.2",
         "josepy",
         "requests",
         "cryptography",
         'djangorestframework',
```

