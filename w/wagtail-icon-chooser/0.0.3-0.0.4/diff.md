# Comparing `tmp/wagtail-icon-chooser-0.0.3.tar.gz` & `tmp/wagtail-icon-chooser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-icon-chooser-0.0.3.tar", last modified: Fri Jun 16 11:14:43 2023, max compression
+gzip compressed data, was "wagtail-icon-chooser-0.0.4.tar", last modified: Mon Jul 10 08:25:52 2023, max compression
```

## Comparing `wagtail-icon-chooser-0.0.3.tar` & `wagtail-icon-chooser-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 11:14:43.000000 wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/css/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.513444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:43.517444 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-16 11:14:28.000000 wagtail-icon-chooser-0.0.3/wagtailiconchooser/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/widgets.py
```

### Comparing `wagtail-icon-chooser-0.0.3/PKG-INFO` & `wagtail-icon-chooser-0.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-icon-chooser-0.0.3/README.md` & `wagtail-icon-chooser-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.3/setup.cfg` & `wagtail-icon-chooser-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-icon-chooser
-version = 0.0.3
+version = 0.0.4
 description = Wagtail Icon Chooser
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-icon-chooser
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/PKG-INFO` & `wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-icon-chooser-0.0.3/wagtail_icon_chooser.egg-info/SOURCES.txt` & `wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.3/wagtailiconchooser/blocks.py` & `wagtail-icon-chooser-0.0.4/wagtailiconchooser/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css` & `wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.3/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js` & `wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.3/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html` & `wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.3/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py` & `wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.3/wagtailiconchooser/utils.py` & `wagtail-icon-chooser-0.0.4/wagtailiconchooser/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,33 +13,38 @@
     if not _svg_icons:
         icon_hooks = hooks.get_hooks("register_icons")
         all_icons = sorted(
             itertools.chain.from_iterable(hook([]) for hook in icon_hooks)
         )
         for icon in all_icons:
             svg_str = render_to_string(icon)
-            doc = minidom.parseString(svg_str)
-            svg = doc.getElementsByTagName("svg")
-            if svg:
-                svg = svg[0]
-                icon_id = svg.getAttribute("id")
-                if icon_id:
-                    if icon_id.startswith("icon-"):
-                        icon_id = icon_id.replace("icon-", "")
-                    _svg_icons[icon_id] = svg_str
-            else:
-                symbol = doc.getElementsByTagName("symbol")
-                if symbol:
-                    symbol = symbol[0]
-                    icon_id = symbol.getAttribute("id")
+
+            try:
+                doc = minidom.parseString(svg_str)
+                svg = doc.getElementsByTagName("svg")
+                if svg:
+                    svg = svg[0]
+                    icon_id = svg.getAttribute("id")
                     if icon_id:
                         if icon_id.startswith("icon-"):
                             icon_id = icon_id.replace("icon-", "")
-                            svg_str = symbol.toxml().replace("symbol", "svg")
-                            doc = minidom.parseString(svg_str)
-                            svg = doc.getElementsByTagName("svg")
-                            if svg:
-                                svg = svg[0]
-                                svg.setAttribute('xmlns', 'http://www.w3.org/2000/svg')
-                                svg.setAttribute("id", icon_id)
-                                _svg_icons[icon_id] = mark_safe(svg.toxml())
+                        _svg_icons[icon_id] = svg_str
+                else:
+                    symbol = doc.getElementsByTagName("symbol")
+                    if symbol:
+                        symbol = symbol[0]
+                        icon_id = symbol.getAttribute("id")
+                        if icon_id:
+                            if icon_id.startswith("icon-"):
+                                icon_id = icon_id.replace("icon-", "")
+                                svg_str = symbol.toxml().replace("symbol", "svg")
+                                doc = minidom.parseString(svg_str)
+                                svg = doc.getElementsByTagName("svg")
+                                if svg:
+                                    svg = svg[0]
+                                    svg.setAttribute('xmlns', 'http://www.w3.org/2000/svg')
+                                    svg.setAttribute("id", icon_id)
+                                    _svg_icons[icon_id] = mark_safe(svg.toxml())
+            except Exception:
+                pass
+
     return _svg_icons
```

### Comparing `wagtail-icon-chooser-0.0.3/wagtailiconchooser/widgets.py` & `wagtail-icon-chooser-0.0.4/wagtailiconchooser/widgets.py`

 * *Files identical despite different names*

