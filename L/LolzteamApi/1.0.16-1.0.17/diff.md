# Comparing `tmp/LolzteamApi-1.0.16.tar.gz` & `tmp/LolzteamApi-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.16.tar", last modified: Sun Jul  9 10:42:00 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.17.tar", last modified: Mon Jul 10 00:38:56 2023, max compression
```

## Comparing `LolzteamApi-1.0.16.tar` & `LolzteamApi-1.0.17.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 10:42:00.142315 LolzteamApi-1.0.16/
--rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.16/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-09 10:42:00.114534 LolzteamApi-1.0.16/LolzteamApi/
--rw-rw-rw-   0        0        0   164017 2023-07-09 10:35:34.000000 LolzteamApi-1.0.16/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0      111 2023-07-08 01:36:03.000000 LolzteamApi-1.0.16/LolzteamApi/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-07-08 01:42:28.000000 LolzteamApi-1.0.16/LolzteamApi/check_updates.py
-drwxrwxrwx   0        0        0        0 2023-07-09 10:42:00.138999 LolzteamApi-1.0.16/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2260 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2260 2023-07-09 10:42:00.138999 LolzteamApi-1.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-07-08 18:11:39.000000 LolzteamApi-1.0.16/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 10:42:00.142829 LolzteamApi-1.0.16/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-09 09:09:11.000000 LolzteamApi-1.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 00:38:56.634084 LolzteamApi-1.0.17/
+-rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.17/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-10 00:38:56.608044 LolzteamApi-1.0.17/LolzteamApi/
+-rw-rw-rw-   0        0        0   166121 2023-07-10 00:33:36.000000 LolzteamApi-1.0.17/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0       36 2023-07-10 00:23:41.000000 LolzteamApi-1.0.17/LolzteamApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 00:38:56.631810 LolzteamApi-1.0.17/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2260 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2260 2023-07-10 00:38:56.634084 LolzteamApi-1.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-07-08 18:11:39.000000 LolzteamApi-1.0.17/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 00:38:56.635590 LolzteamApi-1.0.17/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-07-10 00:14:50.000000 LolzteamApi-1.0.17/setup.py
```

### Comparing `LolzteamApi-1.0.16/LICENSE` & `LolzteamApi-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.16/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.17/LolzteamApi/LolzteamApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 import requests
 import time
 import json
 
+from importlib.metadata import version
+from bs4 import BeautifulSoup
+
 
 class LolzteamApi:
-    def __init__(self, token: str, bypass_429: bool = True, language: str = "RU"):
+    def __init__(self, token: str, bypass_429: bool = True, language: str = "RU", disable_update_check: bool = False):
         """
         :param token: Your token. You can get in there -> https://zelenka.guru/account/api
         :param bypass_429: Bypass status code 429 by sleep
         :param language: Language for your api responses. Pass "en" if you want to get responses in english or pass "ru" if you want to get responses in russian.
+        :param disable_update_check: Pass True if you don't want to see annoying update message
         """
 
+        if not disable_update_check:
+            self.__check_for_new_version()
+
         self.__token = token
         self.__headers = {'Authorization': f"bearer {self.__token}"}
 
         self.__bypass_429 = bypass_429
         self.__auto_delay_time = time.time() - 3
         self.__locale = language
-        self.__token_user_id = self.__set_user_id()
+        self.__token_user_id = self.__set_user_id
 
         self.market = self.__Market(self, self.__token_user_id)
         self.forum = self.__Forum(self)
 
     def send_request(self, method: str, url: str, params: dict = None, data=None, files=None):
         method = method.upper()
         LolzteamApi.__auto_delay(self)
 
         if params is None:
             params = {}
         params["locale"] = self.__locale
-
         match method:
             case "GET":
                 response = requests.get(url=url, params=params, data=data, files=files, headers=self.__headers)
             case "POST":
                 response = requests.post(url=url, params=params, data=data, files=files, headers=self.__headers)
             case "PUT":
                 response = requests.put(url=url, params=params, data=data, files=files, headers=self.__headers)
             case "DELETE":
                 response = requests.delete(url=url, params=params, data=data, files=files, headers=self.__headers)
             case _:
                 response = {"error": "Создатель либы где-то проебался. Отпиши @AS7RID в тг, он починит"}
         self.__auto_delay_time = time.time()
+        print(time.time())
         try:
             return response.json()
         except requests.exceptions.JSONDecodeError:
             return response.text
 
     def __set_user_id(self):
         url = "https://api.lzt.market/me"
@@ -62,14 +69,33 @@
         if self.__bypass_429:
             current_time = time.time()
             time_diff = current_time - self.__auto_delay_time
             if time_diff < 3.0:  # if difference between current and last call > 3 seconds we will sleep the rest of the time
 
                 time.sleep(3.003 - time_diff)
 
+    @staticmethod
+    def __check_for_new_version():
+        current_version = version('LolzteamApi')
+        response = requests.get("https://pypi.org/project/LolzteamApi/")
+        newest_version = BeautifulSoup(response.text, 'html.parser').select(
+            selector="#content > div.banner > div > div.package-header__left > h1")[0].text.replace("LolzteamApi",
+                                                                                                    "").replace(" ",
+                                                                                                                "").replace(
+            "\n", "")
+        if current_version != newest_version:
+            print(f"Your version of LolzteamApi is outdated.")
+            print(f"It has problems that have been solved in the new version")
+            print(f"Your version:   {current_version}")
+            print(f"Newest version: {newest_version}")
+            print()
+            print(f"You can update your package using the command below")
+            print(f"pip install LolzteamApi --upgrade")
+            print()
+
     def change_token(self, new_token: str):
         self.__token = new_token
         self.__token_user_id = self.__set_user_id()
         self.__headers = {'Authorization': f"bearer {self.__token}"}
 
     class __Forum:
         def __init__(self, api_self):
@@ -2421,14 +2447,16 @@
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
                 if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/items"
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
@@ -2508,14 +2536,16 @@
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
                 if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             # Copy of __List.favorite
             def favorite(self, page: int = None):
                 """
@@ -2890,14 +2920,16 @@
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
                 if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/items"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def purchased(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
                           title: str = None):
                 """
@@ -2969,14 +3001,16 @@
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
                 if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def favorite(self, page: int = None):
                 """
                 GET https://api.lzt.market/fave
@@ -3095,14 +3129,16 @@
                     "end_date": end_date,
                     "wallet": wallet,
                     "comment": comment,
                     "is_hold": is_hold,
                     "show_payments_stats": show_payments_stats
                 }
                 if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/payments"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def transfer(self, amount: int, secret_answer: str, currency: str = "rub", user_id: int = None,
                          username: str = None, comment: str = None, transfer_hold: bool = None,
                          hold_length_option: str = None,
```

### Comparing `LolzteamApi-1.0.16/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.17/LolzteamApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.16
+Version: 1.0.17
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.16 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.17 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.16/PKG-INFO` & `LolzteamApi-1.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.16
+Version: 1.0.17
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.16 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.17 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.16/README.md` & `LolzteamApi-1.0.17/README.md`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.16/setup.py` & `LolzteamApi-1.0.17/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests", "beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.16",
+    version="1.0.17",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
```

