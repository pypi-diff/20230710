# Comparing `tmp/django-twilio-access-token-0.0.4.tar.gz` & `tmp/django-twilio-access-token-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-twilio-access-token-0.0.4.tar", last modified: Mon Aug 31 07:03:52 2020, max compression
+gzip compressed data, was "django-twilio-access-token-0.0.5.tar", last modified: Mon Jul 10 05:00:04 2023, max compression
```

## Comparing `django-twilio-access-token-0.0.4.tar` & `django-twilio-access-token-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)     3642 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/PKG-INFO
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)     2209 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/README.md
-drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)      102 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/__init__.py
-drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/serializers/
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)      338 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/serializers/__init__.py
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)     1715 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/serializers/twilio_access_token_serializer.py
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)     3557 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/serializers/twilio_room_serializer.py
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)      370 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/urls.py
-drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/views/
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)      254 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/views/__init__.py
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)      608 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/views/twilio_room_view.py
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)      361 2020-08-10 06:17:54.000000 django-twilio-access-token-0.0.4/django_twilio_access_token/views/twilio_video_access_token_view.py
-drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)     3642 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/PKG-INFO
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)      695 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/SOURCES.txt
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)        1 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/dependency_links.txt
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)       69 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/requires.txt
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)       27 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/top_level.txt
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)       38 2020-08-31 07:03:52.000000 django-twilio-access-token-0.0.4/setup.cfg
--rw-r--r--   0 panjiyudasetya   (501) staff       (20)     1393 2020-08-31 06:43:43.000000 django-twilio-access-token-0.0.4/setup.py
+drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2023-07-10 05:00:04.471347 django-twilio-access-token-0.0.5/
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)     3247 2023-07-10 05:00:04.471083 django-twilio-access-token-0.0.5/PKG-INFO
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)     2209 2022-06-02 03:40:21.000000 django-twilio-access-token-0.0.5/README.md
+drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2023-07-10 05:00:04.465498 django-twilio-access-token-0.0.5/django_twilio_access_token/
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)      102 2023-07-10 04:58:41.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/__init__.py
+drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2023-07-10 05:00:04.468943 django-twilio-access-token-0.0.5/django_twilio_access_token/serializers/
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)      338 2022-06-02 03:40:21.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/serializers/__init__.py
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)     1715 2022-06-02 03:40:21.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/serializers/twilio_access_token_serializer.py
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)     3614 2023-07-10 04:58:41.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/serializers/twilio_room_serializer.py
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)      370 2022-06-02 03:40:21.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/urls.py
+drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2023-07-10 05:00:04.470527 django-twilio-access-token-0.0.5/django_twilio_access_token/views/
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)      254 2022-06-02 03:40:21.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/views/__init__.py
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)      608 2022-06-02 03:40:21.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/views/twilio_room_view.py
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)      361 2022-06-02 03:40:21.000000 django-twilio-access-token-0.0.5/django_twilio_access_token/views/twilio_video_access_token_view.py
+drwxr-xr-x   0 panjiyudasetya   (501) staff       (20)        0 2023-07-10 05:00:04.467477 django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)     3247 2023-07-10 05:00:04.000000 django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/PKG-INFO
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)      695 2023-07-10 05:00:04.000000 django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/SOURCES.txt
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)        1 2023-07-10 05:00:04.000000 django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/dependency_links.txt
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)       69 2023-07-10 05:00:04.000000 django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/requires.txt
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)       27 2023-07-10 05:00:04.000000 django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/top_level.txt
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)       38 2023-07-10 05:00:04.471447 django-twilio-access-token-0.0.5/setup.cfg
+-rw-r--r--   0 panjiyudasetya   (501) staff       (20)     1393 2023-07-10 04:58:41.000000 django-twilio-access-token-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-twilio-access-token-0.0.4/PKG-INFO` & `django-twilio-access-token-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,15 @@
 Metadata-Version: 2.1
 Name: django-twilio-access-token
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django app to generate Twilio access token for particular Twilio services.
 Home-page: https://github.com/senseobservationsystems/django-twilio-access-token/
 Author: Panji Y. Wiwaha
 Author-email: panjiyudasetya@gmail.com
 License: UNKNOWN
