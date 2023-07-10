# Comparing `tmp/netbox-device-view-0.1.1.tar.gz` & `tmp/netbox-device-view-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-device-view-0.1.1.tar", last modified: Wed Jul  5 20:35:05 2023, max compression
+gzip compressed data, was "netbox-device-view-0.1.2.tar", last modified: Mon Jul 10 17:30:15 2023, max compression
```

## Comparing `netbox-device-view-0.1.1.tar` & `netbox-device-view-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/netbox_device_view/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/netbox_device_view/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/netbox_device_view/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.008170 netbox-device-view-0.1.1/netbox_device_view/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.008170 netbox-device-view-0.1.1/netbox_device_view/static/netbox_device_view/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/netbox_device_view/static/netbox_device_view/css/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/static/netbox_device_view/css/device_view.css
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.008170 netbox-device-view-0.1.1/netbox_device_view/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/netbox_device_view/templates/netbox_device_view/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/templates/netbox_device_view/deviceview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/templates/netbox_device_view/ports.html
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/netbox_device_view/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/netbox_device_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-05 20:35:04.000000 netbox-device-view-0.1.1/netbox_device_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-05 20:35:05.000000 netbox-device-view-0.1.1/netbox_device_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:35:05.000000 netbox-device-view-0.1.1/netbox_device_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:35:04.000000 netbox-device-view-0.1.1/netbox_device_view.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 20:35:05.000000 netbox-device-view-0.1.1/netbox_device_view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:35:05.012170 netbox-device-view-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-05 20:34:45.000000 netbox-device-view-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.666301 netbox-device-view-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-10 17:30:15.666301 netbox-device-view-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.658301 netbox-device-view-0.1.2/netbox_device_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.662301 netbox-device-view-0.1.2/netbox_device_view/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.662301 netbox-device-view-0.1.2/netbox_device_view/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.654302 netbox-device-view-0.1.2/netbox_device_view/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.654302 netbox-device-view-0.1.2/netbox_device_view/static/netbox_device_view/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.662301 netbox-device-view-0.1.2/netbox_device_view/static/netbox_device_view/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/static/netbox_device_view/css/device_view.css
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.654302 netbox-device-view-0.1.2/netbox_device_view/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.662301 netbox-device-view-0.1.2/netbox_device_view/templates/netbox_device_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/templates/netbox_device_view/deviceview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/templates/netbox_device_view/ports.html
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/netbox_device_view/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:30:15.662301 netbox-device-view-0.1.2/netbox_device_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-10 17:30:15.000000 netbox-device-view-0.1.2/netbox_device_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-10 17:30:15.000000 netbox-device-view-0.1.2/netbox_device_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:30:15.000000 netbox-device-view-0.1.2/netbox_device_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:30:15.000000 netbox-device-view-0.1.2/netbox_device_view.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 17:30:15.000000 netbox-device-view-0.1.2/netbox_device_view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:30:15.666301 netbox-device-view-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-10 17:30:05.000000 netbox-device-view-0.1.2/setup.py
```

### Comparing `netbox-device-view-0.1.1/PKG-INFO` & `netbox-device-view-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-view
-Version: 0.1.1
+Version: 0.1.2
 Summary: NetBox Device View plugin
 Home-page: https://github.com/peterbaumert/netbox-device-view
 Author: Peter Baumert
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `netbox-device-view-0.1.1/README.md` & `netbox-device-view-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.1/netbox_device_view/__init__.py` & `netbox-device-view-0.1.2/netbox_device_view/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.1/netbox_device_view/migrations/0001_initial.py` & `netbox-device-view-0.1.2/netbox_device_view/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.1/netbox_device_view/static/netbox_device_view/css/device_view.css` & `netbox-device-view-0.1.2/netbox_device_view/static/netbox_device_view/css/device_view.css`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.1/netbox_device_view/template_content.py` & `netbox-device-view-0.1.2/netbox_device_view/template_content.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,23 +7,26 @@
     def page(self):
         obj = self.context["object"]
         request = self.context["request"]
         url = request.build_absolute_uri(obj.get_absolute_url())
 
         dv, modules, ports_chassis = prepare(obj)
 
