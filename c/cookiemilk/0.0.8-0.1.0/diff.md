# Comparing `tmp/cookiemilk-0.0.8.tar.gz` & `tmp/cookiemilk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiemilk-0.0.8.tar", last modified: Thu Mar 23 06:21:35 2023, max compression
+gzip compressed data, was "cookiemilk-0.1.0.tar", last modified: Mon Jul 10 07:37:23 2023, max compression
```

## Comparing `cookiemilk-0.0.8.tar` & `cookiemilk-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 weiziqian   (501) staff       (20)        0 2023-03-23 06:21:35.006888 cookiemilk-0.0.8/
--rw-rw-r--   0 weiziqian   (501) staff       (20)    35149 2022-09-15 08:11:47.000000 cookiemilk-0.0.8/LICENSE
--rw-rw-r--   0 weiziqian   (501) staff       (20)      188 2022-09-15 08:11:47.000000 cookiemilk-0.0.8/MANIFEST.in
--rw-r--r--   0 weiziqian   (501) staff       (20)      766 2023-03-23 06:21:35.006731 cookiemilk-0.0.8/PKG-INFO
--rw-rw-r--   0 weiziqian   (501) staff       (20)      420 2023-03-08 05:16:31.000000 cookiemilk-0.0.8/README.md
-drwxr-xr-x   0 weiziqian   (501) staff       (20)        0 2023-03-23 06:21:35.005839 cookiemilk-0.0.8/cookiemilk/
--rw-rw-r--   0 weiziqian   (501) staff       (20)      398 2023-03-13 05:53:53.000000 cookiemilk-0.0.8/cookiemilk/__init__.py
--rw-r--r--   0 weiziqian   (501) staff       (20)     2375 2023-03-23 06:01:41.000000 cookiemilk-0.0.8/cookiemilk/average_graph.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)      700 2023-03-19 12:49:19.000000 cookiemilk-0.0.8/cookiemilk/calc_gcent.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)      315 2023-03-19 12:49:19.000000 cookiemilk-0.0.8/cookiemilk/calc_graphical_matching.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)      300 2023-03-19 12:49:19.000000 cookiemilk-0.0.8/cookiemilk/calc_surface_matching.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)     4964 2023-03-23 06:12:59.000000 cookiemilk-0.0.8/cookiemilk/calc_tversky.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)     3685 2023-03-19 12:49:40.000000 cookiemilk-0.0.8/cookiemilk/cmap2graph.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)     4323 2023-03-19 12:50:24.000000 cookiemilk-0.0.8/cookiemilk/draw.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)      405 2022-09-15 08:11:47.000000 cookiemilk-0.0.8/cookiemilk/get_data_files_name.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)     1958 2023-03-19 12:50:24.000000 cookiemilk-0.0.8/cookiemilk/graph2prxfile.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)      158 2023-03-19 12:50:24.000000 cookiemilk-0.0.8/cookiemilk/numerical_sim.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)     3545 2023-03-19 12:50:24.000000 cookiemilk-0.0.8/cookiemilk/pathfinder_network.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)      698 2023-03-19 12:50:24.000000 cookiemilk-0.0.8/cookiemilk/read_file.py
--rw-rw-r--   0 weiziqian   (501) staff       (20)     5273 2023-03-19 12:50:24.000000 cookiemilk-0.0.8/cookiemilk/text2graph.py
-drwxr-xr-x   0 weiziqian   (501) staff       (20)        0 2023-03-23 06:21:35.006552 cookiemilk-0.0.8/cookiemilk.egg-info/
--rw-r--r--   0 weiziqian   (501) staff       (20)      766 2023-03-23 06:21:34.000000 cookiemilk-0.0.8/cookiemilk.egg-info/PKG-INFO
--rw-r--r--   0 weiziqian   (501) staff       (20)      600 2023-03-23 06:21:35.000000 cookiemilk-0.0.8/cookiemilk.egg-info/SOURCES.txt
--rw-r--r--   0 weiziqian   (501) staff       (20)        1 2023-03-23 06:21:34.000000 cookiemilk-0.0.8/cookiemilk.egg-info/dependency_links.txt
--rw-r--r--   0 weiziqian   (501) staff       (20)       25 2023-03-23 06:21:34.000000 cookiemilk-0.0.8/cookiemilk.egg-info/requires.txt
--rw-r--r--   0 weiziqian   (501) staff       (20)       11 2023-03-23 06:21:34.000000 cookiemilk-0.0.8/cookiemilk.egg-info/top_level.txt
--rw-r--r--   0 weiziqian   (501) staff       (20)       38 2023-03-23 06:21:35.006927 cookiemilk-0.0.8/setup.cfg
--rw-rw-r--   0 weiziqian   (501) staff       (20)      691 2023-03-23 06:21:02.000000 cookiemilk-0.0.8/setup.py
+drwxr-xr-x   0 weiziqian   (501) staff       (20)        0 2023-07-10 07:37:23.398359 cookiemilk-0.1.0/
+-rw-rw-r--   0 weiziqian   (501) staff       (20)    35149 2022-09-15 08:11:47.000000 cookiemilk-0.1.0/LICENSE
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      188 2022-09-15 08:11:47.000000 cookiemilk-0.1.0/MANIFEST.in
+-rw-r--r--   0 weiziqian   (501) staff       (20)      766 2023-07-10 07:37:23.398233 cookiemilk-0.1.0/PKG-INFO
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      420 2023-03-08 05:16:31.000000 cookiemilk-0.1.0/README.md
+drwxr-xr-x   0 weiziqian   (501) staff       (20)        0 2023-07-10 07:37:23.397434 cookiemilk-0.1.0/cookiemilk/
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      385 2023-07-10 06:31:06.000000 cookiemilk-0.1.0/cookiemilk/__init__.py
+-rw-r--r--   0 weiziqian   (501) staff       (20)     2464 2023-04-04 06:48:37.000000 cookiemilk-0.1.0/cookiemilk/average_graph.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      419 2023-04-04 07:23:25.000000 cookiemilk-0.1.0/cookiemilk/calc_gcent.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      331 2023-04-04 07:13:05.000000 cookiemilk-0.1.0/cookiemilk/calc_graphical_matching.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      316 2023-04-04 07:13:10.000000 cookiemilk-0.1.0/cookiemilk/calc_surface_matching.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)     1475 2023-04-04 07:23:25.000000 cookiemilk-0.1.0/cookiemilk/calc_tversky.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)     3510 2023-04-04 07:17:39.000000 cookiemilk-0.1.0/cookiemilk/cmap2graph.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)     4376 2023-04-04 07:12:00.000000 cookiemilk-0.1.0/cookiemilk/draw.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      195 2023-04-04 07:18:32.000000 cookiemilk-0.1.0/cookiemilk/numerical_sim.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)     3562 2023-04-04 06:45:05.000000 cookiemilk-0.1.0/cookiemilk/pathfinder_network.py
+-rw-r--r--   0 weiziqian   (501) staff       (20)     8016 2023-07-10 07:21:42.000000 cookiemilk-0.1.0/cookiemilk/quick_analysis.py
+-rw-rw-r--   0 weiziqian   (501) staff       (20)     3298 2023-04-04 06:13:41.000000 cookiemilk-0.1.0/cookiemilk/text2graph.py
+drwxr-xr-x   0 weiziqian   (501) staff       (20)        0 2023-07-10 07:37:23.398096 cookiemilk-0.1.0/cookiemilk.egg-info/
+-rw-r--r--   0 weiziqian   (501) staff       (20)      766 2023-07-10 07:37:23.000000 cookiemilk-0.1.0/cookiemilk.egg-info/PKG-INFO
+-rw-r--r--   0 weiziqian   (501) staff       (20)      543 2023-07-10 07:37:23.000000 cookiemilk-0.1.0/cookiemilk.egg-info/SOURCES.txt
+-rw-r--r--   0 weiziqian   (501) staff       (20)        1 2023-07-10 07:37:23.000000 cookiemilk-0.1.0/cookiemilk.egg-info/dependency_links.txt
+-rw-r--r--   0 weiziqian   (501) staff       (20)       25 2023-07-10 07:37:23.000000 cookiemilk-0.1.0/cookiemilk.egg-info/requires.txt
+-rw-r--r--   0 weiziqian   (501) staff       (20)       11 2023-07-10 07:37:23.000000 cookiemilk-0.1.0/cookiemilk.egg-info/top_level.txt
+-rw-r--r--   0 weiziqian   (501) staff       (20)       38 2023-07-10 07:37:23.398393 cookiemilk-0.1.0/setup.cfg
+-rw-rw-r--   0 weiziqian   (501) staff       (20)      691 2023-07-10 07:37:06.000000 cookiemilk-0.1.0/setup.py
```

### Comparing `cookiemilk-0.0.8/LICENSE` & `cookiemilk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiemilk-0.0.8/PKG-INFO` & `cookiemilk-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiemilk
-Version: 0.0.8
+Version: 0.1.0
 Summary: An easy-to-use Python package to process knowledge structure data automatically
 Home-page: https://github.com/weiziqianpsych/cookiemilk
 Author: Wei Ziqian
 Author-email: weiziqianpsych@outlook.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cookiemilk-0.0.8/cookiemilk/average_graph.py` & `cookiemilk-0.1.0/cookiemilk/average_graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,65 +4,67 @@
 from .cmap2graph import *
 import networkx as nx
 from heapq import nlargest
 
 
 def average_graph(
         data,
-        keyterms,
+        key_terms,
         pfnet=True,
         max=1,
         min=0.1,
         r=np.inf,
-        n_core=None
+        n_core=None,
+        detailed=True
 ):
 
     # Step 1: obtain matrix data. For each graph, convert data into an n*n similarity matrix (n = number of the given
