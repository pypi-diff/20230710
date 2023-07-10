# Comparing `tmp/nginx-set-conf-equitania-0.8.3.tar.gz` & `tmp/nginx-set-conf-equitania-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.8.3.tar", last modified: Thu Jun  1 11:54:45 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.9.0.tar", last modified: Mon Jul 10 09:33:10 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.8.3.tar` & `nginx-set-conf-equitania-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-06-01 11:54:45.594727 nginx-set-conf-equitania-0.8.3/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.8.3/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-06-01 11:54:45.594399 nginx-set-conf-equitania-0.8.3/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.8.3/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-06-01 11:54:45.589441 nginx-set-conf-equitania-0.8.3/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    21092 2023-05-25 09:54:50.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     4006 2023-05-02 13:29:17.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-06-01 11:54:45.593795 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-06-01 11:54:45.594819 nginx-set-conf-equitania-0.8.3/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      903 2023-06-01 11:54:09.000000 nginx-set-conf-equitania-0.8.3/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 09:33:10.976610 nginx-set-conf-equitania-0.9.0/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.0/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 09:33:10.976482 nginx-set-conf-equitania-0.9.0/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2861 2023-07-10 09:23:12.000000 nginx-set-conf-equitania-0.9.0/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 09:33:10.975491 nginx-set-conf-equitania-0.9.0/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    20241 2023-07-10 09:15:04.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     3951 2023-07-10 09:23:47.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 09:33:10.976326 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-07-10 09:33:10.000000 nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-07-10 09:33:10.976651 nginx-set-conf-equitania-0.9.0/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      880 2023-07-10 09:27:03.000000 nginx-set-conf-equitania-0.9.0/setup.py
```

### Comparing `nginx-set-conf-equitania-0.8.3/LICENSE.txt` & `nginx-set-conf-equitania-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.3/PKG-INFO` & `nginx-set-conf-equitania-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.3
-Summary: A package to create configurations for nginx with/without pagespeed for different web applications
+Version: 0.9.0
+Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -44,15 +44,14 @@
                           We support:
 
                           - ngx_code_server (code-server with ssl)
                           - ngx_fast_report (FastReport with ssl)
                           - ngx_nextcloud (NextCloud with ssl)
                           - ngx_odoo_http (Odoo only http)
                           - ngx_odoo_ssl (Odoo with ssl)
-                          - ngx_odoo_ssl_pagespeed (Odoo with ssl and PageSpeed)
                           - ngx_pgadmin (pgAdmin4 with ssl)
                           - ngx_portainer (NextCloud with ssl)
                           - ngx_pwa (Progressive Web App with ssl)
                           - ngx_redirect (Redirect Domain without ssl)
                           - ngx_redirect_ssl (Redirect Domain with ssl)
   --ip TEXT               IP address of the server
   --domain TEXT           Name of the domain
@@ -70,20 +69,22 @@
 ```bash
 # Execution with config file
 nginx-set-conf --config_path server_config
 f.e.
 nginx-set-conf --config_path=$HOME/docker-builds/ngx-conf
   
 # Execution without config file
-nginx-set-conf --config_template ngx_odoo_ssl_pagespeed --ip 1.2.3.4 --domain www.equitania.de --port 8069 --cert_name www.equitania.de --pollport 8072 
+nginx-set-conf --config_template ngx_odoo_ssl --ip 1.2.3.4 --domain www.equitania.de --port 8069 --cert_name www.equitania.de --pollport 8072 
 
 # Create your cert with
 certbot certonly --standalone --agree-tos --register-unsafely-without-email -d www.equitania.de
-# Install certbot on Ubuntu with
+# Install certbot on Debian/Ubuntu with
 apt-get install certbot
 ```
   
-## Compile your nginx with PageSpeed   
+## nginx template settings  
   
