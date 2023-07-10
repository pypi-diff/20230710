# Comparing `tmp/datatransform-1.2.tar.gz` & `tmp/datatransform-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransform-1.2.tar", last modified: Mon Jul 10 16:05:27 2023, max compression
+gzip compressed data, was "datatransform-1.3.tar", last modified: Mon Jul 10 17:46:06 2023, max compression
```

## Comparing `datatransform-1.2.tar` & `datatransform-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 16:05:27.624008 datatransform-1.2/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 16:05:27.623905 datatransform-1.2/PKG-INFO
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 16:05:27.623279 datatransform-1.2/datatransform/
--rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.2/datatransform/__init__.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1555 2023-07-05 21:04:03.000000 datatransform-1.2/datatransform/datatransform.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      733 2023-07-05 20:59:32.000000 datatransform-1.2/datatransform/leave_one_out.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1302 2023-07-05 21:00:25.000000 datatransform-1.2/datatransform/mca.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      718 2023-07-05 21:00:27.000000 datatransform-1.2/datatransform/pca.py
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 16:05:27.623762 datatransform-1.2/datatransform.egg-info/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/PKG-INFO
--rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/SOURCES.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/dependency_links.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 16:05:27.000000 datatransform-1.2/datatransform.egg-info/top_level.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 16:05:27.624038 datatransform-1.2/setup.cfg
--rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 16:04:40.000000 datatransform-1.2/setup.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 17:46:06.375855 datatransform-1.3/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 17:46:06.375713 datatransform-1.3/PKG-INFO
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 17:46:06.374908 datatransform-1.3/datatransform/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.3/datatransform/__init__.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1608 2023-07-10 17:17:05.000000 datatransform-1.3/datatransform/datatransform.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      793 2023-07-10 17:38:12.000000 datatransform-1.3/datatransform/leave_one_out.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1318 2023-07-10 17:38:07.000000 datatransform-1.3/datatransform/mca.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      775 2023-07-10 17:38:01.000000 datatransform-1.3/datatransform/pca.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 17:46:06.375506 datatransform-1.3/datatransform.egg-info/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/PKG-INFO
+-rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/SOURCES.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/dependency_links.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/top_level.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 17:46:06.375894 datatransform-1.3/setup.cfg
+-rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 17:45:23.000000 datatransform-1.3/setup.py
```

### Comparing `datatransform-1.2/datatransform/datatransform.py` & `datatransform-1.3/datatransform/datatransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,21 @@
         with open('dt_params.yaml', 'r') as file:
             dt_params = yaml.safe_load(file)
         return dt_params
     '''
     
     def ready_data(self, data):
         dataframe = pd.read_csv(data)
-        X = dataframe.drop('Decision', 'user_name', axis=1)
+        X = dataframe.drop(['Decision', 'user_name'], axis=1)
         y = dataframe['Decision']
         for column in X.columns:
             X[column].fillna('Unknown', inplace=True)
             X[column] = X[column].astype(str)
-        return X, y
+        output_size = len(y.unique())
+        return X, y, output_size
         
     def split_data(self, X, y, test_size = 0.2, random_state = 40):
         X_train, X_test, y_train, y_test = train_test_split(X, y, test_size, random_state)
         X_train, X_val, y_train, y_val = train_test_split(X_train, y_train, test_size, random_state)
         return X_train, X_test, X_val, y_train, y_test, y_val
 
     def label_encode(self, y_train, y_test, y_val, num_classes=3):
```

### Comparing `datatransform-1.2/datatransform/leave_one_out.py` & `datatransform-1.3/datatransform/leave_one_out.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from category_encoders import LeaveOneOutEncoder
 from .datatransform import Data_Transform
 
 class LeaveOneOut:
     def transform(self, data):
         data_transformer = Data_Transform()
 
-        X, y = data_transformer.ready_data(data)
+        X, y, output_size = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
-        y_train, y_test, y_val, y_train_cat, y_test_cat, y_val_cat = data_transformer.label_encode(y_train, y_test, y_val)
+        y_train_cat, y_test_cat, y_val_cat = data_transformer.label_encode(y_train, y_test, y_val)
 
         encoder = LeaveOneOutEncoder(cols=X_train.columns)
         X_train = encoder.fit_transform(X_train, y_train)
         X_val = encoder.transform(X_val)
         X_test = encoder.transform(X_test)
+        n_components = len(X_train.columns)
 
-        return X_train, X_test, X_val, y_train_cat, y_test_cat, y_val_cat
+        return X_train, X_test, X_val, y_train_cat, y_test_cat, y_val_cat, output_size, n_components
```

### Comparing `datatransform-1.2/datatransform/mca.py` & `datatransform-1.3/datatransform/mca.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import prince
 from .datatransform import Data_Transform
 
 class MCA():
     def transform(self, data):
         data_transformer = Data_Transform()
 
-        X, y = data_transformer.ready_data(data)
+        X, y, output_size = data_transformer.ready_data(data)
         X_train, X_test, X_val, y_train, y_test, y_val = data_transformer.split_data(X, y)
-        y_train, y_test, y_val, y_train_cat, y_test_cat, y_val_cat = data_transformer.label_encode(y_train, y_test, y_val)
+        y_train_cat, y_test_cat, y_val_cat = data_transformer.label_encode(y_train, y_test, y_val)
 
         one_hot = pd.get_dummies(X)
         n_components = self.get_n_components(one_hot)
 
         mca = prince.MCA(n_components, n_iter=20, copy=True, check_input=True, engine='sklearn')
         X_train = mca.fit_transform(X_train)
         X_test = mca.fit_transform(X_test)
         X_val = mca.fit_transform(X_val)
-        return X_train, X_test, X_val, y_train_cat, y_test_cat, y_val_cat
+        return X_train, X_test, X_val, y_train_cat, y_test_cat, y_val_cat, output_size, n_components
 
     def get_n_components(self, data, threshold=0.9):
         covariance_matrix = np.cov(data.values.T)
         eigenvalues, _ = np.linalg.eigv(covariance_matrix)
         total_variance = np.sum(eigenvalues)
         explained_variance_ratio = eigenvalues / total_variance
         cumulative_explained_variance = np.cumsum(explained_variance_ratio)
```

