# Comparing `tmp/nutorious-0.1.8.tar.gz` & `tmp/nutorious-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutorious-0.1.8.tar", max compression
+gzip compressed data, was "nutorious-0.1.9.tar", max compression
```

## Comparing `nutorious-0.1.8.tar` & `nutorious-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-06-12 22:39:28.357649 nutorious-0.1.8/LICENSE
--rw-r--r--   0        0        0     6727 2023-06-12 22:39:28.357649 nutorious-0.1.8/README.md
--rw-r--r--   0        0        0      879 2023-06-12 22:39:28.357649 nutorious-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1559 2023-06-12 22:39:28.357649 nutorious-0.1.8/src/nutorious/__init__.py
--rw-r--r--   0        0        0      770 2023-06-12 22:39:28.357649 nutorious-0.1.8/src/nutorious/cli/__init__.py
--rw-r--r--   0        0        0     1219 2023-06-12 22:39:28.357649 nutorious-0.1.8/src/nutorious/config/__init__.py
--rw-r--r--   0        0        0      376 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/config/default.yml
--rw-r--r--   0        0        0      204 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/context/__init__.py
--rw-r--r--   0        0        0     4365 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/journal/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/__init__.py
--rw-r--r--   0        0        0     1457 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/base.py
--rw-r--r--   0        0        0     2556 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/daily.py
--rw-r--r--   0        0        0        0 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/diff.py
--rw-r--r--   0        0        0     1094 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/ui/__init__.py
--rw-r--r--   0        0        0      336 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/utils/collections.py
--rw-r--r--   0        0        0      570 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/utils/commons.py
--rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 nutorious-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-10 17:31:46.044866 nutorious-0.1.9/LICENSE
+-rw-r--r--   0        0        0     7171 2023-07-10 17:31:46.044866 nutorious-0.1.9/README.md
+-rw-r--r--   0        0        0      879 2023-07-10 17:31:46.044866 nutorious-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1559 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/__init__.py
+-rw-r--r--   0        0        0      770 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/cli/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/config/__init__.py
+-rw-r--r--   0        0        0      818 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/config/default.yml
+-rw-r--r--   0        0        0      204 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/context/__init__.py
+-rw-r--r--   0        0        0     4365 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/journal/__init__.py
+-rw-r--r--   0        0        0     1994 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/report/__init__.py
+-rw-r--r--   0        0        0     1435 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/report/base.py
+-rw-r--r--   0        0        0     2556 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/report/daily.py
+-rw-r--r--   0        0        0        0 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/report/diff.py
+-rw-r--r--   0        0        0     1094 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/ui/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/utils/collections.py
+-rw-r--r--   0        0        0      532 2023-07-10 17:31:46.048866 nutorious-0.1.9/src/nutorious/utils/commons.py
+-rw-r--r--   0        0        0     7949 1970-01-01 00:00:00.000000 nutorious-0.1.9/PKG-INFO
```

### Comparing `nutorious-0.1.8/LICENSE` & `nutorious-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/README.md` & `nutorious-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -166,37 +166,46 @@
 
 Example usage:
 
 ![example-journal](assets/journal-example.png)
 
 
 ### Configuration