-    # keyterms) with 1 = 'connected' and 0 = 'unconnected', and then save in 'all_m'
+    # "key_terms") with 1 = 'connected' and 0 = 'unconnected', and then save in 'all_m'
     all_m = []
     for x in range(0, len(data)):
-        m = [[0 for i in range(len(keyterms))] for j in range(len(keyterms))]  # an n*n zero matrix
+        m = [[0 for i in range(len(key_terms))] for j in range(len(key_terms))]  # an n*n zero matrix
 
         for pair in data[x].edges:  # add edges
-            i = keyterms.index(pair[0])
-            j = keyterms.index(pair[1])
+            i = key_terms.index(pair[0])
+            j = key_terms.index(pair[1])
             m[i][j] = 1
             m[j][i] = 1
 
         all_m.append(m)
 
     # Step 2: generate an average matrix
-    average_m = np.array([[0 for i in range(len(keyterms))] for j in range(len(keyterms))])  # an n*n zero matrix
+    average_m = np.array([[0 for i in range(len(key_terms))] for j in range(len(key_terms))])  # an n*n zero matrix
     for i in range(0, len(all_m)):
         average_m = average_m + np.array(all_m[i])
     average_m = average_m/len(all_m)
 
-    # Step 3: define a NetworkX graph, calculate PFNet if necessary
+    # Step 3: define a NetworkX graph and calculate the corresponding PFNet if pfnet=True
     if not pfnet:
         average_ks = nx.Graph()
