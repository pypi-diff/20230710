# Comparing `tmp/cubicweb-rqlcontroller-0.9.4.tar.gz` & `tmp/cubicweb-rqlcontroller-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-rqlcontroller-0.9.4.tar", last modified: Tue Mar 29 09:15:36 2022, max compression
+gzip compressed data, was "cubicweb-rqlcontroller-1.0.0.tar", last modified: Mon Jul 10 14:00:11 2023, max compression
```

## Comparing `cubicweb-rqlcontroller-0.9.4.tar` & `cubicweb-rqlcontroller-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 09:15:36.675944 cubicweb-rqlcontroller-0.9.4/
--rw-rw-rw-   0 root         (0) root         (0)      401 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2636 2022-03-29 09:15:36.667944 cubicweb-rqlcontroller-0.9.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2068 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 09:15:36.611944 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 09:15:36.663944 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)      716 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     5258 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/rql_schema_holder.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 09:15:36.647944 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2636 2022-03-29 09:15:33.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      642 2022-03-29 09:15:35.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-29 09:15:33.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2022-03-29 09:15:34.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-29 09:15:33.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-03-29 09:15:35.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-03-29 09:15:35.000000 cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-29 09:15:36.675944 cubicweb-rqlcontroller-0.9.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2641 2022-03-29 09:14:14.000000 cubicweb-rqlcontroller-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:00:11.914573 cubicweb-rqlcontroller-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      401 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2616 2023-07-10 14:00:11.914573 cubicweb-rqlcontroller-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:00:11.894572 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:00:11.910573 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     5226 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/rql_schema_holder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10498 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:00:11.898573 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2616 2023-07-10 14:00:11.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-10 14:00:11.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:00:11.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-10 14:00:11.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:00:11.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-10 14:00:11.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-10 14:00:11.000000 cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:00:11.914573 cubicweb-rqlcontroller-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-07-10 13:59:17.000000 cubicweb-rqlcontroller-1.0.0/setup.py
```

### Comparing `cubicweb-rqlcontroller-0.9.4/PKG-INFO` & `cubicweb-rqlcontroller-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-rqlcontroller
-Version: 0.9.4
+Version: 1.0.0
 Summary: restfull rql edition capabilities
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-rqlcontroller
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
 
@@ -68,9 +67,7 @@
             {'u': '__r0', 'g': '__r1'})
            ]
 
     resp = requests.post('https://myinstance.example.com/rqlio/1.0'),
                          data=json.dumps(args),
                          headers={'Content-Type': 'application/json'})
     assert resp.status_code == 200
-
-
```

### Comparing `cubicweb-rqlcontroller-0.9.4/README.rst` & `cubicweb-rqlcontroller-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/__pkginfo__.py` & `cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/__pkginfo__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # pylint: disable=W0622
 """cubicweb-rqlcontroller application packaging information"""
 
 modname = "rqlcontroller"
 distname = "cubicweb-rqlcontroller"
 
-numversion = (0, 9, 4)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "restfull rql edition capabilities"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {
-    "cubicweb": ">= 3.32.2, < 3.37.0",
+    "cubicweb": ">= 4.0.0, < 5.0.0",
+    "cubicweb-web": ">=1.1.0, < 2.0.0",
 }
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python",
```

### Comparing `cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/predicates.py` & `cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/rql_schema_holder.py` & `cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/rql_schema_holder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -16,15 +15,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import hashlib
 
 from cubicweb.utils import json_dumps
 
 
-class RqlIOSchemaHolder(object):
+class RqlIOSchemaHolder:
     """Class used to load the schema and its hash.
     Both can be fetched by the client via dedicated views,
     so it can decide to update the locally stored schema if
     the integrity is not valid.
     """
 
     _schema = None
```

### Comparing `cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller/views.py` & `cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -25,17 +24,17 @@
     match_form_params,
     match_http_method,
     anonymous_user,
     authenticated_user,
 )
 from cubicweb.uilib import exc_message
 from cubicweb.utils import json_dumps
-from cubicweb.web import RemoteCallFailed, DirectResponse
-from cubicweb.web.controller import Controller
-from cubicweb.web.views.urlrewrite import rgx_action, SchemaBasedRewriter
+from cubicweb_web import RemoteCallFailed, DirectResponse
+from cubicweb_web.controller import Controller
+from cubicweb_web.views.urlrewrite import rgx_action, SchemaBasedRewriter
 from cubicweb import Binary
 from cubicweb_rqlcontroller.rql_schema_holder import RqlIOSchemaHolder
 
 from cubicweb_rqlcontroller.predicates import match_all_http_headers, match_basic_auth
 
 
 ARGRE = re.compile(r"__r(?P<ref>\d+)$")
@@ -48,24 +47,20 @@
             continue
         match = ARGRE.match(v)
         if match:
             numref = int(match.group("ref"))
             if 0 <= numref <= len(output):
                 rset = output[numref]
                 if not rset:
-                    raise Exception("%s references empty result set %s" % (v, rset))
+                    raise Exception(f"{v} references empty result set {rset}")
                 if len(rset) > 1:
-                    raise Exception(
-                        "%s references multi lines result set %s" % (v, rset)
-                    )
+                    raise Exception(f"{v} references multi lines result set {rset}")
                 row = rset.rows[0]
                 if len(row) > 1:
-                    raise Exception(
-                        "%s references multi column result set %s" % (v, rset)
-                    )
+                    raise Exception(f"{v} references multi column result set {rset}")
                 args[k] = row[0]
             continue
         match = DATARE.match(v)
         if match:
             args[k] = Binary(form[v][1].read())
```

### Comparing `cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/PKG-INFO` & `cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-rqlcontroller
-Version: 0.9.4
+Version: 1.0.0
 Summary: restfull rql edition capabilities
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-rqlcontroller
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
 
@@ -68,9 +67,7 @@
             {'u': '__r0', 'g': '__r1'})
            ]
 
     resp = requests.post('https://myinstance.example.com/rqlio/1.0'),
                          data=json.dumps(args),
                          headers={'Content-Type': 'application/json'})
     assert resp.status_code == 200
-
-
```

### Comparing `cubicweb-rqlcontroller-0.9.4/cubicweb_rqlcontroller.egg-info/SOURCES.txt` & `cubicweb-rqlcontroller-1.0.0/cubicweb_rqlcontroller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-rqlcontroller-0.9.4/setup.py` & `cubicweb-rqlcontroller-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
 
-install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

