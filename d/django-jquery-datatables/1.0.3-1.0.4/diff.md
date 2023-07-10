# Comparing `tmp/django_jquery_datatables-1.0.3.tar.gz` & `tmp/django_jquery_datatables-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jquery_datatables-1.0.3.tar", last modified: Mon Jul  3 09:55:36 2023, max compression
+gzip compressed data, was "django_jquery_datatables-1.0.4.tar", last modified: Mon Jul 10 11:30:30 2023, max compression
```

## Comparing `django_jquery_datatables-1.0.3.tar` & `django_jquery_datatables-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 09:55:36.113152 django_jquery_datatables-1.0.3/
--rw-rw-rw-   0        0        0     1067 2023-07-01 10:38:41.000000 django_jquery_datatables-1.0.3/License.txt
--rw-rw-rw-   0        0        0     9325 2023-07-03 09:55:36.111154 django_jquery_datatables-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8947 2023-07-01 10:35:25.000000 django_jquery_datatables-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 09:55:36.081173 django_jquery_datatables-1.0.3/django_jquery_datatables/
--rw-rw-rw-   0        0        0        0 2023-06-27 11:10:40.000000 django_jquery_datatables-1.0.3/django_jquery_datatables/__init__.py
--rw-rw-rw-   0        0        0     4810 2023-06-27 11:43:36.000000 django_jquery_datatables-1.0.3/django_jquery_datatables/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:55:36.106161 django_jquery_datatables-1.0.3/django_jquery_datatables.egg-info/
--rw-rw-rw-   0        0        0     9325 2023-07-03 09:55:35.000000 django_jquery_datatables-1.0.3/django_jquery_datatables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-07-03 09:55:35.000000 django_jquery_datatables-1.0.3/django_jquery_datatables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 09:55:35.000000 django_jquery_datatables-1.0.3/django_jquery_datatables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-03 09:55:35.000000 django_jquery_datatables-1.0.3/django_jquery_datatables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-03 09:55:35.000000 django_jquery_datatables-1.0.3/django_jquery_datatables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 09:55:36.113152 django_jquery_datatables-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-07-03 09:55:16.000000 django_jquery_datatables-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:30:30.276504 django_jquery_datatables-1.0.4/
+-rw-rw-rw-   0        0        0     1067 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.4/License.txt
+-rw-rw-rw-   0        0        0     9329 2023-07-10 11:30:30.275508 django_jquery_datatables-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8951 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 11:30:30.262512 django_jquery_datatables-1.0.4/django_jquery_datatables/
+-rw-rw-rw-   0        0        0        0 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.4/django_jquery_datatables/__init__.py
+-rw-rw-rw-   0        0        0     5014 2023-07-10 11:28:41.000000 django_jquery_datatables-1.0.4/django_jquery_datatables/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:30:30.272508 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/
+-rw-rw-rw-   0        0        0     9329 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 11:30:30.276504 django_jquery_datatables-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-07-10 11:30:01.000000 django_jquery_datatables-1.0.4/setup.py
```

### Comparing `django_jquery_datatables-1.0.3/License.txt` & `django_jquery_datatables-1.0.4/License.txt`

 * *Files identical despite different names*

### Comparing `django_jquery_datatables-1.0.3/PKG-INFO` & `django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_jquery_datatables
-Version: 1.0.3
+Name: django-jquery-datatables
+Version: 1.0.4
 Summary: Python library that integrates the popular jQuery DataTables library with Django projects.
 Home-page: https://github.com/Saliksheraz/django_jquery_datatables.git
 Author: Salik Sheraz
 Author-email: salik.sheraz@it-masons.com
 Description-Content-Type: text/markdown
 License-File: License.txt
 
@@ -29,15 +29,17 @@
 To use Django jQuery DataTables in your Django project, follow these steps:
 
 1. Install Django jQuery DataTables by `pip install django_jquery_datatables`.
 2. Import the main datatables function by using `from django_jquery_datatables.utils import JqueryDatatable`
 3. This JqueryDatatable is used in the view function of django, it returns all the data required by jquery datatables library in the form of JSON.
 
 ## Basic Example
+
 #####Frontend:
+
 ```html
 <table id="users_table" class="table">
     <thead>
     <tr>
         <th>Username</th>
         <th>Is Staff</th>
         <th>Is Superuser</th>
```

### Comparing `django_jquery_datatables-1.0.3/README.md` & `django_jquery_datatables-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 To use Django jQuery DataTables in your Django project, follow these steps:
 
 1. Install Django jQuery DataTables by `pip install django_jquery_datatables`.
 2. Import the main datatables function by using `from django_jquery_datatables.utils import JqueryDatatable`
 3. This JqueryDatatable is used in the view function of django, it returns all the data required by jquery datatables library in the form of JSON.
 
 ## Basic Example
+
 #####Frontend:
+
 ```html
 <table id="users_table" class="table">
     <thead>
     <tr>
         <th>Username</th>
         <th>Is Staff</th>
         <th>Is Superuser</th>
```

### Comparing `django_jquery_datatables-1.0.3/django_jquery_datatables/utils.py` & `django_jquery_datatables-1.0.4/django_jquery_datatables/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from django.http import JsonResponse
 
 
 def JqueryDatatable(request, queryset, SerializerClass, columnRemapping=None, additionalColumns=None):
+    requestType = request.GET.get('requestType')
     allColumns = []
     ctr = 0
     columnValue = request.GET.get(f"columns[{ctr}][data]")
     while columnValue:
         try:
             int(columnValue)
         except:
             allColumns.append(columnValue.replace(".", "__"))
         ctr = ctr + 1
         columnValue = request.GET.get(f"columns[{ctr}][data]")
 
     if additionalColumns and isinstance(additionalColumns, list):
         allColumns = allColumns + additionalColumns
 
+    if requestType == 'export':
+        serializer = SerializerClass(queryset, many=True)
+        return JsonResponse({"data": serializer.data})
+
     # For main search
     search = request.GET.get("search[value]")
     if search:
         for eachWord in search.strip().split(" "):
             filteredDataEachWord = queryset.none()
             for eachColumn in allColumns:
                 try:
@@ -92,10 +97,10 @@
     length = int(request.GET.get("length", 10))
 
     data = queryset[start: start + length]
     total_records = queryset.count()
 
     serializer = SerializerClass(data, many=True)
     serialized_data = serializer.data
-
     return JsonResponse(
-        {"draw": draw, "recordsTotal": total_records, "recordsFiltered": total_records, "data": serialized_data})
+        {"draw": draw, "recordsTotal": total_records, "recordsFiltered": total_records, "data": serialized_data}
+    )
```

### Comparing `django_jquery_datatables-1.0.3/django_jquery_datatables.egg-info/PKG-INFO` & `django_jquery_datatables-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-jquery-datatables
-Version: 1.0.3
+Name: django_jquery_datatables
+Version: 1.0.4
 Summary: Python library that integrates the popular jQuery DataTables library with Django projects.
 Home-page: https://github.com/Saliksheraz/django_jquery_datatables.git
 Author: Salik Sheraz
 Author-email: salik.sheraz@it-masons.com
 Description-Content-Type: text/markdown
 License-File: License.txt
 
@@ -29,15 +29,17 @@
 To use Django jQuery DataTables in your Django project, follow these steps:
 
 1. Install Django jQuery DataTables by `pip install django_jquery_datatables`.
 2. Import the main datatables function by using `from django_jquery_datatables.utils import JqueryDatatable`
 3. This JqueryDatatable is used in the view function of django, it returns all the data required by jquery datatables library in the form of JSON.
 
 ## Basic Example
+
 #####Frontend:
+
 ```html
 <table id="users_table" class="table">
     <thead>
     <tr>
         <th>Username</th>
         <th>Is Staff</th>
         <th>Is Superuser</th>
```

### Comparing `django_jquery_datatables-1.0.3/setup.py` & `django_jquery_datatables-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='django_jquery_datatables',
-    version='1.0.3',
+    version='1.0.4',
     description='Python library that integrates the popular jQuery DataTables library with Django projects.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Salik Sheraz',
     author_email='salik.sheraz@it-masons.com',
     url='https://github.com/Saliksheraz/django_jquery_datatables.git',
     packages=find_packages(),
```

