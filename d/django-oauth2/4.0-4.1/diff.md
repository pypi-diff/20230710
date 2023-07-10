# Comparing `tmp/django-oauth2-4.0.tar.gz` & `tmp/django-oauth2-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oauth2-4.0.tar", last modified: Sat Feb  4 19:33:53 2023, max compression
+gzip compressed data, was "django-oauth2-4.1.tar", last modified: Mon Jul 10 04:13:12 2023, max compression
```

## Comparing `django-oauth2-4.0.tar` & `django-oauth2-4.1.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.395874 django-oauth2-4.0/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1058 2019-01-05 07:26:42.000000 django-oauth2-4.0/LICENSE
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      155 2019-01-05 07:26:42.000000 django-oauth2-4.0/MANIFEST.in
--rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)     1198 2023-02-04 19:33:53.394898 django-oauth2-4.0/PKG-INFO
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      467 2019-01-07 06:48:00.000000 django-oauth2-4.0/README.rst
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.322912 django-oauth2-4.0/django_oauth2.egg-info/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1198 2023-02-04 19:33:53.000000 django-oauth2-4.0/django_oauth2.egg-info/PKG-INFO
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1254 2023-02-04 19:33:53.000000 django-oauth2-4.0/django_oauth2.egg-info/SOURCES.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        1 2023-02-04 19:33:53.000000 django-oauth2-4.0/django_oauth2.egg-info/dependency_links.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        1 2019-01-05 07:48:18.000000 django-oauth2-4.0/django_oauth2.egg-info/not-zip-safe
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)       46 2023-02-04 19:33:53.000000 django-oauth2-4.0/django_oauth2.egg-info/requires.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        9 2023-02-04 19:33:53.000000 django-oauth2-4.0/django_oauth2.egg-info/top_level.txt
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.341456 django-oauth2-4.0/provider/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)       97 2023-02-04 19:21:17.000000 django-oauth2-4.0/provider/__init__.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.343408 django-oauth2-4.0/provider/compat/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      254 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/compat/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1230 2019-01-07 06:27:25.000000 django-oauth2-4.0/provider/constants.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     2007 2019-01-07 06:27:25.000000 django-oauth2-4.0/provider/forms.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)       57 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/models.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.365618 django-oauth2-4.0/provider/oauth2/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)       51 2019-01-07 06:27:25.000000 django-oauth2-4.0/provider/oauth2/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      944 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/oauth2/admin.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      147 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/oauth2/apps.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     3408 2020-10-08 05:13:28.000000 django-oauth2-4.0/provider/oauth2/backends.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.367570 django-oauth2-4.0/provider/oauth2/fixtures/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     2703 2020-10-08 05:13:28.000000 django-oauth2-4.0/provider/oauth2/fixtures/test_oauth2.json
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)    11531 2023-02-03 16:42:17.000000 django-oauth2-4.0/provider/oauth2/forms.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     3296 2020-10-08 05:13:28.000000 django-oauth2-4.0/provider/oauth2/middleware.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.375378 django-oauth2-4.0/provider/oauth2/migrations/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     6448 2019-01-07 06:27:25.000000 django-oauth2-4.0/provider/oauth2/migrations/0001_initial.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1363 2019-08-17 05:05:49.000000 django-oauth2-4.0/provider/oauth2/migrations/0002_fix_scope_size.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      655 2020-10-08 05:13:28.000000 django-oauth2-4.0/provider/oauth2/migrations/0003_public_client_options.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/oauth2/migrations/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1095 2019-07-30 05:33:40.000000 django-oauth2-4.0/provider/oauth2/mixins.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     8709 2020-10-08 05:13:28.000000 django-oauth2-4.0/provider/oauth2/models.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.383185 django-oauth2-4.0/provider/oauth2/tests/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2019-07-30 05:33:40.000000 django-oauth2-4.0/provider/oauth2/tests/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     3211 2019-07-30 05:33:40.000000 django-oauth2-4.0/provider/oauth2/tests/test_middleware.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)    25523 2020-10-08 05:50:30.000000 django-oauth2-4.0/provider/oauth2/tests/test_views.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1158 2023-02-03 16:45:00.000000 django-oauth2-4.0/provider/oauth2/tests/urls.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1745 2023-02-03 16:39:37.000000 django-oauth2-4.0/provider/oauth2/urls.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     5597 2020-10-08 05:50:55.000000 django-oauth2-4.0/provider/oauth2/views.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     2438 2019-01-07 06:27:25.000000 django-oauth2-4.0/provider/scope.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1104 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/sphinx.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.303392 django-oauth2-4.0/provider/templates/
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.385137 django-oauth2-4.0/provider/templates/provider/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1680 2020-10-08 05:13:28.000000 django-oauth2-4.0/provider/templates/provider/authorize.html
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.389041 django-oauth2-4.0/provider/templatetags/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/templatetags/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      283 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/templatetags/scope.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-02-04 19:33:53.392946 django-oauth2-4.0/provider/tests/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/tests/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      151 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/tests/test_utils.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2019-01-05 07:26:42.000000 django-oauth2-4.0/provider/urls.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1331 2019-01-07 06:27:25.000000 django-oauth2-4.0/provider/utils.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)    21121 2023-02-03 16:42:17.000000 django-oauth2-4.0/provider/views.py
--rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)       38 2023-02-04 19:33:53.395874 django-oauth2-4.0/setup.cfg
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     1016 2023-02-03 06:41:09.000000 django-oauth2-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.703464 django-oauth2-4.1/
+-rw-rw-rw-   0        0        0     1058 2019-01-05 07:26:42.000000 django-oauth2-4.1/LICENSE
+-rw-rw-rw-   0        0        0      155 2023-07-10 04:13:09.000000 django-oauth2-4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1130 2023-07-10 04:13:12.703464 django-oauth2-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2019-01-07 06:48:00.000000 django-oauth2-4.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.651045 django-oauth2-4.1/django_oauth2.egg-info/
+-rw-rw-rw-   0        0        0     1130 2023-07-10 04:13:12.000000 django-oauth2-4.1/django_oauth2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1453 2023-07-10 04:13:12.000000 django-oauth2-4.1/django_oauth2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 04:13:12.000000 django-oauth2-4.1/django_oauth2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2019-01-05 07:48:18.000000 django-oauth2-4.1/django_oauth2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-10 04:13:12.000000 django-oauth2-4.1/django_oauth2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 04:13:12.000000 django-oauth2-4.1/django_oauth2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.660021 django-oauth2-4.1/provider/
+-rw-rw-rw-   0        0        0       97 2023-07-10 03:45:28.000000 django-oauth2-4.1/provider/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.662015 django-oauth2-4.1/provider/compat/
+-rw-rw-rw-   0        0        0      254 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/compat/__init__.py
+-rw-rw-rw-   0        0        0     1230 2019-01-07 06:27:25.000000 django-oauth2-4.1/provider/constants.py
+-rw-rw-rw-   0        0        0     2007 2019-01-07 06:27:25.000000 django-oauth2-4.1/provider/forms.py
+-rw-rw-rw-   0        0        0       57 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/models.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.674542 django-oauth2-4.1/provider/oauth2/
+-rw-rw-rw-   0        0        0       51 2019-01-07 06:27:25.000000 django-oauth2-4.1/provider/oauth2/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-07-10 03:18:40.000000 django-oauth2-4.1/provider/oauth2/admin.py
+-rw-rw-rw-   0        0        0      147 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/oauth2/apps.py
+-rw-rw-rw-   0        0        0     3408 2020-10-08 05:13:28.000000 django-oauth2-4.1/provider/oauth2/backends.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.675540 django-oauth2-4.1/provider/oauth2/fixtures/
+-rw-rw-rw-   0        0        0     2703 2020-10-08 05:13:28.000000 django-oauth2-4.1/provider/oauth2/fixtures/test_oauth2.json
+-rw-rw-rw-   0        0        0    11531 2023-07-10 03:18:34.000000 django-oauth2-4.1/provider/oauth2/forms.py
+-rw-rw-rw-   0        0        0     3296 2020-10-08 05:13:28.000000 django-oauth2-4.1/provider/oauth2/middleware.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.685513 django-oauth2-4.1/provider/oauth2/migrations/
+-rw-rw-rw-   0        0        0     6448 2019-01-07 06:27:25.000000 django-oauth2-4.1/provider/oauth2/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1363 2019-08-17 05:05:49.000000 django-oauth2-4.1/provider/oauth2/migrations/0002_fix_scope_size.py
+-rw-rw-rw-   0        0        0      655 2020-10-08 05:13:28.000000 django-oauth2-4.1/provider/oauth2/migrations/0003_public_client_options.py
+-rw-rw-rw-   0        0        0     3454 2023-07-10 03:30:18.000000 django-oauth2-4.1/provider/oauth2/migrations/0004_temp_scopes.py
+-rw-rw-rw-   0        0        0      742 2023-07-10 03:43:42.000000 django-oauth2-4.1/provider/oauth2/migrations/0005_delete_scope.py
+-rw-rw-rw-   0        0        0     3350 2023-07-10 03:38:06.000000 django-oauth2-4.1/provider/oauth2/migrations/0006_recreate_scope.py
+-rw-rw-rw-   0        0        0      654 2023-07-10 03:39:53.000000 django-oauth2-4.1/provider/oauth2/migrations/0007_remove_temp_scopes.py
+-rw-rw-rw-   0        0        0        0 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/oauth2/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1095 2019-07-30 05:33:40.000000 django-oauth2-4.1/provider/oauth2/mixins.py
+-rw-rw-rw-   0        0        0     8758 2023-07-10 03:43:08.000000 django-oauth2-4.1/provider/oauth2/models.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.689503 django-oauth2-4.1/provider/oauth2/tests/
+-rw-rw-rw-   0        0        0        0 2019-07-30 05:33:40.000000 django-oauth2-4.1/provider/oauth2/tests/__init__.py
+-rw-rw-rw-   0        0        0     3211 2019-07-30 05:33:40.000000 django-oauth2-4.1/provider/oauth2/tests/test_middleware.py
+-rw-rw-rw-   0        0        0    25523 2020-10-08 05:50:30.000000 django-oauth2-4.1/provider/oauth2/tests/test_views.py
+-rw-rw-rw-   0        0        0     1158 2023-02-03 16:45:00.000000 django-oauth2-4.1/provider/oauth2/tests/urls.py
+-rw-rw-rw-   0        0        0     1745 2023-02-03 16:39:37.000000 django-oauth2-4.1/provider/oauth2/urls.py
+-rw-rw-rw-   0        0        0     5597 2020-10-08 05:50:55.000000 django-oauth2-4.1/provider/oauth2/views.py
+-rw-rw-rw-   0        0        0     2438 2019-01-07 06:27:25.000000 django-oauth2-4.1/provider/scope.py
+-rw-rw-rw-   0        0        0     1104 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/sphinx.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.639077 django-oauth2-4.1/provider/templates/
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.691496 django-oauth2-4.1/provider/templates/provider/
+-rw-rw-rw-   0        0        0     1680 2020-10-08 05:13:28.000000 django-oauth2-4.1/provider/templates/provider/authorize.html
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.699475 django-oauth2-4.1/provider/templatetags/
+-rw-rw-rw-   0        0        0        0 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      283 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/templatetags/scope.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:13:12.701471 django-oauth2-4.1/provider/tests/
+-rw-rw-rw-   0        0        0        0 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/tests/__init__.py
+-rw-rw-rw-   0        0        0      151 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/tests/test_utils.py
+-rw-rw-rw-   0        0        0        0 2019-01-05 07:26:42.000000 django-oauth2-4.1/provider/urls.py
+-rw-rw-rw-   0        0        0     1331 2019-01-07 06:27:25.000000 django-oauth2-4.1/provider/utils.py
+-rw-rw-rw-   0        0        0    21121 2023-02-03 16:42:17.000000 django-oauth2-4.1/provider/views.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 04:13:12.703464 django-oauth2-4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-02-03 06:41:09.000000 django-oauth2-4.1/setup.py
```

### Comparing `django-oauth2-4.0/LICENSE` & `django-oauth2-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/PKG-INFO` & `django-oauth2-4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-Metadata-Version: 1.1
-Name: django-oauth2
-Version: 4.0
-Summary: Provide OAuth2 access to your app (fork of django-oauth2-provider)
-Home-page: https://github.com/stormsherpa/django-oauth2-provider
-Author: Shaun Kruger
-Author-email: shaun.kruger@gmail.com
-License: The MIT License: http://www.opensource.org/licenses/mit-license.php
-Description: django-oauth2
-        ======================
-        
-        .. image:: https://travis-ci.org/stormsherpa/django-oauth2-provider.png?branch=master
-        
-        *django-oauth2* is a Django application that provides
-        customizable OAuth2\-authentication for your Django projects.
-        
-        `Documentation <https://new-django-oauth2.readthedocs.io/en/latest/>`_
-        
-        License
-        =======
-        
-        *django-oauth2* is a fork of *django-oauth2-provider* which is released under the MIT License. Please see the LICENSE file for details.
-        
-Platform: all
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Framework :: Django
+Metadata-Version: 2.1
+Name: django-oauth2
+Version: 4.1
+Summary: Provide OAuth2 access to your app (fork of django-oauth2-provider)
+Home-page: https://github.com/stormsherpa/django-oauth2-provider
+Author: Shaun Kruger
+Author-email: shaun.kruger@gmail.com
+License: The MIT License: http://www.opensource.org/licenses/mit-license.php
+Platform: all
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Framework :: Django
+License-File: LICENSE
+
+django-oauth2
+======================
+
+.. image:: https://travis-ci.org/stormsherpa/django-oauth2-provider.png?branch=master
+
+*django-oauth2* is a Django application that provides
+customizable OAuth2\-authentication for your Django projects.
+
+`Documentation <https://new-django-oauth2.readthedocs.io/en/latest/>`_
+
+License
+=======
+
+*django-oauth2* is a fork of *django-oauth2-provider* which is released under the MIT License. Please see the LICENSE file for details.
+
+
```

### Comparing `django-oauth2-4.0/django_oauth2.egg-info/PKG-INFO` & `django-oauth2-4.1/django_oauth2.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-Metadata-Version: 1.1
-Name: django-oauth2
-Version: 4.0
-Summary: Provide OAuth2 access to your app (fork of django-oauth2-provider)
-Home-page: https://github.com/stormsherpa/django-oauth2-provider
-Author: Shaun Kruger
-Author-email: shaun.kruger@gmail.com
-License: The MIT License: http://www.opensource.org/licenses/mit-license.php
-Description: django-oauth2
-        ======================
-        
-        .. image:: https://travis-ci.org/stormsherpa/django-oauth2-provider.png?branch=master
-        
-        *django-oauth2* is a Django application that provides
-        customizable OAuth2\-authentication for your Django projects.
-        
-        `Documentation <https://new-django-oauth2.readthedocs.io/en/latest/>`_
-        
-        License
-        =======
-        
-        *django-oauth2* is a fork of *django-oauth2-provider* which is released under the MIT License. Please see the LICENSE file for details.
-        
-Platform: all
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Framework :: Django
+Metadata-Version: 2.1
+Name: django-oauth2
+Version: 4.1
+Summary: Provide OAuth2 access to your app (fork of django-oauth2-provider)
+Home-page: https://github.com/stormsherpa/django-oauth2-provider
+Author: Shaun Kruger
+Author-email: shaun.kruger@gmail.com
+License: The MIT License: http://www.opensource.org/licenses/mit-license.php
+Platform: all
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Framework :: Django
+License-File: LICENSE
+
+django-oauth2
+======================
+
+.. image:: https://travis-ci.org/stormsherpa/django-oauth2-provider.png?branch=master
+
+*django-oauth2* is a Django application that provides
+customizable OAuth2\-authentication for your Django projects.
+
+`Documentation <https://new-django-oauth2.readthedocs.io/en/latest/>`_
+
+License
+=======
+
+*django-oauth2* is a fork of *django-oauth2-provider* which is released under the MIT License. Please see the LICENSE file for details.
+
+
```

### Comparing `django-oauth2-4.0/django_oauth2.egg-info/SOURCES.txt` & `django-oauth2-4.1/django_oauth2.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 provider/oauth2/models.py
 provider/oauth2/urls.py
 provider/oauth2/views.py
 provider/oauth2/fixtures/test_oauth2.json
 provider/oauth2/migrations/0001_initial.py
 provider/oauth2/migrations/0002_fix_scope_size.py
 provider/oauth2/migrations/0003_public_client_options.py
