# Comparing `tmp/streamlit-binary-tree-0.1.9.tar.gz` & `tmp/streamlit-binary-tree-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.1.9.tar", last modified: Mon Jul 10 20:10:59 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.2.0.tar", last modified: Mon Jul 10 21:51:34 2023, max compression
```

## Comparing `streamlit-binary-tree-0.1.9.tar` & `streamlit-binary-tree-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.536018 streamlit-binary-tree-0.1.9/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-10 20:10:59.536018 streamlit-binary-tree-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.1.9/README.md
--rw-rw-rw-   0        0        0       86 2023-07-10 20:10:59.537019 streamlit-binary-tree-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-10 20:10:42.000000 streamlit-binary-tree-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.433161 streamlit-binary-tree-0.1.9/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    11907 2023-07-10 20:04:44.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.416300 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.468085 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.417301 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.476618 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     7643 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css
--rw-rw-rw-   0        0        0    14797 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.535018 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   667302 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405682 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
--rw-rw-rw-   0        0        0     4405 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js
--rw-rw-rw-   0        0        0    14767 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-10 20:10:59.460440 streamlit-binary-tree-0.1.9/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-10 20:10:59.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-10 20:10:59.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 20:10:59.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 20:10:59.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-10 20:10:59.000000 streamlit-binary-tree-0.1.9/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.108615 streamlit-binary-tree-0.2.0/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-10 21:51:34.108615 streamlit-binary-tree-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-10 21:51:34.110616 streamlit-binary-tree-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-10 21:51:23.000000 streamlit-binary-tree-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.079563 streamlit-binary-tree-0.2.0/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    12516 2023-07-10 21:51:11.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.071562 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.092976 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.072561 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.094977 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     7643 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css
+-rw-rw-rw-   0        0        0    14797 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.107621 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   667302 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405682 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
+-rw-rw-rw-   0        0        0     4405 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js
+-rw-rw-rw-   0        0        0    14767 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-10 18:55:31.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-10 21:51:34.091977 streamlit-binary-tree-0.2.0/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-10 21:51:33.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-10 21:51:34.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 21:51:33.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 21:51:33.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-10 21:51:33.000000 streamlit-binary-tree-0.2.0/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.1.9/LICENSE` & `streamlit-binary-tree-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/setup.py` & `streamlit-binary-tree-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.1.9",
+    version="0.2.0",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,20 +60,28 @@
 
     text = (
         f"{perc_text} ({num_text})" if percentage_first else f"{num_text} ({perc_text})"
     )
     return text
 
 
+def get_class_weight(y):
+    unique, counts = np.unique(np.array(y), return_counts=True)
+    counts = counts / counts[0]
+    class_weights = {u: c for u, c in zip(unique, counts)}
+    return class_weights
+
+
 def export_dict(
     tree: DCTClass,
     feature_names=None,
     feature_value_formats=None,
     class_names=None,
     class_colors=None,
+    class_weights=None,
     sample_header="Samples",
     bads_header="Events",
     percentage_first=True,
     sample_perc_precision=1,
     bads_perc_precision=1,
     binary_formatting=False,
 ):
@@ -136,24 +144,30 @@
     class_equal_color = "#fff"
     if class_names is None:
         class_names = [str(i) for i in range(int(tree_.n_classes))]
     classes = [
         {"id": i, "name": c, "color": class_colors[i]}
         for i, c in enumerate(class_names)
     ]
+    tmp_class_weights = {k: 1 for k in range(int(tree_.n_classes[0]))}
+    if class_weights is not None:
+        for k, class_weight in class_weights.items():
+            tmp_class_weights[k] = class_weight
+    class_weights = list(tmp_class_weights.values())
 
     # i is the element in the tree_ to create a dict for
     def recur(i, master_dict, path="", depth=0):
         if i == _tree.TREE_LEAF:
             return None
 
         feature_idx = int(tree_.feature[i])
         threshold = float(tree_.threshold[i])
         samples = tree_.n_node_samples[i]
         value = tree_.value[i].tolist()[0]
+        value = [v / cw for v, cw in zip(value, class_weights)]
         value_perc = value / samples
 
         hasChildren = feature_idx != _tree.TREE_UNDEFINED
         left_idx = int(tree_.children_left[i])
         right_idx = int(tree_.children_right[i])
 
         samples_value = content_text(
@@ -380,15 +394,18 @@
     clf = tree.DecisionTreeClassifier(class_weight={0: 1, 1: 10}, random_state=42)
     iris = load_iris()
     clf = clf.fit(
         iris.data,
         iris.target,
     )
     data, classes = export_dict(
-        clf, feature_names=iris.feature_names, class_names=iris.target_names
+        clf,
+        feature_names=iris.feature_names,
+        class_names=iris.target_names,
+        class_weights={0: 1, 1: 10},
     )
 
     st.markdown("---")
     node_id = binary_tree(
         data, key="dct_sample_dataset", show_node_ids=True, style={"node_size": "200px"}
     )
     node_data = get_node_data(data, node_id)
```

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css.map` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/css/main.216de144.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js.map` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/main.bdff17c6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.9/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.2.0/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

