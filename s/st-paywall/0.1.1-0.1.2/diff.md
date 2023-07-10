# Comparing `tmp/st-paywall-0.1.1.tar.gz` & `tmp/st-paywall-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-paywall-0.1.1.tar", last modified: Sun Jul  9 23:50:06 2023, max compression
+gzip compressed data, was "st-paywall-0.1.2.tar", last modified: Mon Jul 10 04:35:47 2023, max compression
```

## Comparing `st-paywall-0.1.1.tar` & `st-paywall-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-09 23:50:06.653084 st-paywall-0.1.1/
--rw-r--r--   0 trichards   (501) staff       (20)     6242 2023-07-09 23:50:06.652613 st-paywall-0.1.1/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     6019 2023-07-09 23:45:39.000000 st-paywall-0.1.1/README.md
--rw-r--r--   0 trichards   (501) staff       (20)      358 2023-07-09 23:47:20.000000 st-paywall-0.1.1/pyproject.toml
--rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-09 23:50:06.653169 st-paywall-0.1.1/setup.cfg
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-09 23:50:06.647039 st-paywall-0.1.1/src/
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-09 23:50:06.650367 st-paywall-0.1.1/src/st_paywall/
--rw-r--r--   0 trichards   (501) staff       (20)       36 2023-07-09 23:48:52.000000 st-paywall-0.1.1/src/st_paywall/__init__.py
--rw-r--r--   0 trichards   (501) staff       (20)     1507 2023-07-09 23:48:40.000000 st-paywall-0.1.1/src/st_paywall/aggregate_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-09 03:17:19.000000 st-paywall-0.1.1/src/st_paywall/google_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1077 2023-07-09 03:17:19.000000 st-paywall-0.1.1/src/st_paywall/stripe_auth.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-09 23:50:06.652233 st-paywall-0.1.1/src/st_paywall.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)     6242 2023-07-09 23:50:06.000000 st-paywall-0.1.1/src/st_paywall.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      333 2023-07-09 23:50:06.000000 st-paywall-0.1.1/src/st_paywall.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-09 23:50:06.000000 st-paywall-0.1.1/src/st_paywall.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-09 23:50:06.000000 st-paywall-0.1.1/src/st_paywall.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)       11 2023-07-09 23:50:06.000000 st-paywall-0.1.1/src/st_paywall.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.621211 st-paywall-0.1.2/
+-rw-r--r--   0 trichards   (501) staff       (20)     6062 2023-07-10 04:35:47.621000 st-paywall-0.1.2/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     5839 2023-07-10 04:34:35.000000 st-paywall-0.1.2/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)      358 2023-07-10 04:35:29.000000 st-paywall-0.1.2/pyproject.toml
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-10 04:35:47.621272 st-paywall-0.1.2/setup.cfg
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.616163 st-paywall-0.1.2/src/
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.618414 st-paywall-0.1.2/src/st_paywall/
+-rw-r--r--   0 trichards   (501) staff       (20)       36 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/__init__.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1616 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/aggregate_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/google_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1077 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/stripe_auth.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.620691 st-paywall-0.1.2/src/st_paywall.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)     6062 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      333 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       11 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/top_level.txt
```

### Comparing `st-paywall-0.1.1/PKG-INFO` & `st-paywall-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-paywall
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for creating subscription Streamlit apps
 Author-email: Tyler <tylerjrichards@gmail.com>
 License: MIT
 Description-Content-Type: text/markdown
 
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
@@ -24,22 +24,22 @@
 
 Basic example: https://subscription.streamlit.app
 
 <p>&nbsp;</p>
 
 # 🥟 st-paywall
 
-<strong>A python package for creating subscription Streamlit apps </strong>
+<strong>A python package for creating paid Streamlit apps with a paywall! </strong>
 
 ## Overview
 
