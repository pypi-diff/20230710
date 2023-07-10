# Comparing `tmp/django-allow-cidr-0.6.0.tar.gz` & `tmp/django-allow-cidr-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-allow-cidr-0.6.0.tar", last modified: Thu Jan  5 10:03:25 2023, max compression
+gzip compressed data, was "django-allow-cidr-0.7.0.tar", last modified: Mon Jul 10 12:28:00 2023, max compression
```

## Comparing `django-allow-cidr-0.6.0.tar` & `django-allow-cidr-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:03:25.260041 django-allow-cidr-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-01-05 10:03:25.260041 django-allow-cidr-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:03:25.260041 django-allow-cidr-0.6.0/allow_cidr/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/allow_cidr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/allow_cidr/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/allow_cidr/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:03:25.260041 django-allow-cidr-0.6.0/django_allow_cidr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-01-05 10:03:25.000000 django-allow-cidr-0.6.0/django_allow_cidr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-05 10:03:25.000000 django-allow-cidr-0.6.0/django_allow_cidr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 10:03:25.000000 django-allow-cidr-0.6.0/django_allow_cidr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 10:03:24.000000 django-allow-cidr-0.6.0/django_allow_cidr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-05 10:03:25.000000 django-allow-cidr-0.6.0/django_allow_cidr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-05 10:03:25.000000 django-allow-cidr-0.6.0/django_allow_cidr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-05 10:03:25.260041 django-allow-cidr-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1936 2023-01-05 10:03:03.000000 django-allow-cidr-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/allow_cidr/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/allow_cidr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/allow_cidr/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/allow_cidr/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1936 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/tests/test_middleware.py
```

### Comparing `django-allow-cidr-0.6.0/CONTRIBUTING.rst` & `django-allow-cidr-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.6.0/HISTORY.rst` & `django-allow-cidr-0.7.0/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. :changelog:
 
 History
 -------
 
+0.7.0 (2023-07-10)
+++++++++++++++++++
+
+* Add IPv6 support - thanks @rissson!
+* Add Django 4.2 to CI; freshen up CI config
+
+
 0.6.0 (2023-01-05)
 ++++++++++++++++++
 
 * Drop dev-related dependencies (incl vulnerable version of wheel, which was not installed in general use)
 * Remove redundant code from setup.py now we're auto-publishing via Github
 * Update testing matrix: Drop Python 3.6; add Python 3.11; add Django 4.1
```

### Comparing `django-allow-cidr-0.6.0/LICENSE` & `django-allow-cidr-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.6.0/PKG-INFO` & `django-allow-cidr-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allow-cidr
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Django Middleware to enable use of CIDR IP ranges in ALLOWED_HOSTS.
 Home-page: https://github.com/mozmeao/django-allow-cidr
 Author: Paul McLanahan
 Author-email: pmac@mozilla.com
 License: Apache Software License 2.0
 Keywords: django-allow-cidr
 Classifier: Development Status :: 4 - Beta
@@ -103,14 +103,21 @@
 
 
 
 
 History
 -------
 
+0.7.0 (2023-07-10)
+++++++++++++++++++
+
+* Add IPv6 support - thanks @rissson!
+* Add Django 4.2 to CI; freshen up CI config
+
+
 0.6.0 (2023-01-05)
 ++++++++++++++++++
 
 * Drop dev-related dependencies (incl vulnerable version of wheel, which was not installed in general use)
 * Remove redundant code from setup.py now we're auto-publishing via Github
 * Update testing matrix: Drop Python 3.6; add Python 3.11; add Django 4.1
```

### Comparing `django-allow-cidr-0.6.0/README.rst` & `django-allow-cidr-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.6.0/allow_cidr/middleware.py` & `django-allow-cidr-0.7.0/allow_cidr/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 from django.http.request import split_domain_port, validate_host
 
 ORIG_ALLOWED_HOSTS = []
 
 
 class AllowCIDRMiddleware:
     def __init__(self, get_response, *args, **kwargs):
-
         self.get_response = get_response
 
         if Version(django.get_version()) < Version("2.2"):
             raise NotImplementedError(
                 "This version of django-allow-cidr requires at least Django 2.2"
             )
 
         super(AllowCIDRMiddleware, self).__init__(*args, **kwargs)
 
         allowed_cidr_nets = getattr(settings, "ALLOWED_CIDR_NETS", None)
 
         if not allowed_cidr_nets:
             raise MiddlewareNotUsed()
 
-        self.allowed_cidr_nets = [ipaddress.ip_network(net) for net in allowed_cidr_nets]
+        self.allowed_cidr_nets = [
+            ipaddress.ip_network(net) for net in allowed_cidr_nets
+        ]
         if settings.ALLOWED_HOSTS != ["*"]:
             # add them to a global so that we keep the original setting
             # for multiple instances of the middleware.
             ORIG_ALLOWED_HOSTS.extend(settings.ALLOWED_HOSTS)
             settings.ALLOWED_HOSTS = ["*"]
         elif not ORIG_ALLOWED_HOSTS:
             # ALLOWED_HOSTS was originally set to '*' so no checking is necessary
@@ -43,14 +44,17 @@
     def __call__(self, request):
         # Processing the request before we generate the response
         host = request.get_host()
         domain, port = split_domain_port(host)
 
         if not domain or not validate_host(domain, ORIG_ALLOWED_HOSTS):
             should_raise = True
+            if domain and domain[-1] == "]":
+                # It's an IPv6, ignore beginning [ and end ]
+                domain = domain[1:-1]
             for net in self.allowed_cidr_nets:
                 try:
                     if ipaddress.ip_address(domain) in net:
                         should_raise = False
                         break
                 except ValueError:
                     # not an IP
```

### Comparing `django-allow-cidr-0.6.0/django_allow_cidr.egg-info/PKG-INFO` & `django-allow-cidr-0.7.0/django_allow_cidr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allow-cidr
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Django Middleware to enable use of CIDR IP ranges in ALLOWED_HOSTS.
 Home-page: https://github.com/mozmeao/django-allow-cidr
 Author: Paul McLanahan
 Author-email: pmac@mozilla.com
 License: Apache Software License 2.0
 Keywords: django-allow-cidr
 Classifier: Development Status :: 4 - Beta
@@ -103,14 +103,21 @@
 
 
 
 
 History
 -------
 
+0.7.0 (2023-07-10)
+++++++++++++++++++
+
+* Add IPv6 support - thanks @rissson!
+* Add Django 4.2 to CI; freshen up CI config
+
+
 0.6.0 (2023-01-05)
 ++++++++++++++++++
 
 * Drop dev-related dependencies (incl vulnerable version of wheel, which was not installed in general use)
 * Remove redundant code from setup.py now we're auto-publishing via Github
 * Update testing matrix: Drop Python 3.6; add Python 3.11; add Django 4.1
```

### Comparing `django-allow-cidr-0.6.0/setup.py` & `django-allow-cidr-0.7.0/setup.py`

 * *Files identical despite different names*

