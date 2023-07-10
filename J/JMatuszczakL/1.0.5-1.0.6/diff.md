# Comparing `tmp/JMatuszczakL-1.0.5.tar.gz` & `tmp/JMatuszczakL-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JMatuszczakL-1.0.5.tar", last modified: Mon Jul 10 21:35:27 2023, max compression
+gzip compressed data, was "JMatuszczakL-1.0.6.tar", last modified: Mon Jul 10 21:40:13 2023, max compression
```

## Comparing `JMatuszczakL-1.0.5.tar` & `JMatuszczakL-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:35:27.263471 JMatuszczakL-1.0.5/
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:35:27.262071 JMatuszczakL-1.0.5/JMatuszczakL/
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)     1156 2023-07-10 21:35:02.000000 JMatuszczakL-1.0.5/JMatuszczakL/__init__.py
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:35:27.262948 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/PKG-INFO
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      212 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/SOURCES.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        1 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/dependency_links.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        6 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/requires.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       13 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/top_level.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:35:27.263195 JMatuszczakL-1.0.5/PKG-INFO
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       38 2023-07-10 21:35:27.263532 JMatuszczakL-1.0.5/setup.cfg
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      296 2023-07-10 21:35:00.000000 JMatuszczakL-1.0.5/setup.py
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:40:13.809199 JMatuszczakL-1.0.6/
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:40:13.807767 JMatuszczakL-1.0.6/JMatuszczakL/
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)     1205 2023-07-10 21:37:58.000000 JMatuszczakL-1.0.6/JMatuszczakL/__init__.py
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:40:13.808755 JMatuszczakL-1.0.6/JMatuszczakL.egg-info/
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:40:13.000000 JMatuszczakL-1.0.6/JMatuszczakL.egg-info/PKG-INFO
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      212 2023-07-10 21:40:13.000000 JMatuszczakL-1.0.6/JMatuszczakL.egg-info/SOURCES.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        1 2023-07-10 21:40:13.000000 JMatuszczakL-1.0.6/JMatuszczakL.egg-info/dependency_links.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        6 2023-07-10 21:40:13.000000 JMatuszczakL-1.0.6/JMatuszczakL.egg-info/requires.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       13 2023-07-10 21:40:13.000000 JMatuszczakL-1.0.6/JMatuszczakL.egg-info/top_level.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:40:13.809033 JMatuszczakL-1.0.6/PKG-INFO
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       38 2023-07-10 21:40:13.809273 JMatuszczakL-1.0.6/setup.cfg
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      296 2023-07-10 21:38:02.000000 JMatuszczakL-1.0.6/setup.py
```

### Comparing `JMatuszczakL-1.0.5/JMatuszczakL/__init__.py` & `JMatuszczakL-1.0.6/JMatuszczakL/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
         sys.exit(app.exec())
 
     @staticmethod
     def calculate(input_field, output_field, calculate_function):
         input_value = input_field.text()
         output_value = calculate_function(input_value)
-        output_field.setText(output_value)
+        output_field.setText(str(output_value))  # Convert to string before setting as text
```