-At github you can find the script to do that: [nginx build script](https://github.com/equitania/myodoo-docker/tree/2022/scripts/build_nginx)  
+You can download our settings: [nginx.conf](https://rm.ownerp.io/staff/nginx.conf)  
+and the : [nginxconfig.io.zip](https://rm.ownerp.io/staff/nginxconfig.io.zip)  
+based on [https://www.digitalocean.com/community/tools/nginx](https://www.digitalocean.com/community/tools/nginx)  
   
 This project is licensed under the terms of the **AGPLv3** license.
```

### Comparing `nginx-set-conf-equitania-0.8.3/README.md` & `nginx-set-conf-equitania-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,14 @@
                           We support:
 
                           - ngx_code_server (code-server with ssl)
                           - ngx_fast_report (FastReport with ssl)
                           - ngx_nextcloud (NextCloud with ssl)
                           - ngx_odoo_http (Odoo only http)
                           - ngx_odoo_ssl (Odoo with ssl)
-                          - ngx_odoo_ssl_pagespeed (Odoo with ssl and PageSpeed)
                           - ngx_pgadmin (pgAdmin4 with ssl)
                           - ngx_portainer (NextCloud with ssl)
                           - ngx_pwa (Progressive Web App with ssl)
                           - ngx_redirect (Redirect Domain without ssl)
                           - ngx_redirect_ssl (Redirect Domain with ssl)
   --ip TEXT               IP address of the server
   --domain TEXT           Name of the domain
@@ -57,20 +56,22 @@
 ```bash
 # Execution with config file
 nginx-set-conf --config_path server_config
 f.e.
 nginx-set-conf --config_path=$HOME/docker-builds/ngx-conf
   
 # Execution without config file
-nginx-set-conf --config_template ngx_odoo_ssl_pagespeed --ip 1.2.3.4 --domain www.equitania.de --port 8069 --cert_name www.equitania.de --pollport 8072 
+nginx-set-conf --config_template ngx_odoo_ssl --ip 1.2.3.4 --domain www.equitania.de --port 8069 --cert_name www.equitania.de --pollport 8072 
 
 # Create your cert with
 certbot certonly --standalone --agree-tos --register-unsafely-without-email -d www.equitania.de
-# Install certbot on Ubuntu with
+# Install certbot on Debian/Ubuntu with
 apt-get install certbot
 ```
   
-## Compile your nginx with PageSpeed   
+## nginx template settings  
   
-At github you can find the script to do that: [nginx build script](https://github.com/equitania/myodoo-docker/tree/2022/scripts/build_nginx)  
+You can download our settings: [nginx.conf](https://rm.ownerp.io/staff/nginx.conf)  
+and the : [nginxconfig.io.zip](https://rm.ownerp.io/staff/nginxconfig.io.zip)  
+based on [https://www.digitalocean.com/community/tools/nginx](https://www.digitalocean.com/community/tools/nginx)  
   
 This project is licensed under the terms of the **AGPLv3** license.
```

### Comparing `nginx-set-conf-equitania-0.8.3/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.9.0/nginx_set_conf/config_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 config_template_dict = {
 "ngx_code_server": """# Template for code-server configuration nginx incl. SSL/http2
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -13,16 +13,16 @@
 
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log warn flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
@@ -30,14 +30,20 @@
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
 
     # limit ciphers
     ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
 
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
     #general proxy settings
     # force timeouts if the backend dies
@@ -63,15 +69,15 @@
         # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
 
 "ngx_fast_report": """# Template for FastReport configuration nginx incl. SSL/http2
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -80,16 +86,16 @@
 
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log warn flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
@@ -103,14 +109,20 @@
 
     index index.html;
 
     # set max upload size
     client_max_body_size 10G;
     fastcgi_buffers 64 4K;
 
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
     #general proxy settings
     # force timeouts if the backend dies
@@ -130,15 +142,15 @@
         # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
 
 "ngx_nextcloud": """# Template for NextCloud configuration nginx incl. SSL/http2
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -148,16 +160,16 @@
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
     add_header Referrer-Policy no-referrer always;
 
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
@@ -169,15 +181,21 @@
     ssl_session_timeout  5m;
 
     # Path to the root of your installation
     #root /var/www/owncloud/;
     root /var/www/nextcloud/;
     index index.html;
 
-    location = /robots.txt {
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
+        location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
     # Raise file upload size
     client_max_body_size 10G;
     # Limit download size
@@ -208,15 +226,15 @@
         proxy_set_header X-Forwarded-Proto $scheme;        # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
 
 "ngx_portainer": """# Template for Portainer configuration nginx incl. SSL/http2
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -226,31 +244,37 @@
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
     add_header Referrer-Policy no-referrer always;
 
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
 
     # limit ciphers
     ssl_session_timeout  5m;
 
-    #general proxy settings
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
+        #general proxy settings
     # force timeouts if the backend dies
     proxy_connect_timeout 1200s;
     proxy_send_timeout 1200s;
     proxy_read_timeout 1200s;
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
     # Proxy for portainer docker
@@ -263,25 +287,25 @@
         proxy_set_header X-Real-PORT $remote_port;
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
 
 "ngx_odoo_http": """# Template for Odoo configuration nginx
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     client_max_body_size 8192m;
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log flush=2m;
 
     # increase proxy buffer to handle some Odoo web requests
     proxy_buffers 16 64k;
     proxy_buffer_size 128k;
     proxy_headers_hash_max_size 76800;
     proxy_headers_hash_bucket_size 9600;
 
@@ -305,14 +329,20 @@
     proxy_set_header X-Forward-For $proxy_add_x_forwarded_for;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
     location / {
         proxy_pass http://127.0.0.1:oldport;
         proxy_redirect off;
         #auth_basic       "Restricted Area";
         #auth_basic_user_file  htpasswd/testmyodoo;
         #proxy_set_header Host $host;
         #proxy_set_header X-Forwarded-For $remote_addr;
@@ -329,31 +359,31 @@
         expires 864000;
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
 
 "ngx_odoo_ssl": """# Template for Odoo configuration nginx incl. SSL
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
     client_max_body_size 8192m;
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
@@ -386,14 +416,20 @@
     }
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
     # Add Headers for odoo proxy mode
     proxy_set_header X-Forwarded-Host $host;
     proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
     proxy_set_header X-Forwarded-Proto $scheme;
     proxy_set_header X-Real-IP $remote_addr;
 
     location / {
@@ -413,107 +449,16 @@
         proxy_buffering    on;
         expires 864000;
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
 
-"ngx_odoo_ssl_pagespeed": """# Template for Odoo configuration nginx incl. SSL/http2 and Google PageSpeed
-# source: https://github.com/apache/incubator-pagespeed-ngx/blob/master/scripts/build_ngx_pagespeed.sh
-# Version 3.8 from 10.05.2023
-# upstream server.domain.de {
-#     server ip.ip.ip.ip weight=1 fail_timeout=0;
-# }
-
-server {
-    listen server.domain.de:80;
-    server_name server.domain.de;
-    rewrite ^/.*$ https://$host$request_uri? permanent;
-}
-
-server {
-    listen server.domain.de:443 ssl http2;
-    server_name server.domain.de;
-    client_max_body_size 8192m;
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
-
-    # ssl certificate files
-    ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
-    ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
-
-    # add ssl specific settings
-    keepalive_timeout    60;
-    ssl_protocols        TLSv1.3 TLSv1.2;
-    ssl_prefer_server_ciphers on;
-    ssl_ciphers         HIGH:!aNULL:!MD5;
-
-    # limit ciphers
-    ssl_session_cache    shared:SSL:1m;
-    ssl_session_timeout  5m;
-
-    # increase proxy buffer to handle some Odoo web requests
-    proxy_buffers 16 64k;
-    proxy_buffer_size 128k;
-    proxy_headers_hash_max_size 76800;
-    proxy_headers_hash_bucket_size 9600;
-
-    #general proxy settings
-    # force timeouts if the backend dies
-    proxy_connect_timeout 3000s;
-    proxy_send_timeout 3000s;
-    proxy_read_timeout 3000s;
-    proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
-
-    # error pages
-    error_page 500 502 503 504 /custom_50x.html;
-    location = /custom_50x.html {
-        root /etc/nginx/html/;
-        internal;
-    }
-
-    #location = /robots.txt {
-    #    add_header Content-Type text/plain;
-    #    return 200 "User-agent: *Disallow: /";
-    #}
-
-    # Add Headers for odoo proxy mode
-    proxy_set_header X-Forwarded-Host $host;
-    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
-    proxy_set_header X-Forwarded-Proto $scheme;
-    proxy_set_header X-Real-IP $remote_addr;
-
-    location / {
-        proxy_pass http://127.0.0.1:oldport;
-        proxy_redirect off;
-        #proxy_set_header Host $host;
-        #proxy_set_header X-Forwarded-For $remote_addr;
-        #auth_basic       "Restricted Area";
-        #auth_basic_user_file  htpasswd/testmyodoo;
-    }
-
-    # Chat Odoo
-    location /longpolling {
-        proxy_pass http://127.0.0.1:oldpollport;
-    }
-
-    location ~* /web/static/ {
-        proxy_cache_valid 200 60m;
-        proxy_buffering    on;
-        expires 864000;
-        proxy_pass http://127.0.0.1:oldport;
-    }
-
-    include "pagespeed_main.conf";
-    # Pagespeed
-    pagespeed on;
-}""",
-
 "ngx_pgadmin": """# Template for pgAdmin configuration nginx incl. SSL/http2
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -522,16 +467,16 @@
 
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
@@ -544,14 +489,20 @@
     ssl_session_timeout  5m;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
     #general proxy settings
     # force timeouts if the backend dies
     proxy_connect_timeout 1200s;
     proxy_send_timeout 1200s;
     proxy_read_timeout 1200s;
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
@@ -564,15 +515,15 @@
         proxy_set_header X-Forwarded-Proto https;
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
 
 "ngx_pwa": """# Template for Progressive Web App .NET Core configuration nginx incl. SSL/http2
-# Version 3.9 from 25.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -581,16 +532,16 @@
 
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
-    access_log /var/log/nginx/server.domain.de-access.log;
-    error_log /var/log/nginx/server.domain.de-error.log;
+    access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/server.domain.de-error.log flush=2m;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
@@ -612,14 +563,20 @@
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # security
+    include                 nginxconfig.io/security.conf;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
+
     # Add Headers for odoo proxy mode
     proxy_set_header X-Forwarded-Host $host;
     proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
     proxy_set_header X-Forwarded-Proto $scheme;
     proxy_set_header X-Real-IP $remote_addr;
 
     # Proxy for docker
@@ -636,44 +593,50 @@
     server ip.ip.ip.ip weight=1 fail_timeout=0;
 }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ http://target.domain.de$request_uri? permanent;
-    access_log /var/log/nginx/target.domain.de-access.log;
-    error_log /var/log/nginx/target.domain.de-error.log;
+    access_log /var/log/nginx/target.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/target.domain.de-error.log flush=2m;
 }
 """,
 
 "ngx_redirect_ssl": """# Template for Redirect domain configuration nginx ssl/http2
-# Version 3.8 from 10.05.2023
+# Version 4.0 from 10.07.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ http://target.domain.de$request_uri? permanent;
-    access_log /var/log/nginx/target.domain.de-access.log;
-    error_log /var/log/nginx/target.domain.de-error.log;
+    access_log /var/log/nginx/target.domain.de-access.log combined buffer=512k flush=1m;
+    error_log /var/log/nginx/target.domain.de-error.log flush=2m;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
 }
 
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
     rewrite ^/.*$ https://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
+    # security
+    include                 nginxconfig.io/security.conf;
+
     #general proxy settings
     # force timeouts if the backend dies
     proxy_connect_timeout 1200s;
     proxy_send_timeout 1200s;
     proxy_read_timeout 1200s;
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
@@ -682,14 +645,17 @@
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
 
     # limit ciphers
     ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
+
+    # additional config
+    include                 nginxconfig.io/general.conf;
 }
 """
 }
 
 
 def get_config_template(config_template_name):
     if config_template_name in config_template_dict:
```

### Comparing `nginx-set-conf-equitania-0.8.3/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.9.0/nginx_set_conf/nginx_set_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 We support:\f
 \b
 - ngx_code_server (code-server with ssl)
 - ngx_fast_report (FastReport with ssl)
 - ngx_nextcloud (NextCloud with ssl)
 - ngx_odoo_http (Odoo only http)
 - ngx_odoo_ssl (Odoo with ssl)
-- ngx_odoo_ssl_pagespeed (Odoo with ssl and PageSpeed)
 - ngx_pgadmin (pgAdmin4 with ssl)
 - ngx_portainer (Portainer with ssl)
 - ngx_pwa (Progressive Web App with ssl)
 - ngx_redirect (Redirect Domain without ssl)
 - ngx_redirect_ssl (Redirect Domain with ssl)
 \b
 """
```

### Comparing `nginx-set-conf-equitania-0.8.3/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.9.0/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.9.0/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.3
-Summary: A package to create configurations for nginx with/without pagespeed for different web applications
+Version: 0.9.0
+Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -44,15 +44,14 @@
                           We support:
 
                           - ngx_code_server (code-server with ssl)
                           - ngx_fast_report (FastReport with ssl)
                           - ngx_nextcloud (NextCloud with ssl)
                           - ngx_odoo_http (Odoo only http)
                           - ngx_odoo_ssl (Odoo with ssl)
-                          - ngx_odoo_ssl_pagespeed (Odoo with ssl and PageSpeed)
                           - ngx_pgadmin (pgAdmin4 with ssl)
                           - ngx_portainer (NextCloud with ssl)
                           - ngx_pwa (Progressive Web App with ssl)
                           - ngx_redirect (Redirect Domain without ssl)
                           - ngx_redirect_ssl (Redirect Domain with ssl)
   --ip TEXT               IP address of the server
   --domain TEXT           Name of the domain
@@ -70,20 +69,22 @@
 ```bash
 # Execution with config file
 nginx-set-conf --config_path server_config
 f.e.
 nginx-set-conf --config_path=$HOME/docker-builds/ngx-conf
   
 # Execution without config file
-nginx-set-conf --config_template ngx_odoo_ssl_pagespeed --ip 1.2.3.4 --domain www.equitania.de --port 8069 --cert_name www.equitania.de --pollport 8072 
+nginx-set-conf --config_template ngx_odoo_ssl --ip 1.2.3.4 --domain www.equitania.de --port 8069 --cert_name www.equitania.de --pollport 8072 
 
 # Create your cert with
 certbot certonly --standalone --agree-tos --register-unsafely-without-email -d www.equitania.de
-# Install certbot on Ubuntu with
+# Install certbot on Debian/Ubuntu with
 apt-get install certbot
 ```
   
-## Compile your nginx with PageSpeed   
+## nginx template settings  
   
-At github you can find the script to do that: [nginx build script](https://github.com/equitania/myodoo-docker/tree/2022/scripts/build_nginx)  
+You can download our settings: [nginx.conf](https://rm.ownerp.io/staff/nginx.conf)  
+and the : [nginxconfig.io.zip](https://rm.ownerp.io/staff/nginxconfig.io.zip)  
+based on [https://www.digitalocean.com/community/tools/nginx](https://www.digitalocean.com/community/tools/nginx)  
   
 This project is licensed under the terms of the **AGPLv3** license.
```

### Comparing `nginx-set-conf-equitania-0.8.3/setup.py` & `nginx-set-conf-equitania-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.8.3",
+    version="0.9.0",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
-    description="A package to create configurations for nginx with/without pagespeed for different web applications",
+    description="A package to create configurations for nginx for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
```