+provider/oauth2/migrations/0004_temp_scopes.py
+provider/oauth2/migrations/0005_delete_scope.py
+provider/oauth2/migrations/0006_recreate_scope.py
+provider/oauth2/migrations/0007_remove_temp_scopes.py
 provider/oauth2/migrations/__init__.py
 provider/oauth2/tests/__init__.py
 provider/oauth2/tests/test_middleware.py
 provider/oauth2/tests/test_views.py
 provider/oauth2/tests/urls.py
 provider/templates/provider/authorize.html
 provider/templatetags/__init__.py
```

### Comparing `django-oauth2-4.0/provider/constants.py` & `django-oauth2-4.1/provider/constants.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/forms.py` & `django-oauth2-4.1/provider/forms.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/admin.py` & `django-oauth2-4.1/provider/oauth2/admin.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/backends.py` & `django-oauth2-4.1/provider/oauth2/backends.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/fixtures/test_oauth2.json` & `django-oauth2-4.1/provider/oauth2/fixtures/test_oauth2.json`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/forms.py` & `django-oauth2-4.1/provider/oauth2/forms.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/middleware.py` & `django-oauth2-4.1/provider/oauth2/middleware.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/migrations/0001_initial.py` & `django-oauth2-4.1/provider/oauth2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/migrations/0002_fix_scope_size.py` & `django-oauth2-4.1/provider/oauth2/migrations/0002_fix_scope_size.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/migrations/0003_public_client_options.py` & `django-oauth2-4.1/provider/oauth2/migrations/0003_public_client_options.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/mixins.py` & `django-oauth2-4.1/provider/oauth2/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/models.py` & `django-oauth2-4.1/provider/oauth2/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     class Meta:
         app_label = 'oauth2'
         db_table = 'oauth2_client'
 
 
 class Scope(models.Model):
-    name = models.CharField(max_length=50, primary_key=True)
+    name = models.CharField(max_length=150, primary_key=True)  # This length can't change due to a django bug
     description = models.CharField(max_length=256, default='', blank=True)
 
     def __unicode__(self):
         return self.name
 
     class Meta:
         app_label = 'oauth2'
```

### Comparing `django-oauth2-4.0/provider/oauth2/tests/test_middleware.py` & `django-oauth2-4.1/provider/oauth2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/tests/test_views.py` & `django-oauth2-4.1/provider/oauth2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/tests/urls.py` & `django-oauth2-4.1/provider/oauth2/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/urls.py` & `django-oauth2-4.1/provider/oauth2/urls.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/oauth2/views.py` & `django-oauth2-4.1/provider/oauth2/views.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/scope.py` & `django-oauth2-4.1/provider/scope.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/sphinx.py` & `django-oauth2-4.1/provider/sphinx.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/templates/provider/authorize.html` & `django-oauth2-4.1/provider/templates/provider/authorize.html`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/utils.py` & `django-oauth2-4.1/provider/utils.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/provider/views.py` & `django-oauth2-4.1/provider/views.py`

 * *Files identical despite different names*

### Comparing `django-oauth2-4.0/setup.py` & `django-oauth2-4.1/setup.py`

 * *Files identical despite different names*

