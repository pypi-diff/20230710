# Comparing `tmp/jplaw-0.1.6.tar.gz` & `tmp/jplaw-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jplaw-0.1.6.tar", last modified: Sat Jul  8 19:09:46 2023, max compression
+gzip compressed data, was "jplaw-0.1.7.tar", last modified: Sun Jul  9 23:47:50 2023, max compression
```

## Comparing `jplaw-0.1.6.tar` & `jplaw-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 19:09:33.000000 jplaw-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-08 19:09:46.552229 jplaw-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-08 19:09:33.000000 jplaw-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/jplaw/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/api_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/community.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/jplaw/types/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/comment_sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/http_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/listing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/modlog_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/post_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/registration_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/search_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/subscribed_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/jplaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 19:09:33.000000 jplaw-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:09:46.552229 jplaw-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.999112 jplaw-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-09 23:47:36.000000 jplaw-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-09 23:47:49.999112 jplaw-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-09 23:47:36.000000 jplaw-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.995112 jplaw-0.1.7/jplaw/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/api_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.999112 jplaw-0.1.7/jplaw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/comment_sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/http_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/listing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/modlog_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/post_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/registration_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/search_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/subscribed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.999112 jplaw-0.1.7/jplaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-09 23:47:36.000000 jplaw-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 23:47:49.999112 jplaw-0.1.7/setup.cfg
```

### Comparing `jplaw-0.1.6/LICENSE` & `jplaw-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/PKG-INFO` & `jplaw-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,21 +53,29 @@
 print(lem.Community.get("test@lemmy.ml"))
 ```
 
 # Documentation
 See [the documentation](https://amarpersaud.github.io/python-jplaw/) for more information on how to use jplaw.
 
 # Roadmap 
-### v0.1.7
 - Work on return types and usability.
-
-### v0.1.6
 - Work on testing functions and finding / squashing bugs
 
 # Changelog
+
+### v0.1.7
+- Fix bug with "fixed" boolean values
+
+### v0.1.6
+- Fixes boolean and Enum parameters
+- Adds show_nsfw to communities
+- Add open_links_in_new_tab saveUserSettings
+- Removes auth_token parameter from functions. To get an auth_token, a new Lemmy object can be created and logged in with. Accessing other instances via a Lemmy object can be done via the instance parameter, but does not authenticate
+- Fix documentation for jplaw.types and jplaw.comment
+
 ### v0.1.5
 - Fix namespace issues
 - Fix build issues
 - Fix missing instance argument in list communities
 
 ### v0.1.4
 - Created documentation
```

### Comparing `jplaw-0.1.6/README.md` & `jplaw-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,21 +39,29 @@
 print(lem.Community.get("test@lemmy.ml"))
 ```
 
 # Documentation
 See [the documentation](https://amarpersaud.github.io/python-jplaw/) for more information on how to use jplaw.
 
 # Roadmap 
-### v0.1.7
 - Work on return types and usability.
-
-### v0.1.6
 - Work on testing functions and finding / squashing bugs
 
 # Changelog
+
+### v0.1.7
+- Fix bug with "fixed" boolean values
+
+### v0.1.6
+- Fixes boolean and Enum parameters
+- Adds show_nsfw to communities
+- Add open_links_in_new_tab saveUserSettings
+- Removes auth_token parameter from functions. To get an auth_token, a new Lemmy object can be created and logged in with. Accessing other instances via a Lemmy object can be done via the instance parameter, but does not authenticate
+- Fix documentation for jplaw.types and jplaw.comment
+
 ### v0.1.5
 - Fix namespace issues
 - Fix build issues
 - Fix missing instance argument in list communities
 
 ### v0.1.4
 - Created documentation
```

### Comparing `jplaw-0.1.6/jplaw/api_paths.py` & `jplaw-0.1.7/jplaw/api_paths.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/comment.py` & `jplaw-0.1.7/jplaw/comment.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/community.py` & `jplaw-0.1.7/jplaw/community.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/emoji.py` & `jplaw-0.1.7/jplaw/emoji.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/lemmy.py` & `jplaw-0.1.7/jplaw/lemmy.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/post.py` & `jplaw-0.1.7/jplaw/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         optional = {
             "id": post_id,
             "comment_id": comment_id,
             }
         res = self._req.lemmyRequest("getPost", instance=instance, form=form, optional=optional, auth=auth)
         return res["post_view"]
         
-    def create(self, community_id:int, title:str=None, body:str=None, remote_url:str=None, honeypot:str=None, nsfw=False, language_id:int=None, instance:str=None):
+    def create(self, community_id:int, title:str=None, body:str=None, remote_url:str=None, honeypot:str=None, nsfw:bool=False, language_id:int=None, instance:str=None):
         """
         Create a post
         
         Args:
             community_id (int): ID of the community the post is in. Optional
             title (str): Title of the post. Optional.
             body (str): Text contents of the post. Optional
```

### Comparing `jplaw-0.1.6/jplaw/private_message.py` & `jplaw-0.1.7/jplaw/private_message.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/requestor.py` & `jplaw-0.1.7/jplaw/requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,25 +122,23 @@
         """
         if(bool_val is None):
             return "none"
         return str(bool_val).lower() if isinstance(bool_val, bool) else bool_val
         
     def fixFormValues(self, form: Dict[str, Any]):
         """
-        Fix value types for requests (e.g. bool and Enum types)
+        Fix value types for requests (e.g. Enum types)
         
         Args:
             form (Dict[str, Any]): Dictionary of keys and items in form
         
         Returns:
             Form with fixed values
         """
         for key, value in form.items():
-            if(isinstance(value, bool)):
-                form[key] = self.boolToStr(value)
             if(isinstance(value, Enum)):
                 form[key] = value.value
         return form
     
     def AddIfValue(self, name:str, value: Any, form: Dict[str, Any]):
         """
         Adds items to form if not None
```

### Comparing `jplaw-0.1.6/jplaw/site.py` & `jplaw-0.1.7/jplaw/site.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/types/modlog_action_type.py` & `jplaw-0.1.7/jplaw/types/modlog_action_type.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/types/sort_type.py` & `jplaw-0.1.7/jplaw/types/sort_type.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw/user.py` & `jplaw-0.1.7/jplaw/user.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/jplaw.egg-info/PKG-INFO` & `jplaw-0.1.7/jplaw.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,21 +53,29 @@
 print(lem.Community.get("test@lemmy.ml"))
 ```
 
 # Documentation
 See [the documentation](https://amarpersaud.github.io/python-jplaw/) for more information on how to use jplaw.
 
 # Roadmap 
-### v0.1.7
 - Work on return types and usability.
-
-### v0.1.6
 - Work on testing functions and finding / squashing bugs
 
 # Changelog
+
+### v0.1.7
+- Fix bug with "fixed" boolean values
+
+### v0.1.6
+- Fixes boolean and Enum parameters
+- Adds show_nsfw to communities
+- Add open_links_in_new_tab saveUserSettings
+- Removes auth_token parameter from functions. To get an auth_token, a new Lemmy object can be created and logged in with. Accessing other instances via a Lemmy object can be done via the instance parameter, but does not authenticate
+- Fix documentation for jplaw.types and jplaw.comment
+
 ### v0.1.5
 - Fix namespace issues
 - Fix build issues
 - Fix missing instance argument in list communities
 
 ### v0.1.4
 - Created documentation
```

### Comparing `jplaw-0.1.6/jplaw.egg-info/SOURCES.txt` & `jplaw-0.1.7/jplaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.6/pyproject.toml` & `jplaw-0.1.7/pyproject.toml`

 * *Files identical despite different names*

