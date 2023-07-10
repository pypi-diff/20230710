# Comparing `tmp/starlette_securecookies-1.1.0.tar.gz` & `tmp/starlette_securecookies-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_securecookies-1.1.0.tar", last modified: Tue Apr 25 21:24:36 2023, max compression
+gzip compressed data, was "starlette_securecookies-1.1.1.tar", last modified: Mon Jul 10 05:10:56 2023, max compression
```

## Comparing `starlette_securecookies-1.1.0.tar` & `starlette_securecookies-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      673 2022-05-19 02:58:14.878342 starlette_securecookies-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1521 2022-05-19 02:25:27.525844 starlette_securecookies-1.1.0/LICENSE
--rw-r--r--   0        0        0     4494 2023-04-25 21:21:43.979609 starlette_securecookies-1.1.0/README.md
--rw-r--r--   0        0        0     1360 2023-04-25 21:24:36.033554 starlette_securecookies-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      202 2023-04-25 21:21:43.984607 starlette_securecookies-1.1.0/securecookies/__init__.py
--rw-r--r--   0        0        0      551 2023-04-25 21:21:43.985607 starlette_securecookies-1.1.0/securecookies/extras/__init__.py
--rw-r--r--   0        0        0     1611 2023-04-25 21:21:43.985607 starlette_securecookies-1.1.0/securecookies/extras/csrf.py
--rw-r--r--   0        0        0     6991 2023-04-25 21:21:43.986607 starlette_securecookies-1.1.0/securecookies/middleware.py
--rw-r--r--   0        0        0        0 2022-05-19 02:25:27.533836 starlette_securecookies-1.1.0/securecookies/py.typed
--rw-r--r--   0        0        0     3146 2023-04-25 21:21:43.987607 starlette_securecookies-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1078 2023-04-25 21:21:43.988607 starlette_securecookies-1.1.0/tests/extras/test_csrf.py
--rw-r--r--   0        0        0      943 2023-04-25 21:21:43.988607 starlette_securecookies-1.1.0/tests/test_other-party.py
--rw-r--r--   0        0        0     3900 2023-04-24 01:08:05.010116 starlette_securecookies-1.1.0/tests/test_securecookies.py
--rw-r--r--   0        0        0     7120 1970-01-01 00:00:00.000000 starlette_securecookies-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1467 2023-07-10 04:57:59.123550 starlette_securecookies-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1521 2022-05-19 02:25:27.525844 starlette_securecookies-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4551 2023-07-10 05:01:56.901248 starlette_securecookies-1.1.1/README.md
+-rw-r--r--   0        0        0     1360 2023-07-10 05:10:56.870910 starlette_securecookies-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-25 21:21:43.984607 starlette_securecookies-1.1.1/securecookies/__init__.py
+-rw-r--r--   0        0        0      551 2023-04-25 21:21:43.985607 starlette_securecookies-1.1.1/securecookies/extras/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-25 21:21:43.985607 starlette_securecookies-1.1.1/securecookies/extras/csrf.py
+-rw-r--r--   0        0        0     7680 2023-07-10 04:44:22.604492 starlette_securecookies-1.1.1/securecookies/middleware.py
+-rw-r--r--   0        0        0        0 2022-05-19 02:25:27.533836 starlette_securecookies-1.1.1/securecookies/py.typed
+-rw-r--r--   0        0        0     3146 2023-04-25 21:21:43.987607 starlette_securecookies-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1078 2023-04-25 21:21:43.988607 starlette_securecookies-1.1.1/tests/extras/test_csrf.py
+-rw-r--r--   0        0        0      943 2023-04-25 21:21:43.988607 starlette_securecookies-1.1.1/tests/test_other-party.py
+-rw-r--r--   0        0        0     4242 2023-07-10 04:44:22.605485 starlette_securecookies-1.1.1/tests/test_securecookies.py
+-rw-r--r--   0        0        0     7177 1970-01-01 00:00:00.000000 starlette_securecookies-1.1.1/PKG-INFO
```

### Comparing `starlette_securecookies-1.1.0/LICENSE` & `starlette_securecookies-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_securecookies-1.1.0/README.md` & `starlette_securecookies-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 
 Tested support on Python 3.7, 3.8, 3.9, and 3.10, 3.11 on macOS, Windows, and Linux.
 
 ## How it works?
 
 ```mermaid
 sequenceDiagram
-    Browser->>+Middleware: Encrypted 'Cookie' header
+    Browser->>+Middleware: Encrypted 'Cookie' headers
     Middleware->>+Application: Decrypted cookies
     Application->>-Middleware: Plaintext cookies
-    Middleware->>-Browser: Encrypted 'Set-Cookie' header
+    Middleware->>-Browser: Encrypted 'Set-Cookie' headers
     Note over Application: *The Application may be your service<br />or any additional middleware.
 ```
 
 For any incoming cookies:
 
 1. Requests sent from the client's browser to your application are intercepted by `SecureCookiesMiddleware`.
