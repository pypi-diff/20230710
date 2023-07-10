# Comparing `tmp/datatransform-1.1.tar.gz` & `tmp/datatransform-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransform-1.1.tar", last modified: Wed Jul  5 19:51:51 2023, max compression
+gzip compressed data, was "datatransform-1.2.tar", last modified: Mon Jul 10 16:05:27 2023, max compression
```

## Comparing `datatransform-1.1.tar` & `datatransform-1.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-05 19:51:51.992252 datatransform-1.1/
--rw-r--r--   0 janitsharma   (501) staff       (20)      117 2023-07-05 19:51:51.992131 datatransform-1.1/PKG-INFO
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-05 19:51:51.990965 datatransform-1.1/datatransform/
--rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 19:21:50.000000 datatransform-1.1/datatransform/__init__.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1615 2023-07-05 19:45:55.000000 datatransform-1.1/datatransform/data_transform.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      734 2023-07-05 19:00:58.000000 datatransform-1.1/datatransform/leave_one_out.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1303 2023-07-05 19:01:04.000000 datatransform-1.1/datatransform/mca.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      719 2023-07-05 19:01:07.000000 datatransform-1.1/datatransform/pca.py
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-05 19:51:51.991910 datatransform-1.1/datatransform.egg-info/
--rw-r--r--   0 janitsharma   (501) staff       (20)      117 2023-07-05 19:51:51.000000 datatransform-1.1/datatransform.egg-info/PKG-INFO
--rw-r--r--   0 janitsharma   (501) staff       (20)      323 2023-07-05 19:51:51.000000 datatransform-1.1/datatransform.egg-info/SOURCES.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-05 19:51:51.000000 datatransform-1.1/datatransform.egg-info/dependency_links.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-05 19:25:52.000000 datatransform-1.1/datatransform.egg-info/not-zip-safe
--rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-05 19:51:51.000000 datatransform-1.1/datatransform.egg-info/top_level.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-05 19:51:51.992285 datatransform-1.1/setup.cfg
--rw-r--r--   0 janitsharma   (501) staff       (20)      216 2023-07-05 19:48:07.000000 datatransform-1.1/setup.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 16:05:27.624008 datatransform-1.2/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 16:05:27.623905 datatransform-1.2/PKG-INFO
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 16:05:27.623279 datatransform-1.2/datatransform/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.2/datatransform/__init__.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1555 2023-07-05 21:04:03.000000 datatransform-1.2/datatransform/datatransform.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      733 2023-07-05 20:59:32.000000 datatransform-1.2/datatransform/leave_one_out.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1302 2023-07-05 21:00:25.000000 datatransform-1.2/datatransform/mca.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      718 2023-07-05 21:00:27.000000 datatransform-1.2/datatransform/pca.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 16:05:27.623762 datatransform-1.2/datatransform.egg-info/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/PKG-INFO
+-rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/SOURCES.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/dependency_links.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/top_level.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 16:05:27.624038 datatransform-1.2/setup.cfg
+-rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 16:04:40.000000 datatransform-1.2/setup.py
```

### Comparing `datatransform-1.1/datatransform/data_transform.py` & `datatransform-1.2/datatransform/datatransform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import yaml
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder
 from keras.utils import to_categorical
 
 class Data_Transform:
     '''
     def yaml_setup(self):
         with open('dt_params.yaml', 'r') as file:
             dt_params = yaml.safe_load(file)
         return dt_params
     '''
     
-    def ready_data(self, data, ):
-        dt_params = self.yaml_setup()
+    def ready_data(self, data):
         dataframe = pd.read_csv(data)
         X = dataframe.drop('Decision', 'user_name', axis=1)
         y = dataframe['Decision']
         for column in X.columns:
             X[column].fillna('Unknown', inplace=True)
             X[column] = X[column].astype(str)
         return X, y
@@ -33,12 +31,7 @@
         y_train = label_encoder.transform(y_train)
         y_test = label_encoder.transform(y_test)
         y_val = label_encoder.transform(y_val)
         y_train_categorical = to_categorical(y_train, num_classes)
         y_test_categorical = to_categorical(y_test, num_classes)
         y_val_categorical = to_categorical(y_val, num_classes)
         return y_train_categorical, y_test_categorical, y_val_categorical
-
-
-
-
-
```

### Comparing `datatransform-1.1/datatransform/leave_one_out.py` & `datatransform-1.2/datatransform/leave_one_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from category_encoders import LeaveOneOutEncoder
-from .data_transform import Data_Transform
+from .datatransform import Data_Transform
 
 class LeaveOneOut:
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
```

### Comparing `datatransform-1.1/datatransform/mca.py` & `datatransform-1.2/datatransform/mca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas as pd
 import prince
-from .data_transform import Data_Transform
+from .datatransform import Data_Transform
 
 class MCA():
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
```

### Comparing `datatransform-1.1/datatransform/pca.py` & `datatransform-1.2/datatransform/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 from sklearn.decomposition import PCA
-from .data_transform import Data_Transform
+from .datatransform import Data_Transform
 
 class PCA():
     def transform(self, data):
         data_transformer = Data_Transform()
 
         X, y = data_transformer.ready_data(data)
         X = pd.get_dummies(X)
```