-Description: 
-        # django-twilio-access-token
-        
-        This is a Django application that can be used to generate Twilio access token for particular services, such as Voice, Chat, and Video.
-        
-        ## Prerequisite
-        
-        ### Twilio
-        
-        We use Twilio client for [python](https://www.twilio.com/docs/libraries/python#install-the-library) to generate an access token for Twilio services. To make the package works on your project, you need to install Twilio client either through [pip](https://pip.pypa.io/en/stable/) command;
-        
-        ```
-        pip install twilio
-        ```
-        
-        or simply add Twilio on your `requirements.txt`
-        
-        ```
-        twilio~=6.32.0
-        ```
-        
-        ### Twilio keys
-        
-        In order to make the package works with your django project, you need to define the Twilio keys inside your project `settings.py`, for example:
-        ```
-        TWILIO_ACCOUNT_SID = 'PUT_YOUR_TWILIO_ACCOUNT_SID_HERE'  # You can find Twilio Account SID at the top right section of this page https://www.twilio.com/console/
-        
-        TWILIO_VIDEO_API_KEY_SID = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SID_HERE'  # You can obtain these keys by creating it through https://www.twilio.com/console/video/project/api-keys/
-        TWILIO_VIDEO_API_KEY_SECRET = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SECRET_HERE'
-        ```
-        
-        Or see the `test_project/test_app/settings.py` if you need to know more.
-        
-        ## How to run the test project
-        
-        To try out the package, you can run our test application by following these steps:
-        1. Ensure pip installed on your local machine. If you don't have it, you can follow the installation guide [here](https://pip.pypa.io/en/stable/installing/).
-        2. Open terminal and go to the root directory of where the package live, for instance: `$ cd Documents/py-projects/django-twilio-access-token`.
-        3. Run `$ ./scripts/requirement-install.sh` from your command line.
-        4. Run `$ source venv/bin/activate`.
-        5. Run `$ python manage.py runserver 0.0.0.0:8000` and enjoy the token API's.
-        
-        ## Get involved!
-        
-        We are happy to receive bug reports, fixes, documentation enhancements, and other improvements.
-        
-        Please report bugs via the github [issue tracker](https://github.com/senseobservationsystems/django-twilio-access-token/issues).
-        
-        Master git repository [django-twilio-access-token](https://github.com/senseobservationsystems/django-twilio-access-token).
 Keywords: django,twilio,access,token
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -66,7 +17,58 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+
+
+# django-twilio-access-token
+
+This is a Django application that can be used to generate Twilio access token for particular services, such as Voice, Chat, and Video.
+
+## Prerequisite
+
+### Twilio
+
+We use Twilio client for [python](https://www.twilio.com/docs/libraries/python#install-the-library) to generate an access token for Twilio services. To make the package works on your project, you need to install Twilio client either through [pip](https://pip.pypa.io/en/stable/) command;
+
+```
+pip install twilio
+```
+
+or simply add Twilio on your `requirements.txt`
+
+```
+twilio~=6.32.0
+```
+
+### Twilio keys
+
+In order to make the package works with your django project, you need to define the Twilio keys inside your project `settings.py`, for example:
+```
+TWILIO_ACCOUNT_SID = 'PUT_YOUR_TWILIO_ACCOUNT_SID_HERE'  # You can find Twilio Account SID at the top right section of this page https://www.twilio.com/console/
+
+TWILIO_VIDEO_API_KEY_SID = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SID_HERE'  # You can obtain these keys by creating it through https://www.twilio.com/console/video/project/api-keys/
+TWILIO_VIDEO_API_KEY_SECRET = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SECRET_HERE'
+```
+
+Or see the `test_project/test_app/settings.py` if you need to know more.
+
+## How to run the test project
+
+To try out the package, you can run our test application by following these steps:
+1. Ensure pip installed on your local machine. If you don't have it, you can follow the installation guide [here](https://pip.pypa.io/en/stable/installing/).
+2. Open terminal and go to the root directory of where the package live, for instance: `$ cd Documents/py-projects/django-twilio-access-token`.
+3. Run `$ ./scripts/requirement-install.sh` from your command line.
+4. Run `$ source venv/bin/activate`.
+5. Run `$ python manage.py runserver 0.0.0.0:8000` and enjoy the token API's.
+
+## Get involved!
+
+We are happy to receive bug reports, fixes, documentation enhancements, and other improvements.
+
+Please report bugs via the github [issue tracker](https://github.com/senseobservationsystems/django-twilio-access-token/issues).
+
+Master git repository [django-twilio-access-token](https://github.com/senseobservationsystems/django-twilio-access-token).
+
```

### Comparing `django-twilio-access-token-0.0.4/README.md` & `django-twilio-access-token-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django-twilio-access-token-0.0.4/django_twilio_access_token/serializers/twilio_access_token_serializer.py` & `django-twilio-access-token-0.0.5/django_twilio_access_token/serializers/twilio_access_token_serializer.py`

 * *Files identical despite different names*

### Comparing `django-twilio-access-token-0.0.4/django_twilio_access_token/serializers/twilio_room_serializer.py` & `django-twilio-access-token-0.0.5/django_twilio_access_token/serializers/twilio_room_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     GROUP_SMALL = 'group-small'
     GROUP_ROOM_CHOICES = (
         (GROUP, 'Group room can hold up to 50 participants.'),
         (GROUP_SMALL, 'Group small room can hold up to 4 participants.'),
     )
     record_participants_on_connect = serializers.BooleanField(default=False)
     type = serializers.ChoiceField(choices=GROUP_ROOM_CHOICES)
+    media_region = serializers.CharField(required=False)
 
 
 class PeerToPeerRoomDeserializer(BaseRoomDeserializer):
     """
     Deserializer that can be used to peer-to-peer Twilio Room via REST
     @see https://www.twilio.com/docs/video/api/rooms-resource#example-2-create-a-peer-to-peer-room-called-salesmeeting-with-network-traversal-service-turn-disabled-and-the-status-callback-url-set
     """
```

### Comparing `django-twilio-access-token-0.0.4/django_twilio_access_token/views/twilio_room_view.py` & `django-twilio-access-token-0.0.5/django_twilio_access_token/views/twilio_room_view.py`

 * *Files identical despite different names*

### Comparing `django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/PKG-INFO` & `django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,15 @@
 Metadata-Version: 2.1
 Name: django-twilio-access-token
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django app to generate Twilio access token for particular Twilio services.
 Home-page: https://github.com/senseobservationsystems/django-twilio-access-token/
 Author: Panji Y. Wiwaha
 Author-email: panjiyudasetya@gmail.com
 License: UNKNOWN
-Description: 
-        # django-twilio-access-token
-        
-        This is a Django application that can be used to generate Twilio access token for particular services, such as Voice, Chat, and Video.
-        
-        ## Prerequisite
-        
-        ### Twilio
-        
-        We use Twilio client for [python](https://www.twilio.com/docs/libraries/python#install-the-library) to generate an access token for Twilio services. To make the package works on your project, you need to install Twilio client either through [pip](https://pip.pypa.io/en/stable/) command;
-        
-        ```
-        pip install twilio
-        ```
-        
-        or simply add Twilio on your `requirements.txt`
-        
-        ```
-        twilio~=6.32.0
-        ```
-        
-        ### Twilio keys
-        
-        In order to make the package works with your django project, you need to define the Twilio keys inside your project `settings.py`, for example:
-        ```
-        TWILIO_ACCOUNT_SID = 'PUT_YOUR_TWILIO_ACCOUNT_SID_HERE'  # You can find Twilio Account SID at the top right section of this page https://www.twilio.com/console/
-        
-        TWILIO_VIDEO_API_KEY_SID = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SID_HERE'  # You can obtain these keys by creating it through https://www.twilio.com/console/video/project/api-keys/
-        TWILIO_VIDEO_API_KEY_SECRET = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SECRET_HERE'
-        ```
-        
-        Or see the `test_project/test_app/settings.py` if you need to know more.
-        
-        ## How to run the test project
-        
-        To try out the package, you can run our test application by following these steps:
-        1. Ensure pip installed on your local machine. If you don't have it, you can follow the installation guide [here](https://pip.pypa.io/en/stable/installing/).
-        2. Open terminal and go to the root directory of where the package live, for instance: `$ cd Documents/py-projects/django-twilio-access-token`.
-        3. Run `$ ./scripts/requirement-install.sh` from your command line.
-        4. Run `$ source venv/bin/activate`.
-        5. Run `$ python manage.py runserver 0.0.0.0:8000` and enjoy the token API's.
-        
-        ## Get involved!
-        
-        We are happy to receive bug reports, fixes, documentation enhancements, and other improvements.
-        
-        Please report bugs via the github [issue tracker](https://github.com/senseobservationsystems/django-twilio-access-token/issues).
-        
-        Master git repository [django-twilio-access-token](https://github.com/senseobservationsystems/django-twilio-access-token).
 Keywords: django,twilio,access,token
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -66,7 +17,58 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+
+
+# django-twilio-access-token
+
+This is a Django application that can be used to generate Twilio access token for particular services, such as Voice, Chat, and Video.
+
+## Prerequisite
+
+### Twilio
+
+We use Twilio client for [python](https://www.twilio.com/docs/libraries/python#install-the-library) to generate an access token for Twilio services. To make the package works on your project, you need to install Twilio client either through [pip](https://pip.pypa.io/en/stable/) command;
+
+```
+pip install twilio
+```
+
+or simply add Twilio on your `requirements.txt`
+
+```
+twilio~=6.32.0
+```
+
+### Twilio keys
+
+In order to make the package works with your django project, you need to define the Twilio keys inside your project `settings.py`, for example:
+```
+TWILIO_ACCOUNT_SID = 'PUT_YOUR_TWILIO_ACCOUNT_SID_HERE'  # You can find Twilio Account SID at the top right section of this page https://www.twilio.com/console/
+
+TWILIO_VIDEO_API_KEY_SID = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SID_HERE'  # You can obtain these keys by creating it through https://www.twilio.com/console/video/project/api-keys/
+TWILIO_VIDEO_API_KEY_SECRET = 'PUT_YOUR_TWILIO_VIDEO_API_KEY_SECRET_HERE'
+```
+
+Or see the `test_project/test_app/settings.py` if you need to know more.
+
+## How to run the test project
+
+To try out the package, you can run our test application by following these steps:
+1. Ensure pip installed on your local machine. If you don't have it, you can follow the installation guide [here](https://pip.pypa.io/en/stable/installing/).
+2. Open terminal and go to the root directory of where the package live, for instance: `$ cd Documents/py-projects/django-twilio-access-token`.
+3. Run `$ ./scripts/requirement-install.sh` from your command line.
+4. Run `$ source venv/bin/activate`.
+5. Run `$ python manage.py runserver 0.0.0.0:8000` and enjoy the token API's.
+
+## Get involved!
+
+We are happy to receive bug reports, fixes, documentation enhancements, and other improvements.
+
+Please report bugs via the github [issue tracker](https://github.com/senseobservationsystems/django-twilio-access-token/issues).
+
+Master git repository [django-twilio-access-token](https://github.com/senseobservationsystems/django-twilio-access-token).
+
```

### Comparing `django-twilio-access-token-0.0.4/django_twilio_access_token.egg-info/SOURCES.txt` & `django-twilio-access-token-0.0.5/django_twilio_access_token.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-twilio-access-token-0.0.4/setup.py` & `django-twilio-access-token-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-twilio-access-token",
-    version="0.0.4",
+    version="0.0.5",
     author="Panji Y. Wiwaha",
     author_email="panjiyudasetya@gmail.com",
     description="A Django app to generate Twilio access token for particular Twilio services.",
     keywords=['django', 'twilio', 'access', 'token'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/senseobservationsystems/django-twilio-access-token/",
```

