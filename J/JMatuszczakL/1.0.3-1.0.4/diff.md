# Comparing `tmp/JMatuszczakL-1.0.3.tar.gz` & `tmp/JMatuszczakL-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JMatuszczakL-1.0.3.tar", last modified: Mon Jul 10 21:26:03 2023, max compression
+gzip compressed data, was "JMatuszczakL-1.0.4.tar", last modified: Mon Jul 10 21:30:31 2023, max compression
```

## Comparing `JMatuszczakL-1.0.3.tar` & `JMatuszczakL-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:26:03.102481 JMatuszczakL-1.0.3/
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:26:03.100981 JMatuszczakL-1.0.3/JMatuszczakL/
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)     1179 2023-07-10 21:25:11.000000 JMatuszczakL-1.0.3/JMatuszczakL/__init__.py
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:26:03.101988 JMatuszczakL-1.0.3/JMatuszczakL.egg-info/
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:26:03.000000 JMatuszczakL-1.0.3/JMatuszczakL.egg-info/PKG-INFO
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      212 2023-07-10 21:26:03.000000 JMatuszczakL-1.0.3/JMatuszczakL.egg-info/SOURCES.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        1 2023-07-10 21:26:03.000000 JMatuszczakL-1.0.3/JMatuszczakL.egg-info/dependency_links.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        6 2023-07-10 21:26:03.000000 JMatuszczakL-1.0.3/JMatuszczakL.egg-info/requires.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       13 2023-07-10 21:26:03.000000 JMatuszczakL-1.0.3/JMatuszczakL.egg-info/top_level.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:26:03.102229 JMatuszczakL-1.0.3/PKG-INFO
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       38 2023-07-10 21:26:03.102542 JMatuszczakL-1.0.3/setup.cfg
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      296 2023-07-10 21:25:53.000000 JMatuszczakL-1.0.3/setup.py
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:30:31.797935 JMatuszczakL-1.0.4/
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:30:31.796602 JMatuszczakL-1.0.4/JMatuszczakL/
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)     1188 2023-07-10 21:30:14.000000 JMatuszczakL-1.0.4/JMatuszczakL/__init__.py
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:30:31.797526 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/PKG-INFO
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      212 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/SOURCES.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        1 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/dependency_links.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        6 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/requires.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       13 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/top_level.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:30:31.797784 JMatuszczakL-1.0.4/PKG-INFO
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       38 2023-07-10 21:30:31.797998 JMatuszczakL-1.0.4/setup.cfg
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      296 2023-07-10 21:29:53.000000 JMatuszczakL-1.0.4/setup.py
```

### Comparing `JMatuszczakL-1.0.3/JMatuszczakL/__init__.py` & `JMatuszczakL-1.0.4/JMatuszczakL/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,19 @@
         output_field = QLabel()
         layout.addWidget(output_label)
         layout.addWidget(output_field)
 
         calculate_button = QPushButton(calculate_text)
         calculate_button.clicked.connect(lambda: JM.calculate(input_field, output_field, calculate_function))
         layout.addWidget(calculate_button)
+        sys.exit(app.exec())
 
     @staticmethod
     def calculate(input_field, output_field, calculate_function):
         input_value = input_field.text()
         output_value = calculate_function(input_value)
         output_field.setText(output_value)
 
         window.setLayout(layout)
         window.show()
 
-        sys.exit(app.exec())
+
```

