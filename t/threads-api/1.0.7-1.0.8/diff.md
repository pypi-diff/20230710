# Comparing `tmp/threads-api-1.0.7.tar.gz` & `tmp/threads-api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.0.7.tar", last modified: Sun Jul  9 21:01:32 2023, max compression
+gzip compressed data, was "threads-api-1.0.8.tar", last modified: Mon Jul 10 21:19:44 2023, max compression
```

## Comparing `threads-api-1.0.7.tar` & `threads-api-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.7/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 21:01:32.037741 threads-api-1.0.7/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9548 2023-07-09 20:54:06.000000 threads-api-1.0.7/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.7/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-09 21:01:32.037741 threads-api-1.0.7/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      785 2023-07-09 21:01:29.000000 threads-api-1.0.7/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.033741 threads-api-1.0.7/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.7/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.7/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    18797 2023-07-09 21:00:53.000000 threads-api-1.0.7/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.7/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.7/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.623238 threads-api-1.0.8/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.8/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11140 2023-07-10 21:19:44.619238 threads-api-1.0.8/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10610 2023-07-10 21:06:25.000000 threads-api-1.0.8/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      384 2023-07-10 21:19:18.000000 threads-api-1.0.8/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-10 21:19:44.623238 threads-api-1.0.8/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      789 2023-07-10 21:19:24.000000 threads-api-1.0.8/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.8/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.8/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    25108 2023-07-10 21:19:03.000000 threads-api-1.0.8/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.8/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.8/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11140 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.0.7/LICENSE` & `threads-api-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.7/PKG-INFO` & `threads-api-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.7
-Summary: Unofficial Python client for Meta Threads API
+Version: 1.0.8
+Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,34 +23,67 @@
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
-Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to retrieve user profile information, user IDs, and user profile threads.
+Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, post, retrieve user profile information, user IDs and user profile threads.
 
 Table of content:
 