-This package gives you two basic functions (`require_auth` and `add_auth`) that add subscription functionality to your Streamlit apps. `require_auth` will add both a Google login button and a Stripe subscription button to your sidebar, and will stop your entire app with `st.stop()` if the user is not logged in and subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email. If the user is not logged in or subscribed, they will be prompted to do so in the sidebar.
-`add_auth` does the same, except it does not stop the app but instead just surfaces the `st.session_state` information detailed above, which means the developer can control exactly what they would like to show to the subscribed vs unsubscribed user!
+This package gives you one basic functions (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
+If the `required` parameter is `True`, the app will stop with `st.stop()` if the user is not logged in and subscribed. Otherwise, you the developer will have control over exactly how you want to paywall the apps!
 
- I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
+ I hope you use this to create tons of value, and capture some of it with the magic of Streamlit.
 
 This package expects that you have a `.streamlit/secrets.toml` file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
```

### Comparing `st-paywall-0.1.1/README.md` & `st-paywall-0.1.2/src/st_paywall.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: st-paywall
+Version: 0.1.2
+Summary: A Python package for creating subscription Streamlit apps
+Author-email: Tyler <tylerjrichards@gmail.com>
+License: MIT
+Description-Content-Type: text/markdown
+
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 Author: [@tylerjrichards](https://twitter.com/tylerjrichards)
 
 Kind consultant: [@blackary](https://github.com/blackary)
@@ -16,22 +24,22 @@
 
 Basic example: https://subscription.streamlit.app
 
 <p>&nbsp;</p>
 
 # 🥟 st-paywall
 
-<strong>A python package for creating subscription Streamlit apps </strong>
+<strong>A python package for creating paid Streamlit apps with a paywall! </strong>
 
 ## Overview
 
-This package gives you two basic functions (`require_auth` and `add_auth`) that add subscription functionality to your Streamlit apps. `require_auth` will add both a Google login button and a Stripe subscription button to your sidebar, and will stop your entire app with `st.stop()` if the user is not logged in and subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email. If the user is not logged in or subscribed, they will be prompted to do so in the sidebar.
-`add_auth` does the same, except it does not stop the app but instead just surfaces the `st.session_state` information detailed above, which means the developer can control exactly what they would like to show to the subscribed vs unsubscribed user!
+This package gives you one basic functions (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
+If the `required` parameter is `True`, the app will stop with `st.stop()` if the user is not logged in and subscribed. Otherwise, you the developer will have control over exactly how you want to paywall the apps!
 
- I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
+ I hope you use this to create tons of value, and capture some of it with the magic of Streamlit.
 
 This package expects that you have a `.streamlit/secrets.toml` file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
@@ -97,8 +105,8 @@
 For my test application at subscription.streamlit.app, my Google console looks like this.
 
 <img src="readme_img/google_oauth_console.png" width="300">
 
 
 ### Feedback:
 
-If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
+If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
```

### Comparing `st-paywall-0.1.1/src/st_paywall/aggregate_auth.py` & `st-paywall-0.1.2/src/st_paywall/aggregate_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,30 +22,32 @@
         st.session_state.user_subscribed = False
         st.stop()
     elif user_email in customer_emails:
         st.session_state.user_subscribed = True
 
     if st.sidebar.button("Logout", type="primary"):
         del st.session_state.email
+        del st.session_state.user_subscribed
         st.experimental_rerun()
 
 def optional_auth():
     user_email = get_logged_in_user_email()
+    customer_emails = get_customer_emails()
 
     if not user_email:
         show_login_button()
         st.session_state.email = ""
         st.sidebar.markdown("")
 
-    customer_emails = get_customer_emails()
-    if user_email not in customer_emails:
+    if user_email and user_email not in customer_emails:
         redirect_button(text="Subscribe now!", customer_email="")
         st.sidebar.markdown("")
         st.session_state.user_subscribed = False
 
     elif user_email in customer_emails:
         st.session_state.user_subscribed = True
 
     if st.session_state.email != "":
         if st.sidebar.button("Logout", type="primary"):
             del st.session_state.email
+            del st.session_state.user_subscribed
             st.experimental_rerun()
```

### Comparing `st-paywall-0.1.1/src/st_paywall/google_auth.py` & `st-paywall-0.1.2/src/st_paywall/google_auth.py`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.1/src/st_paywall/stripe_auth.py` & `st-paywall-0.1.2/src/st_paywall/stripe_auth.py`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.1/src/st_paywall.egg-info/PKG-INFO` & `st-paywall-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: st-paywall
-Version: 0.1.1
-Summary: A Python package for creating subscription Streamlit apps
-Author-email: Tyler <tylerjrichards@gmail.com>
-License: MIT
-Description-Content-Type: text/markdown
-
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 Author: [@tylerjrichards](https://twitter.com/tylerjrichards)
 
 Kind consultant: [@blackary](https://github.com/blackary)
@@ -24,22 +16,22 @@
 
 Basic example: https://subscription.streamlit.app
 
 <p>&nbsp;</p>
 
 # 🥟 st-paywall
 
-<strong>A python package for creating subscription Streamlit apps </strong>
+<strong>A python package for creating paid Streamlit apps with a paywall! </strong>
 
 ## Overview
 
-This package gives you two basic functions (`require_auth` and `add_auth`) that add subscription functionality to your Streamlit apps. `require_auth` will add both a Google login button and a Stripe subscription button to your sidebar, and will stop your entire app with `st.stop()` if the user is not logged in and subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email. If the user is not logged in or subscribed, they will be prompted to do so in the sidebar.
-`add_auth` does the same, except it does not stop the app but instead just surfaces the `st.session_state` information detailed above, which means the developer can control exactly what they would like to show to the subscribed vs unsubscribed user!
+This package gives you one basic functions (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
+If the `required` parameter is `True`, the app will stop with `st.stop()` if the user is not logged in and subscribed. Otherwise, you the developer will have control over exactly how you want to paywall the apps!
 
- I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
+ I hope you use this to create tons of value, and capture some of it with the magic of Streamlit.
 
 This package expects that you have a `.streamlit/secrets.toml` file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
@@ -105,8 +97,8 @@
 For my test application at subscription.streamlit.app, my Google console looks like this.
 
 <img src="readme_img/google_oauth_console.png" width="300">
 
 
 ### Feedback:
 
-If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
+If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
```

