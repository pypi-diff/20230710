# Comparing `tmp/LolzteamApi-1.0.17.tar.gz` & `tmp/LolzteamApi-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.17.tar", last modified: Mon Jul 10 00:38:56 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.18.tar", last modified: Mon Jul 10 05:30:26 2023, max compression
```

## Comparing `LolzteamApi-1.0.17.tar` & `LolzteamApi-1.0.18.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 00:38:56.634084 LolzteamApi-1.0.17/
--rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.17/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-10 00:38:56.608044 LolzteamApi-1.0.17/LolzteamApi/
--rw-rw-rw-   0        0        0   166121 2023-07-10 00:33:36.000000 LolzteamApi-1.0.17/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0       36 2023-07-10 00:23:41.000000 LolzteamApi-1.0.17/LolzteamApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 00:38:56.631810 LolzteamApi-1.0.17/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2260 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-10 00:38:56.000000 LolzteamApi-1.0.17/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2260 2023-07-10 00:38:56.634084 LolzteamApi-1.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-07-08 18:11:39.000000 LolzteamApi-1.0.17/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 00:38:56.635590 LolzteamApi-1.0.17/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-10 00:14:50.000000 LolzteamApi-1.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:30:26.608044 LolzteamApi-1.0.18/
+-rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.18/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-10 05:30:26.602043 LolzteamApi-1.0.18/LolzteamApi/
+-rw-rw-rw-   0        0        0   167776 2023-07-10 05:28:40.000000 LolzteamApi-1.0.18/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0       36 2023-07-10 00:23:41.000000 LolzteamApi-1.0.18/LolzteamApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:30:26.606045 LolzteamApi-1.0.18/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2261 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2261 2023-07-10 05:30:26.607045 LolzteamApi-1.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2023-07-10 01:19:44.000000 LolzteamApi-1.0.18/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 05:30:26.608044 LolzteamApi-1.0.18/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-07-10 01:23:22.000000 LolzteamApi-1.0.18/setup.py
```

### Comparing `LolzteamApi-1.0.17/LICENSE` & `LolzteamApi-1.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.17/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.18/LolzteamApi/LolzteamApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
             case "PUT":
                 response = requests.put(url=url, params=params, data=data, files=files, headers=self.__headers)
             case "DELETE":
                 response = requests.delete(url=url, params=params, data=data, files=files, headers=self.__headers)
             case _:
                 response = {"error": "Создатель либы где-то проебался. Отпиши @AS7RID в тг, он починит"}
         self.__auto_delay_time = time.time()
-        print(time.time())
         try:
             return response.json()
         except requests.exceptions.JSONDecodeError:
             return response.text
 
     def __set_user_id(self):
         url = "https://api.lzt.market/me"
@@ -2529,24 +2528,25 @@
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
+
+                if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
+                    user_id = self.__token_user_id
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
-                if user_id is None:  # Tweak
-                    if type(self.__token_user_id) is not int:
-                        self.__token_user_id = self.__token_user_id()
-                    user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             # Copy of __List.favorite
             def favorite(self, page: int = None):
                 """
                 GET https://api.lzt.market/fave
@@ -2912,25 +2912,26 @@
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
+
+                if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
+                    user_id = self.__token_user_id
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
-                if user_id is None:  # Tweak
-                    if type(self.__token_user_id) is not int:
-                        self.__token_user_id = self.__token_user_id()
-                    user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/items"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def purchased(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
                           title: str = None):
                 """
                 GET https://api.lzt.market/user/user_id/orders
@@ -2994,24 +2995,25 @@
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
+
+                if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
+                    user_id = self.__token_user_id
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
-                if user_id is None:  # Tweak
-                    if type(self.__token_user_id) is not int:
-                        self.__token_user_id = self.__token_user_id()
-                    user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def favorite(self, page: int = None):
                 """
                 GET https://api.lzt.market/fave
 
@@ -3073,15 +3075,15 @@
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
         class __Payments:
             def __init__(self, api_self, token_user_id):
                 self.__api = api_self
                 self.__token_user_id = token_user_id
 
-            def history(self, user_id: int, operation_type: str = None, pmin: int = None, pmax: int = None,
+            def history(self, user_id: int = None, operation_type: str = None, pmin: int = None, pmax: int = None,
                         page: int = None,
                         operation_id_lt: int = None, receiver: str = None, sender: str = None, start_date: str = None,
                         end_date: str = None, wallet: str = None, comment: str = None, is_hold: bool = None,
                         show_payments_stats: bool = None):
                 """
                 GET https://api.lzt.market/user/user_id/payments
 