+* [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
-* [Usage Examples](#Usage-Examples)
+* [Usage Examples](#usage-examples)
+* [Roadmap](#📌-roadmap)
+* [License](#license)
+
+# Demo
+<img src=".github/user_example1.jpeg" alt="drawing" width="500"/>
 
 
 ## Getting Started
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
 or
 ```bash
 poetry install threads-api
 ```
 
+Example using threads-api to post to Threads.net:
+``` python
+from threads_api.src.threads_api import ThreadsAPI
+import asyncio
+import os
+from dotenv import load_dotenv
+
+load_dotenv()
+
+async def post():
+    threads_api = ThreadsAPI()
+    await threads_api.login(os.environ.get('USERNAME'), os.environ,get('PASSWORD'))
+    result = await threads_api.post("I am posting this from the threads api!")
+
+    if result:
+        print("Post has been successfully posted")
+    else:
+        print("Unable to post.")
+
+async def main():
+    await post()
+
+# Create an event loop and run the main function
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
 ## Usage Examples
 <details>
   <summary>"get_user_id_from_username" Function</summary>
 
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
@@ -274,23 +307,31 @@
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login as User
 - [x] ✅ Write Posts
-- [x] ✅ Read public data\
-  - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
+  - [x] ✅ Posts with just text
+  - [x] ✅ Posts with text and an image
+  - [x] ✅ Posts with text that share a url
+- [x] ✅ Perform Actions
+  - [x] ✅ Like Posts
+  - [x] ✅ Unlike Posts
+  - [x] ✅ Follow User
+  - [x] ✅ Unfollow User
+- [x] ✅ Read Data\
+  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
   - [x] ✅ Read user profile info
   - [x] ✅ Read list of user Threads
   - [x] ✅ Read list of user Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ]🚧  Upload images and videos
-- [ ]🚧  Reply to Posts
-- [ ]🚧  CI/CD
-  - [ ]🚧  Pytest
-  - [ ]🚧  GitHub Actions Pipeline
+- [ ] 🚧  Upload images and videos
+- [ ] 🚧  Reply to Posts
+- [x] ✅  CI/CD
+  - [ ] 🚧  Pytest
+  - [x] ✅  GitHub Actions Pipeline
 
 
 # License
 This project is licensed under the MIT license.
```

### Comparing `threads-api-1.0.7/README.md` & `threads-api-1.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,34 +6,67 @@
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
-Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to retrieve user profile information, user IDs, and user profile threads.
+Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, post, retrieve user profile information, user IDs and user profile threads.
 
 Table of content:
 
+* [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
-* [Usage Examples](#Usage-Examples)
+* [Usage Examples](#usage-examples)
+* [Roadmap](#📌-roadmap)
+* [License](#license)
+
+# Demo
+<img src=".github/user_example1.jpeg" alt="drawing" width="500"/>
 
 
 ## Getting Started
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
 or
 ```bash
 poetry install threads-api
 ```
 
+Example using threads-api to post to Threads.net:
+``` python
+from threads_api.src.threads_api import ThreadsAPI
+import asyncio
+import os
+from dotenv import load_dotenv
+
+load_dotenv()
+
+async def post():
+    threads_api = ThreadsAPI()
+    await threads_api.login(os.environ.get('USERNAME'), os.environ,get('PASSWORD'))
+    result = await threads_api.post("I am posting this from the threads api!")
+
+    if result:
+        print("Post has been successfully posted")
+    else:
+        print("Unable to post.")
+
+async def main():
+    await post()
+
+# Create an event loop and run the main function
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
 ## Usage Examples
 <details>
   <summary>"get_user_id_from_username" Function</summary>
 
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
@@ -257,22 +290,30 @@
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login as User
 - [x] ✅ Write Posts
-- [x] ✅ Read public data\
-  - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
+  - [x] ✅ Posts with just text
+  - [x] ✅ Posts with text and an image
+  - [x] ✅ Posts with text that share a url
+- [x] ✅ Perform Actions
+  - [x] ✅ Like Posts
+  - [x] ✅ Unlike Posts
+  - [x] ✅ Follow User
+  - [x] ✅ Unfollow User
+- [x] ✅ Read Data\
+  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
   - [x] ✅ Read user profile info
   - [x] ✅ Read list of user Threads
   - [x] ✅ Read list of user Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ]🚧  Upload images and videos
-- [ ]🚧  Reply to Posts
-- [ ]🚧  CI/CD
-  - [ ]🚧  Pytest
-  - [ ]🚧  GitHub Actions Pipeline
+- [ ] 🚧  Upload images and videos
+- [ ] 🚧  Reply to Posts
+- [x] ✅  CI/CD
+  - [ ] 🚧  Pytest
+  - [x] ✅  GitHub Actions Pipeline
 
 
 # License
 This project is licensed under the MIT license.
```

### Comparing `threads-api-1.0.7/setup.py` & `threads-api-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.0.7',
-    description='Unofficial Python client for Meta Threads API',
+    version='1.0.8',
+    description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
     install_requires=[
```

### Comparing `threads-api-1.0.7/threads_api/src/threads_api.py` & `threads-api-1.0.8/threads_api/src/threads_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 import urllib.parse
 import random
 import urllib
 import os
 import mimetypes
 import uuid
 import time
+import traceback
+
+BASE_URL = "https://i.instagram.com/api/v1"
+LOGIN_URL = BASE_URL + "/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
+POST_URL_TEXTONLY = BASE_URL + "/media/configure_text_only_post/"
+POST_URL_IMAGE = BASE_URL + "/media/configure_text_post_app_feed/"
 
 class ThreadsAPIOptions:
     def __init__(self, fbLSDToken: Optional[str] = None, 
                        token: Optional[str] = None):
         self.fbLSDToken = fbLSDToken
         self.token = token
 
@@ -29,18 +35,20 @@
 
         if options and options.fbLSDToken:
             self.fbLSDToken = options.fbLSDToken
 
         if options and options.token:
             self.token = options.token
 
+        self.is_logged_in = False
+
     async def login(self, username, password):
         if username is None or password is None:
-            return None
-        
+            raise Exception("Username or password are invalid")
+
         self.username = username
 
         try:
             blockVersion = "5f56efad68e1edec7801f630b5c122704ec5378adbee6609a448f105f34a9c73"
             headers = {
                 "User-Agent": "Barcelona 289.0.0.77.109 Android",
                 "Sec-Fetch-Site": "same-origin",
@@ -59,64 +67,75 @@
                     },
                 }
             )
             bk_client_context = json.dumps(
                 {"bloks_version": blockVersion, "styles_id": "instagram"}
             )
 
-            LOGIN_URL = "https://i.instagram.com/api/v1/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
             payload = f"params={urllib.parse.quote(params)}&bk_client_context={urllib.parse.quote(bk_client_context)}&bloks_versioning_id={blockVersion}"
             
             async with aiohttp.ClientSession() as session:
                 async with session.post(LOGIN_URL, timeout=60 * 1000, headers=headers, data=payload) as response:
                     data = await response.text()
-            
+
             if data == "Oops, an error occurred.":
                 raise Exception("Failed to login")
-            
-            pos = data.split("Bearer IGT:2:")
 
+            pos = data.split("Bearer IGT:2:")
             if len(pos) > 1:
                 pos = pos[1]
                 pos = pos.split("==")[0]
                 token = f"{pos}=="
                 self.token = token
 
                 self.user_id = await self.get_user_id_from_username(username)
+                self.is_logged_in = True
                 return True
-            return False
+            else:
+                raise Exception("Error with the login response")
         except Exception as e:
             print("[ERROR] ", e)
             raise
 
+    async def __auth_required_post_request(self, url: str):
+        headers = {
+                'Authorization': f'Bearer IGT:2:{self.token}',
+                'User-Agent': 'Barcelona 289.0.0.77.109 Android',
+                'Sec-Fetch-Site': 'same-origin',
+                'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
+            }
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url, headers=headers) as response:
+                return await response.json()
+            
     async def get_user_id_from_username(self, username: str) -> str:
         url = f"https://www.threads.net/@{username}"
         headers = {
             "authority": "www.threads.net",
             "accept": "*/*",
-            "accept-language": "ko",
+            'accept-language': 'en-US,en;q=0.9',
             "cache-control": "no-cache",
             "origin": "https://www.threads.net",
             "pragma": "no-cache",
             "referer": f"https://www.threads.net/@{username}",
             "x-asbd-id": "129477",
-            "x-fb-lsd": self.fbLSDToken,
+            "x-fb-lsd": "NjppQDEgONsU_1LCzrmp6q",
             "x-ig-app-id": "238260118697367",
         }
-
+        
         async with aiohttp.ClientSession() as session:
             async with session.get(url, headers=headers) as response:
                 text = await response.text()
 
         text = text.replace('\\s', "").replace('\\n', "")
         user_id = re.search(r'"props":{"user_id":"(\d+)"},', text)
 
         lsd_token_match = re.search('"LSD",\[\],{"token":"(\w+)"},\d+\]', text)
         lsd_token = lsd_token_match.group(1) if lsd_token_match else None
-        self.fbLSDToken = lsd_token
+        #self.fbLSDToken = lsd_token
 
         return user_id.group(1) if user_id else None
 
     async def get_user_profile(self, username: str, user_id: str):
         url = 'https://www.threads.net/api/graphql'
         headers = {
             'authority': 'www.threads.net',
@@ -303,15 +322,15 @@
         return threads
     
     async def get_post_id_from_url(self, post_url, options=None):
         url = post_url
         headers = {
             "authority": "www.threads.net",
             "accept": "*/*",
-            "accept-language": "ko",
+            'accept-language': 'en-US,en;q=0.9',
             "cache-control": "no-cache",
             "origin": "https://www.threads.net",
             "pragma": "no-cache",
             "referer": post_url,
             "x-asbd-id": "129477",
             "x-fb-lsd": self.fbLSDToken,
             "x-ig-app-id": "238260118697367",
@@ -372,66 +391,187 @@
         '__spin_t': '1688761899',
         '__jssesw': '1',
         'fb_api_caller_class': 'RelayModern',
         'fb_api_req_friendly_name': 'BarcelonaPostPageQuery',
         'variables': '{"postID":"3141737961795561608"}',
         'server_timestamps': 'true',
         'doc_id': '6529829603744567',
-    }
+        }
         
 
         async with aiohttp.ClientSession() as session:
             async with session.post(url, headers=headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['data']
         return threads
-                
-    async def post(self, caption: str) -> bool:
-        if self.user_id is None:
-            raise Exception("Failed to resolve user_id. You must login to post posts")
-
-        if self.token is None:
-            raise Exception("Failed to resolve token. You must login to post posts")
-
-        params = json.dumps(
-            {
-                "publish_mode": "text_post",
-                "text_post_app_info": '{"reply_control":0}',
-                "timezone_offset": "-25200",
-                "source_type": "4",
-                "_uid": self.user_id,
-                "device_id": f"android-{random.randint(0, 1e24):x}",
-                "caption": caption,
-                "upload_id": str(int(datetime.now().timestamp() * 1000)),
-                "device": {
-                    "manufacturer": "OnePlus",
-                    "model": "ONEPLUS+A3010",
-                    "android_version": 25,
-                    "android_release": "7.1.1",
+    
+    async def post(
+        self, caption: str, image_path: str = None, url: str = None, parent_post_id: str = None
+    ) -> bool:
+        def __get_app_headers() -> dict:
+            headers = {
+                "User-Agent": f"Barcelona 289.0.0.77.109 Android",
+                "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+            }
+            if self.token is not None:
+                headers["Authorization"] = f"Bearer IGT:2:{self.token}"
+            return headers
+
+        async def __is_valid_url(url: str) -> bool:
+            url_pattern = re.compile(
+                r"^(https?://)?"
+                r"((([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9-]*[a-zA-Z0-9])\.)+[a-zA-Z]{2,})"
+                r"(/?|/[-a-zA-Z0-9_%+.~!@#$^&*(){}[\]|/\\<>]*)$"
+            )
+            if re.match(url_pattern, url) is not None:
+                try:
+                    async with aiohttp.ClientSession() as session:
+                        async with session.head(url) as response:
+                            return response.status == 200
+                except aiohttp.ClientError:
+                    return False
+            return False
+
+        async def __download(url: str) -> bytes:
+            try:
+                async with aiohttp.ClientSession() as session:
+                    async with session.get(url) as response:
+                        response.raise_for_status()
+                        return await response.read()
+            except aiohttp.ClientError as e:
+                raise Exception("[ERROR] failed to load file: ", e)
+
+        async def __upload_image(image_url: str, image_content: bytes) -> str:
+            headers = __get_app_headers().copy()
+
+            upload_id = int(time.time() * 1000)
+            name = f"{upload_id}_0_{random.randint(1000000000, 9999999999)}"
+            url = "https://www.instagram.com/rupload_igphoto/" + name
+            mime_type = None
+            if image_content is None:
+                with open(image_url, mode="rb") as f:
+                    content = f.read()
+                mime_type, _ = mimetypes.guess_type(image_url)
+            else:
+                content = image_content
+                async with aiohttp.ClientSession() as session:
+                    async with session.head(image_url) as response:
+                        content_type = response.headers.get("Content-Type")
+                        if not content_type:
+                            file_name = url.split("/")[-1]
+                            mime_type, _ = mimetypes.guess_type(file_name)
+                        if mime_type is None:
+                            mime_type = "jpeg"
+
+            x_instagram_rupload_params = {
+                "upload_id": f"{upload_id}",
+                "media_type": "1",
+                "sticker_burnin_params": "[]",
+                "image_compression": json.dumps(
+                    {"lib_name": "moz", "lib_version": "3.1.m", "quality": "80"}
+                ),
+                "xsharing_user_ids": "[]",
+                "retry_context": {
+                    "num_step_auto_retry": "0",
+                    "num_reupload": "0",
+                    "num_step_manual_retry": "0",
                 },
+                "IG-FB-Xpost-entry-point-v2": "feed",
+            }
+            content_length = len(content)
+            if mime_type.startswith("image/"):
+                mime_type = mime_type.replace("image/", "")
+            image_headers = {
+                "X_FB_PHOTO_WATERFALL_ID": str(uuid.uuid4()),
+                "X-Entity-Type": "image/" + mime_type,
+                "Offset": "0",
+                "X-Instagram-Rupload-Params": json.dumps(x_instagram_rupload_params),
+                "X-Entity-Name": f"{name}",
+                "X-Entity-Length": f"{content_length}",
+                "Content-Type": "application/octet-stream",
+                "Content-Length": f"{content_length}",
+                "Accept-Encoding": "gzip",
             }
-        )
-        POST_HEADERS_DEFAULT = {
-            "User-Agent": "Barcelona 289.0.0.77.109 Android",
-            "Sec-Fetch-Site": "same-origin",
-            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
-        }
 
+            headers.update(image_headers)
+            async with aiohttp.ClientSession() as session:
+                async with session.post(url, headers=headers, data=content) as response:
+                    if response.status == 200:
+                        return await response.json()
+                    else:
+                        raise Exception("Failed to upload image")
+
+        if not self.is_logged_in:
+            raise Exception("You need to login before posting")
+        
+        now = datetime.now()
+        timezone_offset = (datetime.now() - datetime.utcnow()).seconds
+
+        params = {
+            "text_post_app_info": {"reply_control": 0},
+            "timezone_offset": "-" + str(timezone_offset),
+            "source_type": "4",
+            "_uid": self.user_id,
+            "device_id": str(f"android-{random.randint(0, 1e24):x}"),
+            "caption": caption,
+            "upload_id": str(int(now.timestamp() * 1000)),
+            "device": {
+                "manufacturer": "OnePlus",
+                "model": "ONEPLUS+A3010",
+                "android_version": 25,
+                "android_release": "7.1.1",
+            },
+        }
+        post_url = POST_URL_TEXTONLY
+        if image_path is not None:
+            post_url = POST_URL_IMAGE
+            image_content = None
+            if not (os.path.isfile(image_path) and os.path.exists(image_path)):
+                if not __is_valid_url(image_path):
+                    return False
+                else:
+                    image_content = await __download(image_path)
+            upload_id = await __upload_image(image_url=image_path, image_content=image_content)
+            if upload_id is None:
+                return False
+            params["upload_id"] = upload_id["upload_id"]
+            params["scene_capture_type"] = ""
+        elif url is not None:
+            params["text_post_app_info"]["link_attachment_url"] = url
+        if image_path is None:
+            params["publish_mode"] = "text_post"
+
+        if parent_post_id is not None:
+            params["text_post_app_info"]["reply_id"] = parent_post_id
+        params = json.dumps(params)
         payload = f"signed_body=SIGNATURE.{urllib.parse.quote(params)}"
-        headers = POST_HEADERS_DEFAULT.copy()
-        headers.update({"Authorization": f"Bearer IGT:2:{self.token}"})
+        headers = __get_app_headers().copy()
 
         try:
             async with aiohttp.ClientSession() as session:
-                async with session.post("https://i.instagram.com/api/v1/media/configure_text_only_post/", headers=headers, data=payload) as response:
+                async with session.post(post_url, headers=headers, data=payload) as response:
                     if response.status == 200:
                         return True
                     else:
-                        return False
+                        raise Exception("Failed to post")
         except Exception as e:
             print("[ERROR] ", e)
-            return False
+            raise
+
+    async def follow_user(self, user_id: str) -> bool:
+        if not self.is_logged_in:
+            raise Exception("The action 'follow' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/create/{user_id}/")
+        return res["status"] == "ok"
+
+    async def unfollow_user(self, user_id: str) -> bool:
+        if not self.is_logged_in:
+            raise Exception("The action 'unfollow' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/destroy/{user_id}/")
+        return res["status"] == "ok"
```

### Comparing `threads-api-1.0.7/threads_api.egg-info/PKG-INFO` & `threads-api-1.0.8/threads_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.7
-Summary: Unofficial Python client for Meta Threads API
+Version: 1.0.8
+Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,34 +23,67 @@
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
-Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to retrieve user profile information, user IDs, and user profile threads.
+Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, post, retrieve user profile information, user IDs and user profile threads.
 
 Table of content:
 
+* [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
-* [Usage Examples](#Usage-Examples)
+* [Usage Examples](#usage-examples)
+* [Roadmap](#📌-roadmap)
+* [License](#license)
+
+# Demo
+<img src=".github/user_example1.jpeg" alt="drawing" width="500"/>
 
 
 ## Getting Started
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
 or
 ```bash
 poetry install threads-api
 ```
 
+Example using threads-api to post to Threads.net:
+``` python
+from threads_api.src.threads_api import ThreadsAPI
+import asyncio
+import os
+from dotenv import load_dotenv
+
+load_dotenv()
+
+async def post():
+    threads_api = ThreadsAPI()
+    await threads_api.login(os.environ.get('USERNAME'), os.environ,get('PASSWORD'))
+    result = await threads_api.post("I am posting this from the threads api!")
+
+    if result:
+        print("Post has been successfully posted")
+    else:
+        print("Unable to post.")
+
+async def main():
+    await post()
+
+# Create an event loop and run the main function
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
 ## Usage Examples
 <details>
   <summary>"get_user_id_from_username" Function</summary>
 
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
@@ -274,23 +307,31 @@
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login as User
 - [x] ✅ Write Posts
-- [x] ✅ Read public data\
-  - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
+  - [x] ✅ Posts with just text
+  - [x] ✅ Posts with text and an image
+  - [x] ✅ Posts with text that share a url
+- [x] ✅ Perform Actions
+  - [x] ✅ Like Posts
+  - [x] ✅ Unlike Posts
+  - [x] ✅ Follow User
+  - [x] ✅ Unfollow User
+- [x] ✅ Read Data\
+  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
   - [x] ✅ Read user profile info
   - [x] ✅ Read list of user Threads
   - [x] ✅ Read list of user Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ]🚧  Upload images and videos
-- [ ]🚧  Reply to Posts
-- [ ]🚧  CI/CD
-  - [ ]🚧  Pytest
-  - [ ]🚧  GitHub Actions Pipeline
+- [ ] 🚧  Upload images and videos
+- [ ] 🚧  Reply to Posts
+- [x] ✅  CI/CD
+  - [ ] 🚧  Pytest
+  - [x] ✅  GitHub Actions Pipeline
 
 
 # License
 This project is licensed under the MIT license.
```