-2. All `Cookie` headers are parsed and filter. Only cookies in the `included_cookies` and `excluded_cookies` parameters are parsed. All cookies are included by default.
-3. The cookies are decrypted. If cookie cannot be decrypted, or is otherwise invalid, it is discarded by default (`discard_invalid=True`).
+2. All `Cookie` headers are filtered and parsed. Only cookies in the `included_cookies` and `excluded_cookies` parameters are parsed. All cookies are included by default.
+3. The cookies are decrypted. If a cookie cannot be decrypted, or is otherwise invalid, it is discarded by default (`discard_invalid=True`).
 4. Any included and valid encrypted cookies in the ASGI request scope are replaced by the decrypted ones.
 5. The request scope is passed to any future middleware, and eventually your application. Cookies can be read normally anywhere downstream.
 
 For any outgoing cookies:
 
-7. Your application sets cookies with `response.set_cookie` as usual.
+7. Your application sets cookies with `response.set_cookie`, or by any other means of creating `Set-Cookie` headers.
 8. Other middleware run and add additional cookies, like [SessionMiddleware](https://www.starlette.io/middleware/#sessionmiddleware).
 9. All responses returned by your application are intercepted by `SecureCookiesMiddleware`.
-10. Cookies in the `included_cookies` and `excluded_cookies` parameters are re-encrypted, and their attributes (like `"SameSite"` and `"HttpOnly"`) are overridden by the parameters set in `SecureCookiesMiddleware` if set.
+10. Cookies in the `included_cookies` and not in the `excluded_cookies` parameters are re-encrypted, and their attributes (like `"SameSite"` and `"HttpOnly"`) are overridden by any parameters set in `SecureCookiesMiddleware`.
 11. The cookies in the response are replaced by the re-encrypted cookies, and the response is eventually propagated to the client's browser.
 
 ## Installation
 
 ```sh
 $ pdm add starlette-securecookies
 # or
```

### Comparing `starlette_securecookies-1.1.0/pyproject.toml` & `starlette_securecookies-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "starlette-securecookies"
-version = "1.1.0"
+version = "1.1.1"
 description = "Secure cookie middleware for Starlette applications."
 authors = [
     { name = "Elias Gabriel", email = "me@eliasfgabriel.com" },
 ]
 keywords = [
     "starlette",
     "fastapi",
```

### Comparing `starlette_securecookies-1.1.0/securecookies/extras/__init__.py` & `starlette_securecookies-1.1.1/securecookies/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_securecookies-1.1.0/securecookies/extras/csrf.py` & `starlette_securecookies-1.1.1/securecookies/extras/csrf.py`

 * *Files identical despite different names*

### Comparing `starlette_securecookies-1.1.0/securecookies/middleware.py` & `starlette_securecookies-1.1.1/securecookies/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
+import warnings
 from http.cookies import SimpleCookie
-from typing import Any, List, Optional
+from typing import List, Optional
 
 from cryptography.fernet import Fernet, InvalidToken, MultiFernet
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response
 from starlette.types import ASGIApp
 
@@ -80,18 +81,27 @@
         if excluded_cookies and included_cookies:
             raise BadArgumentError(
                 "It doesn't make sense to specify both excluded and included cookies."
                 " Supply either `excluded_cookies` or `included_cookies` to restrict"
                 " which cookies should be secure."
             )
 
-        if cookie_samesite and cookie_samesite.lower() not in ["strict", "lax", "none"]:
-            raise BadArgumentError(
-                "SameSite attribute must be either 'strict', 'lax' or 'none'"
-            )
+        if cookie_samesite:
+            samesite = cookie_samesite.lower()
+
+            if samesite not in ["strict", "lax", "none"]:
+                raise BadArgumentError(
+                    "SameSite attribute must be either 'strict', 'lax' or 'none'"
+                )
+            elif samesite == "none" and not self.cookie_secure:
+                warnings.warn(
+                    "Insecure cookies with a SameSite='None' attribute may be rejected"
+                    " on newer browser versions (draft-ietf-httpbis-rfc6265bis). See"
+                    " https://caniuse.com/same-site-cookie-attribute for compat notes."
+                )
 
     def set_header(self, request: Request, header: str, value: str) -> None:
         """
         Adds the given Header to the available Request headers. If the Header already
         exists, its value is overwritten.
         """
         hkey = header.encode("latin-1")
@@ -104,26 +114,32 @@
         """Decrypt the given value using any of the configured secrets."""
         return self.mfernet.decrypt(value.encode()).decode()
 
     def encrypt(self, value: str) -> str:
         """Encrypt the given value using the first configured secret."""
         return self.mfernet.encrypt(value.encode()).decode()
 
+    def should_process_cookie(self, cookie: str) -> bool:
+        """Determines if the cookie should be included for processing."""
+        return (
+            (not self.included_cookies and not self.excluded_cookies)
+            or (self.included_cookies is not None and cookie in self.included_cookies)
+            or (
+                self.excluded_cookies is not None
+                and cookie not in self.excluded_cookies
+            )
+        )
+
     async def dispatch(
         self, request: Request, call_next: RequestResponseEndpoint
     ) -> Response:
         if len(request.cookies):
-            cookies: SimpleCookie[Any] = SimpleCookie()
+            cookies: SimpleCookie[str] = SimpleCookie()
             for cookie, value in request.cookies.items():
-                # if the cookie is included or not excluded
-                if (
-                    (not self.included_cookies and not self.excluded_cookies)
-                    or (self.included_cookies and cookie in self.included_cookies)
-                    or (self.excluded_cookies and cookie not in self.excluded_cookies)
-                ):
+                if self.should_process_cookie(cookie):
                     try:
                         # try to decrypt the cookie and pass it along
                         cookies[cookie] = self.decrypt(value)
                     except InvalidToken:
                         # delete invalid or unencrypted cookies unless disabled
                         if not self.discard_invalid:
                             cookies[cookie] = value
@@ -134,31 +150,39 @@
             self.set_header(
                 request, "cookie", cookies.output(header="", sep=";").strip()
             )
 
         # propagate the modified request
         response: Response = await call_next(request)
 
-        # for every cookie in the response
-        for cookie in response.headers.getlist("set-cookie"):
-            # decode it
-            ncookie: SimpleCookie[Any] = SimpleCookie(cookie)
-            key = [*ncookie.keys()][0]
-
-            # if the cookie is included or not excluded
-            if (
-                (not self.included_cookies and not self.excluded_cookies)
-                or (self.included_cookies and key in self.included_cookies)
-                or (self.excluded_cookies and key not in self.excluded_cookies)
-            ):
-                # create a new encrypted cookie with the desired attributes
-                response.set_cookie(
-                    key,
-                    value=self.encrypt(ncookie[key].value),
-                    path=self.cookie_path or ncookie[key]["path"],
-                    domain=self.cookie_domain or ncookie[key]["domain"],
-                    secure=self.cookie_secure or ncookie[key]["secure"],
-                    httponly=self.cookie_httponly or ncookie[key]["httponly"],
-                    samesite=self.cookie_samesite or ncookie[key]["samesite"],
-                )
+        # Extract the cookie headers to be mutated
+        cookie_headers = response.headers.getlist("set-cookie")
+        del response.headers["set-cookie"]
+
+        for cookie_header in cookie_headers:
+            ncookie: SimpleCookie[str] = SimpleCookie(cookie_header)
+            key = next(iter(ncookie.keys()))
+
+            if self.should_process_cookie(key):
+                ncookie[key] = self.encrypt(ncookie[key].value)
+
+                # Mutate the cookie based on middleware defaults (if provided)
+                if self.cookie_path is not None:
+                    ncookie[key]["path"] = self.cookie_path
+
+                if self.cookie_domain is not None:
+                    ncookie[key]["domain"] = self.cookie_domain
+
+                if self.cookie_secure is not None:
+                    ncookie[key]["secure"] = self.cookie_secure
+
+                if self.cookie_httponly is not None:
+                    ncookie[key]["httponly"] = self.cookie_httponly
+
+                if self.cookie_samesite is not None:
+                    ncookie[key]["samesite"] = self.cookie_samesite
+
+            response.headers.append(
+                "set-cookie", ncookie.output(header="", sep=";").strip()
+            )
 
         return response
```

### Comparing `starlette_securecookies-1.1.0/tests/conftest.py` & `starlette_securecookies-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `starlette_securecookies-1.1.0/tests/extras/test_csrf.py` & `starlette_securecookies-1.1.1/tests/extras/test_csrf.py`

 * *Files identical despite different names*

### Comparing `starlette_securecookies-1.1.0/tests/test_other-party.py` & `starlette_securecookies-1.1.1/tests/test_other-party.py`

 * *Files identical despite different names*

### Comparing `starlette_securecookies-1.1.0/tests/test_securecookies.py` & `starlette_securecookies-1.1.1/tests/test_securecookies.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,25 @@
     client = client_factory(cookie_samesite="strict")
     client.get("/get")
 
     with pytest.raises(BadArgumentError, match="SameSite"):
         client = client_factory(cookie_samesite="invalid")
         client.get("/get")
 
+    with pytest.warns(UserWarning, match="Insecure"):
+        client = client_factory(cookie_secure=False, cookie_samesite="None")
+        client.get("/get")
+
 
 def test_outgoing(client_factory, fernet):
     # api write ginger-molasses, client needs to decrypt
     response = client_factory().get("/get")
     assert response.status_code == 200
 
+    assert len(response.headers.get_list("set-cookie")) == 1
     cookie = response.cookies["type"]
     assert fernet.decrypt(cookie.encode()).decode() == "ginger-molasses"
     assert not next(iter(response.cookies.jar)).secure
 
 
 def test_outgoing_complex(client_factory, fernet):
     # api write ginger-molasses overwrites secure=True, client needs to decrypt
@@ -41,26 +46,28 @@
 
 def test_outgoing_included(client_factory, fernet):
     # only type should be encrypted
     client = client_factory(included_cookies=["type"])
     response = client.get("/getm")
 
     assert response.status_code == 200
+    assert len(response.headers.get_list("set-cookie")) == 2
     assert (
         fernet.decrypt(response.cookies["type"].encode()).decode() == "ginger-molasses"
     )
     assert response.cookies["anothertype"] == "chocolate-chip"
 
 
 def test_outgoing_excluded(client_factory, fernet):
     # type should not be encrypted
     client = client_factory(excluded_cookies=["type"])
     response = client.get("/getm")
     assert response.status_code == 200
 
+    assert len(response.headers.get_list("set-cookie")) == 2
     cookie = response.cookies["anothertype"]
     assert fernet.decrypt(cookie.encode()).decode() == "chocolate-chip"
     assert response.cookies["type"] == "ginger-molasses"
 
 
 def test_incoming(client_factory, mock_cookies, fernet):
     # client passes encrypted, should validate if decrypted in middleware
```

### Comparing `starlette_securecookies-1.1.0/PKG-INFO` & `starlette_securecookies-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-securecookies
-Version: 1.1.0
+Version: 1.1.1
 Summary: Secure cookie middleware for Starlette applications.
 Keywords: starlette fastapi middleware encryption cookies
 Home-page: https://securecookies.thearchitector.dev
 Author-Email: Elias Gabriel <me@eliasfgabriel.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Elias Gabriel
@@ -57,35 +57,35 @@
 
 Tested support on Python 3.7, 3.8, 3.9, and 3.10, 3.11 on macOS, Windows, and Linux.
 
 ## How it works?
 
 ```mermaid
 sequenceDiagram
-    Browser->>+Middleware: Encrypted 'Cookie' header
+    Browser->>+Middleware: Encrypted 'Cookie' headers
     Middleware->>+Application: Decrypted cookies
     Application->>-Middleware: Plaintext cookies
-    Middleware->>-Browser: Encrypted 'Set-Cookie' header
+    Middleware->>-Browser: Encrypted 'Set-Cookie' headers
     Note over Application: *The Application may be your service<br />or any additional middleware.
 ```
 
 For any incoming cookies:
 
 1. Requests sent from the client's browser to your application are intercepted by `SecureCookiesMiddleware`.
-2. All `Cookie` headers are parsed and filter. Only cookies in the `included_cookies` and `excluded_cookies` parameters are parsed. All cookies are included by default.
-3. The cookies are decrypted. If cookie cannot be decrypted, or is otherwise invalid, it is discarded by default (`discard_invalid=True`).
+2. All `Cookie` headers are filtered and parsed. Only cookies in the `included_cookies` and `excluded_cookies` parameters are parsed. All cookies are included by default.
+3. The cookies are decrypted. If a cookie cannot be decrypted, or is otherwise invalid, it is discarded by default (`discard_invalid=True`).
 4. Any included and valid encrypted cookies in the ASGI request scope are replaced by the decrypted ones.
 5. The request scope is passed to any future middleware, and eventually your application. Cookies can be read normally anywhere downstream.
 
 For any outgoing cookies:
 
-7. Your application sets cookies with `response.set_cookie` as usual.
+7. Your application sets cookies with `response.set_cookie`, or by any other means of creating `Set-Cookie` headers.
 8. Other middleware run and add additional cookies, like [SessionMiddleware](https://www.starlette.io/middleware/#sessionmiddleware).
 9. All responses returned by your application are intercepted by `SecureCookiesMiddleware`.
-10. Cookies in the `included_cookies` and `excluded_cookies` parameters are re-encrypted, and their attributes (like `"SameSite"` and `"HttpOnly"`) are overridden by the parameters set in `SecureCookiesMiddleware` if set.
+10. Cookies in the `included_cookies` and not in the `excluded_cookies` parameters are re-encrypted, and their attributes (like `"SameSite"` and `"HttpOnly"`) are overridden by any parameters set in `SecureCookiesMiddleware`.
 11. The cookies in the response are replaced by the re-encrypted cookies, and the response is eventually propagated to the client's browser.
 
 ## Installation
 
 ```sh
 $ pdm add starlette-securecookies
 # or
```

