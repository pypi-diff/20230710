# Comparing `tmp/JMatuszczakL-1.0.4.tar.gz` & `tmp/JMatuszczakL-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JMatuszczakL-1.0.4.tar", last modified: Mon Jul 10 21:30:31 2023, max compression
+gzip compressed data, was "JMatuszczakL-1.0.5.tar", last modified: Mon Jul 10 21:35:27 2023, max compression
```

## Comparing `JMatuszczakL-1.0.4.tar` & `JMatuszczakL-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:30:31.797935 JMatuszczakL-1.0.4/
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:30:31.796602 JMatuszczakL-1.0.4/JMatuszczakL/
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)     1188 2023-07-10 21:30:14.000000 JMatuszczakL-1.0.4/JMatuszczakL/__init__.py
-drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:30:31.797526 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/PKG-INFO
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      212 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/SOURCES.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        1 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/dependency_links.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        6 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/requires.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       13 2023-07-10 21:30:31.000000 JMatuszczakL-1.0.4/JMatuszczakL.egg-info/top_level.txt
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:30:31.797784 JMatuszczakL-1.0.4/PKG-INFO
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       38 2023-07-10 21:30:31.797998 JMatuszczakL-1.0.4/setup.cfg
--rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      296 2023-07-10 21:29:53.000000 JMatuszczakL-1.0.4/setup.py
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:35:27.263471 JMatuszczakL-1.0.5/
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:35:27.262071 JMatuszczakL-1.0.5/JMatuszczakL/
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)     1156 2023-07-10 21:35:02.000000 JMatuszczakL-1.0.5/JMatuszczakL/__init__.py
+drwxr-xr-x   0 jakubmatuszczak   (501) staff       (20)        0 2023-07-10 21:35:27.262948 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/PKG-INFO
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      212 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/SOURCES.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        1 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/dependency_links.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)        6 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/requires.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       13 2023-07-10 21:35:27.000000 JMatuszczakL-1.0.5/JMatuszczakL.egg-info/top_level.txt
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      135 2023-07-10 21:35:27.263195 JMatuszczakL-1.0.5/PKG-INFO
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)       38 2023-07-10 21:35:27.263532 JMatuszczakL-1.0.5/setup.cfg
+-rw-r--r--   0 jakubmatuszczak   (501) staff       (20)      296 2023-07-10 21:35:00.000000 JMatuszczakL-1.0.5/setup.py
```

### Comparing `JMatuszczakL-1.0.4/JMatuszczakL/__init__.py` & `JMatuszczakL-1.0.5/JMatuszczakL/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# jm_library.py
-
 import sys
 from PyQt6.QtWidgets import QApplication, QWidget, QVBoxLayout, QLabel, QLineEdit, QPushButton
 
 class JM:
     @staticmethod
     def CreateWindow(app_title, calculate_text, calculate_function):
-        app = QApplication(sys.argv)
+        app = QApplication([])
         window = QWidget()
         window.setWindowTitle(app_title)
 
         layout = QVBoxLayout()
 
         input_label = QLabel("Input:")
         input_field = QLineEdit()
@@ -21,19 +19,18 @@
         output_field = QLabel()
         layout.addWidget(output_label)
         layout.addWidget(output_field)
 
         calculate_button = QPushButton(calculate_text)
         calculate_button.clicked.connect(lambda: JM.calculate(input_field, output_field, calculate_function))
         layout.addWidget(calculate_button)
+
+        window.setLayout(layout)
+        window.show()
+
         sys.exit(app.exec())
 
     @staticmethod
     def calculate(input_field, output_field, calculate_function):
         input_value = input_field.text()
         output_value = calculate_function(input_value)
         output_field.setText(output_value)
-
-        window.setLayout(layout)
-        window.show()
-
-
```

