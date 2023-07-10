# Comparing `tmp/nginx-set-conf-equitania-0.9.0.tar.gz` & `tmp/nginx-set-conf-equitania-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.9.0.tar", last modified: Mon Jul 10 09:33:10 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.9.1.tar", last modified: Mon Jul 10 13:52:44 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.9.0.tar` & `nginx-set-conf-equitania-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 09:33:10.976610 nginx-set-conf-equitania-0.9.0/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.0/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 09:33:10.976482 nginx-set-conf-equitania-0.9.0/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2861 2023-07-10 09:23:12.000000 nginx-set-conf-equitania-0.9.0/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 09:33:10.975491 nginx-set-conf-equitania-0.9.0/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    20241 2023-07-10 09:15:04.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     3951 2023-07-10 09:23:47.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 09:33:10.976326 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-07-10 09:33:10.976651 nginx-set-conf-equitania-0.9.0/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      880 2023-07-10 09:27:03.000000 nginx-set-conf-equitania-0.9.0/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 13:52:44.331231 nginx-set-conf-equitania-0.9.1/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.1/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 13:52:44.331107 nginx-set-conf-equitania-0.9.1/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2861 2023-07-10 09:23:12.000000 nginx-set-conf-equitania-0.9.1/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 13:52:44.330117 nginx-set-conf-equitania-0.9.1/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    19837 2023-07-10 13:52:00.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     3951 2023-07-10 09:23:47.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 13:52:44.330951 nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 13:52:44.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-07-10 13:52:44.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-07-10 13:52:44.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-07-10 13:52:44.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-07-10 13:52:44.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-07-10 13:52:44.000000 nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-07-10 13:52:44.331267 nginx-set-conf-equitania-0.9.1/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      880 2023-07-10 13:00:48.000000 nginx-set-conf-equitania-0.9.1/setup.py
```

### Comparing `nginx-set-conf-equitania-0.9.0/LICENSE.txt` & `nginx-set-conf-equitania-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.0/PKG-INFO` & `nginx-set-conf-equitania-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.9.0/README.md` & `nginx-set-conf-equitania-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.0/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.9.1/nginx_set_conf/config_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,14 @@
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
-    ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
 
     # security
     include                 nginxconfig.io/security.conf;
 
     # additional config
     include                 nginxconfig.io/general.conf;
@@ -98,17 +95,14 @@
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
-    ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
 
     index index.html;
 
     # set max upload size
     client_max_body_size 10G;
     fastcgi_buffers 64 4K;
@@ -172,16 +166,14 @@
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
     ssl_session_timeout  5m;
 
     # Path to the root of your installation
     #root /var/www/owncloud/;
     root /var/www/nextcloud/;
     index index.html;
 
@@ -256,16 +248,14 @@
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
     ssl_session_timeout  5m;
 
     # security
     include                 nginxconfig.io/security.conf;
 
     # additional config
     include                 nginxconfig.io/general.conf;
@@ -381,22 +371,19 @@
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
-    # add ssl specific settings
+        # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
-    ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
 
     # increase proxy buffer to handle some Odoo web requests
     proxy_buffers 16 64k;
     proxy_buffer_size 128k;
     proxy_headers_hash_max_size 76800;
     proxy_headers_hash_bucket_size 9600;
@@ -479,17 +466,14 @@
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
-    ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
@@ -544,17 +528,14 @@
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
-    ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
 
     index index.html;
 
     #general proxy settings
     # force timeouts if the backend dies
     proxy_connect_timeout 1200s;
@@ -641,17 +622,14 @@
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
-    ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
 
     # additional config
     include                 nginxconfig.io/general.conf;
 }
 """
 }
```

### Comparing `nginx-set-conf-equitania-0.9.0/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.9.1/nginx_set_conf/nginx_set_conf.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.0/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.9.1/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.9.1/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.9.0/setup.py` & `nginx-set-conf-equitania-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.9.0",
+    version="0.9.1",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
```

