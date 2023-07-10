# Comparing `tmp/iitkgp_erp_login-1.0.0.tar.gz` & `tmp/iitkgp_erp_login-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp_erp_login-1.0.0.tar", last modified: Mon Jul 10 14:53:07 2023, max compression
+gzip compressed data, was "iitkgp_erp_login-1.0.1.tar", last modified: Mon Jul 10 21:19:19 2023, max compression
```

## Comparing `iitkgp_erp_login-1.0.0.tar` & `iitkgp_erp_login-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 14:53:07.427153 iitkgp_erp_login-1.0.0/
--rw-r--r--   0 proffapt   (501) staff       (20)     1074 2023-07-09 19:05:06.000000 iitkgp_erp_login-1.0.0/LICENSE
--rw-r--r--   0 proffapt   (501) staff       (20)    11995 2023-07-10 14:53:07.426543 iitkgp_erp_login-1.0.0/PKG-INFO
--rw-r--r--   0 proffapt   (501) staff       (20)    11437 2023-07-10 14:52:05.000000 iitkgp_erp_login-1.0.0/README.md
--rw-r--r--   0 proffapt   (501) staff       (20)      773 2023-07-10 14:53:02.000000 iitkgp_erp_login-1.0.0/pyproject.toml
--rw-r--r--   0 proffapt   (501) staff       (20)       38 2023-07-10 14:53:07.427239 iitkgp_erp_login-1.0.0/setup.cfg
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 14:53:07.423674 iitkgp_erp_login-1.0.0/src/
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 14:53:07.425070 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login/
--rw-r--r--   0 proffapt   (501) staff       (20)        0 2023-07-09 19:54:19.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login/__init__.py
--rw-r--r--   0 proffapt   (501) staff       (20)      403 2023-07-09 21:13:18.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login/endpoints.py
--rw-r--r--   0 proffapt   (501) staff       (20)     2613 2023-07-09 21:13:45.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login/erp.py
--rw-r--r--   0 proffapt   (501) staff       (20)     2373 2023-07-09 21:37:06.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login/read_mail.py
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 14:53:07.426091 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login.egg-info/
--rw-r--r--   0 proffapt   (501) staff       (20)    11995 2023-07-10 14:53:07.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login.egg-info/PKG-INFO
--rw-r--r--   0 proffapt   (501) staff       (20)      394 2023-07-10 14:53:07.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login.egg-info/SOURCES.txt
--rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-10 14:53:07.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login.egg-info/dependency_links.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       92 2023-07-10 14:53:07.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login.egg-info/requires.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       17 2023-07-10 14:53:07.000000 iitkgp_erp_login-1.0.0/src/iitkgp_erp_login.egg-info/top_level.txt
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 14:53:07.426271 iitkgp_erp_login-1.0.0/tests/
--rw-r--r--   0 proffapt   (501) staff       (20)      459 2023-07-09 20:54:15.000000 iitkgp_erp_login-1.0.0/tests/test.py
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.992432 iitkgp_erp_login-1.0.1/
+-rw-r--r--   0 proffapt   (501) staff       (20)     1074 2023-07-09 19:05:06.000000 iitkgp_erp_login-1.0.1/LICENSE
+-rw-r--r--   0 proffapt   (501) staff       (20)    13061 2023-07-10 21:19:19.992189 iitkgp_erp_login-1.0.1/PKG-INFO
+-rw-r--r--   0 proffapt   (501) staff       (20)    12503 2023-07-10 21:18:56.000000 iitkgp_erp_login-1.0.1/README.md
+-rw-r--r--   0 proffapt   (501) staff       (20)      773 2023-07-10 21:19:15.000000 iitkgp_erp_login-1.0.1/pyproject.toml
+-rw-r--r--   0 proffapt   (501) staff       (20)       38 2023-07-10 21:19:19.992509 iitkgp_erp_login-1.0.1/setup.cfg
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.987967 iitkgp_erp_login-1.0.1/src/
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.990158 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/
+-rw-r--r--   0 proffapt   (501) staff       (20)        0 2023-07-09 19:54:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/__init__.py
+-rw-r--r--   0 proffapt   (501) staff       (20)      403 2023-07-09 21:13:18.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/endpoints.py
+-rw-r--r--   0 proffapt   (501) staff       (20)     2613 2023-07-09 21:13:45.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/erp.py
+-rw-r--r--   0 proffapt   (501) staff       (20)     2373 2023-07-09 21:37:06.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/read_mail.py
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.991390 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/
+-rw-r--r--   0 proffapt   (501) staff       (20)    13061 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO
+-rw-r--r--   0 proffapt   (501) staff       (20)      394 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/SOURCES.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/dependency_links.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)       92 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/requires.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)       17 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/top_level.txt
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.991578 iitkgp_erp_login-1.0.1/tests/
+-rw-r--r--   0 proffapt   (501) staff       (20)      459 2023-07-09 20:54:15.000000 iitkgp_erp_login-1.0.1/tests/test.py
```

### Comparing `iitkgp_erp_login-1.0.0/LICENSE` & `iitkgp_erp_login-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-1.0.0/PKG-INFO` & `iitkgp_erp_login-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp_erp_login
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,30 +49,30 @@
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
    └── read_mail.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains implementation of `getOTP(OTP_WAIT_INTERVAL)` function along with various helper functions for it. These functions are not intended to be used by _you_ - the user - as the only case, where, OTP will be required is during the login process which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script be an abstraction for general user. Obviously, if you want to tweak the OTP fetching process feel free to have a look at the script [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py).
+[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
-[endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) contains all the required endpoints for the ERP login workflow.
+The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
 <div id="endpoints-about"></div>
 
 #### About
 - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage.
 - `SECRET_QUESTION_URL`: The URL for retrieving the secret question for authentication.
 - `OTP_URL`: The URL for requesting the OTP (One-Time Password) for authentication.
 - `LOGIN_URL`: The URL for ERP login.
-- `WELCOMEPAGE_URL`: The URL of the welcome page, which is only accessible when the user is **NOT** logged-in and behaves exactly as `HOMEPAGE_URL` but when logged-in returns `404` error.
+- `WELCOMEPAGE_URL`: The URL of the welcome page, which is accessible only when the user is **NOT** logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user is logged in, it returns a `404` error.
 
 <div id="endpoints-usage"></div>
 
 #### Usage
 ```python
 from iitkgp_erp_login.endpoints import *
 
@@ -83,75 +83,74 @@
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
 <div id="usage-in-login-workflow"></div>
 
 #### Usage in login workflow
 
-To automate login into ERP, the endpoints are hit in the following order:
+To automate the login process into ERP, the endpoints are hit in the following order:
 
-1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step is necessary to establish the initial session and retrieve `sessionToken`.
+1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step establishes the initial session and retrieves `sessionToken`.
 2. Hit `SECRET_QUESTION_URL` using `session.post(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER}, headers=headers)`. This step fetches the secret question required for authentication.
 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee': 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests an OTP (One-Time Password) for authentication.
 4. Finally, hit `LOGIN_URL` using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step performs the actual ERP login with the provided login details and OTP.
 
 > **Note**  `session` = [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) is used to persist the session parameters throughout the workflow
 
 <div id="login"></div>
 
 ### Login
 
-ERP Login workflow is implemented in : `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` inside [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py).<br>
-The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
 The function requires following arguments:
-1. `headers`: Headers for the post requests.
+1. `headers`: Headers for the post requests. An example is given below.
     ```python
     headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
     }
     ``` 
-2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported.
+2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported into python file.
     ```python
     import erpcreds
     ```
-3.  `OTP_WAIT_INTERVAL`: Interval after which api checks continuously for new OTP mail.
-4.  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+3.  `OTP_WAIT_INTERVAL`: The interval after which the API continuously checks for new OTP mail.
+4.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
     ```python
     import requests
 
     session = requests.Session()
     ```
 
 <div id="login-output"></div>
 
 #### Output
-1. The function returns:
-   - [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
-   - [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
-2. It also modifies the `session` object which now contains parameters for the logged in session, which can be used for further navigation in ERP.
-3. Has exhastive loggin inbuilt. It prints the status of each step.
+1. The function returns the following in the order of occurrence as here (`sessionToken, ssoToekn`):
+   1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
+   2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
+2. It also modifies the `session` object, which now includes parameters for the logged-in session. These parameters can be utilized for further navigation within the ERP system.
+3. It incorporates **comprehensive logging**. It prints the status of each step, providing detailed information throughout the process.
 
 <div id="login-usage"></div>
 
 #### Usage
-It is recommended to use the login function as shown below:
+It is recommended to use the `login` function in the following manner:
 ```python
 # importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # using the login function inside erp.py
 sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
 ```
 
-Combining everything we looked about the `login` function till now:
+Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
 import iitkgp_erp_login.erp as erp
 
 headers = {
@@ -162,19 +161,20 @@
 session = requests.Session()
 
 sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
    
 print(sessionToken, ssoToken)
 ```
 
+> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+
 <div id="session-alive"></div>
 
 ### Session status check
-The logic for status check of session is implemented in `session_alive(session)`. It tells whether the given session is valid/alive or not.<br>
-The input and output specifications for the function are mentioned below.
+The logic for checking the status of the session is implemented in the `session_alive(session)` function  n [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
 The function requires following argument:
 
  -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
@@ -182,29 +182,30 @@
     import requests
 
     session = requests.Session()
      ```
 <div id="session-alive-output"></div>
 
 #### Output
-Returns the status of session in boolean. __True if alive and False if not__.
+The `session_alive(session)` function returns the status of the session as a boolean value: **True** if it is alive and **False** if it is not.
 
 <div id="session-alive-usage"></div>
 
 #### Usage
-It is recommended to use the session_alive function as shown below:
+It is recommended to use the `session_alive` function in the following manner:
 ```python
-# importing the erp.py file
+# Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
-# using the session_alive function inside erp.py
+# Using the session_alive function inside erp.py
 print(erp.session_alive(session))
 ```
 
-Combining everything we looked about the `session_alive` and `login` functions till now:
+Here's an example combining all the aspects we have discussed so far about the `login` function and `session_alive` function:
+
 ```python
 import requests
 import time
 import creds
 import iitkgp_erp_login.erp as erp
 
 headers = {
@@ -219,38 +220,40 @@
         erp.login(headers, creds, 2, session)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
+> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+
 <div id="package-usage"></div>
 
 ## Usage
 
 <div id="prerequisites"></div>
 
 ### Prerequisites
-Following scripts are required, and **MUST** be present in the same directory as that of the script in which `iitkgp_erp_login` (yes, this module) is being imported.
+
+The following scripts are required and **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported:
 
 - <a href="#erpcreds">erpcreds.py</a>
 - <a href="#token">token.json</a>
 
 <div id="erpcreds"></div>
 
 #### ERP credentials file
 
 <div id="erpcreds-creating"></div>
 
 ##### Creating
 
-Create a `.py` file with your ERP credentials stored in it.<br>
-Following are the instructions for creating this file:
-- Name of the file can be any valid python file's name
-- **Variable names must not be changed**, copy the below format and **ONLY update values** inside `"` - _double quotes_.
+Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
+- You can choose any valid name for the file, adhering to Python's naming conventions.
+- **Do not change the variable names**. Simply copy the format provided below and update the values inside the `double quotes` (").
   ```python
   # ERP Credentials
   ROLL_NUMBER = "XXYYXXXXX"
   PASSWORD = "**********"
   SECURITY_QUESTIONS_ANSWERS = {
       "Q1" : "A1",
       "Q2" : "A2",
@@ -258,66 +261,67 @@
   }
   ```
 
 <div id="erpcreds-using"></div>
 
 ##### Using
 
-Let's suppose you saved the erp creds file as `erpcreds.py`. Then in order to use it you will just have to import it:
+Let's suppose you have saved the ERP credentials file as `erpcreds.py`. To use it, you can simply import it in your Python script using the following code:
+
 ```python
 import erpcreds
 
 print(erpcreds.ROLL_NUMBER)
 # Output: XXYYXXXXX
 
 print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"])
 # Output: A2
 ```
 
 <div id="token"></div>
 
 #### Generating token for GMail enabled googleapi
 
-1. Follow the steps at [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to get `credentials.json`.
-   > **Note** `credentials.json` is permanent until you delete it in your google clound console.
+1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
+   > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
 
-2. Follow the steps below to generate `token.json`:
-    - Download [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) in the same folder containing `credentials.json`
-    - Import the required module
+2. To generate the `token.json` file, follow the steps below:
+    - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
+    - Import the required module, `google-auth-oauthlib`
       
       ```bash
       pip install google-auth-oauthlib
       ```
-    - Execute `gentokenjson.py` with `readonly` argument
+    - Execute `gentokenjson.py` with the `readonly` argument
    
       ```bash
       python3 gentokenjson.py readonly
       ```
-    - Browser window will open and ask you to select the account, choose the one receiving OTP for login
-    - Allow permission on that email to use just enabled __GMAIL API__
+    - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
+    - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
        - Click on `Continue` instead of __Back To Safety__
-       - Then press `Continue` again
-    - `token.json` will be generated in same folder as that of `credentials.json`
+       - Then, press `Continue` again
+    - The `token.json` file will be generated in the same folder as the `credentials.json` file
   
-    > **Warning** `token.json` expires after sometime. So make sure to check that in your projects and keep refreshing it.
+    > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
 
 <div id="example"></div>
 
 ### Example
 
-Now, we will create a script which will open ERP on your default browser with a logged in session.
+Now, we will create a script that opens the ERP system on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
    pip install iitkgp_erp_login
    ````
-2. Make sure <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> exist in the same directory as that of the script we are about to create.
+2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
 
-3. Create `open_erp.py` and append the following content into it.
+3. Create a file named `open_erp.py` and include the following code:
 
    ```python
    import requests
    import webbrowser
    import erpcreds
    import iitkgp_erp_login.erp as erp
    from iitkgp_erp_login.endpoints import HOMEPAGE_URL
@@ -330,11 +334,11 @@
    session = requests.Session()
 
    _, ssoToken = erp.login(headers, erpcreds, 2, session)
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
-4. Run the script
+4. Run the script.
    ```bash
    python3 open_erp.py
    ```
```

#### html2text {}

```diff
@@ -1,142 +1,153 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 1.0.0 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 1.0.1 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module A python package/module to automate login process in
 ERP for IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage -
 Usage_in_login_workflow - Login - Input - Output - Usage - Session_status_check
 - Input - Output - Usage - Usage - Prerequisites - ERP_credentials_file -
 Creating - Using - Generating_token_for_GMail_enabled_googleapi - Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
 erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains
-implementation of `getOTP(OTP_WAIT_INTERVAL)` function along with various
-helper functions for it. These functions are not intended to be used by _you_ -
-the user - as the only case, where, OTP will be required is during the login
-process which is handled by functions in [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this
-script be an abstraction for general user. Obviously, if you want to tweak the
-OTP fetching process feel free to have a look at the script [read_mail.py]
-(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
-iitkgp_erp_login/read_mail.py).
-### Endpoints [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/
-blob/main/src/iitkgp_erp_login/endpoints.py) contains all the required
-endpoints for the ERP login workflow.
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
+implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various
+helper functions. These functions are not intended to be used by _you_, the
+user. The only case where OTP is required is during the login process, which is
+handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
+pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
+abstraction for general users. If you want to modify the OTP fetching process,
+feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
+erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
+pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
+necessary endpoints for the ERP login workflow.
 #### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
-The URL of the welcome page, which is only accessible when the user is **NOT**
-logged-in and behaves exactly as `HOMEPAGE_URL` but when logged-in returns
-`404` error.
+The URL of the welcome page, which is accessible only when the user is **NOT**
+logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
+is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
-#### Usage in login workflow To automate login into ERP, the endpoints are hit
-in the following order: 1. Hit `HOMEPAGE_URL` using `session.get
-(HOMEPAGE_URL)`. This step is necessary to establish the initial session and
-retrieve `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
+#### Usage in login workflow To automate the login process into ERP, the
+endpoints are hit in the following order: 1. Hit `HOMEPAGE_URL` using
+`session.get(HOMEPAGE_URL)`. This step establishes the initial session and
+retrieves `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
 (SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER},
 headers=headers)`. This step fetches the secret question required for
 authentication. 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee':
 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests
 an OTP (One-Time Password) for authentication. 4. Finally, hit `LOGIN_URL`
 using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step
 performs the actual ERP login with the provided login details and OTP. >
 **Note** `session` = [requests.Session()](https://docs.python-requests.org/en/
 latest/_modules/requests/sessions/) is used to persist the session parameters
 throughout the workflow
-### Login ERP Login workflow is implemented in : `login(headers, erp_creds,
-OTP_WAIT_INTERVAL, session)` inside [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py).
-The input and output specifications for the function are mentioned below.
+### Login ERP login workflow is implemented in `login(headers, erp_creds,
+OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
+output specifications for the function are mentioned below.
 #### Input The function requires following arguments: 1. `headers`: Headers for
-the post requests. ```python headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } ``` 2. `erp_creds`:
-ERP_Login_Credentials_file, which is imported. ```python import erpcreds ``` 3.
-`OTP_WAIT_INTERVAL`: Interval after which api checks continuously for new OTP
-mail. 4. `session`: [requests.Session()](https://docs.python-requests.org/en/
-latest/_modules/requests/sessions/) object, to persist the session parameters
-throughout the workflow. ```python import requests session = requests.Session()
-```
-#### Output 1. The function returns: - [sessionToken](https://en.wikipedia.org/
-wiki/Session_ID) - [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
-It also modifies the `session` object which now contains parameters for the
-logged in session, which can be used for further navigation in ERP. 3. Has
-exhastive loggin inbuilt. It prints the status of each step.
-#### Usage It is recommended to use the login function as shown below:
-```python # importing the erp.py file import iitkgp_erp_login.erp as erp #
-using the login function inside erp.py sessionToken, ssoToken = erp.login
-(headers, erpcreds, 2, session) ``` Combining everything we looked about the
-`login` function till now: ```python import requests import erpcreds import
-iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
-requests.Session() sessionToken, ssoToken = erp.login(headers, erpcreds, 2,
-session) print(sessionToken, ssoToken) ```
-### Session status check The logic for status check of session is implemented
-in `session_alive(session)`. It tells whether the given session is valid/alive
-or not.
-The input and output specifications for the function are mentioned below.
+the post requests. An example is given below. ```python headers = { 'timeout':
+'20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
+like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+``` 2. `erp_creds`: ERP_Login_Credentials_file, which is imported into python
+file. ```python import erpcreds ``` 3. `OTP_WAIT_INTERVAL`: The interval after
+which the API continuously checks for new OTP mail. 4. `session`: A
+[requests.Session()](https://docs.python-requests.org/en/latest/_modules/
+requests/sessions/) object, to persist the session parameters throughout the
+workflow. ```python import requests session = requests.Session() ```
+#### Output 1. The function returns the following in the order of occurrence as
+here (`sessionToken, ssoToekn`): 1. [sessionToken](https://en.wikipedia.org/
+wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
+It also modifies the `session` object, which now includes parameters for the
+logged-in session. These parameters can be utilized for further navigation
+within the ERP system. 3. It incorporates **comprehensive logging**. It prints
+the status of each step, providing detailed information throughout the process.
+#### Usage It is recommended to use the `login` function in the following
+manner: ```python # importing the erp.py file import iitkgp_erp_login.erp as
+erp # using the login function inside erp.py sessionToken, ssoToken = erp.login
+(headers, erpcreds, 2, session) ``` Here's an example combining all the aspects
+we have discussed so far about the `login` function: ```python import requests
+import erpcreds import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
+'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
+Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+session = requests.Session() sessionToken, ssoToken = erp.login(headers,
+erpcreds, 2, session) print(sessionToken, ssoToken) ``` > **Note** The code
+snippet above will not work unless the prerequisites are fulfilled
+### Session status check The logic for checking the status of the session is
+implemented in the `session_alive(session)` function n [erp.py](https://
+github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+erp.py). This function determines whether the given session is valid/alive or
+not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
 requests/sessions/) object, to persist the session parameters throughout the
 workflow. ```python import requests session = requests.Session() ```
-#### Output Returns the status of session in boolean. __True if alive and False
-if not__.
-#### Usage It is recommended to use the session_alive function as shown below:
-```python # importing the erp.py file import iitkgp_erp_login.erp as erp #
-using the session_alive function inside erp.py print(erp.session_alive
-(session)) ``` Combining everything we looked about the `session_alive` and
-`login` functions till now: ```python import requests import time import creds
-import iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
+#### Output The `session_alive(session)` function returns the status of the
+session as a boolean value: **True** if it is alive and **False** if it is not.
+#### Usage It is recommended to use the `session_alive` function in the
+following manner: ```python # Importing the erp.py file import
+iitkgp_erp_login.erp as erp # Using the session_alive function inside erp.py
+print(erp.session_alive(session)) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function and `session_alive`
+function: ```python import requests import time import creds import
+iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
 Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
 requests.Session() while True: if not erp.session_alive(session): erp.login
 (headers, creds, 2, session) else: print("Session is alive.") time.sleep(2) ```
+> **Note** The code snippet above will not work unless the prerequisites are
+fulfilled
 ## Usage
-### Prerequisites Following scripts are required, and **MUST** be present in
-the same directory as that of the script in which `iitkgp_erp_login` (yes, this
-module) is being imported. - erpcreds.py - token.json
+### Prerequisites The following scripts are required and **MUST** be present in
+the same directory as the script where `iitkgp_erp_login` module is being
+imported: - erpcreds.py - token.json
 #### ERP credentials file
 ##### Creating Create a `.py` file with your ERP credentials stored in it.
-Following are the instructions for creating this file: - Name of the file can
-be any valid python file's name - **Variable names must not be changed**, copy
-the below format and **ONLY update values** inside `"` - _double quotes_.
-```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********"
-SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
-##### Using Let's suppose you saved the erp creds file as `erpcreds.py`. Then
-in order to use it you will just have to import it: ```python import erpcreds
-print(erpcreds.ROLL_NUMBER) # Output: XXYYXXXXX print
-(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2 ```
-#### Generating token for GMail enabled googleapi 1. Follow the steps at [Gmail
-API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
-python) guide to get `credentials.json`. > **Note** `credentials.json` is
-permanent until you delete it in your google clound console. 2. Follow the
-steps below to generate `token.json`: - Download [gentokenjson.py](https://
-gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) in the same folder
-containing `credentials.json` - Import the required module ```bash pip install
-google-auth-oauthlib ``` - Execute `gentokenjson.py` with `readonly` argument
-```bash python3 gentokenjson.py readonly ``` - Browser window will open and ask
-you to select the account, choose the one receiving OTP for login - Allow
-permission on that email to use just enabled __GMAIL API__ - Click on
-`Continue` instead of __Back To Safety__ - Then press `Continue` again -
-`token.json` will be generated in same folder as that of `credentials.json` >
-**Warning** `token.json` expires after sometime. So make sure to check that in
-your projects and keep refreshing it.
-### Example Now, we will create a script which will open ERP on your default
-browser with a logged in session. 1. Install the package. ```bash pip install
-iitkgp_erp_login ```` 2. Make sure erpcreds.py & token.json exist in the same
-directory as that of the script we are about to create. 3. Create `open_erp.py`
-and append the following content into it. ```python import requests import
-webbrowser import erpcreds import iitkgp_erp_login.erp as erp from
-iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout': '20',
-'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
-Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+Please follow the instructions below to create this file: - You can choose any
+valid name for the file, adhering to Python's naming conventions. - **Do not
+change the variable names**. Simply copy the format provided below and update
+the values inside the `double quotes` ("). ```python # ERP Credentials
+ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********" SECURITY_QUESTIONS_ANSWERS =
+{ "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
+##### Using Let's suppose you have saved the ERP credentials file as
+`erpcreds.py`. To use it, you can simply import it in your Python script using
+the following code: ```python import erpcreds print(erpcreds.ROLL_NUMBER) #
+Output: XXYYXXXXX print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2
+```
+#### Generating token for GMail enabled googleapi 1. Follow the steps in the
+[Gmail API - Python Quickstart](https://developers.google.com/gmail/api/
+quickstart/python) guide to obtain `credentials.json` file. > **Note** The
+`credentials.json` file is permanent unless you manually delete its reference
+in your Google Cloud Console. 2. To generate the `token.json` file, follow the
+steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
+adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
+contains the `credentials.json` file - Import the required module, `google-
+auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
+`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
+readonly ``` - A browser window will open, prompting you to select the Google
+account associated with receiving OTP for login. - Grant permission to the
+selected email address to utilize the newly enabled **Gmail API**. - Click on
+`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
+`token.json` file will be generated in the same folder as the
+`credentials.json` file > **Warning** The `token.json` file has an expiration
+time, so it's important to periodically check and refresh it in your projects
+to ensure uninterrupted access.
+### Example Now, we will create a script that opens the ERP system on your
+default browser with a logged-in session. 1. Install the package. ```bash pip
+install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
+exist in the same directory as the script we are about to create. 3. Create a
+file named `open_erp.py` and include the following code: ```python import
+requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
+from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
+'20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
+like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 session = requests.Session() _, ssoToken = erp.login(headers, erpcreds, 2,
 session) logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open
-(logged_in_url) ``` 4. Run the script ```bash python3 open_erp.py ```
+(logged_in_url) ``` 4. Run the script. ```bash python3 open_erp.py ```
```

### Comparing `iitkgp_erp_login-1.0.0/README.md` & `iitkgp_erp_login-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
    └── read_mail.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains implementation of `getOTP(OTP_WAIT_INTERVAL)` function along with various helper functions for it. These functions are not intended to be used by _you_ - the user - as the only case, where, OTP will be required is during the login process which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script be an abstraction for general user. Obviously, if you want to tweak the OTP fetching process feel free to have a look at the script [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py).
+[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
-[endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) contains all the required endpoints for the ERP login workflow.
+The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
 <div id="endpoints-about"></div>
 
 #### About
 - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage.
 - `SECRET_QUESTION_URL`: The URL for retrieving the secret question for authentication.
 - `OTP_URL`: The URL for requesting the OTP (One-Time Password) for authentication.
 - `LOGIN_URL`: The URL for ERP login.
-- `WELCOMEPAGE_URL`: The URL of the welcome page, which is only accessible when the user is **NOT** logged-in and behaves exactly as `HOMEPAGE_URL` but when logged-in returns `404` error.
+- `WELCOMEPAGE_URL`: The URL of the welcome page, which is accessible only when the user is **NOT** logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user is logged in, it returns a `404` error.
 
 <div id="endpoints-usage"></div>
 
 #### Usage
 ```python
 from iitkgp_erp_login.endpoints import *
 
@@ -69,75 +69,74 @@
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
 <div id="usage-in-login-workflow"></div>
 
 #### Usage in login workflow
 
-To automate login into ERP, the endpoints are hit in the following order:
+To automate the login process into ERP, the endpoints are hit in the following order:
 
-1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step is necessary to establish the initial session and retrieve `sessionToken`.
+1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step establishes the initial session and retrieves `sessionToken`.
 2. Hit `SECRET_QUESTION_URL` using `session.post(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER}, headers=headers)`. This step fetches the secret question required for authentication.
 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee': 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests an OTP (One-Time Password) for authentication.
 4. Finally, hit `LOGIN_URL` using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step performs the actual ERP login with the provided login details and OTP.
 
 > **Note**  `session` = [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) is used to persist the session parameters throughout the workflow
 
 <div id="login"></div>
 
 ### Login
 
-ERP Login workflow is implemented in : `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` inside [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py).<br>
-The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
 The function requires following arguments:
-1. `headers`: Headers for the post requests.
+1. `headers`: Headers for the post requests. An example is given below.
     ```python
     headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
     }
     ``` 
-2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported.
+2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported into python file.
     ```python
     import erpcreds
     ```
-3.  `OTP_WAIT_INTERVAL`: Interval after which api checks continuously for new OTP mail.
-4.  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+3.  `OTP_WAIT_INTERVAL`: The interval after which the API continuously checks for new OTP mail.
+4.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
     ```python
     import requests
 
     session = requests.Session()
     ```
 
 <div id="login-output"></div>
 
 #### Output
-1. The function returns:
-   - [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
-   - [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
-2. It also modifies the `session` object which now contains parameters for the logged in session, which can be used for further navigation in ERP.
-3. Has exhastive loggin inbuilt. It prints the status of each step.
+1. The function returns the following in the order of occurrence as here (`sessionToken, ssoToekn`):
+   1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
+   2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
+2. It also modifies the `session` object, which now includes parameters for the logged-in session. These parameters can be utilized for further navigation within the ERP system.
+3. It incorporates **comprehensive logging**. It prints the status of each step, providing detailed information throughout the process.
 
 <div id="login-usage"></div>
 
 #### Usage
-It is recommended to use the login function as shown below:
+It is recommended to use the `login` function in the following manner:
 ```python
 # importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # using the login function inside erp.py
 sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
 ```
 
-Combining everything we looked about the `login` function till now:
+Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
 import iitkgp_erp_login.erp as erp
 
 headers = {
@@ -148,19 +147,20 @@
 session = requests.Session()
 
 sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
    
 print(sessionToken, ssoToken)
 ```
 
+> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+
 <div id="session-alive"></div>
 
 ### Session status check
-The logic for status check of session is implemented in `session_alive(session)`. It tells whether the given session is valid/alive or not.<br>
-The input and output specifications for the function are mentioned below.
+The logic for checking the status of the session is implemented in the `session_alive(session)` function  n [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
 The function requires following argument:
 
  -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
@@ -168,29 +168,30 @@
     import requests
 
     session = requests.Session()
      ```
 <div id="session-alive-output"></div>
 
 #### Output
-Returns the status of session in boolean. __True if alive and False if not__.
+The `session_alive(session)` function returns the status of the session as a boolean value: **True** if it is alive and **False** if it is not.
 
 <div id="session-alive-usage"></div>
 
 #### Usage
-It is recommended to use the session_alive function as shown below:
+It is recommended to use the `session_alive` function in the following manner:
 ```python
-# importing the erp.py file
+# Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
-# using the session_alive function inside erp.py
+# Using the session_alive function inside erp.py
 print(erp.session_alive(session))
 ```
 
-Combining everything we looked about the `session_alive` and `login` functions till now:
+Here's an example combining all the aspects we have discussed so far about the `login` function and `session_alive` function:
+
 ```python
 import requests
 import time
 import creds
 import iitkgp_erp_login.erp as erp
 
 headers = {
@@ -205,38 +206,40 @@
         erp.login(headers, creds, 2, session)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
+> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+
 <div id="package-usage"></div>
 
 ## Usage
 
 <div id="prerequisites"></div>
 
 ### Prerequisites
-Following scripts are required, and **MUST** be present in the same directory as that of the script in which `iitkgp_erp_login` (yes, this module) is being imported.
+
+The following scripts are required and **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported:
 
 - <a href="#erpcreds">erpcreds.py</a>
 - <a href="#token">token.json</a>
 
 <div id="erpcreds"></div>
 
 #### ERP credentials file
 
 <div id="erpcreds-creating"></div>
 
 ##### Creating
 
-Create a `.py` file with your ERP credentials stored in it.<br>
-Following are the instructions for creating this file:
-- Name of the file can be any valid python file's name
-- **Variable names must not be changed**, copy the below format and **ONLY update values** inside `"` - _double quotes_.
+Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
+- You can choose any valid name for the file, adhering to Python's naming conventions.
+- **Do not change the variable names**. Simply copy the format provided below and update the values inside the `double quotes` (").
   ```python
   # ERP Credentials
   ROLL_NUMBER = "XXYYXXXXX"
   PASSWORD = "**********"
   SECURITY_QUESTIONS_ANSWERS = {
       "Q1" : "A1",
       "Q2" : "A2",
@@ -244,66 +247,67 @@
   }
   ```
 
 <div id="erpcreds-using"></div>
 
 ##### Using
 
-Let's suppose you saved the erp creds file as `erpcreds.py`. Then in order to use it you will just have to import it:
+Let's suppose you have saved the ERP credentials file as `erpcreds.py`. To use it, you can simply import it in your Python script using the following code:
+
 ```python
 import erpcreds
 
 print(erpcreds.ROLL_NUMBER)
 # Output: XXYYXXXXX
 
 print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"])
 # Output: A2
 ```
 
 <div id="token"></div>
 
 #### Generating token for GMail enabled googleapi
 
-1. Follow the steps at [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to get `credentials.json`.
-   > **Note** `credentials.json` is permanent until you delete it in your google clound console.
+1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
+   > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
 
-2. Follow the steps below to generate `token.json`:
-    - Download [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) in the same folder containing `credentials.json`
-    - Import the required module
+2. To generate the `token.json` file, follow the steps below:
+    - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
+    - Import the required module, `google-auth-oauthlib`
       
       ```bash
       pip install google-auth-oauthlib
       ```
-    - Execute `gentokenjson.py` with `readonly` argument
+    - Execute `gentokenjson.py` with the `readonly` argument
    
       ```bash
       python3 gentokenjson.py readonly
       ```
-    - Browser window will open and ask you to select the account, choose the one receiving OTP for login
-    - Allow permission on that email to use just enabled __GMAIL API__
+    - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
+    - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
        - Click on `Continue` instead of __Back To Safety__
-       - Then press `Continue` again
-    - `token.json` will be generated in same folder as that of `credentials.json`
+       - Then, press `Continue` again
+    - The `token.json` file will be generated in the same folder as the `credentials.json` file
   
-    > **Warning** `token.json` expires after sometime. So make sure to check that in your projects and keep refreshing it.
+    > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
 
 <div id="example"></div>
 
 ### Example
 
-Now, we will create a script which will open ERP on your default browser with a logged in session.
+Now, we will create a script that opens the ERP system on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
    pip install iitkgp_erp_login
    ````
-2. Make sure <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> exist in the same directory as that of the script we are about to create.
+2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
 
-3. Create `open_erp.py` and append the following content into it.
+3. Create a file named `open_erp.py` and include the following code:
 
    ```python
    import requests
    import webbrowser
    import erpcreds
    import iitkgp_erp_login.erp as erp
    from iitkgp_erp_login.endpoints import HOMEPAGE_URL
@@ -316,11 +320,11 @@
    session = requests.Session()
 
    _, ssoToken = erp.login(headers, erpcreds, 2, session)
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
-4. Run the script
+4. Run the script.
    ```bash
    python3 open_erp.py
    ```
```

#### html2text {}

```diff
@@ -1,135 +1,146 @@
 # ERP Login Module A python package/module to automate login process in ERP for
 IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage - Usage
 in_login_workflow - Login - Input - Output - Usage - Session_status_check -
 Input - Output - Usage - Usage - Prerequisites - ERP_credentials_file -
 Creating - Using - Generating_token_for_GMail_enabled_googleapi - Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
 erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains
-implementation of `getOTP(OTP_WAIT_INTERVAL)` function along with various
-helper functions for it. These functions are not intended to be used by _you_ -
-the user - as the only case, where, OTP will be required is during the login
-process which is handled by functions in [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this
-script be an abstraction for general user. Obviously, if you want to tweak the
-OTP fetching process feel free to have a look at the script [read_mail.py]
-(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
-iitkgp_erp_login/read_mail.py).
-### Endpoints [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/
-blob/main/src/iitkgp_erp_login/endpoints.py) contains all the required
-endpoints for the ERP login workflow.
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
+implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various
+helper functions. These functions are not intended to be used by _you_, the
+user. The only case where OTP is required is during the login process, which is
+handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
+pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
+abstraction for general users. If you want to modify the OTP fetching process,
+feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
+erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
+pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
+necessary endpoints for the ERP login workflow.
 #### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
-The URL of the welcome page, which is only accessible when the user is **NOT**
-logged-in and behaves exactly as `HOMEPAGE_URL` but when logged-in returns
-`404` error.
+The URL of the welcome page, which is accessible only when the user is **NOT**
+logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
+is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
-#### Usage in login workflow To automate login into ERP, the endpoints are hit
-in the following order: 1. Hit `HOMEPAGE_URL` using `session.get
-(HOMEPAGE_URL)`. This step is necessary to establish the initial session and
-retrieve `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
+#### Usage in login workflow To automate the login process into ERP, the
+endpoints are hit in the following order: 1. Hit `HOMEPAGE_URL` using
+`session.get(HOMEPAGE_URL)`. This step establishes the initial session and
+retrieves `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
 (SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER},
 headers=headers)`. This step fetches the secret question required for
 authentication. 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee':
 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests
 an OTP (One-Time Password) for authentication. 4. Finally, hit `LOGIN_URL`
 using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step
 performs the actual ERP login with the provided login details and OTP. >
 **Note** `session` = [requests.Session()](https://docs.python-requests.org/en/
 latest/_modules/requests/sessions/) is used to persist the session parameters
 throughout the workflow
-### Login ERP Login workflow is implemented in : `login(headers, erp_creds,
-OTP_WAIT_INTERVAL, session)` inside [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py).
-The input and output specifications for the function are mentioned below.
+### Login ERP login workflow is implemented in `login(headers, erp_creds,
+OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
+output specifications for the function are mentioned below.
 #### Input The function requires following arguments: 1. `headers`: Headers for
-the post requests. ```python headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } ``` 2. `erp_creds`:
-ERP_Login_Credentials_file, which is imported. ```python import erpcreds ``` 3.
-`OTP_WAIT_INTERVAL`: Interval after which api checks continuously for new OTP
-mail. 4. `session`: [requests.Session()](https://docs.python-requests.org/en/
-latest/_modules/requests/sessions/) object, to persist the session parameters
-throughout the workflow. ```python import requests session = requests.Session()
-```
-#### Output 1. The function returns: - [sessionToken](https://en.wikipedia.org/
-wiki/Session_ID) - [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
-It also modifies the `session` object which now contains parameters for the
-logged in session, which can be used for further navigation in ERP. 3. Has
-exhastive loggin inbuilt. It prints the status of each step.
-#### Usage It is recommended to use the login function as shown below:
-```python # importing the erp.py file import iitkgp_erp_login.erp as erp #
-using the login function inside erp.py sessionToken, ssoToken = erp.login
-(headers, erpcreds, 2, session) ``` Combining everything we looked about the
-`login` function till now: ```python import requests import erpcreds import
-iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
-requests.Session() sessionToken, ssoToken = erp.login(headers, erpcreds, 2,
-session) print(sessionToken, ssoToken) ```
-### Session status check The logic for status check of session is implemented
-in `session_alive(session)`. It tells whether the given session is valid/alive
-or not.
-The input and output specifications for the function are mentioned below.
+the post requests. An example is given below. ```python headers = { 'timeout':
+'20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
+like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+``` 2. `erp_creds`: ERP_Login_Credentials_file, which is imported into python
+file. ```python import erpcreds ``` 3. `OTP_WAIT_INTERVAL`: The interval after
+which the API continuously checks for new OTP mail. 4. `session`: A
+[requests.Session()](https://docs.python-requests.org/en/latest/_modules/
+requests/sessions/) object, to persist the session parameters throughout the
+workflow. ```python import requests session = requests.Session() ```
+#### Output 1. The function returns the following in the order of occurrence as
+here (`sessionToken, ssoToekn`): 1. [sessionToken](https://en.wikipedia.org/
+wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
+It also modifies the `session` object, which now includes parameters for the
+logged-in session. These parameters can be utilized for further navigation
+within the ERP system. 3. It incorporates **comprehensive logging**. It prints
+the status of each step, providing detailed information throughout the process.
+#### Usage It is recommended to use the `login` function in the following
+manner: ```python # importing the erp.py file import iitkgp_erp_login.erp as
+erp # using the login function inside erp.py sessionToken, ssoToken = erp.login
+(headers, erpcreds, 2, session) ``` Here's an example combining all the aspects
+we have discussed so far about the `login` function: ```python import requests
+import erpcreds import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
+'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
+Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+session = requests.Session() sessionToken, ssoToken = erp.login(headers,
+erpcreds, 2, session) print(sessionToken, ssoToken) ``` > **Note** The code
+snippet above will not work unless the prerequisites are fulfilled
+### Session status check The logic for checking the status of the session is
+implemented in the `session_alive(session)` function n [erp.py](https://
+github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+erp.py). This function determines whether the given session is valid/alive or
+not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
 requests/sessions/) object, to persist the session parameters throughout the
 workflow. ```python import requests session = requests.Session() ```
-#### Output Returns the status of session in boolean. __True if alive and False
-if not__.
-#### Usage It is recommended to use the session_alive function as shown below:
-```python # importing the erp.py file import iitkgp_erp_login.erp as erp #
-using the session_alive function inside erp.py print(erp.session_alive
-(session)) ``` Combining everything we looked about the `session_alive` and
-`login` functions till now: ```python import requests import time import creds
-import iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
+#### Output The `session_alive(session)` function returns the status of the
+session as a boolean value: **True** if it is alive and **False** if it is not.
+#### Usage It is recommended to use the `session_alive` function in the
+following manner: ```python # Importing the erp.py file import
+iitkgp_erp_login.erp as erp # Using the session_alive function inside erp.py
+print(erp.session_alive(session)) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function and `session_alive`
+function: ```python import requests import time import creds import
+iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
 Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
 requests.Session() while True: if not erp.session_alive(session): erp.login
 (headers, creds, 2, session) else: print("Session is alive.") time.sleep(2) ```
+> **Note** The code snippet above will not work unless the prerequisites are
+fulfilled
 ## Usage
-### Prerequisites Following scripts are required, and **MUST** be present in
-the same directory as that of the script in which `iitkgp_erp_login` (yes, this
-module) is being imported. - erpcreds.py - token.json
+### Prerequisites The following scripts are required and **MUST** be present in
+the same directory as the script where `iitkgp_erp_login` module is being
+imported: - erpcreds.py - token.json
 #### ERP credentials file
 ##### Creating Create a `.py` file with your ERP credentials stored in it.
-Following are the instructions for creating this file: - Name of the file can
-be any valid python file's name - **Variable names must not be changed**, copy
-the below format and **ONLY update values** inside `"` - _double quotes_.
-```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********"
-SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
-##### Using Let's suppose you saved the erp creds file as `erpcreds.py`. Then
-in order to use it you will just have to import it: ```python import erpcreds
-print(erpcreds.ROLL_NUMBER) # Output: XXYYXXXXX print
-(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2 ```
-#### Generating token for GMail enabled googleapi 1. Follow the steps at [Gmail
-API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
-python) guide to get `credentials.json`. > **Note** `credentials.json` is
-permanent until you delete it in your google clound console. 2. Follow the
-steps below to generate `token.json`: - Download [gentokenjson.py](https://
-gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) in the same folder
-containing `credentials.json` - Import the required module ```bash pip install
-google-auth-oauthlib ``` - Execute `gentokenjson.py` with `readonly` argument
-```bash python3 gentokenjson.py readonly ``` - Browser window will open and ask
-you to select the account, choose the one receiving OTP for login - Allow
-permission on that email to use just enabled __GMAIL API__ - Click on
-`Continue` instead of __Back To Safety__ - Then press `Continue` again -
-`token.json` will be generated in same folder as that of `credentials.json` >
-**Warning** `token.json` expires after sometime. So make sure to check that in
-your projects and keep refreshing it.
-### Example Now, we will create a script which will open ERP on your default
-browser with a logged in session. 1. Install the package. ```bash pip install
-iitkgp_erp_login ```` 2. Make sure erpcreds.py & token.json exist in the same
-directory as that of the script we are about to create. 3. Create `open_erp.py`
-and append the following content into it. ```python import requests import
-webbrowser import erpcreds import iitkgp_erp_login.erp as erp from
-iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout': '20',
-'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
-Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+Please follow the instructions below to create this file: - You can choose any
+valid name for the file, adhering to Python's naming conventions. - **Do not
+change the variable names**. Simply copy the format provided below and update
+the values inside the `double quotes` ("). ```python # ERP Credentials
+ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********" SECURITY_QUESTIONS_ANSWERS =
+{ "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
+##### Using Let's suppose you have saved the ERP credentials file as
+`erpcreds.py`. To use it, you can simply import it in your Python script using
+the following code: ```python import erpcreds print(erpcreds.ROLL_NUMBER) #
+Output: XXYYXXXXX print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2
+```
+#### Generating token for GMail enabled googleapi 1. Follow the steps in the
+[Gmail API - Python Quickstart](https://developers.google.com/gmail/api/
+quickstart/python) guide to obtain `credentials.json` file. > **Note** The
+`credentials.json` file is permanent unless you manually delete its reference
+in your Google Cloud Console. 2. To generate the `token.json` file, follow the
+steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
+adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
+contains the `credentials.json` file - Import the required module, `google-
+auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
+`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
+readonly ``` - A browser window will open, prompting you to select the Google
+account associated with receiving OTP for login. - Grant permission to the
+selected email address to utilize the newly enabled **Gmail API**. - Click on
+`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
+`token.json` file will be generated in the same folder as the
+`credentials.json` file > **Warning** The `token.json` file has an expiration
+time, so it's important to periodically check and refresh it in your projects
+to ensure uninterrupted access.
+### Example Now, we will create a script that opens the ERP system on your
+default browser with a logged-in session. 1. Install the package. ```bash pip
+install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
+exist in the same directory as the script we are about to create. 3. Create a
+file named `open_erp.py` and include the following code: ```python import
+requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
+from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
+'20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
+like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 session = requests.Session() _, ssoToken = erp.login(headers, erpcreds, 2,
 session) logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open
-(logged_in_url) ``` 4. Run the script ```bash python3 open_erp.py ```
+(logged_in_url) ``` 4. Run the script. ```bash python3 open_erp.py ```
```

### Comparing `iitkgp_erp_login-1.0.0/pyproject.toml` & `iitkgp_erp_login-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iitkgp_erp_login"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Arpit Bhardwaj", email="proffapt@pm.me" },
 ]
 description = "A package to automate login process in ERP for IIT-KGP"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `iitkgp_erp_login-1.0.0/src/iitkgp_erp_login/erp.py` & `iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/erp.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-1.0.0/src/iitkgp_erp_login/read_mail.py` & `iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/read_mail.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-1.0.0/src/iitkgp_erp_login.egg-info/PKG-INFO` & `iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp-erp-login
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,30 +49,30 @@
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
    └── read_mail.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains implementation of `getOTP(OTP_WAIT_INTERVAL)` function along with various helper functions for it. These functions are not intended to be used by _you_ - the user - as the only case, where, OTP will be required is during the login process which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script be an abstraction for general user. Obviously, if you want to tweak the OTP fetching process feel free to have a look at the script [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py).
+[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
-[endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) contains all the required endpoints for the ERP login workflow.
+The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
 <div id="endpoints-about"></div>
 
 #### About
 - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage.
 - `SECRET_QUESTION_URL`: The URL for retrieving the secret question for authentication.
 - `OTP_URL`: The URL for requesting the OTP (One-Time Password) for authentication.
 - `LOGIN_URL`: The URL for ERP login.
-- `WELCOMEPAGE_URL`: The URL of the welcome page, which is only accessible when the user is **NOT** logged-in and behaves exactly as `HOMEPAGE_URL` but when logged-in returns `404` error.
+- `WELCOMEPAGE_URL`: The URL of the welcome page, which is accessible only when the user is **NOT** logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user is logged in, it returns a `404` error.
 
 <div id="endpoints-usage"></div>
 
 #### Usage
 ```python
 from iitkgp_erp_login.endpoints import *
 
@@ -83,75 +83,74 @@
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
 <div id="usage-in-login-workflow"></div>
 
 #### Usage in login workflow
 
-To automate login into ERP, the endpoints are hit in the following order:
+To automate the login process into ERP, the endpoints are hit in the following order:
 
-1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step is necessary to establish the initial session and retrieve `sessionToken`.
+1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step establishes the initial session and retrieves `sessionToken`.
 2. Hit `SECRET_QUESTION_URL` using `session.post(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER}, headers=headers)`. This step fetches the secret question required for authentication.
 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee': 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests an OTP (One-Time Password) for authentication.
 4. Finally, hit `LOGIN_URL` using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step performs the actual ERP login with the provided login details and OTP.
 
 > **Note**  `session` = [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) is used to persist the session parameters throughout the workflow
 
 <div id="login"></div>
 
 ### Login
 
-ERP Login workflow is implemented in : `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` inside [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py).<br>
-The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
 The function requires following arguments:
-1. `headers`: Headers for the post requests.
+1. `headers`: Headers for the post requests. An example is given below.
     ```python
     headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
     }
     ``` 
-2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported.
+2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported into python file.
     ```python
     import erpcreds
     ```
-3.  `OTP_WAIT_INTERVAL`: Interval after which api checks continuously for new OTP mail.
-4.  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+3.  `OTP_WAIT_INTERVAL`: The interval after which the API continuously checks for new OTP mail.
+4.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
     ```python
     import requests
 
     session = requests.Session()
     ```
 
 <div id="login-output"></div>
 
 #### Output
-1. The function returns:
-   - [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
-   - [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
-2. It also modifies the `session` object which now contains parameters for the logged in session, which can be used for further navigation in ERP.
-3. Has exhastive loggin inbuilt. It prints the status of each step.
+1. The function returns the following in the order of occurrence as here (`sessionToken, ssoToekn`):
+   1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
+   2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
+2. It also modifies the `session` object, which now includes parameters for the logged-in session. These parameters can be utilized for further navigation within the ERP system.
+3. It incorporates **comprehensive logging**. It prints the status of each step, providing detailed information throughout the process.
 
 <div id="login-usage"></div>
 
 #### Usage
-It is recommended to use the login function as shown below:
+It is recommended to use the `login` function in the following manner:
 ```python
 # importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # using the login function inside erp.py
 sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
 ```
 
-Combining everything we looked about the `login` function till now:
+Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
 import iitkgp_erp_login.erp as erp
 
 headers = {
@@ -162,19 +161,20 @@
 session = requests.Session()
 
 sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
    
 print(sessionToken, ssoToken)
 ```
 
+> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+
 <div id="session-alive"></div>
 
 ### Session status check
-The logic for status check of session is implemented in `session_alive(session)`. It tells whether the given session is valid/alive or not.<br>
-The input and output specifications for the function are mentioned below.
+The logic for checking the status of the session is implemented in the `session_alive(session)` function  n [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
 The function requires following argument:
 
  -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
@@ -182,29 +182,30 @@
     import requests
 
     session = requests.Session()
      ```
 <div id="session-alive-output"></div>
 
 #### Output
-Returns the status of session in boolean. __True if alive and False if not__.
+The `session_alive(session)` function returns the status of the session as a boolean value: **True** if it is alive and **False** if it is not.
 
 <div id="session-alive-usage"></div>
 
 #### Usage
-It is recommended to use the session_alive function as shown below:
+It is recommended to use the `session_alive` function in the following manner:
 ```python
-# importing the erp.py file
+# Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
-# using the session_alive function inside erp.py
+# Using the session_alive function inside erp.py
 print(erp.session_alive(session))
 ```
 
-Combining everything we looked about the `session_alive` and `login` functions till now:
+Here's an example combining all the aspects we have discussed so far about the `login` function and `session_alive` function:
+
 ```python
 import requests
 import time
 import creds
 import iitkgp_erp_login.erp as erp
 
 headers = {
@@ -219,38 +220,40 @@
         erp.login(headers, creds, 2, session)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
+> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+
 <div id="package-usage"></div>
 
 ## Usage
 
 <div id="prerequisites"></div>
 
 ### Prerequisites
-Following scripts are required, and **MUST** be present in the same directory as that of the script in which `iitkgp_erp_login` (yes, this module) is being imported.
+
+The following scripts are required and **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported:
 
 - <a href="#erpcreds">erpcreds.py</a>
 - <a href="#token">token.json</a>
 
 <div id="erpcreds"></div>
 
 #### ERP credentials file
 
 <div id="erpcreds-creating"></div>
 
 ##### Creating
 
-Create a `.py` file with your ERP credentials stored in it.<br>
-Following are the instructions for creating this file:
-- Name of the file can be any valid python file's name
-- **Variable names must not be changed**, copy the below format and **ONLY update values** inside `"` - _double quotes_.
+Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
+- You can choose any valid name for the file, adhering to Python's naming conventions.
+- **Do not change the variable names**. Simply copy the format provided below and update the values inside the `double quotes` (").
   ```python
   # ERP Credentials
   ROLL_NUMBER = "XXYYXXXXX"
   PASSWORD = "**********"
   SECURITY_QUESTIONS_ANSWERS = {
       "Q1" : "A1",
       "Q2" : "A2",
@@ -258,66 +261,67 @@
   }
   ```
 
 <div id="erpcreds-using"></div>
 
 ##### Using
 
-Let's suppose you saved the erp creds file as `erpcreds.py`. Then in order to use it you will just have to import it:
+Let's suppose you have saved the ERP credentials file as `erpcreds.py`. To use it, you can simply import it in your Python script using the following code:
+
 ```python
 import erpcreds
 
 print(erpcreds.ROLL_NUMBER)
 # Output: XXYYXXXXX
 
 print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"])
 # Output: A2
 ```
 
 <div id="token"></div>
 
 #### Generating token for GMail enabled googleapi
 
-1. Follow the steps at [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to get `credentials.json`.
-   > **Note** `credentials.json` is permanent until you delete it in your google clound console.
+1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
+   > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
 
-2. Follow the steps below to generate `token.json`:
-    - Download [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) in the same folder containing `credentials.json`
-    - Import the required module
+2. To generate the `token.json` file, follow the steps below:
+    - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
+    - Import the required module, `google-auth-oauthlib`
       
       ```bash
       pip install google-auth-oauthlib
       ```
-    - Execute `gentokenjson.py` with `readonly` argument
+    - Execute `gentokenjson.py` with the `readonly` argument
    
       ```bash
       python3 gentokenjson.py readonly
       ```
-    - Browser window will open and ask you to select the account, choose the one receiving OTP for login
-    - Allow permission on that email to use just enabled __GMAIL API__
+    - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
+    - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
        - Click on `Continue` instead of __Back To Safety__
-       - Then press `Continue` again
-    - `token.json` will be generated in same folder as that of `credentials.json`
+       - Then, press `Continue` again
+    - The `token.json` file will be generated in the same folder as the `credentials.json` file
   
-    > **Warning** `token.json` expires after sometime. So make sure to check that in your projects and keep refreshing it.
+    > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
 
 <div id="example"></div>
 
 ### Example
 
-Now, we will create a script which will open ERP on your default browser with a logged in session.
+Now, we will create a script that opens the ERP system on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
    pip install iitkgp_erp_login
    ````
-2. Make sure <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> exist in the same directory as that of the script we are about to create.
+2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
 
-3. Create `open_erp.py` and append the following content into it.
+3. Create a file named `open_erp.py` and include the following code:
 
    ```python
    import requests
    import webbrowser
    import erpcreds
    import iitkgp_erp_login.erp as erp
    from iitkgp_erp_login.endpoints import HOMEPAGE_URL
@@ -330,11 +334,11 @@
    session = requests.Session()
 
    _, ssoToken = erp.login(headers, erpcreds, 2, session)
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
-4. Run the script
+4. Run the script.
    ```bash
    python3 open_erp.py
    ```
```

#### html2text {}

```diff
@@ -1,142 +1,153 @@
-Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 1.0.0 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 1.0.1 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module A python package/module to automate login process in
 ERP for IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage -
 Usage_in_login_workflow - Login - Input - Output - Usage - Session_status_check
 - Input - Output - Usage - Usage - Prerequisites - ERP_credentials_file -
 Creating - Using - Generating_token_for_GMail_enabled_googleapi - Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
 erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains
-implementation of `getOTP(OTP_WAIT_INTERVAL)` function along with various
-helper functions for it. These functions are not intended to be used by _you_ -
-the user - as the only case, where, OTP will be required is during the login
-process which is handled by functions in [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this
-script be an abstraction for general user. Obviously, if you want to tweak the
-OTP fetching process feel free to have a look at the script [read_mail.py]
-(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
-iitkgp_erp_login/read_mail.py).
-### Endpoints [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/
-blob/main/src/iitkgp_erp_login/endpoints.py) contains all the required
-endpoints for the ERP login workflow.
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
+implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various
+helper functions. These functions are not intended to be used by _you_, the
+user. The only case where OTP is required is during the login process, which is
+handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
+pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
+abstraction for general users. If you want to modify the OTP fetching process,
+feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
+erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
+pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
+necessary endpoints for the ERP login workflow.
 #### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
-The URL of the welcome page, which is only accessible when the user is **NOT**
-logged-in and behaves exactly as `HOMEPAGE_URL` but when logged-in returns
-`404` error.
+The URL of the welcome page, which is accessible only when the user is **NOT**
+logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
+is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
-#### Usage in login workflow To automate login into ERP, the endpoints are hit
-in the following order: 1. Hit `HOMEPAGE_URL` using `session.get
-(HOMEPAGE_URL)`. This step is necessary to establish the initial session and
-retrieve `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
+#### Usage in login workflow To automate the login process into ERP, the
+endpoints are hit in the following order: 1. Hit `HOMEPAGE_URL` using
+`session.get(HOMEPAGE_URL)`. This step establishes the initial session and
+retrieves `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
 (SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER},
 headers=headers)`. This step fetches the secret question required for
 authentication. 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee':
 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests
 an OTP (One-Time Password) for authentication. 4. Finally, hit `LOGIN_URL`
 using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step
 performs the actual ERP login with the provided login details and OTP. >
 **Note** `session` = [requests.Session()](https://docs.python-requests.org/en/
 latest/_modules/requests/sessions/) is used to persist the session parameters
 throughout the workflow
-### Login ERP Login workflow is implemented in : `login(headers, erp_creds,
-OTP_WAIT_INTERVAL, session)` inside [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py).
-The input and output specifications for the function are mentioned below.
+### Login ERP login workflow is implemented in `login(headers, erp_creds,
+OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
+output specifications for the function are mentioned below.
 #### Input The function requires following arguments: 1. `headers`: Headers for
-the post requests. ```python headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } ``` 2. `erp_creds`:
-ERP_Login_Credentials_file, which is imported. ```python import erpcreds ``` 3.
-`OTP_WAIT_INTERVAL`: Interval after which api checks continuously for new OTP
-mail. 4. `session`: [requests.Session()](https://docs.python-requests.org/en/
-latest/_modules/requests/sessions/) object, to persist the session parameters
-throughout the workflow. ```python import requests session = requests.Session()
-```
-#### Output 1. The function returns: - [sessionToken](https://en.wikipedia.org/
-wiki/Session_ID) - [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
-It also modifies the `session` object which now contains parameters for the
-logged in session, which can be used for further navigation in ERP. 3. Has
-exhastive loggin inbuilt. It prints the status of each step.
-#### Usage It is recommended to use the login function as shown below:
-```python # importing the erp.py file import iitkgp_erp_login.erp as erp #
-using the login function inside erp.py sessionToken, ssoToken = erp.login
-(headers, erpcreds, 2, session) ``` Combining everything we looked about the
-`login` function till now: ```python import requests import erpcreds import
-iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
-requests.Session() sessionToken, ssoToken = erp.login(headers, erpcreds, 2,
-session) print(sessionToken, ssoToken) ```
-### Session status check The logic for status check of session is implemented
-in `session_alive(session)`. It tells whether the given session is valid/alive
-or not.
-The input and output specifications for the function are mentioned below.
+the post requests. An example is given below. ```python headers = { 'timeout':
+'20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
+like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+``` 2. `erp_creds`: ERP_Login_Credentials_file, which is imported into python
+file. ```python import erpcreds ``` 3. `OTP_WAIT_INTERVAL`: The interval after
+which the API continuously checks for new OTP mail. 4. `session`: A
+[requests.Session()](https://docs.python-requests.org/en/latest/_modules/
+requests/sessions/) object, to persist the session parameters throughout the
+workflow. ```python import requests session = requests.Session() ```
+#### Output 1. The function returns the following in the order of occurrence as
+here (`sessionToken, ssoToekn`): 1. [sessionToken](https://en.wikipedia.org/
+wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
+It also modifies the `session` object, which now includes parameters for the
+logged-in session. These parameters can be utilized for further navigation
+within the ERP system. 3. It incorporates **comprehensive logging**. It prints
+the status of each step, providing detailed information throughout the process.
+#### Usage It is recommended to use the `login` function in the following
+manner: ```python # importing the erp.py file import iitkgp_erp_login.erp as
+erp # using the login function inside erp.py sessionToken, ssoToken = erp.login
+(headers, erpcreds, 2, session) ``` Here's an example combining all the aspects
+we have discussed so far about the `login` function: ```python import requests
+import erpcreds import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
+'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
+Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+session = requests.Session() sessionToken, ssoToken = erp.login(headers,
+erpcreds, 2, session) print(sessionToken, ssoToken) ``` > **Note** The code
+snippet above will not work unless the prerequisites are fulfilled
+### Session status check The logic for checking the status of the session is
+implemented in the `session_alive(session)` function n [erp.py](https://
+github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+erp.py). This function determines whether the given session is valid/alive or
+not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
 requests/sessions/) object, to persist the session parameters throughout the
 workflow. ```python import requests session = requests.Session() ```
-#### Output Returns the status of session in boolean. __True if alive and False
-if not__.
-#### Usage It is recommended to use the session_alive function as shown below:
-```python # importing the erp.py file import iitkgp_erp_login.erp as erp #
-using the session_alive function inside erp.py print(erp.session_alive
-(session)) ``` Combining everything we looked about the `session_alive` and
-`login` functions till now: ```python import requests import time import creds
-import iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
+#### Output The `session_alive(session)` function returns the status of the
+session as a boolean value: **True** if it is alive and **False** if it is not.
+#### Usage It is recommended to use the `session_alive` function in the
+following manner: ```python # Importing the erp.py file import
+iitkgp_erp_login.erp as erp # Using the session_alive function inside erp.py
+print(erp.session_alive(session)) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function and `session_alive`
+function: ```python import requests import time import creds import
+iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
 Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
 requests.Session() while True: if not erp.session_alive(session): erp.login
 (headers, creds, 2, session) else: print("Session is alive.") time.sleep(2) ```
+> **Note** The code snippet above will not work unless the prerequisites are
+fulfilled
 ## Usage
-### Prerequisites Following scripts are required, and **MUST** be present in
-the same directory as that of the script in which `iitkgp_erp_login` (yes, this
-module) is being imported. - erpcreds.py - token.json
+### Prerequisites The following scripts are required and **MUST** be present in
+the same directory as the script where `iitkgp_erp_login` module is being
+imported: - erpcreds.py - token.json
 #### ERP credentials file
 ##### Creating Create a `.py` file with your ERP credentials stored in it.
-Following are the instructions for creating this file: - Name of the file can
-be any valid python file's name - **Variable names must not be changed**, copy
-the below format and **ONLY update values** inside `"` - _double quotes_.
-```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********"
-SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
-##### Using Let's suppose you saved the erp creds file as `erpcreds.py`. Then
-in order to use it you will just have to import it: ```python import erpcreds
-print(erpcreds.ROLL_NUMBER) # Output: XXYYXXXXX print
-(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2 ```
-#### Generating token for GMail enabled googleapi 1. Follow the steps at [Gmail
-API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
-python) guide to get `credentials.json`. > **Note** `credentials.json` is
-permanent until you delete it in your google clound console. 2. Follow the
-steps below to generate `token.json`: - Download [gentokenjson.py](https://
-gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) in the same folder
-containing `credentials.json` - Import the required module ```bash pip install
-google-auth-oauthlib ``` - Execute `gentokenjson.py` with `readonly` argument
-```bash python3 gentokenjson.py readonly ``` - Browser window will open and ask
-you to select the account, choose the one receiving OTP for login - Allow
-permission on that email to use just enabled __GMAIL API__ - Click on
-`Continue` instead of __Back To Safety__ - Then press `Continue` again -
-`token.json` will be generated in same folder as that of `credentials.json` >
-**Warning** `token.json` expires after sometime. So make sure to check that in
-your projects and keep refreshing it.
-### Example Now, we will create a script which will open ERP on your default
-browser with a logged in session. 1. Install the package. ```bash pip install
-iitkgp_erp_login ```` 2. Make sure erpcreds.py & token.json exist in the same
-directory as that of the script we are about to create. 3. Create `open_erp.py`
-and append the following content into it. ```python import requests import
-webbrowser import erpcreds import iitkgp_erp_login.erp as erp from
-iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout': '20',
-'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
-Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+Please follow the instructions below to create this file: - You can choose any
+valid name for the file, adhering to Python's naming conventions. - **Do not
+change the variable names**. Simply copy the format provided below and update
+the values inside the `double quotes` ("). ```python # ERP Credentials
+ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********" SECURITY_QUESTIONS_ANSWERS =
+{ "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
+##### Using Let's suppose you have saved the ERP credentials file as
+`erpcreds.py`. To use it, you can simply import it in your Python script using
+the following code: ```python import erpcreds print(erpcreds.ROLL_NUMBER) #
+Output: XXYYXXXXX print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2
+```
+#### Generating token for GMail enabled googleapi 1. Follow the steps in the
+[Gmail API - Python Quickstart](https://developers.google.com/gmail/api/
+quickstart/python) guide to obtain `credentials.json` file. > **Note** The
+`credentials.json` file is permanent unless you manually delete its reference
+in your Google Cloud Console. 2. To generate the `token.json` file, follow the
+steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
+adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
+contains the `credentials.json` file - Import the required module, `google-
+auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
+`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
+readonly ``` - A browser window will open, prompting you to select the Google
+account associated with receiving OTP for login. - Grant permission to the
+selected email address to utilize the newly enabled **Gmail API**. - Click on
+`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
+`token.json` file will be generated in the same folder as the
+`credentials.json` file > **Warning** The `token.json` file has an expiration
+time, so it's important to periodically check and refresh it in your projects
+to ensure uninterrupted access.
+### Example Now, we will create a script that opens the ERP system on your
+default browser with a logged-in session. 1. Install the package. ```bash pip
+install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
+exist in the same directory as the script we are about to create. 3. Create a
+file named `open_erp.py` and include the following code: ```python import
+requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
+from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
+'20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
+like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 session = requests.Session() _, ssoToken = erp.login(headers, erpcreds, 2,
 session) logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open
-(logged_in_url) ``` 4. Run the script ```bash python3 open_erp.py ```
+(logged_in_url) ``` 4. Run the script. ```bash python3 open_erp.py ```
```