-        average_ks.add_nodes_from(keyterms)
+        average_ks.add_nodes_from(key_terms)
         pairs = []
         for i in range(0, len(average_m)):
             for j in range(0, len(average_m)):
                 if i != j:
-                    pairs.append([keyterms[i], keyterms[j], average_m[i, j]])
+                    pairs.append([key_terms[i], key_terms[j], average_m[i, j]])
         average_ks.add_weighted_edges_from(pairs)
     else:
-        average_ks = cmap2graph(file=average_m, data_type='array', keyterms=keyterms,
-                                  read_from_file=False, pfnet=True, max=max, min=min, r=r)
+        average_ks = cmap2graph(data=average_m, data_type='array', key_terms=key_terms, read_from_file=False,
+                                pfnet=True, max=max, min=min, r=r)
 
-    # Step 4: remove non-core terms and related links if necessary
+    # Step 4: remove non-core terms and related links if n_core is not None
     if n_core:
         degree = dict(nx.degree_centrality(average_ks))
         core = nlargest(n_core, degree, key=degree.get)
 
         for pair in list(average_ks.edges):  # remove links
             if pair[0] not in core or pair[1] not in core:
                 average_ks.remove_edge(pair[0], pair[1])
-        for term in keyterms:
+        for term in key_terms:
             if term not in core:
                 if term in average_ks.nodes:
                     average_ks.remove_node(term)
 
