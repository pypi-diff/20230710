# Comparing `tmp/giant_utils-0.1.tar.gz` & `tmp/giant_utils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_utils-0.1.tar", max compression
+gzip compressed data, was "giant_utils-0.2.tar", max compression
```

## Comparing `giant_utils-0.1.tar` & `giant_utils-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-06-09 10:02:35.479386 giant_utils-0.1/LICENSE
--rw-r--r--   0        0        0     2545 2023-06-10 11:26:46.462221 giant_utils-0.1/README.md
--rw-r--r--   0        0        0       22 2023-06-09 10:07:03.052582 giant_utils-0.1/giant_utils/__init__.py
--rw-r--r--   0        0        0       96 2023-06-09 10:27:49.220595 giant_utils-0.1/giant_utils/apps.py
--rw-r--r--   0        0        0      480 2023-06-09 10:28:04.392713 giant_utils-0.1/giant_utils/fields.py
--rw-r--r--   0        0        0      457 2023-06-16 08:45:57.391745 giant_utils-0.1/giant_utils/format_bytes.py
--rw-r--r--   0        0        0     1720 2023-06-09 10:07:03.052582 giant_utils-0.1/giant_utils/sender.py
--rw-r--r--   0        0        0     2849 2023-06-10 11:14:14.283981 giant_utils-0.1/giant_utils/widgets.py
--rw-r--r--   0        0        0     1454 2023-06-16 12:39:49.169899 giant_utils-0.1/pyproject.toml
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 giant_utils-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 10:02:35.479386 giant_utils-0.2/LICENSE
+-rw-r--r--   0        0        0     2545 2023-06-10 11:26:46.462221 giant_utils-0.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-09 10:07:03.052582 giant_utils-0.2/giant_utils/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-09 10:27:49.220595 giant_utils-0.2/giant_utils/apps.py
+-rw-r--r--   0        0        0      480 2023-06-09 10:28:04.392713 giant_utils-0.2/giant_utils/fields.py
+-rw-r--r--   0        0        0      457 2023-06-16 08:45:57.391745 giant_utils-0.2/giant_utils/format_bytes.py
+-rw-r--r--   0        0        0     2337 2023-07-10 07:41:30.477944 giant_utils-0.2/giant_utils/sender.py
+-rw-r--r--   0        0        0     2849 2023-06-10 11:14:14.283981 giant_utils-0.2/giant_utils/widgets.py
+-rw-r--r--   0        0        0     1454 2023-07-10 08:19:58.798037 giant_utils-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 giant_utils-0.2/PKG-INFO
```

### Comparing `giant_utils-0.1/LICENSE` & `giant_utils-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giant_utils-0.1/README.md` & `giant_utils-0.2/README.md`

 * *Files identical despite different names*

### Comparing `giant_utils-0.1/giant_utils/sender.py` & `giant_utils-0.2/giant_utils/sender.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,73 @@
+import re
+
 from django.conf import settings
 from django.core.mail.message import EmailMultiAlternatives
+from django.template import engines
 from django.template.loader import render_to_string
+from django.utils.html import strip_tags
+
+
+def extract_body_content(template_content, context):
+    django_engine = engines["django"]
+
+    # endblock pattern could include the block name at the end so
+    # " %}" is omitted
+    pattern = r"{% block body %}(.*?)\{% endblock"
+    body_content = re.search(pattern, template_content, re.DOTALL).group(1).strip()
+
+    return django_engine.from_string(body_content).render(context)
 
 
 def send_email_from_template(
     to,
     email_subject: str,
-    txt_template: str,
-    html_template: str = None,
+    html_template: str,
+    text_template: str = None,
     pk: int = None,
     model_class: object = None,
     scheme: str = "",
     host: str = "",
 ):
     """
     A core template method which sends an email given the following parameters:
         obj: Usually set as self, but is the instance of the model you are using
         to: The recipient of the mail
-        txt_template: this is the path to the txt version of the template
         html_template: this is the path to the html version of the template
         pk: The model instance's pk to be pulled through into the email templates.
         model_class: The model class to be pulled through into the email templates.
         host: The site's host domain to be pulled through into the email templates
             for correct image url.
     """
     context = {
         "subject": email_subject,
         "scheme": scheme,
         "host": host,
     }
 
     if model_class and pk:
         instance = model_class.objects.get(pk=pk)
-        context = {"object": instance, "model": model_class, **context}
+        context = {"obj": instance, "model": model_class, **context}
+
+    with open("src/core/templates/" + html_template, "r") as file:
+        raw_html_content = file.read()
 
-    txt_result = render_to_string(txt_template, context=context)
+    if text_template:
+        txt_result = render_to_string(text_template, context=context)
+    else:
+        html_content = extract_body_content(raw_html_content, context)
+        txt_result = strip_tags(html_content)
 
     email = EmailMultiAlternatives(
         subject=context["subject"],
         body=txt_result,
         from_email=settings.DEFAULT_FROM_EMAIL,
         to=to,
     )
 
-    if html_template:
-        html_result = render_to_string(html_template, context=context)
-        email.attach_alternative(
-            content=html_result,
-            mimetype="text/html",
-        )
+    html_result = render_to_string(html_template, context=context)
+    email.attach_alternative(
+        content=html_result,
+        mimetype="text/html",
+    )
 
     email.send()
```

### Comparing `giant_utils-0.1/giant_utils/widgets.py` & `giant_utils-0.2/giant_utils/widgets.py`

 * *Files identical despite different names*

### Comparing `giant_utils-0.1/pyproject.toml` & `giant_utils-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-utils"
-version = "0.1"
+version = "0.2"
 description = "A small reusable package that adds small commonly used functions to a project"
 authors = ["Dominic-Chaple <dominic.chaple@giantdigital.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-utils"
 repository = "https://github.com/giantmade/giant-utils"
 keywords = ["app"]
```

### Comparing `giant_utils-0.1/PKG-INFO` & `giant_utils-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giant-utils
-Version: 0.1
+Version: 0.2
 Summary: A small reusable package that adds small commonly used functions to a project
 Home-page: https://github.com/giantmade/giant-utils
 License: MIT
 Keywords: app
 Author: Dominic-Chaple
 Author-email: dominic.chaple@giantdigital.co.uk
 Requires-Python: >3.7,<4
```