@@ -3112,14 +3114,18 @@
                         is_hold = 1
                     else:
                         is_hold = 0
                     if show_payments_stats:
                         show_payments_stats = 1
                     else:
                         show_payments_stats = 0
+                if user_id is None:  # Tweak
+                    if type(self.__token_user_id) is not int:
+                        self.__token_user_id = self.__token_user_id()
+                    user_id = self.__token_user_id
                 params = {
                     "user_id": user_id,
                     "operation_type": operation_type,
                     "pmin": pmin,
                     "pmax": pmax,
                     "page": page,
                     "operation_id_lt": operation_id_lt,
@@ -3128,18 +3134,14 @@
                     "start_date": start_date,
                     "end_date": end_date,
                     "wallet": wallet,
                     "comment": comment,
                     "is_hold": is_hold,
                     "show_payments_stats": show_payments_stats
                 }
-                if user_id is None:  # Tweak
-                    if type(self.__token_user_id) is not int:
-                        self.__token_user_id = self.__token_user_id()
-                    user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/payments"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def transfer(self, amount: int, secret_answer: str, currency: str = "rub", user_id: int = None,
                          username: str = None, comment: str = None, transfer_hold: bool = None,
                          hold_length_option: str = None,
                          hold_length_value: int = None):
@@ -3166,20 +3168,57 @@
                 params = {
                     "amount": amount,
                     "secret_answer": secret_answer,
                     "user_id": user_id,
                     "username": username,
                     "currency": currency,
                     "comment": comment,
-                    "transfer_hold": transfer_hold,
+                    "hold": transfer_hold,
                     "hold_length_value": hold_length_value,
                     "hold_length_option": hold_length_option
                 }
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
+            @staticmethod
+            def generate_link(amount: int, user_id: int = None, username: str = None, comment: str = None,
+                              redirect_url: str = None, currency: str = None,hold:bool=None):
+                """
+                Generate payment link
+
+                Required scopes: None
+
+                :param amount: Amount to send in your currency.
+                :param user_id: ID of user to transfer money
+                :param username: Username to transfer money
+                :param comment: Payment comment.
+                :param redirect_url: Redirect url. User who paid on this link will be redirected to this url
+                :param currency: Using currency for amount. Allowed values: cny, usd, rub, eur, uah, kzt, byn, gbp
+                :param hold: Hold transfer or not
+
+                :return: string payment url
+                """
+                if True:  # Костыль, пока не пофиксят недочет #43
+                    if hold:
+                        hold = 1
+                    else:
+                        hold = 0
+                params = {
+                    "user_id": user_id,
+                    "username": username,
+                    "amount": amount,
+                    "comment": comment,
+                    "redirect": redirect_url,
+                    "currency": currency,
+                    "hold":hold
+                }
+                url = "https://lzt.market/balance/transfer"
+                req = requests.models.PreparedRequest()
+                req.prepare_url(url=url, params=params)
+                return req.url
+
         class __Managing:
             def __init__(self, api_self):
                 self.__api = api_self
                 self.tag = self.__Tag(self.__api)
 
             class __Tag:  # To Managing
                 def __init__(self, api_self):
```

### Comparing `LolzteamApi-1.0.17/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.18/LolzteamApi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.17
+Version: 1.0.18
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Lolzteam Python API
 
 <p align="center">
-    <a href="https://zelenka.guru/members/2410024"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
+    <a href="https://zelenka.guru/threads/5523020/"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
 
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE)
 
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.17 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.18 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.17/PKG-INFO` & `LolzteamApi-1.0.18/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.17
+Version: 1.0.18
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Lolzteam Python API
 
 <p align="center">
-    <a href="https://zelenka.guru/members/2410024"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
+    <a href="https://zelenka.guru/threads/5523020/"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
 
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE)
 
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.17 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.18 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.17/README.md` & `LolzteamApi-1.0.18/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # Lolzteam Python API
 
 <p align="center">
-    <a href="https://zelenka.guru/members/2410024"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
+    <a href="https://zelenka.guru/threads/5523020/"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
 
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE)
 
 
 ## Installation
```

### Comparing `LolzteamApi-1.0.17/setup.py` & `LolzteamApi-1.0.18/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests", "beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.17",
+    version="1.0.18",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
```