-    print('an average graph containing {} terms is generated successfully'.format(len(average_ks.nodes)))
+    if detailed:
+        print('An average graph containing {} terms is generated successfully'.format(len(average_ks.nodes)))
 
     return average_ks
```

### Comparing `cookiemilk-0.0.8/cookiemilk/draw.py` & `cookiemilk-0.1.0/cookiemilk/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,23 @@
         show=True,
         save=False,
         filename='filename',
         encoding='utf-8',
         canvas_size=(500, 500),
         node_font='sans-serif',
         node_fontsize=12,
-        node_fontcolor='crimson',
-        node_fillcolor='#ffebcd',
+        node_fontcolour='black',
+        node_fillcolour='lightgrey',
         node_size=12,
-        edge_color='#7ab8cc',
+        edge_colour='lightgrey',
         edge_size=2,
         edge_distance=100,
         charge=-300,
-        detailed=False
+        window_size=(600, 600),
+        detailed=True
 ):
 
     # edges information
     edges = []
     for (u, v, wt) in graph.edges.data():
         # u and v are each node in a proposition
         edges.append({'source': f"{u}", 'target': f"{v}"})
@@ -35,27 +36,27 @@
 
     html = f"""
 <!DOCTYPE html>
 <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
 <style>
 
 .link {{
-    fill: {edge_color};
-    stroke: {edge_color};
+    fill: {edge_colour};
+    stroke: {edge_colour};
     stroke-width: {edge_size}px;
 }}
 
 .node circle {{
-    fill: {node_fillcolor};
-    stroke: {node_fillcolor};
+    fill: {node_fillcolour};
+    stroke: {node_fillcolour};
     stroke-width: {node_size}px;
 }}
 
 text {{
-    fill: {node_fontcolor};
+    fill: {node_fontcolour};
     font: {node_fontsize}px {node_font};
     font-weight: bold;
     pointer-events: none;
 }}
 
 </style>
 <body>
@@ -142,30 +143,26 @@
 //             downloadSVG();
 //         }});
 
 </script>
 
     """
 
-    if detailed is True:
-        print(html)
-
     if save:
         f = open(f'{filename}.html', 'a', encoding=encoding)
         f.write(html)
         f.close()
-        print(f'Save graph to "{filename}.html" successfully.')
+        if detailed:
+            print(f'The visualized graph is saved as a file named "{filename}.html" successfully.')
 
     if graph.name:
         title = graph.name
     else:
         title = 'test'
 
     create_window(title=title,
                   html=html,
-                  width=600,
-                  height=600,
+                  width=window_size[0],
+                  height=window_size[1],
                   on_top=True)
     if show:
         start()
-
-    return edges
```

### Comparing `cookiemilk-0.0.8/cookiemilk/pathfinder_network.py` & `cookiemilk-0.1.0/cookiemilk/pathfinder_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import networkx as nx
 
 
-def pathfinder_network(G, max, min, r=np.inf):
+def pathfinder_network(
+        G,
+        max,
+        min,
+        r=np.inf
+):
 
-    # get adjacency matrix from a graph
+    # Get adjacency matrix from a graph
     array = nx.to_numpy_array(G)
-    origin = array.copy()
     nodes = list(G.nodes)
 
-    # similarity --> dissimilarity (if necessary)
+    # Similarity --> dissimilarity (if necessary)
     if max is not None and min is not None:
         array = max - array + min
 