+        height = obj.device_type.u_height * 2 * 20 + obj.device_type.u_height * 2
+
         if dv is None or modules is None or ports_chassis is None:
             return ""
 
         return self.render(
             "netbox_device_view/ports.html",
             extra_context={
-                "ports_chassis": ports_chassis,
                 "dv": dv,
                 "modules": modules,
+                "height": height,
+                "ports_chassis": ports_chassis,
             },
         )
 
 
 class DevicePorts(Ports):
     model = "dcim.device"
```

### Comparing `netbox-device-view-0.1.1/netbox_device_view/templates/netbox_device_view/deviceview.html` & `netbox-device-view-0.1.2/netbox_device_view/templates/netbox_device_view/deviceview.html`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 />
 <style>
 	{% autoescape off %}
 	{% for id, ddv in dv.items %}
 	{{ ddv }}
 	{% endfor %}
 	{% endautoescape %}
+	{% if height %}
+	
+	.deviceview {
+		height:{{ height }}px;
+	}
+	{% endif %}
 </style>
 {% endblock %}
 {% block content %}
 <div class="card">
 	<div class="card-body htmx-container">
 		{% spaceless %} {% for device, interfaces in ports_chassis.items %} Device
 		{{device}}
```

### Comparing `netbox-device-view-0.1.1/netbox_device_view/templates/netbox_device_view/ports.html` & `netbox-device-view-0.1.2/netbox_device_view/templates/netbox_device_view/ports.html`

 * *Files 19% similar despite different names*

```diff
@@ -5,23 +5,29 @@
 />
 <style>
 	{% autoescape off %}
 	{% for id, ddv in dv.items %}
 	{{ ddv }}
 	{% endfor %}
 	{% endautoescape %}
+	{% if height %}
+
+	.deviceview {
+		height:{{ height }}px;
+	}
+	{% endif %}
 </style>
 {% endblock %} {% block content %}
 <div class="card">
-	<h2 class="card-header">Switchview {{ object.name }}</h2>
+	<h2 class="card-header">Deviceview {{ object.name }}</h2>
 	<div class="card-body">
-		{% spaceless %} {% for switch, interfaces in ports_chassis.items %} Switch
+		{% spaceless %} {% for switch, interfaces in ports_chassis.items %} Device
 		{{switch}}
 		<div
-			class="switchview area{{switch}}{% for sw, modules in modules.items %}{% if sw == switch %}{% for module in modules %} module{{module.module_type.model}}{% endfor %}{% endif %}{% endfor %}"
+			class="deviceview area d{{switch}}{% for sw, modules in modules.items %}{% if sw == switch %}{% for module in modules %} module{{module.module_type.model}}{% endfor %}{% endif %}{% endfor %}"
 		>
 			{% for int in interfaces %}
 			<a
 				href="{{int.get_absolute_url}}trace/"
 				class="{% if int.enabled and int.connected_endpoints|length > 0 %}bg-success{% elif int.enabled %}bg-secondary{% else %}bg-danger{% endif %}"
 				title="{{ int.name }}{% if int.connected_endpoints|length > 0 %}<hr>{{ int.connected_endpoints.0.device }} | {{ int.connected_endpoints.0.name }}{% endif %}"
 				style="grid-area: {{ int.stylename }}"
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% load static %} {% block head %}
  {% endblock %} {% block content %}
-***** Switchview {{ object.name }} *****
-{% spaceless %} {% for switch, interfaces in ports_chassis.items %} Switch {
+***** Deviceview {{ object.name }} *****
+{% spaceless %} {% for switch, interfaces in ports_chassis.items %} Device {
 {switch}}
 {% for int in interfaces %}
 {%_if_int.enabled_and_int.connected_endpoints|length_>_0_%}__{%_elif
 int.enabled_%}__{%_else_%}__{%_endif_%}
  {% endfor %}
 {% endfor %} {% endspaceless %}
 {% endblock %}
```

### Comparing `netbox-device-view-0.1.1/netbox_device_view/urls.py` & `netbox-device-view-0.1.2/netbox_device_view/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.1/netbox_device_view/utils.py` & `netbox-device-view-0.1.2/netbox_device_view/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,24 @@
             if matches:
                 itf.stylename = (
                     (matches["type"] or "")
                     + (matches["module"] or "")
                     + "-"
                     + matches["port"]
                 )
