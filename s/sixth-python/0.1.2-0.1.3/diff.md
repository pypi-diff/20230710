# Comparing `tmp/sixth-python-0.1.2.tar.gz` & `tmp/sixth-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.1.2.tar", last modified: Sat Jul  8 18:57:03 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.1.3.tar", last modified: Mon Jul 10 12:14:22 2023, max compression
```

## Comparing `sixth-python-0.1.2.tar` & `sixth-python-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-08 18:57:03.000000 sixth-python-0.1.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.2/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-08 18:57:03.000000 sixth-python-0.1.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-08 18:53:36.000000 sixth-python-0.1.2/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.2/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.2/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-03 02:16:20.000000 sixth-python-0.1.2/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.2/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-03 02:16:20.000000 sixth-python-0.1.2/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     5856 2023-07-08 18:52:20.000000 sixth-python-0.1.2/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.2/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.1.2/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      921 2023-07-08 18:20:56.000000 sixth-python-0.1.2/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4190 2023-07-03 02:16:20.000000 sixth-python-0.1.2/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.2/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.2/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.2/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-08 18:57:03.000000 sixth-python-0.1.2/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:14:22.000000 sixth-python-0.1.3/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 12:14:22.000000 sixth-python-0.1.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.3/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-10 12:14:22.000000 sixth-python-0.1.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-10 12:13:27.000000 sixth-python-0.1.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.3/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.3/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-10 11:42:02.000000 sixth-python-0.1.3/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.3/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-10 11:42:02.000000 sixth-python-0.1.3/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     7024 2023-07-10 12:10:24.000000 sixth-python-0.1.3/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.3/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      143 2023-07-09 17:50:41.000000 sixth-python-0.1.3/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      978 2023-07-10 11:22:10.000000 sixth-python-0.1.3/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4252 2023-07-10 11:43:36.000000 sixth-python-0.1.3/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.3/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.3/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.3/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-10 12:14:22.000000 sixth-python-0.1.3/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.1.2/PKG-INFO` & `sixth-python-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.2/README.md` & `sixth-python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.2/setup.py` & `sixth-python-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Sixth offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
```

### Comparing `sixth-python-0.1.2/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.1.3/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.2/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.1.3/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.2/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.1.3/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.2/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.1.3/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,26 @@
 class SixRateLimiterMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, apikey: str, fastapi_app: FastAPI, project_config: schemas.ProjectConfig):
         super().__init__(app)
         self._config = project_config
         self._log_dict = {}
         self._app = app
         self._apikey = apikey
+        self._route_last_updated = {}
         for route in fastapi_app.router.routes:
             if type(route.app )== FastAPI:
                 for new_route in route.app.routes:
                     path = "/v"+str(route.app.version)+new_route.path
                     edited_route = re.sub(r'\W+', '~', path)
                     self._log_dict[str(edited_route)] = {}
+                    self._route_last_updated[str(edited_route)] = time.time()
             else:
                 edited_route = re.sub(r'\W+', '~', route.path)
                 self._log_dict[str(edited_route)] = {}
+                self._route_last_updated[str(edited_route)] = time.time()
                 
 
     async def set_body(self, request: Request, body: bytes):
         async def receive() -> Message:
             return {'type': 'http.request', 'body': body}
         request._receive = receive
         
@@ -48,87 +51,106 @@
         if requests == None:
             self._log_dict[route][uid] = []
         if len(self._log_dict[route].get(uid)) < rate_limit:
             self._log_dict[route].get(uid, []).append(timestamp)
             return True
             
         new_req = [new_req for new_req in self._log_dict[route][uid] if new_req > timestamp-interval]
-        
         if len(new_req) < rate_limit:
             self._log_dict[route][uid].append(timestamp)
             return True
         else: 
-            self._log_dict[route][uid].append(timestamp)
             return False
         
     async def _parse_bools(self, string: bytes)-> str:
+        '''
+            used  to parse boolean values in string format and convert it to Python's boolean format
+        '''
         string = string.decode("utf-8")
         string = string.replace(' ', "")
         string = string.replace('true,', "True,")
         string = string.replace(",true", "True,")
         string = string.replace('false,', "False,")
         string = string.replace(",false", "False,")
         out=ast.literal_eval(string)
         return out
         
     async def dispatch(self,request: Request,call_next) -> None:
         host = request.client.host
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
         headers = request.headers
+        query_params = request.query_params
+        rate_limit_resp = None
+        status_code = 200
+        
+        
         #fail safe if there is an internal server error our servers are currenly in maintnance
         try:
-            rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
+            if time.time() - self._route_last_updated[route] >5:
+                #update rate limit details every 5 seconds
+                rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
+                self._route_last_updated[route] = time.time()
+                status_code = rate_limit_resp.status_code
             body = None
 
             try:
                 body = await request.body()
                 await self.set_body(request, body)
                 body = await self._parse_bools(body)
             except:
                 pass
-           
-            if rate_limit_resp.status_code == 200:
+            
+            if status_code == 200: 
                 try:
-                    rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
-                    self._config.rate_limiter[route] = rate_limit
-                    preferred_id = self._config.rate_limiter[route].unique_id
-                   
-                    if preferred_id == "" or preferred_id=="host":
-                        preferred_id = host
-                        
-                    else:
-                        if rate_limit.rate_limit_type == "body":
-                            if body != None:
-                                preferred_id = body[preferred_id]
-                            else:
-                                _response = await call_next(request)
-                                return _response
-                        elif rate_limit.rate_limit_type == "header":
-                            preferred_id = headers[preferred_id]
-                        else:
-                            preferred_id = host
+                    rate_limit = schemas.RateLimiter.model_validate(rate_limit_resp.json()) if rate_limit_resp != None else self._config.rate_limiter[route]
+                    if rate_limit.is_active:
+                        self._config.rate_limiter[route] = rate_limit
+                        preferred_id = self._config.rate_limiter[route].unique_id
                     
+                        if preferred_id == "" or preferred_id=="host":
+                            preferred_id = host
+                            
+                        else:
+                            if rate_limit.rate_limit_type == "body":
+                                if body != None:
+                                    preferred_id = body[preferred_id]
+                                else:
+                                    _response = await call_next(request)
+                                    return _response
+                            elif rate_limit.rate_limit_type == "header":
+                                preferred_id = headers[preferred_id]
+                            elif rate_limit.rate_limit_type == "args":
+                                preferred_id = query_params[preferred_id]
+                            else:
+                                preferred_id = host
+                        
 
-                    if self._is_rate_limit_reached(preferred_id, route): 
+                        if self._is_rate_limit_reached(preferred_id, route): 
+                            _response = await call_next(request)
+                            return _response
+                        else:
+                            temp_payload = rate_limit.error_payload.values()
+                            final = {}
+                            for c in temp_payload:
+                                for keys in c:
+                                    if keys != "uid":
+                                        final[keys] = c[keys]
+                            output= final
+                            headers = MutableHeaders(headers={"content-length": str(len(str(output).encode())), 'content-type': 'application/json'})
+                            return Response(json.dumps(output), status_code=420, headers=headers)
+                    else:
+                       
                         _response = await call_next(request)
                         return _response
-                    else:
-                        temp_payload = rate_limit.error_payload.values()
-                        final = {}
-                        for c in temp_payload:
-                            for keys in c:
-                                if keys != "uid":
-                                    final[keys] = c[keys]
-                        output= final
-                        headers = MutableHeaders(headers={"content-length": str(len(str(output).encode())), 'content-type': 'application/json'})
-                        return Response(json.dumps(output), status_code=401, headers=headers)
                 except Exception as e:
+                   
                     _response = await call_next(request)
                     return _response
             else:
                 #fail safe if there is an internal server error our servers are currenly in maintnance
                 _response = await call_next(request)
                 return _response
         except Exception as e:
+            
             _response = await call_next(request)
             return _response