-    # the value that out of range would be set as inf
+    # Values that out of range would be set as inf
     array = np.where((array >= min) & (array <= max), array, np.inf)
 
-    # pathfinder algorithm
-    array = floyd(dis=array, r=r)  # this array is a PFNet
+    # Pathfinder algorithm
+    array = floyd(dis=array, r=r)
 
-    # diagonal
+    # Values in the diagonal
     np.fill_diagonal(array, False)
 
     # convert the PFNet to a NetworkX graph
     start, end = np.where(np.tril(array) == True)
     pairs = []
     for i in range(0, len(start)):
         pairs.append([nodes[start[i]], nodes[end[i]]])
     G = nx.Graph()
     G.add_edges_from(pairs)
 
     return G
 
 
-def floyd(dis, r=np.inf):
+def floyd(
+        dis,
+        r=np.inf
+):
     """
-
-    derived from:
     Roger Schvaneveldt (2021).
     Pathfinder Networks
     (https://www.mathworks.com/matlabcentral/fileexchange/59378-pathfinder-networks),
     MATLAB Central File Exchange. Retrieved March 23, 2021.
 
     Copyright (c) 2016, Roger Schvaneveldt
     All rights reserved.
@@ -72,26 +77,25 @@
     dis    | dissimilarity matrix
     r      | value of the r parameter
     mindis | minimum distance between nodes
     links  | links in the PFnet(q=n-1,r)
     (based on Floyd algorithm for finding shortest paths)
 
     in this function, parameter q = n - 1, n = number of nodes
-
-    :param dis: dissimilarity matrix
-    :param r: value of the r parameter
-    :return: a PFNet.
     """
 
     mindis = dis.copy()
 
     for ind in range(0, dis.shape[0]):
         for row in range(0, dis.shape[0]):
             for col in range(0, dis.shape[0]):
+
                 # indirect = minkowski(mindis(row,ind), mindis(ind,col),r)
+                # The above is the original code, and I replaced it with the following code, which works as the same
                 indirect = np.linalg.norm([mindis[row, ind], mindis[ind, col]], r)
+
                 if indirect < mindis[row, col]:
                     mindis[row, col] = indirect
 
     tflinks = (dis < np.inf) & (abs(mindis - dis) < 1e-14)
 
     return tflinks
```

### Comparing `cookiemilk-0.0.8/cookiemilk.egg-info/PKG-INFO` & `cookiemilk-0.1.0/cookiemilk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiemilk
-Version: 0.0.8
+Version: 0.1.0
 Summary: An easy-to-use Python package to process knowledge structure data automatically
 Home-page: https://github.com/weiziqianpsych/cookiemilk
 Author: Wei Ziqian
 Author-email: weiziqianpsych@outlook.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cookiemilk-0.0.8/cookiemilk.egg-info/SOURCES.txt` & `cookiemilk-0.1.0/cookiemilk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 cookiemilk/average_graph.py
 cookiemilk/calc_gcent.py
 cookiemilk/calc_graphical_matching.py
 cookiemilk/calc_surface_matching.py
 cookiemilk/calc_tversky.py
 cookiemilk/cmap2graph.py
 cookiemilk/draw.py
-cookiemilk/get_data_files_name.py
-cookiemilk/graph2prxfile.py
 cookiemilk/numerical_sim.py
 cookiemilk/pathfinder_network.py
-cookiemilk/read_file.py
+cookiemilk/quick_analysis.py
 cookiemilk/text2graph.py
 cookiemilk.egg-info/PKG-INFO
 cookiemilk.egg-info/SOURCES.txt
 cookiemilk.egg-info/dependency_links.txt
 cookiemilk.egg-info/requires.txt
 cookiemilk.egg-info/top_level.txt
```

### Comparing `cookiemilk-0.0.8/setup.py` & `cookiemilk-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="cookiemilk",
-    version="0.0.8",
+    version="0.1.0",
     author="Wei Ziqian",
     author_email="weiziqianpsych@outlook.com",
     description="An easy-to-use Python package to process knowledge structure data automatically",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/weiziqianpsych/cookiemilk",
     include_package_data=True,
```