-                sw = int(matches["dev"] or 0)
+                sw = int(matches["dev"] or 999)
                 if (
                     hasattr(itf, "mgmt_only")
                     and itf.mgmt_only
                     and itf.type != "virtual"
                 ) or hasattr(itf, "mgmt_only") == False:
                     sw = dev
-                if sw not in ports_chassis and sw != 0:
+                if sw not in ports_chassis and sw != 999:
                     ports_chassis[sw] = []
-                if sw != 0:
+                if sw != 999:
                     ports_chassis[sw].append(itf)
     return ports_chassis
 
 
 def process_ports(ports, ports_chassis, where):
     if ports is not None:
         for port in ports:
@@ -39,18 +39,18 @@
             port.is_port = True
             if matches:
                 port.stylename = (matches["type"] or "") + "-" + matches["port"]
             else:
                 port.stylename = re.sub(r"[^.a-zA-Z\d]", "-", port.name.lower())
             sw = where
             if port.type == "virtual":
-                sw = 0
-            if sw not in ports_chassis and sw != 0:
+                sw = 999
+            if sw not in ports_chassis and sw != 999:
                 ports_chassis[sw] = []
-            if sw != 0:
+            if sw != 999:
                 ports_chassis[sw].append(port)
     return ports_chassis
 
 
 def prepare(obj):
     ports_chassis = {}
     dv = {}
@@ -62,15 +62,17 @@
                 device_type=obj.device_type
             ).grid_template_area
             modules[1] = obj.modules.all()
             ports_chassis = process_interfaces(obj.interfaces.all(), ports_chassis)
             ports_chassis = process_ports(obj.frontports.all(), ports_chassis, "Front")
             ports_chassis = process_ports(obj.rearports.all(), ports_chassis, "Rear")
             ports_chassis = process_ports(
-                ConsolePort.objects.filter(device_id=obj.id), ports_chassis, 1
+                ConsolePort.objects.filter(device_id=obj.id),
+                ports_chassis,
+                list(ports_chassis.keys())[0],
             )
         else:
             for member in obj.virtual_chassis.members.all():
                 dv[member.vc_position] = DeviceView.objects.get(
                     device_type=member.device_type
                 ).grid_template_area.replace(
                     ".area", ".area.d" + str(member.vc_position)
```

### Comparing `netbox-device-view-0.1.1/netbox_device_view/views.py` & `netbox-device-view-0.1.2/netbox_device_view/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,24 @@
             device_type=obj.device_type
         ).count(),
         hide_if_empty=True,
     )
 
     def get_extra_context(self, request, instance):
         dv, modules, ports_chassis = prepare(instance)
+        height = (
+            instance.device_type.u_height * 2 * 20 + instance.device_type.u_height * 2
+        )
         return {
             "device_view": models.DeviceView.objects.filter(
                 device_type=instance.device_type
             ).first(),
             "dv": dv,
-            "moduels": modules,
+            "modules": modules,
+            "height": height,
             "ports_chassis": ports_chassis,
             "cable_colors": request.GET.get("cable_colors", "off"),
             "something_else": request.GET.get("something_else", "off"),
         }
 
     def get_object(self, **kwargs):
         return Device.objects.get(pk=kwargs.get("pk"))
```

### Comparing `netbox-device-view-0.1.1/netbox_device_view.egg-info/PKG-INFO` & `netbox-device-view-0.1.2/netbox_device_view.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-view
-Version: 0.1.1
+Version: 0.1.2
 Summary: NetBox Device View plugin
 Home-page: https://github.com/peterbaumert/netbox-device-view
 Author: Peter Baumert
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `netbox-device-view-0.1.1/netbox_device_view.egg-info/SOURCES.txt` & `netbox-device-view-0.1.2/netbox_device_view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.1/setup.py` & `netbox-device-view-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="netbox-device-view",
-    version="0.1.1",
+    version="0.1.2",
     description="NetBox Device View plugin",
     packages=find_packages(),
     author="Peter Baumert",
     include_package_data=True,
     zip_safe=False,
     install_requires=[],
     long_description=long_description,
```