-If journal directory contains file named `config.yml`, it will be treated as a custom configuration file.
-
-This file will be merged on top of the default to determine the full final configuration.
+If journal directory contains file named `config.yml`, it will be treated as a custom configuration file. This file will be merged on top of the default one to determine the full final configuration.
 
 The default configuration file is [here](https://github.com/dzmitry-paulenka/nutorious/blob/master/src/nutorious/config/default.yml) and looks like this:
 ```yaml
 meals:
   - breakfast
   - lunch
   - snack
   - dinner
 
 ui:
   daily:
+    # title on top of the report table, substitutes "{dt}" with the date of the report
     title: Nutrition report on {dt}
     columns:
+      # the ingredient name to show in the column
       - data: title
+        # title to show in the table header
+        title: Title
+        # styling, as supported by rich - https://rich.readthedocs.io/en/stable/style.html
         style: cyan
+        # justification, 'right' be default
         justify: left
       - data: amount
+        title: Amount
         style: green
       - data: kcal
+        title: Kcal
         style: blue
       - data: prot
+        title: Protein
         style: white
       - data: carb
+        title: Carbs
         style: yellow
       - data: fat
+        title: Fat
         style: red
-```
+```
```

### Comparing `nutorious-0.1.8/pyproject.toml` & `nutorious-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutorious"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Dzmitry Paulenka"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dzmitry-paulenka/nutorious"
 
 [tool.poetry.dependencies]
```

### Comparing `nutorious-0.1.8/src/nutorious/__init__.py` & `nutorious-0.1.9/src/nutorious/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/src/nutorious/cli/__init__.py` & `nutorious-0.1.9/src/nutorious/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/src/nutorious/config/__init__.py` & `nutorious-0.1.9/src/nutorious/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/src/nutorious/journal/__init__.py` & `nutorious-0.1.9/src/nutorious/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/src/nutorious/model/__init__.py` & `nutorious-0.1.9/src/nutorious/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/src/nutorious/report/base.py` & `nutorious-0.1.9/src/nutorious/report/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
 class YmlFilesFilter(DefaultFilter):
     def __call__(self, change: "Change", path: str) -> bool:
         return path.endswith(".yml") and super().__call__(change, path)
 
 
 def display_report(options: BaseOptions, build_report_table_fn: Callable[[Context], Table]):
-    context = __load_context(options)
+    def build_table_or_error():
+        try:
+            context = __load_context(options)
+            return build_report_table_fn(context)
+        except ValueError as e:
+            return f"[red]Error: {e}![/red]"
 
     if options.watch:
-        with Live(build_report_table_fn(context), auto_refresh=False) as live:
+        with Live(build_table_or_error(), auto_refresh=False) as live:
             for changes in watch(options.journal_path, watch_filter=YmlFilesFilter()):
-                context = __load_context(options)
-                live.update(build_report_table_fn(context), refresh=True)
+                live.update(build_table_or_error(), refresh=True)
     else:
         console = Console()
-        try:
-            table = build_report_table_fn(context)
-            console.print(table)
-        except ValueError as e:
-            console.print(f"[red]Error: {e}![/red]")
+        console.print(build_table_or_error())
 
 
 def __load_context(options: BaseOptions) -> Context:
     config = load_config(options.journal_path)
     journal = load_journal(config, options.journal_path)
 
     return Context(config, journal, options)
```

### Comparing `nutorious-0.1.8/src/nutorious/report/daily.py` & `nutorious-0.1.9/src/nutorious/report/daily.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/src/nutorious/ui/__init__.py` & `nutorious-0.1.9/src/nutorious/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.8/src/nutorious/utils/commons.py` & `nutorious-0.1.9/src/nutorious/utils/commons.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from yaml.error import YAMLError
 
 
 def mkstring(xs, sep=""):
     return sep.join(xs)
 
 
-def print_(a):
-    print(a, end="")
-
-
 def coalsece(*values):
     for v in values:
         if v is not None:
             return v
     return None
```

### Comparing `nutorious-0.1.8/PKG-INFO` & `nutorious-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutorious
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/dzmitry-paulenka/nutorious
 License: MIT
 Author: Dzmitry Paulenka
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -188,38 +188,46 @@
 
 Example usage:
 
 ![example-journal](assets/journal-example.png)
 
 
 ### Configuration
-If journal directory contains file named `config.yml`, it will be treated as a custom configuration file.
-
-This file will be merged on top of the default to determine the full final configuration.
+If journal directory contains file named `config.yml`, it will be treated as a custom configuration file. This file will be merged on top of the default one to determine the full final configuration.
 
 The default configuration file is [here](https://github.com/dzmitry-paulenka/nutorious/blob/master/src/nutorious/config/default.yml) and looks like this:
 ```yaml
 meals:
   - breakfast
   - lunch
   - snack
   - dinner
 
 ui:
   daily:
+    # title on top of the report table, substitutes "{dt}" with the date of the report
     title: Nutrition report on {dt}
     columns:
+      # the ingredient name to show in the column
       - data: title
+        # title to show in the table header
+        title: Title
+        # styling, as supported by rich - https://rich.readthedocs.io/en/stable/style.html
         style: cyan
+        # justification, 'right' be default
         justify: left
       - data: amount
+        title: Amount
         style: green
       - data: kcal
+        title: Kcal
         style: blue
       - data: prot
+        title: Protein
         style: white
       - data: carb
+        title: Carbs
         style: yellow
       - data: fat
+        title: Fat
         style: red
 ```
-
```