```

### Comparing `sixth-python-0.1.2/sixth/schemas.py` & `sixth-python-0.1.3/sixth/schemas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from pydantic import BaseModel
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Union
 import uuid
 
 
 class RateLimiter(BaseModel): 
     error_payload_id: str = str(uuid.uuid4())
     id: str
     route: str
-    interval: int 
+    interval: Union[float, int, str]
     rate_limit: int
     last_updated: float 
     created_at: float
-    rate_limit_type: str = "ip address" #ip address, header, body
+    rate_limit_type: str = "ip address" #ip address, header, body, query_param
     unique_id: str = "host"
     error_payload: Dict[str , dict] = {
         error_payload_id:{
             "message": "max_limit_request_reached", 
             "uid": error_payload_id
         }
     }
+    is_active:bool
 
 class Encryption(BaseModel):
     public_key: str 
     private_key: str 
     use_count: int
     last_updated: float
     created_at: float
```

### Comparing `sixth-python-0.1.2/sixth/sdk.py` & `sixth-python-0.1.3/sixth/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,37 +48,37 @@
                     path = "/v"+str(route.app.version)+new_route.path
                     edited_route = re.sub(r'\W+', '~', path)
                     if config and edited_route in config.rate_limiter.keys():
                         #default config has been set earlier on so skip
                         _rl_configs[edited_route] = config.rate_limiter[edited_route]
                         continue
                     #set the default values
-                    _rl_config = schemas.RateLimiter(id = edited_route, route=edited_route, interval=60, rate_limit=10, last_updated=get_time_now(), created_at=get_time_now(), unique_id="host", rate_limit_type="ip address")
+                    _rl_config = schemas.RateLimiter(id = edited_route, route=edited_route, interval=60, rate_limit=10, last_updated=get_time_now(), created_at=get_time_now(), unique_id="host", rate_limit_type="ip address", is_active=False)
                     _rl_configs[edited_route] = _rl_config
             else:
                 edited_route = re.sub(r'\W+', '~', route.path)
                 if config and edited_route in config.rate_limiter.keys():
                         #default config has been set earlier on so skip
                         _rl_configs[edited_route] = config.rate_limiter[edited_route]
                         continue
                     #set the default values
-                _rl_config = schemas.RateLimiter(id = edited_route, route=edited_route, interval=60, rate_limit=10, last_updated=get_time_now(), created_at=get_time_now(), unique_id="host")
+                _rl_config = schemas.RateLimiter(id = edited_route, route=edited_route, interval=60, rate_limit=10, last_updated=get_time_now(), created_at=get_time_now(), unique_id="host", is_active=False)
                 _rl_configs[edited_route] = _rl_config
 
         _config = schemas.ProjectConfig(
             user_id = self._apikey, 
             rate_limiter = _rl_configs, 
-            encryption = schemas.Encryption(public_key="dummy",private_key="dummy", use_count=0, last_updated=0,created_at=0), 
-            base_url = "op",
+            encryption = schemas.Encryption(public_key="dummy",private_key="dummy", use_count=0, last_updated=0,created_at=0, is_active=False), 
+            base_url = "project",
             last_updated=get_time_now(), 
             created_at=get_time_now(), 
             encryption_enabled=config.encryption_enabled if config != None else False, 
             rate_limiter_enabled=config.rate_limiter_enabled if config != None else True
         )
         _base_url = "https://backend.withsix.co"
-        _project_config_resp = requests.post(_base_url+"/project-config/config/sync-user-config", json=_config.dict())
+        _project_config_resp = requests.post(_base_url+"/project-config/config/sync-user-config", json=_config.model_dump())
         if _project_config_resp.status_code == status.HTTP_200_OK:
             return _config
         else: 
             return _config
```

### Comparing `sixth-python-0.1.2/sixth/utils/encryption_utils.py` & `sixth-python-0.1.3/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.2/sixth/utils/time_utils.py` & `sixth-python-0.1.3/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.2/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.1.3/sixth_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.2/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.1.3/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.2/sixth_python.egg-info/requires.txt` & `sixth-python-0.1.3/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*

