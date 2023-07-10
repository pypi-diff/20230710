# Comparing `tmp/causalgraph-0.0.6.tar.gz` & `tmp/causalgraph-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalgraph-0.0.6.tar", last modified: Mon Jan 23 13:11:26 2023, max compression
+gzip compressed data, was "causalgraph-0.1.0.tar", last modified: Mon Jul 10 11:21:10 2023, max compression
```

## Comparing `causalgraph-0.0.6.tar` & `causalgraph-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-01-23 13:11:26.554487 causalgraph-0.0.6/
--rw-r--r--   0 sven      (1000) sven      (1000)     1136 2023-01-23 13:00:03.000000 causalgraph-0.0.6/LICENSE
--rw-r--r--   0 sven      (1000) sven      (1000)     8244 2023-01-23 13:11:26.554487 causalgraph-0.0.6/PKG-INFO
--rw-r--r--   0 sven      (1000) sven      (1000)     1238 2022-06-28 08:35:57.000000 causalgraph-0.0.6/README.md
-drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-01-23 13:11:26.544487 causalgraph-0.0.6/causalgraph/
--rw-r--r--   0 sven      (1000) sven      (1000)       35 2022-11-07 15:38:26.000000 causalgraph-0.0.6/causalgraph/__init__.py
--rw-r--r--   0 sven      (1000) sven      (1000)    11877 2023-01-23 13:00:03.000000 causalgraph-0.0.6/causalgraph/graph.py
-drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-01-23 13:11:26.554487 causalgraph-0.0.6/causalgraph/store/
--rw-r--r--   0 sven      (1000) sven      (1000)        0 2022-10-11 13:18:50.000000 causalgraph-0.0.6/causalgraph/store/__init__.py
--rw-r--r--   0 sven      (1000) sven      (1000)    11858 2022-12-05 08:52:50.000000 causalgraph-0.0.6/causalgraph/store/add.py
--rw-r--r--   0 sven      (1000) sven      (1000)     7921 2022-12-05 08:52:50.000000 causalgraph-0.0.6/causalgraph/store/edit.py
--rw-r--r--   0 sven      (1000) sven      (1000)     8812 2022-12-05 08:52:50.000000 causalgraph-0.0.6/causalgraph/store/export.py
--rw-r--r--   0 sven      (1000) sven      (1000)     3116 2022-12-05 08:52:50.000000 causalgraph-0.0.6/causalgraph/store/load.py
--rw-r--r--   0 sven      (1000) sven      (1000)    10527 2022-06-02 12:51:07.000000 causalgraph-0.0.6/causalgraph/store/remove.py
-drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-01-23 13:11:26.554487 causalgraph-0.0.6/causalgraph/utils/
--rw-r--r--   0 sven      (1000) sven      (1000)        0 2022-06-02 12:51:07.000000 causalgraph-0.0.6/causalgraph/utils/__init__.py
--rw-r--r--   0 sven      (1000) sven      (1000)     9204 2023-01-11 10:39:45.000000 causalgraph-0.0.6/causalgraph/utils/draw.py
--rw-r--r--   0 sven      (1000) sven      (1000)     3378 2022-12-05 08:52:50.000000 causalgraph-0.0.6/causalgraph/utils/logging_utils.py
--rw-r--r--   0 sven      (1000) sven      (1000)    18681 2022-12-05 08:52:50.000000 causalgraph-0.0.6/causalgraph/utils/mapping.py
--rw-r--r--   0 sven      (1000) sven      (1000)    20820 2022-12-16 15:19:14.000000 causalgraph-0.0.6/causalgraph/utils/owlready2_utils.py
--rw-r--r--   0 sven      (1000) sven      (1000)      539 2022-06-02 12:51:07.000000 causalgraph-0.0.6/causalgraph/utils/path_utils.py
-drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-01-23 13:11:26.554487 causalgraph-0.0.6/causalgraph.egg-info/
--rw-r--r--   0 sven      (1000) sven      (1000)     8244 2023-01-23 13:11:26.000000 causalgraph-0.0.6/causalgraph.egg-info/PKG-INFO
--rw-r--r--   0 sven      (1000) sven      (1000)      657 2023-01-23 13:11:26.000000 causalgraph-0.0.6/causalgraph.egg-info/SOURCES.txt
--rw-r--r--   0 sven      (1000) sven      (1000)        1 2023-01-23 13:11:26.000000 causalgraph-0.0.6/causalgraph.egg-info/dependency_links.txt
--rw-r--r--   0 sven      (1000) sven      (1000)       97 2023-01-23 13:11:26.000000 causalgraph-0.0.6/causalgraph.egg-info/requires.txt
--rw-r--r--   0 sven      (1000) sven      (1000)       17 2023-01-23 13:11:26.000000 causalgraph-0.0.6/causalgraph.egg-info/top_level.txt
-drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-01-23 13:11:26.554487 causalgraph-0.0.6/data/
--rw-r--r--   0 sven      (1000) sven      (1000)        0 2022-06-02 12:51:07.000000 causalgraph-0.0.6/data/__init__.py
--rwxr-xr-x   0 sven      (1000) sven      (1000)    21520 2022-11-07 15:38:26.000000 causalgraph-0.0.6/data/causalgraph.owl
-drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-01-23 13:11:26.554487 causalgraph-0.0.6/data/logs/
--rw-r--r--   0 sven      (1000) sven      (1000)        0 2022-06-02 12:51:07.000000 causalgraph-0.0.6/data/logs/__init__.py
--rw-r--r--   0 sven      (1000) sven      (1000)       38 2023-01-23 13:11:26.554487 causalgraph-0.0.6/setup.cfg
--rw-r--r--   0 sven      (1000) sven      (1000)     1408 2023-01-23 13:00:03.000000 causalgraph-0.0.6/setup.py
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.558392 causalgraph-0.1.0/
+-rw-r--r--   0 sven      (1000) sven      (1000)     1136 2023-01-23 13:00:03.000000 causalgraph-0.1.0/LICENSE
+-rw-r--r--   0 sven      (1000) sven      (1000)     8244 2023-07-10 11:21:10.558392 causalgraph-0.1.0/PKG-INFO
+-rw-r--r--   0 sven      (1000) sven      (1000)     1238 2022-06-28 08:35:57.000000 causalgraph-0.1.0/README.md
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.518392 causalgraph-0.1.0/causalgraph/
+-rw-r--r--   0 sven      (1000) sven      (1000)       35 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/__init__.py
+-rw-r--r--   0 sven      (1000) sven      (1000)    12611 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/graph.py
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.518392 causalgraph-0.1.0/causalgraph/store/
+-rw-r--r--   0 sven      (1000) sven      (1000)        0 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/store/__init__.py
+-rw-r--r--   0 sven      (1000) sven      (1000)    14632 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/store/add.py
+-rw-r--r--   0 sven      (1000) sven      (1000)     9741 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/store/edit.py
+-rw-r--r--   0 sven      (1000) sven      (1000)     9248 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/store/export.py
+-rw-r--r--   0 sven      (1000) sven      (1000)     3164 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/store/load.py
+-rw-r--r--   0 sven      (1000) sven      (1000)    13951 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/store/remove.py
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.518392 causalgraph-0.1.0/causalgraph/utils/
+-rw-r--r--   0 sven      (1000) sven      (1000)        0 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/utils/__init__.py
+-rw-r--r--   0 sven      (1000) sven      (1000)     9184 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/utils/draw.py
+-rw-r--r--   0 sven      (1000) sven      (1000)     3378 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/utils/logging_utils.py
+-rw-r--r--   0 sven      (1000) sven      (1000)    20735 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/utils/mapping.py
+-rw-r--r--   0 sven      (1000) sven      (1000)     2609 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/utils/misc_utils.py
+-rw-r--r--   0 sven      (1000) sven      (1000)    43391 2023-07-10 11:20:33.000000 causalgraph-0.1.0/causalgraph/utils/owlready2_utils.py
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.518392 causalgraph-0.1.0/causalgraph.egg-info/
+-rw-r--r--   0 sven      (1000) sven      (1000)     8244 2023-07-10 11:21:10.000000 causalgraph-0.1.0/causalgraph.egg-info/PKG-INFO
+-rw-r--r--   0 sven      (1000) sven      (1000)      695 2023-07-10 11:21:10.000000 causalgraph-0.1.0/causalgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 sven      (1000) sven      (1000)        1 2023-07-10 11:21:10.000000 causalgraph-0.1.0/causalgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 sven      (1000) sven      (1000)      116 2023-07-10 11:21:10.000000 causalgraph-0.1.0/causalgraph.egg-info/requires.txt
+-rw-r--r--   0 sven      (1000) sven      (1000)       17 2023-07-10 11:21:10.000000 causalgraph-0.1.0/causalgraph.egg-info/top_level.txt
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.518392 causalgraph-0.1.0/data/
+-rw-r--r--   0 sven      (1000) sven      (1000)        0 2022-06-02 12:51:07.000000 causalgraph-0.1.0/data/__init__.py
+-rwxr-xr-x   0 sven      (1000) sven      (1000)    23429 2023-07-07 09:00:32.000000 causalgraph-0.1.0/data/causalgraph.owl
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.518392 causalgraph-0.1.0/data/logs/
+-rw-r--r--   0 sven      (1000) sven      (1000)        0 2022-06-02 12:51:07.000000 causalgraph-0.1.0/data/logs/__init__.py
+-rw-r--r--   0 sven      (1000) sven      (1000) 58232612 2023-07-06 07:59:43.000000 causalgraph-0.1.0/data/logs/cg.json
+-rw-r--r--   0 sven      (1000) sven      (1000)       38 2023-07-10 11:21:10.558392 causalgraph-0.1.0/setup.cfg
+-rw-r--r--   0 sven      (1000) sven      (1000)     1409 2023-07-10 11:20:09.000000 causalgraph-0.1.0/setup.py
+drwxr-xr-x   0 sven      (1000) sven      (1000)        0 2023-07-10 11:21:10.558392 causalgraph-0.1.0/tests/
+-rw-r--r--   0 sven      (1000) sven      (1000)     9743 2023-07-07 09:00:32.000000 causalgraph-0.1.0/tests/test_graph.py
```

### Comparing `causalgraph-0.0.6/LICENSE` & `causalgraph-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causalgraph-0.0.6/PKG-INFO` & `causalgraph-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalgraph
-Version: 0.0.6
+Version: 0.1.0
 Summary: A python package for modeling, persisting and visualizing causal graphs embedded in knowledge graphs.
 Author: Fraunhofer IWU
 Author-email: causalgraph@iwu.fraunhofer.de
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: causalgraph Version: 0.0.6 Summary: A python
+Metadata-Version: 2.1 Name: causalgraph Version: 0.1.0 Summary: A python
 package for modeling, persisting and visualizing causal graphs embedded in
 knowledge graphs. Author: Fraunhofer IWU Author-email:
 causalgraph@iwu.fraunhofer.de License: MIT Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
 Content-Type: text/markdown License-File: LICENSE  [![IWU][iwu-shield]](https:/
 /www.iwu.fraunhofer.de/) [![Tests][pytest-shield]](https://github.com/
 causalgraph/causalgraph/actions) [![License][mit-licence]](https://
```

### Comparing `causalgraph-0.0.6/README.md` & `causalgraph-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `causalgraph-0.0.6/causalgraph/graph.py` & `causalgraph-0.1.0/causalgraph/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,111 +19,115 @@
 from causalgraph.store.add import Add
 from causalgraph.store.edit import Edit
 from causalgraph.utils.draw import Draw
 from causalgraph.store.remove import Remove
 from causalgraph.utils.mapping import Mapping
 import causalgraph.utils.owlready2_utils as owlutils
 from causalgraph.utils.logging_utils import init_logger
-from causalgraph.utils.path_utils import get_project_root
+from causalgraph.utils.misc_utils import get_project_root
 CAUSALGRAPH_ONTO_PATH: Path = Path.joinpath(get_project_root(), "data", 'causalgraph.owl')
 
 from causalgraph.store.load import Load
 from causalgraph.store.export import Export
 from typing import Union
 import networkx
 
 class Graph():
     """ Graph with causal information embedded in knowledge graph.
     """
     def __init__(self, 
-                sql_db_filename: str = "causalgraph.sqlite3",
+                sql_db_filename: str = None,
                 sql_exclusive: bool = False,
                 log_file_dir: str = None,
                 logger_level: int = logging.WARNING,
                 external_ontos: list[str] = None,
                 external_graph: Union[networkx.MultiDiGraph, tuple] = None,
+                validate_domain_range: bool = True
     ) -> None:
         """Instantiates a Graph as the central object of causalgraph.
 
-        :param sql_db_filename: path to sqlite3.db for storage, defaults to "causalgraph.sqlite3"
+        :param sql_db_filename: Optional path to a sqlite3-DB (path ending with .sqlite3) for storing the graph in a db. Set None for storing on memory, defaults to None
         :type sql_db_filename: str, optional
         :param sql_exclusive: if sql-db should be closed for parallel requests, defaults to False
         :type sql_exclusive: bool, optional
         :param log_file_dir: path to the log-file directory, defaults to '{project_root}/data/logs/cg.json'
         :type log_file_dir: str, optional
         :param logger_level: Verbosity level of logger
         :type logger_level: int
         :param external_ontos: List of local Paths to file or URL to ontology in web.
         :type external_ontos: list[str], optional
         :param external_graph: NetworkX.MultiDiGraph or Tigramite Graph representation.
         :type external_graph: Union[networkx.MultiDiGraph, Tuple(list, dict, ndarray, ndarray, int)], optional
+        :param validate_domain_range: If True, all properties will be evaluated with domain and range before creating new individuals, defaults to True
+        :type validate_domain_range: bool, optional
         """
         # Store attributes if necessary
         self.sql_db_filename = sql_db_filename
         self.core_onto_path = CAUSALGRAPH_ONTO_PATH.absolute()
+        self.validate_domain_range = validate_domain_range
         # Check if necessary onto_file is present:
         if self.core_onto_path.is_file() is False:
             raise FileNotFoundError("The necessary base ontology 'causalgraph' was not found at " +
                                     f"expected location {self.core_onto_path}.")
         ## Initialize
         self.logger = init_logger(logger_name= "cg",
                                   file_handler_level=logging.DEBUG,
                                   console_handler_level=logger_level,
                                   file_handler=True,
                                   elastic_style_json=True,
                                   log_file_dir=log_file_dir)
         self.store = self._init_store_backend_sqldb(self.sql_db_filename, sql_exclusive)
         self.individuals_onto, self.classes_onto = self._init_namespaces(self.core_onto_path, self.store)
-        self.map = Mapping(graph=self, logger=self.logger)
         # Include functionalities wrapped in singleton objects
-        self.add = Add(store=self.store, logger=self.logger)
-        self.edit = Edit(store=self.store, logger=self.logger)
+        self.add = Add(store=self.store, logger=self.logger, validate_domain_range=self.validate_domain_range)
+        self.edit = Edit(store=self.store, logger=self.logger, validate_domain_range=self.validate_domain_range)
         self.remove = Remove(store=self.store, logger=self.logger)
+        self.map = Mapping(graph=self, logger=self.logger)
         self.export = Export(graph=self, logger=self.logger)
         self.load = Load(graph=self, logger=self.logger)
         self.draw = Draw(graph=self)
-
         # Check if there are third party ontos to be loaded directly at start
         if external_ontos is not None:
             for onto_path in external_ontos:
                 self.import_ontology(onto_path)
-        
-        ### Check if nx or tigra was passed
+        ### Check if external graph (nx or tigra) was passed
         if external_graph is not None:
-            if type(external_graph) is networkx.MultiDiGraph:
-                graph_dict = self.map.graph_dict_from_nx(external_graph)
-                #print(graph_dict)
+            self._init_external_graph(external_graph)
+        self.logger.info("Initialized the Causal Knowledge Graph.")
+
+        
+    def _init_external_graph(self, external_graph: Union[networkx.MultiDiGraph, tuple]):
+        if type(external_graph) is networkx.MultiDiGraph:
+            graph_dict = self.map.graph_dict_from_nx(external_graph)
+            _ = self.map.fill_empty_graph_from_dict(graph_dict)
+            graph_dict = self.map.all_individuals_to_dict()
+            if graph_dict != {}:
+                self.logger.info("Init by importing a MultiDiGraph has been successful.")
+            else:
+                self.logger.error("Importing the MultiDiGraph did not result in any instantiation of individuals in the new graph.")
+        elif type(external_graph) in [tuple, Tuple]:
+            if len(external_graph) == 5:
+                graph_dict = self.map.graph_dict_from_tigra(
+                    node_names=external_graph[0],
+                    edge_names=external_graph[1],
+                    link_matrix=external_graph[2],
+                    q_matrix=external_graph[3],
+                    timestep_len_s=external_graph[4])
                 _ = self.map.fill_empty_graph_from_dict(graph_dict)
                 graph_dict = self.map.all_individuals_to_dict()
                 if graph_dict != {}:
-                    self.logger.info("Init by importing a MultiDiGraph has been successful.")
-                else:
-                    self.logger.error("Importing the MultiDiGraph did not result in any instantiation of individuals in the new graph.")
-            elif type(external_graph) in [tuple, Tuple]:
-                if len(external_graph) == 5:
-                    graph_dict = self.map.graph_dict_from_tigra(
-                        external_graph[0],
-                        external_graph[1],
-                        external_graph[2],
-                        external_graph[3],
-                        external_graph[4])
-                    _ = self.map.fill_empty_graph_from_dict(graph_dict)
-                    graph_dict = self.map.all_individuals_to_dict()
-                    if graph_dict != {}:
-                        self.logger.info("Init by importing a Tigramite Tuple has been successful.")
-                    else:
-                        self.logger.error("Importing the Tigramite Tuple did not result in any instantiation of individuals in the new graph.")
+                    self.logger.info("Init by importing a Tigramite Tuple has been successful.")
                 else:
-                    self.logger.error("Passed Tigramite Tuple has the wrong format. Please pass a Tuple with the Format " + 
-                    "(node_names, edge_names, link_matrix, q_matrix, timestep_len_s).")
+                    self.logger.error("Importing the Tigramite Tuple did not result in any instantiation of individuals in the new graph.")
             else:
-                self.logger.error("Wrong external graph format. Please pass a MultiDiGraph or Tigramite Tuple. " + 
-                "A empty causalgraph has been initialized.")
-
-        self.logger.info("Initialized the Graph.")
+                self.logger.error("Passed Tigramite Tuple has the wrong format. Please pass a Tuple with the Format " + 
+                "(node_names, edge_names, link_matrix, q_matrix, timestep_len_s).")
+        else:
+            self.logger.error("Wrong external graph format. Please pass a MultiDiGraph or Tigramite Tuple. " + 
+            "A empty causalgraph has been initialized.")
 
 
     def _init_store_backend_sqldb(self, sql_db_path: str, sql_exclusive: bool) -> owlready2.World:
         """Initializes the Graph store as an owlready2.World which stores data in a SQL-DB.
 
         Per default, the Store is persisted in a SQLite3 file, specified by sql_db_filepath.
         For multi-user_access to the SQL-DB, choose sql_exclusive= False.
@@ -132,15 +136,18 @@
         :type sql_db_path: str
         :param sql_exclusive: Protect SQL from other users= exclusive, disable for multi-access
         :type sql_exclusive: bool
         :return: Graphstore Backend
         :rtype: owlready2.World
         """
         store = owlready2.World()
-        if Path(sql_db_path).is_file:
+        if sql_db_path is None:
+            self.logger.info(f"Using in memory ontology store. Graph will not be saved after stopping the program.")
+            return store
+        elif Path(sql_db_path).is_file():
             store.set_backend(filename=sql_db_path, exclusive=sql_exclusive)
             self.logger.warning(f"Using existing ontology store at {Path(sql_db_path).absolute()}")
         else:
             store.set_backend(filename=sql_db_path, exclusive=sql_exclusive)
             self.logger.info(f"Created empty ontology storage at {Path(sql_db_path).absolute()}")
         return store
```

### Comparing `causalgraph-0.0.6/causalgraph/store/add.py` & `causalgraph-0.1.0/causalgraph/store/add.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 """ Contains Add Class to add things to the store.
 Store is equivalent to owlready2 World """
 
 # general imports
 import itertools
 from logging import Logger
 import owlready2
+from typing import Union
 # causalgraph imports
 import causalgraph.utils.owlready2_utils as owlutils
+from causalgraph.utils.misc_utils import strict_types
 from causalgraph.utils.logging_utils import init_logger
 
 
 class Add():
     """ Contains all methods to add resources to the store """
-    def __init__(self, store: owlready2.World, logger: Logger = None) -> None:
+    def __init__(self, store: owlready2.World, logger: Logger = None, validate_domain_range: bool = True) -> None:
         self.store = store
+        self.validate_domain_range = validate_domain_range
         if logger is not None:
             self.logger = logger
         else:
             self.logger = init_logger("Add")
         self.logger.info("Initialized the 'add' functionalities.")
         self.classes_prohibited_from_causal_connections = self._init_classes_prohibited_for_causal_connections()
 
@@ -38,100 +41,133 @@
         base_prohibitions = ['CausalEdge', 'CausalGraph', 'Creator']
         # get subclasses as well and flatten list
         prohibited_with_subtypes = [owlutils.get_subclasses(class_name, self.store) for class_name in base_prohibitions]
         flattened_prohibited_with_subtypes = list(itertools.chain.from_iterable(prohibited_with_subtypes))
         return flattened_prohibited_with_subtypes
 
 
-    def individual_of_type(self, class_of_individual: str, name_for_individual: str= None, **kwargs) -> str:
+    @strict_types
+    def individual_of_type(self, class_of_individual: Union[str, owlready2.Thing], name_for_individual: str = None, 
+                           validate_domain_range: bool = None, **kwargs) -> owlready2.EntityClass:
         """Instantiates an individual of the class(type) specified.
 
         Wraps the default owlready2 functions with error handling and logging.
         Via the optional **kwargs one can also set properties, similar to description here:
         https://owlready2.readthedocs.io/en/v0.35/class.html#creating-individuals
 
         Example:
         edge_name = graph.add.individual_of_type(class_of_individual= "CausalEdge",
-                                                 hasCause= [node1],
-                                                 hasEffect= [node2],
+                                                 hasCause=node1,
+                                                 hasEffect=node2,
                                                  comment= ["an optional comment"])
 
-        :param class_of_individual: class name of individual
+        :param class_of_individual: class of individual as name or object
         :type class_of_individual: str
         :param name_for_individual: name for individual, defaults to <class_name><no>
         :type name_for_individual: str, optional
-        :return: final name of individual or 'None' if creation failed
-        :rtype: str
+        :param validate_domain_range: Switch to only allow creation of new individuals with valid domain and range for all properties, defaults to 'Graph.validate_domain_range'
+        :type validate_domain_range: bool, optional
+        :return: Entity Object (class/property/individual) of the created individual or 'None' if creation failed
+        :rtype: owlready2.EntityClass
         """
-        return owlutils.create_individual_of_type(class_of_individual= class_of_individual,
-                                                  store= self.store,
-                                                  name_for_individual= name_for_individual,
-                                                  logger= self.logger,
+        if validate_domain_range is None:
+            validate_domain_range = self.validate_domain_range
+        return owlutils.create_individual_of_type(class_of_individual=class_of_individual,
+                                                  store=self.store,
+                                                  name_for_individual=name_for_individual,
+                                                  logger=self.logger,
+                                                  validate_domain_range=validate_domain_range,
                                                   **kwargs)
 
 
-    def causal_node(self, individual_name: str = None, **kwargs) -> str:
+    @strict_types
+    def causal_node(self, individual_name: str = None, validate_domain_range: bool = None, **kwargs) -> owlready2.EntityClass:
         """Creates an individual of class "CausalNode" with the name 'individual_name'.
         If no name is given, the name is automatically generated from the Class name and a number.
         Via the optional **kwargs, arbitrary properties can be set, similar to description here:
         https://owlready2.readthedocs.io/en/v0.35/class.html#creating-individuals
 
         Example for adding a creator individual named 'supercreator':
         causal_node_name = add.causal_node(hasCreator=[creator_node], comment=["optional comment"])
 
         :param instance_name: desired name for individual, defaults to causalnode<no>
         :type instance_name: str, optional
-        :return: name of created individual or None if no node is created
-        :rtype: str
+        :param validate_domain_range: Switch to only allow creation of new individuals with valid domain and range for all properties, defaults to 'Graph.validate_domain_range'
+        :type validate_domain_range: bool, optional
+        :return: Entity Object of the created CausalNode or 'None' if no new CausalNode was created
+        :rtype: owlready2.EntityClass
         """
-        causal_node_name = owlutils.create_individual_of_type(class_of_individual= 'CausalNode',
+        if validate_domain_range is None:
+            validate_domain_range = self.validate_domain_range
+        causal_node_object = owlutils.create_individual_of_type(class_of_individual= 'CausalNode',
                                                               store= self.store,
                                                               name_for_individual= individual_name,
                                                               logger= self.logger,
+                                                              validate_domain_range=validate_domain_range,
                                                               **kwargs)
         self.store.save()
-        return causal_node_name
+        return causal_node_object
 
 
-    def causal_edge(self, cause_node_name: str, effect_node_name: str, name_for_edge: str = None,
-                    confidence: float = None, time_lag_s: float = None, force_create: bool = False, **kwargs) -> str:
-        """Adds a 'CausalEdge' between Nodes with names 'cause_node_name' and 'effect_node_name'.
+    @strict_types
+    def causal_edge(self, cause_node: Union[str, owlready2.Thing], effect_node: Union[str, owlready2.Thing], name_for_edge: str = None,
+                    confidence: float = None, time_lag_s: float = None, force_create: bool = False, validate_domain_range: bool = None,
+                    **kwargs) -> owlready2.EntityClass:
+       
+        """Adds a 'CausalEdge' between Nodes with names 'cause_node' and 'effect_node'.
 
         Via the optional **kwargs, arbitrary properties can be set, similar to description here:
         https://owlready2.readthedocs.io/en/v0.35/class.html#creating-individuals
 
         Example (equivalent):
-        - edge_name= graph.add.causal_edge(cause_node_name= cause_node,
-                                            effect_node_name = effect_node,
+        - edge_name= graph.add.causal_edge(cause_node= cause_node,
+                                            effect_node = effect_node,
                                             confidence= 0.2,
                                             comment= ["an optional comment"])
-        - edge_name2= graph.add.causal_edge(cause_node_name= cause_node,
-                                            effect_node_name= effect_node,
+        - edge_name2= graph.add.causal_edge(cause_node= cause_node,
+                                            effect_node= effect_node,
                                             hasConfidence= 0.2,
                                             comment= ["an optional comment"])
 
-        :param cause_node_name: name of the cause node, where the edge originates
-        :type cause_node_name: str
-        :param effect_node_name: name of the effect node, where the edge ends
-        :type effect_node_name: str
+        :param cause_node: A existing CausalNode object or the name of it. Describes the cause node.
+        :type cause_node: Union[str, owlready2.Thing]
+        :param effect_node: A existing CausalNode object or the name of it. Describes the effect node.
+        :type effect_node: Union[str, owlready2.Thing]
         :param name_for_edge: optional name for the edge, defaults to None
         :type name_for_edge: str, optional
         :param confidence: confidence in the edge's existence, defaults to None
         :type confidence: float, optional
         :param time_lag_s: time lag between cause and effect in seconds, defaults to None
         :type time_lag_s: float, optional
         :param force_create: Enable force creation of missing cause/effect node with type
         'CausalNode', defaults to False
         :type force_create: bool, optional
-        :return: edge_name of created edge if successful, None otherwise
-        :rtype: str
+        :param validate_domain_range: Switch to only allow creation of new individuals with valid domain and range for all properties, defaults to 'Graph.validate_domain_range'
+        :type validate_domain_range: bool, optional
+        :return: Entity Object of the created CausalEdge or 'None' if no new CausalEdge was created
+        :rtype: owlready2.EntityClass
         """
+        if validate_domain_range is None:
+            validate_domain_range = self.validate_domain_range
+
+        # Get names and objects of cause and effect node
+        cause_node_name, cause_node_obj = owlutils.get_name_and_object(cause_node, self.store, True)
+        effect_node_name, effect_node_obj = owlutils.get_name_and_object(effect_node, self.store, True)
+
+        # If a Thing was passed, then check if it (still) exists
+        if (cause_node_name is None and cause_node_obj is None):
+            self.logger.error(f"The passed cause object '{cause_node}' does not exist.")
+            return None
+        elif (effect_node_name is None and effect_node_obj is None):
+            self.logger.error(f"The passed effect object '{effect_node}' does not exist.")
+            return None
+
         # Check if edge already exists
-        individual_names = [ind.name for ind in self.store.individuals()]
-        if name_for_edge in individual_names:
+        edge_existing = owlutils.get_entity_by_name(name_for_edge, self.store, suppress_warn=True)
+        if edge_existing is not None:
             self.logger.warning(f"Can't create CausalEdge {name_for_edge}. Name already taken.")
             return None
         # Check if both nodes exist, else: return None or force create node if specified
         for node_name in (cause_node_name, effect_node_name):
             if not owlutils.entity_exists(node_name, self.store):
                 if force_create is False:
                     self.logger.error(f"Cannot create CausalEdge between {cause_node_name} --> " +
@@ -142,15 +178,15 @@
                 self.logger.warning(f"Node '{node_name}' did not exist. Creating Node " +
                                     f"of type 'CausalNode' with name '{node_name}' now.")
                 self.causal_node(node_name)
         # Check if Nodes have Type CausalNode, if not: Store to add CausalNode type
         # (only if NOT of a type which is excluded from drawing CausalEdges in between)
         nodes_that_need_causal_node_type_added = []
         for node_name in (cause_node_name, effect_node_name):
-            if owlutils.is_instance_of_class(node_name, 'CausalNode', self.store, include_subtypes=True):
+            if owlutils.is_instance_of_type(node_name, 'CausalNode', self.store, include_subtypes=True):
                 pass
             else:
                 # Check if class_type is part of types prohibited for new nodes:
                 node = owlutils.get_entity_by_name(node_name, self.store)
                 class_type = node.is_a
                 if class_type not in self.classes_prohibited_from_causal_connections:
                     nodes_that_need_causal_node_type_added.append(node)
@@ -172,49 +208,51 @@
             else:
                 # if not: don't append
                 pass
         # Get Object representation of nodes
         cause_node = owlutils.get_entity_by_name(cause_node_name, self.store, logger=self.logger)
         effect_node = owlutils.get_entity_by_name(effect_node_name, self.store, logger=self.logger)
         # Add additional properties to edge, depending on inputs
-        edge_properties_dict = dict(hasCause=[cause_node], hasEffect=[effect_node])
+        edge_properties_dict = dict(hasCause=cause_node, hasEffect=effect_node)
         if confidence is not None:
-            if 0.0 < confidence <= 1.0:
+            if 0.0 <= confidence <= 1.0:
                 edge_properties_dict['hasConfidence'] = confidence
             else:
                 self.logger.error(f"Cannot create CausalEdge between {cause_node_name} --> " +
                                   f"{effect_node_name}. Specified confidence {confidence} " +
                                    "exceeds range [0,1]. ")
                 return None
         if time_lag_s is not None:
-            if time_lag_s > 0.0:
+            if time_lag_s >= 0.0:
                 edge_properties_dict['hasTimeLag'] = time_lag_s
             else:
                 self.logger.error(f"Cannot create CausalEdge between '{cause_node_name}--> " +
                                   f"{effect_node_name}. Specified time_lag_s {time_lag_s} " +
                                    "is negative.")
                 return None
         # Create edge with objects
         if name_for_edge is not None:                    
-            edge_name = owlutils.create_individual_of_type(
+            new_edge_object = owlutils.create_individual_of_type(
                 class_of_individual="CausalEdge",
                 store=self.store,
                 name_for_individual=name_for_edge,
                 logger=self.logger,
+                validate_domain_range=validate_domain_range,
                 **edge_properties_dict, **kwargs
             )
         else:
-            edge_name = owlutils.create_individual_of_type(
+            new_edge_object = owlutils.create_individual_of_type(
                 class_of_individual="CausalEdge",
                 store=self.store,
                 name_for_individual=None,
                 logger=self.logger,
+                validate_domain_range=validate_domain_range,
                 **edge_properties_dict, **kwargs
             )
-        if edge_name is not None:
+        if new_edge_object is not None:
             self.logger.info(f"Created CausalEdge between cause '{cause_node_name}' and effect " +
                             f"'{effect_node_name}'")
             self.store.save()
         else:
             self.logger.warning("Creation failed. No Edge added between cause" +
                                 f"{cause_node_name} and effect {effect_node_name}")
-        return edge_name
+        return new_edge_object
```

### Comparing `causalgraph-0.0.6/causalgraph/store/edit.py` & `causalgraph-0.1.0/causalgraph/store/edit.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,168 +4,191 @@
 
 """ Contains Edit Class to edit things in the store.
 Store is equivalent to owlready2 World """
 
 # general imports
 from logging import Logger
 import owlready2
+from typing import Union
 # causalgraph imports
 import causalgraph.utils.owlready2_utils as owlutils
+from causalgraph.utils.misc_utils import strict_types
 from causalgraph.utils.logging_utils import init_logger
 
 
 class Edit():
     """ Contains all methods to edit resources in the store"""
-    def __init__(self, store: owlready2.World, logger: Logger = None) -> None:
+    def __init__(self, store: owlready2.World, logger: Logger = None, validate_domain_range: bool = True) -> None:
         self.store = store
+        self.validate_domain_range = validate_domain_range
         if logger is not None:
             self.logger = logger
         else:
             self.logger = init_logger("Edit")
         self.logger.info("Initialized the 'edit' functionalities.")
 
 
-    def rename_individual(self, old_name: str, new_name: str) -> bool:
-        """This method changes the name of an individual. To change it, pass the old name as
-        well as the new desired name. The return value is True if the change was successful,
-        False if not.
+    @strict_types
+    def rename_individual(self, old_name_obj: Union[str, owlready2.Thing], new_name: str) -> bool:
+        """This method changes the name of an individual. To change it, pass the old name or the
+        the individual it self as well as the new desired name. The return value is True if the
+        change was successful, False if not.
 
-        :param old_name: Current name of the individual to be renamed.
-        :type old_name: str
+        :param old_name_obj: The object of the individual to be changed or its name as str.
+        :type old_name_obj: Union[str, owlready2.Thing],
         :param new_name: Desired new name of the individual
         :type new_name: str
         :return: True if renaming was successful, False if not.
         :rtype: bool
         """
-        # Return False if individual with old_name does not exist.
-        indi_old_name = owlutils.get_entity_by_name(name_of_entity=old_name, store=self.store)
-        if indi_old_name is None:
-            self.logger.warning(f'Name change not successful because the individual {old_name}' +
-                                 'does not exist.')
-            return False
+        indi_old_name_name, ind_old_name_obj = owlutils.get_name_and_object(old_name_obj, self.store)
+
+        # If a Thing was passed, then check if it (still) exists
+        if ind_old_name_obj is None:
+            self.logger.warning(f"Name change not successful because the individual '{indi_old_name_name}'" +
+                                 " does not exist.")
+            return False        
         # Check if new_name is already taken
-        indi_new_name = owlutils.get_entity_by_name(new_name, self.store, suppress_warn=True)
-        if indi_new_name is not None:
-            self.logger.warning(f'Name change not successful because the new name {new_name}' +
-                                 'is already taken.')
+        indi_new_name_obj = owlutils.get_entity_by_name(new_name, self.store, suppress_warn=True)
+        if indi_new_name_obj is not None:
+            self.logger.warning(f"Name change not successful because the new name '{new_name}'" +
+                                 " is already taken.")
             return False
         # Renaming individuals and check success
-        indi_old_name.name = new_name
+        ind_old_name_obj.name = new_name
         # Success check not absolutely necessary, but in there for safety's sake.
-        indi_old_name = owlutils.get_entity_by_name(old_name, self.store, suppress_warn=True)
-        indi_new_name = owlutils.get_entity_by_name(new_name, self.store, suppress_warn=True)
+        ind_old_name_obj = owlutils.get_entity_by_name(indi_old_name_name, self.store, suppress_warn=True)
+        indi_new_name_obj = owlutils.get_entity_by_name(new_name, self.store, suppress_warn=True)
         self.store.save()
-        if indi_old_name is None and indi_new_name is not None:
-            self.logger.info(f'Renaming individual {old_name} to {new_name} has been successful.')
+        if ind_old_name_obj is None and indi_new_name_obj is not None:
+            self.logger.info(f"Renaming individual '{indi_old_name_name}' to '{new_name}' has been successful.")
             return True
-        self.logger.warning(f'Something went wrong while renaming {old_name} to {new_name}' +
-                             'although the required name is not taken.')
+        self.logger.warning(f"Something went wrong while renaming '{indi_old_name_name}' to '{new_name}'" +
+                             " although the required name is not taken.")
         return False
 
 
-    def type_to_subtype(self, name_of_entity: str, new_type: str) -> bool:
+    @strict_types
+    def type_to_subtype(self, entity: Union[str, owlready2.Thing], new_type: Union[str, owlready2.EntityClass]) -> bool:
         """This method changes the type of an individual. Only subtypes are allowed as new types.
         To change the type, pass the name of the individual and the new desired (sub)type.
         The return value is True if the type change was successful, False if not or the new
         type is the same as the current one.
 
-        :param name_of_entity: Name (IRI) of the individual to be changed.
-        :type name_of_entity: str
-        :param new_type: Name (IRI) of the desired type.
-        :type new_type: str
+        :param entity: The individual object to be changed or its name.
+        :type entity: Union[str, owlready2.Thing]
+        :param new_type: The name of the new (sub)type or the owlready EntityClass object.
+        :type new_type: Union[str, owlready2.EntityClass]
         :return: True if type change was successful, False if not or type didn't change
         :rtype: bool
         """
-        # Get individual and its current type(s) by node_name
-        individual = owlutils.get_entity_by_name(name_of_entity=name_of_entity, store=self.store)
+        individual_name, individual_obj = owlutils.get_name_and_object(entity, self.store)
+        # Exit func if individual does not exist
+        if individual_obj is None:
+            self.logger.error(f"Changing subtype failed. Entity '{individual_name}' does not exist.")
+            return False
         # Initiate empty lists for collecting types that should (not) be changed
         types_to_keep = []
         types_to_update = []
+
         # Get new subtype object and check if it exists
-        exists_check = owlutils.entity_exists(entity_name=new_type, store=self.store)
-        if exists_check is False:
+        new_subtype_name, new_subtype_obj = owlutils.get_name_and_object(new_type, self.store)
+        if new_subtype_obj == None:
             self.logger.warning(f'Changing subtype failed. New subtype {new_type} does not ' +
                                  'exist in the Ontology.')
             return False
-        # Check if new_subtype_object is related to current_subtype, if so it needs to be updated
-        new_subtype_object = owlutils.get_entity_by_name(name_of_entity=new_type, store=self.store)
-        for current_type in individual.is_a:
-            current_type_subtypes = owlutils.get_subclasses(current_type.name, self.store)
+        # Check if subtype is valid for passed individual
+        for current_type in individual_obj.is_a:
+            current_type_subtypes = owlutils.get_subclasses(current_type, self.store)
             # If new type is a valid subtype of the old type: substitute old type, else: keep type
-            if [new_subtype_object] in current_type_subtypes:
+            if [new_subtype_obj] in current_type_subtypes:
                 types_to_update.append(current_type)
             else:
                 types_to_keep.append(current_type)
         # The list "types_to_update" will be empty if there is currently no type that is related to
         # "new_type" and therefore also not allowed to be specialized in the subtype "new_type"
         if types_to_update == []:
-            self.logger.warning(f'None of the current types of {name_of_entity} is allowed to be' +
-                                 'changed to the subtype {new_type}')
+            self.logger.warning(f"None of the current types of '{individual_name}' is allowed to be" +
+                                f"changed to the subtype {new_subtype_name}")
             return False
-        # Generate list of new types from types_to_keep and new_subtype_object
+        # Generate list of new types from types_to_keep and new_subtype_obj
         new_types = types_to_keep
-        new_types.append(new_subtype_object)
+        new_types.append(new_subtype_obj)
         # Swap current types of individual with new ones
-        individual.is_a = new_types
+        individual_obj.is_a = new_types
         self.store.save()
         types_to_update_names = [i.name for i in types_to_update]
-        self.logger.info(f'Changing type(s) { {*types_to_update_names} } to {new_type} successful.')
+        self.logger.info(f'Changing type(s) { {*types_to_update_names} } to {new_subtype_name} successful.')
         return True
 
 
-    def properties(self, individual_name: str, prop_dict: dict) -> bool:
+    @strict_types
+    def properties(self, entity: Union[str, owlready2.Thing], prop_dict: dict) -> bool:
         """Updates the properties of an individual with the properties
            and values given in the dictionary.
 
-        :param individual_name: Name of the individual
-        :type individual_name: str
+        :param entity: The individual object to be changed or its name.
+        :type entity: Union[str, owlready2.Thing]
         :param prop_dict: Dictionary containing properties and their new values
         :type prop_dict: dict
         :return: True if update successful, else False
         :rtype: bool
         """
-        update_prop_result = owlutils.update_properties_of_individual(individual_name=individual_name, logger=self.logger, store=self.store, prop_dict=prop_dict)
+        individual_name, _ = owlutils.get_name_and_object(entity, self.store)
+        update_prop_result = owlutils.update_properties_of_individual(individual=individual_name,
+                                                                      logger=self.logger,
+                                                                      store=self.store,
+                                                                      prop_dict=prop_dict,
+                                                                      validate_domain_range=self.validate_domain_range)
         return update_prop_result
 
 
-    def property(self, individual_name: str, property_name: str, value) -> bool:
+    @strict_types
+    def property(self, entity: Union[str, owlready2.Thing], property: Union[str, owlready2.PropertyClass], value) -> bool:
         """Updates one property of an individual
 
-        :param individual_name: Name of the individual
-        :type individual_name: str
-        :param property_name: Property to be updated
-        :type property_name: str
+        :param entity: The individual object to be changed or its name.
+        :type entity: Union[str, owlready2.Thing]
+        :param property: The property name or the owlready PropertyClass object.
+        :type property: Union[str, owlready2.PropertyClass]
         :param value: New value of the property
         :type value: _type_
         :return: True if update successful, else False
         :rtype: bool
         """
+        individual_name, _ = owlutils.get_name_and_object(entity, self.store)
+        property_name, _ = owlutils.get_name_and_object(property, self.store)
         prop_dict = {property_name: value}
         return self.properties(individual_name, prop_dict)
 
 
-    def delete_property(self, individual_name: str, property_name: str) -> bool:
+    @strict_types
+    def delete_property(self, entity: Union[str, owlready2.Thing], property: Union[str, owlready2.PropertyClass]) -> bool:
         """Deletes a property from an individual
 
-        :param individual_name: Name of the individual
-        :type individual_name: str
-        :param property_name: Property to be deleted
-        :type property_name: str
+        :param entity: The individual object to be changed or its name.
+        :type entity: Union[str, owlready2.Thing]
+        :param property_name: Property to be deleted, passed as name string or the owlready PropertyClass object.
+        :type property_name: Union[str, owlready2.PropertyClass]
         :return: True if deletion successful, else False
         :rtype: bool
         """
+        individual_name, _ = owlutils.get_name_and_object(entity, self.store)
+        property_name, _ = owlutils.get_name_and_object(property, self.store)
         prop_dict = {property_name: None}
         return self.properties(individual_name, prop_dict)
 
 
-    def description(self, individual_name: str, new_comment: list) -> bool:
+    @strict_types
+    def description(self, entity: Union[str, owlready2.Thing], new_comment: list) -> bool:
         """Sets/changes the description (comment) of an individual
 
-        :param individual_name: Name of the individual
-        :type individual_name: str
+        :param entity: The individual object to be changed or its name.
+        :type entity: Union[str, owlready2.Thing]
         :param new_comment: New description as a list of strings
         :type new_comment: list
         :return: True if update successful, else False
         :rtype: bool
         """
+        individual_name, _ = owlutils.get_name_and_object(entity, self.store)
         return self.property(individual_name, 'comment', new_comment)
```

### Comparing `causalgraph-0.0.6/causalgraph/store/export.py` & `causalgraph-0.1.0/causalgraph/utils/draw.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,204 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 
-""" Contains Export Class, to export a cg graph to other
-formats like nx, tigramite, graphml, gml."""
+""" Contains Draw class to visualize graphs.
+"""
 
 # general imports
-from typing import Tuple
-from logging import Logger
-import numpy as np
-from networkx import MultiDiGraph, write_graphml, write_gml
-# causalgraph and owlready imports
-import owlready2
-from causalgraph.utils.logging_utils import init_logger
+import networkx as nx
+import matplotlib.pyplot as plt
 
 
-class Export():
-    """ Contains all methods to export cg graphs to other formats like NetworkX, Tigramite,
-    graphml and gml.
+class Draw():
+    """ This Class contains all methods for drawing graphs. There are multiple methods
+    to draw a graph e.g. with nx or neo4j.
     """
-    def __init__(self, graph, logger: Logger = None) -> None:
+
+    def __init__(self, graph) -> None:
+        """Instantiates the Draw() class.
+
+        :param graph: A causalgraph.Graph object
+        :type graph: causalgraph.Graph
+        """
         self.graph = graph
-        if logger is not None:
-            self.logger = logger
-        else:
-            self.logger = init_logger("Export")
-    
-
-    def nx(self) -> MultiDiGraph:
-        """Converts a cg graph into a NetworkX MultiDiGraph and returns it.
-        This method adds the cg properties to the NetworkX individuals as NetworkX attributes.
-        CAUTION: Will not add Creators because NetworkX cannot handle them. But Creators will still
-        be part of properties of Nodes and Edges. Lonely Creators will be lost, because there are 
-        no records of them without the properties of any CausalEdge or CausalNode. Individual types
-        within the properties will be broken down to CausalNode or CausalEdge.
 
-        :return: The converted NetworkX MultiDiGraph.
-        :rtype: nx.MultiDiGraph
+    def nx(self, directory: str=None, filename: str=None) -> None:
+        """Plots the graph with NetworkX methods. Parse a directory to save
+        the plot as an image with a specific filename. By default, a plot of the whole graph will be generated, unless
+        you parse another graph_dict explicitly.
+
+        :param directory: Directory where the plot should be saved, defaults to None
+        :type directory: str, optional
+        :param filename: Filename of the .png to be created, defaults to None
+        :type filename: str, optional
+        :param graph_dict: A properties dict that describes a graph with its nodes, edges and creators, defaults to None
+        :type graph_dict: dict, optional
         """
-        G_nx = MultiDiGraph()
         graph_dict = self.graph.map.all_individuals_to_dict()
+        G_nx = self.graph.export.nx()
+        edge_labels = {}
+        # Get edge labels and fill dict edge_labels with them
         for individual in graph_dict:
             individual_type = graph_dict[individual]["type"]
-            individual_name = individual
-            properties_dict = graph_dict[individual]
-            if individual_type == "CausalNode":
-                G_nx.add_node(individual_name, **properties_dict)
-            elif individual_type == "CausalEdge":
-                cause = graph_dict[individual]["hasCause"][0]
-                effect = graph_dict[individual]["hasEffect"][0]
-                G_nx.add_edge(cause, effect, **properties_dict)
-            else:
-                self.logger.error(f"Individual type '{individual_type}' unknown.")
-                return False
-        return G_nx
-
-
-    def graphml(self, directory: str, filename: str) -> None:
-        """Saves a cg graph to a given path as a .graphml-file.
-
-        :param directory: Path to the directory under which the .graphml-file will be saved.
-        :type directory: str
-        :param filename: Filename of the file to be saved
-        :type filename: str
-        """
-        # Convert cg Graph to NX Graph
-        g_nx = self.nx()
-        nodes = g_nx.nodes.data()
-        edges = g_nx.edges.data()
-        # Covert list properties to raw strings, because graphml cannot handle lists
-        for node in nodes:
-            for i in node[1]:
-                if type(node[1][i]) in [list, owlready2.IndividualValueList]:
-                    node[1][i] = str(node[1][i])
-        # Covert list properties to raw strings, because graphml cannot handle lists
-        for edge in edges:
-            for i in edge[2]:
-                if type(edge[2][i]) in [list, owlready2.IndividualValueList]:
-                    edge[2][i] = str(edge[2][i])
-        # Write gml file to path
-        write_graphml(g_nx, f'{directory}/{filename}.graphml')
-
-
-    def gml(self, directory: str, filename: str) -> None:
-        """Saves a cg graph to a given path as a .gml-file.
+            if individual_type == "CausalEdge":
+                cause = graph_dict[individual].get("hasCause", None)
+                effect = graph_dict[individual].get("hasEffect", None)
+                timelag = graph_dict[individual].get("hasTimeLag", None)
+                confidence = graph_dict[individual].get("hasConfidence", None)
+                # Append to edge_labels dict
+                if confidence is None and timelag is not None:
+                    edge_labels[(cause, effect)] = f"Timelag: {timelag}"
+                if confidence is not None and timelag is None:
+                    edge_labels[(cause, effect)] = f"Confidence: {confidence}"
+                if confidence is not None and timelag is not None:
+                    edge_labels[(cause, effect)] = f"Timelag: {timelag}\nConfidence: {confidence}"
+        # Create plot
+        pos = nx.spring_layout(G_nx, k=2, seed=5)
+        plt.figure()
+        nx.draw(G= G_nx, pos= pos, with_labels= True, node_size= 2000, node_color= '#6fd0a7',font_size= 9)
+        nx.draw_networkx_edge_labels(G=G_nx, pos=pos, edge_labels=edge_labels, font_color='#121212', font_size=7)
+        plt.axis('off')
+        axis = plt.gca()
+        axis.set_xlim([1.1*x for x in axis.get_xlim()])
+        axis.set_ylim([1.1*y for y in axis.get_ylim()])
+        # Show figure or save plot as file
+        if directory is not None and filename is not None:
+            plt.savefig(f'{directory}/{filename}.png', dpi=200)
+            print(f"Plot '{filename}.png' saved at {directory}.")
+            plt.close()
+            return
+        plt.show()
+
+
+    def html(self, directory: str, filename: str, directed: bool=True, graph_dict: dict=None) -> None:
+        """Generates a .html-file which shows all nodes and edges incl. their properties
+        as an interactive graph. This file can be openend by every browser with JS. By
+        default, a plot of the whole graph will be generated, unless you parse another
+        graph_dict explicitly.
 
-        :param directory: Path to the directory under which the .gml-file will be saved.
+        :param directory: Directory where the .html-file will be saved.
         :type directory: str
-        :param filename: Filename of the file to be saved
+        :param filename: Filename of the .html-file to be created.
         :type filename: str
+        :param graph_dict: Properties dict that describes a graph with its nodes, edges
+        and creators, defaults to None
+        :type graph_dict: dict, optional
         """
-        # Convert cg Graph to NX Graph
-        g_nx = self.nx()
-        nodes = g_nx.nodes.data()
-        edges = g_nx.edges.data()
-        # Covert list properties to raw strings, because gml cannot handle lists
-        for node in nodes:
-            for i in node[1]:
-                if type(node[1][i]) in [list, owlready2.IndividualValueList]:
-                    node[1][i] = str(node[1][i])
-        # Covert list properties to raw strings, because gml cannot handle lists
-        for edge in edges:
-            for i in edge[2]:
-                if type(edge[2][i]) in [list, owlready2.IndividualValueList]:
-                    edge[2][i] = str(edge[2][i])
-        # Write gml file to path
-        write_gml(g_nx, f'{directory}/{filename}.gml')
-
-
-    def tigra(self) -> Tuple[list, dict, np.ndarray, np.ndarray, int]:
-        """Creates a Tigramite graph from a cg graph. Right now, this method only can handle
-        edges, nodes, timelags and confidence. Nodes with multiple class types besides CausalNode
-        will be broken down to type CausalNode only.
-
-        :param graph_dict: Properties dict of a cg graph.
-        :type graph_dict: dict
-        :return: Tuple with the links as a boolean matrix, the variable names as a list of
-        strings, the edges as dict with its cause and effect and integer containing the
-        tigra timestep length. [node_names, edge_names, link_matrix, q_matrix, timestep_len_s].
-        :rtype: Tuple[np.ndarray, list, dict, int]
-        """
-        graph_dict = self.graph.map.all_individuals_to_dict()
-        if len(graph_dict) <= 1:
-            raise ValueError("You can't draw an empty graph or a graph with only one node using Tigramite!")
 
-        list_of_edges = []
-        list_cg_timelags = []
-        list_tigra_timelags = []
-        list_edge_confidence = []
-        node_names = []
-        edge_names = {}
-        # Get list of cg timelags:
-        for individual in graph_dict:
-            individual_type = graph_dict[individual]["type"]
-            if individual_type == "CausalEdge":
-                # Get timelag or None
-                time_lag_s = graph_dict[individual].get("time_lag_s", None)
-                if time_lag_s is not None:
-                    list_cg_timelags.append(time_lag_s)
-        # Get timestep length (smallest timelag in list_cg_timelags)
-        try:
-            timestep_len_s = min(list_cg_timelags)
-        except ValueError:
-            timestep_len_s = 1
+        # If graph_dict hasn't been parsed, just create it for the whole graph.
+        if graph_dict is None:
+            #graph_dict = all_individuals_to_dict(self.graph.store)
+            graph_dict = self.graph.map.all_individuals_to_dict()
 
+        nodes_html = []
+        edges_html = []
         for individual in graph_dict:
-            individual_type = graph_dict[individual]["type"]
             individual_name = individual
-            # Fill list of node names
-            if individual_type == "CausalNode":
-                node_names.append(individual_name)
-            # Fill list of edges, incl. their tigramite timelag
+            individual_type = graph_dict[individual]["type"]
+            if "CausalNode" in individual_type:
+                # Generate node dict for visjs
+                node = {'id': individual_name, 'label': individual_name, 'type': 'node', 'color': '#6fd0a7'}
+                try:
+                    message = graph_dict[individual]['message']
+                    errorCode = graph_dict[individual]['errorCode']
+                    node['title']=f"{message}|{errorCode}"
+                except KeyError:
+                    pass
+                # Append to html nodes list
+                nodes_html.append(node)
             if individual_type == "CausalEdge":
-                cause = graph_dict[individual].get("hasCause", [None])[0]
-                effect = graph_dict[individual].get("hasEffect", [None])[0]
-                # If timelag exists for current edge, convert it to tigramite timeframe.
-                # If it doesnt exist, set it to 0. After that add it to list_tigra_timelags
-                time_lag_s = round(graph_dict[individual].get("hasTimeLag", 0)/timestep_len_s)
-                list_tigra_timelags.append(time_lag_s)
-                # Get confidence for current edge. set it to 0 (edge present) if it does not exist
-                confidence = graph_dict[individual].get('hasConfidence', 0)
-                list_edge_confidence.append(confidence)
-                # Add edge with its timelag to list_of_edges
-                list_of_edges.append((cause, effect, time_lag_s))
-                edge_names[individual_name] = {}
-                edge_names[individual_name] = {"hasCause": cause, "hasEffect": effect}
-
-        num_of_nodes = len(node_names)
-        # graph consists of nodes only
-        if len(edge_names) == 0:
-            link_matrix = np.zeros((num_of_nodes, num_of_nodes, 5))
-            q_matrix = np.ones((num_of_nodes, num_of_nodes, 5))
-            return (node_names, [], link_matrix, q_matrix, timestep_len_s)
-        # if there are edges, create list of edge indices with their timelags
-        edge_indices = [(node_names.index(cause), node_names.index(effect), timelag)
-                            for (cause, effect, timelag) in list_of_edges]
-        # Init link_matrix with the proper dimension and fill it with zeros for now.
-        link_matrix = np.zeros((num_of_nodes, num_of_nodes, max(list_tigra_timelags)+1))
-        # Set 1 at the right indices to give information about the timelag value
-        cause_ind, effect_ind, time_ind = zip(*edge_indices)
-        link_matrix[cause_ind, effect_ind, time_ind] = 1
-        # Init q_matrix with the proper dimension and fill it with ones (edges not present) for now
-        q_matrix = np.ones((num_of_nodes, num_of_nodes, max(list_tigra_timelags)+1))
-        q_matrix[cause_ind, effect_ind, time_ind] = list_edge_confidence
-        return (node_names, edge_names, link_matrix, q_matrix, timestep_len_s)
-
+                edge = None
+                cause = graph_dict[individual].get("hasCause", None)
+                effect = graph_dict[individual].get("hasEffect", None)
+                timelag = graph_dict[individual].get("hasTimeLag", None)
+                confidence = graph_dict[individual].get("hasConfidence", None)
+                if ((cause and effect) is not None) and ((confidence and timelag) is None):
+                    edge  = {'from': cause,'to': effect}
+                if ((cause and effect and confidence) is not None) and (timelag is None):
+                    edge  = {'from': cause,'to': effect,'label':f"Confidence: {confidence}"}
+                if ((cause and effect and timelag) is not None) and (confidence is None):
+                    edge  = {'from': cause,'to': effect,'label':f"Timelag: {timelag}"}
+                if (cause and effect and timelag and confidence) is not None:
+                    edge  = {'from': cause,'to': effect,'label':f"Timelag: {timelag}\nConfidence: {confidence}"}
+                edges_html.append(edge)
+            #if individual_type == "Creator":
+            #    creator = {'id': individual_name, 'label': individual_name, 'type': 'creator', 'color': '#f9cbb6'}
+            #    created_by_node = []
+            #    for node in graph_dict[individual].get("created", [None]):
+            #        if node is not None:
+            #            edge = {'from': individual_name,'to': node,'label':f"created"}
+            #            edges_html.append(edge)
+            #    nodes_html.append(creator)
+
+        html  = f"""
+            <html lang="en">
+            <head>
+                <title>Network</title>
+                <script
+                type="text/javascript"
+                src="https://unpkg.com/vis-network/standalone/umd/vis-network.min.js"
+                ></script>
+                <style type="text/css">
+                #mynetwork {{
+                    width: 100%;
+                    height: 100vh;
+                }}
+                </style>
+            </head>
+            <body>
+                <div id="mynetwork"></div>
+                <script type="text/javascript">
+                // create an array with nodes
+                var nodes_data = new vis.DataSet(
+                    {nodes_html}
+                );
+                // create an array with edges
+                var edges_data = new vis.DataSet(
+                    {edges_html}
+                );
+                // create a network
+                var container = document.getElementById("mynetwork");
+                var data = {{
+                    nodes: nodes_data,
+                    edges: edges_data,
+                }};
+                var options = {{
+                    nodes: {{
+                        font: {{ color: 'black',size: 14 }},
+                        size: 25,
+                        shape: 'circle',
+                        widthConstraint: 60
+                        }},
+                    edges: {{
+                        arrows: {{
+                            to: {{enabled: true, scaleFactor: 0.5}}
+                        }},
+                        color: {{
+                            color:'grey',
+                            highlight:'red',
+                            hover: '#d3d2cd',
+                            inherit: false,
+                            opacity:1.0
+                        }},
+                        font: {{size: 14, align: 'middle'}},
+                        "length": 250,
+                        "width": 1,
+                        }},
+                    layout: {{
+                        hierarchical: {{
+                            enabled: {str.lower(str(directed))},
+                            direction: 'UD',
+                            sortMethod: 'directed'
+                            }},
+                    }},
+                }};
+                var network = new vis.Network(container, data, options);
+                </script>
+            </body>
+            </html>
+        """
+        file = open(f"{directory}/{filename}.html", "w")
+        print(f"HTML-file '{filename}.html' saved at {directory}.")
+        file.write(html)
+        file.close()
```

### Comparing `causalgraph-0.0.6/causalgraph/store/load.py` & `causalgraph-0.1.0/causalgraph/store/load.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 # general imports
 from typing import Tuple
 from logging import Logger
 import numpy as np
 import networkx as nx
 # causalgraph and owlready imports
 import causalgraph.graph as cg
-import owlready2
 from causalgraph.utils.logging_utils import init_logger
 
 
 class Load():
     """ Contains all methods to to import formats like NetworkX MultiDiGraph,
     tigramite, graphml or gml into causalgraph Graph format.
     """
     def __init__(self, graph, logger: Logger = None) -> None:
         self.graph = graph
+        self.validate_domain_range = graph.validate_domain_range
         if logger is not None:
             self.logger = logger
         else:
             self.logger = init_logger("Load")
 
 
     def nx(self, nx_graph: nx.MultiDiGraph, sql_db_filename: str, external_ontos: list=[]):
```

### Comparing `causalgraph-0.0.6/causalgraph/store/remove.py` & `causalgraph-0.1.0/causalgraph/store/remove.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 """ Contains Remove Class to remove things from the store.
 Store is equivalent to owlready2 World """
 
 # general imports
 from logging import Logger
 import owlready2
+from typing import Union
 # causalgraph imports
+import causalgraph.utils.owlready2_utils as owlutils
+from causalgraph.utils.misc_utils import strict_types
 from causalgraph.utils.logging_utils import init_logger
-from causalgraph.utils.owlready2_utils import entity_exists, get_entity_by_name, is_instance_of_class
 
 
 class Remove():
     """ Contains all methods to remove resources from the store"""
     def __init__(self, store: owlready2.World, logger: Logger = None) -> None:
         self.store = store
         self.classes_onto_prefix = store.classes_onto.name
@@ -22,160 +24,206 @@
         if logger is not None:
             self.logger = logger
         else:
             self.logger = init_logger("Remove")
         self.logger.info("Initialized the 'remove' functionalities.")
 
 
-    def causal_node(self, individual_name: str) -> bool:
-        """Deletes an individual of the class "CausalNode" with the name "individual_name".
+    @strict_types
+    def causal_node(self, entity: Union[str, owlready2.Thing]) -> bool:
+        """Deletes an individual of the class "CausalNode" or its subtypes with the name "individual_name".
         If the node is connected with edges, these are deleted as well.
 
-        :param individual_name: name for individual
-        :type individual_name: str
+        :param entity: The individual object to be deleted or its name.
+        :type entity: Union[str, owlready2.Thing]
         :return: 'True' if delete successful
         :rtype: bool
         """
-        # return false if individual does not exist
-        if entity_exists(individual_name, self.store) is False:
+        # Check if individual exists and get its name and object
+        individual_name, individual_obj = owlutils.get_name_and_object(entity, self.store)
+        if individual_obj is None:
             self.logger.error(f"Individual '{individual_name}' does not exist.")
             return False
         # return false if individual is no CausalNode
-        entity_of_right_class = is_instance_of_class(individual_name, 'CausalNode', self.store, logger= self.logger)
+        entity_of_right_class = owlutils.is_instance_of_type(individual_name, 'CausalNode', self.store, include_subtypes=True, logger= self.logger)
         if entity_of_right_class is False:
-            self.logger.error(f"Individual '{individual_name}' is not of the class 'CausalNode'")
+            self.logger.error(f"Individual '{individual_name}' is not of the class 'CausalNode' or a subclass.")
             return False
         # Delete entity if both prerequisites are met
         causal_edges_list = self._list_of_all_causal_edges_from_one_node(individual_name)
         if len(causal_edges_list) > 0 :
             self.causal_edges_from_node(individual_name)
-        deletion_succ = self.delete_individual_of_type(str(individual_name), 'CausalNode')
+        deletion_succ = self.delete_individual_of_type(individual_name, 'CausalNode', include_subtypes=True)
         return deletion_succ
 
 
-    def causal_edge_by_name(self, causal_edge_name: str) -> bool:
-        """Deletes an individual of class "CausalEdge" with the name "causal_edge_name".
+    @strict_types
+    def causal_edge(self, causal_edge: Union[str, owlready2.Thing]) -> bool:
+        """Deletes an individual of class "CausalEdge" with the name "causal_edge" or
+        the specific CausalEdge object.
 
-        :param causal_edge_name: name for individual
-        :type causal_edge_name: str
+        :param causal_edge: The individual edge object to be deleted or its name.
+        :type causal_edge: Union[str, owlready2.Thing]
         :return: 'True' if delete successful
         :rtype: bool
         """
-        deletion_successful = self.delete_individual_of_type(str(causal_edge_name), 'CausalEdge')
+        deletion_successful = self.delete_individual_of_type(causal_edge, 'CausalEdge')
         return deletion_successful
 
 
-    def causal_edges(self, causal_node1: str, causal_node2:str) -> bool:
+    @strict_types
+    def causal_edges(self, causal_node1: Union[str, owlready2.Thing], causal_node2: Union[str, owlready2.Thing]) -> bool:
         """Deletes all CausalEdges between 'hasCause' and 'hasEffect'
 
-        :param causalNode1: name for individual 'hasCause' or 'hasEffect'
-        :type causalNode1: str
-        :param causalNode2: name for individual 'hasCause' or 'hasEffect'
-        :type causalNode2: str
+        :param causalNode1: First Node individual object of 'hasCause' or 'hasEffect'. Can also be just the name of it.
+        :type causalNode1: Union[str, owlready2.Thing]
+        :param causalNode2: Second Node individual object of 'hasCause' or 'hasEffect'. Can also be just the name of it.
+        :type causalNode2: Union[str, owlready2.Thing]
         :return: 'True' if deletion successful
         :rtype: bool
         """
-        possibly_existing_entity_cause = get_entity_by_name(causal_node1, self.store, self.logger)
-        possibly_existing_entity_effect = get_entity_by_name(causal_node2, self.store, self.logger)
-        cause_of_specified_class = is_instance_of_class(causal_node1, 'CausalNode', self.store, logger=self.logger)
-        effect_of_specified_class = is_instance_of_class(causal_node2, 'CausalNode', self.store, logger=self.logger)
-        # return false if one of the entities does not exist
-        if possibly_existing_entity_cause is None or possibly_existing_entity_effect is None:
+        causal_node1_name, causal_node1_obj = owlutils.get_name_and_object(causal_node1, self.store)
+        causal_node2_name, causal_node2_obj = owlutils.get_name_and_object(causal_node2, self.store)
+        # Return false if at least one of the nodes does not exist
+        if causal_node1_obj is None or causal_node2_obj is None:
             self.logger.error("Could not delete CausalEdges between " +
-                             f"{causal_node1}:{possibly_existing_entity_cause} and " +
-                             f"{causal_node2}:{possibly_existing_entity_effect}. " +
+                              f"[{causal_node1_name}|{causal_node1_obj}] and " +
+                              f"[{causal_node2_name}|{causal_node2_obj}]. " +
                               "One or more individuals does not exist.")
             return False
-        # return false if one of the entities is no CausalNode
+        # Return false if at least one node is not really a CausalNode
+        cause_of_specified_class = owlutils.is_instance_of_type(causal_node1_name, 'CausalNode', self.store, logger=self.logger, include_subtypes=True)
+        effect_of_specified_class = owlutils.is_instance_of_type(causal_node2_name, 'CausalNode', self.store, logger=self.logger, include_subtypes=True)
         if cause_of_specified_class is False or effect_of_specified_class is False:
-            self.logger.error(f"Could not delete CausalEdges between '{causal_node1}' and" +
-                              f"{causal_node2}. Individuals are not of the specified class" +
+            self.logger.error(f"Could not delete CausalEdges between '[{causal_node1_name}|{causal_node1_obj}]' and " +
+                              f"[{causal_node2_name}|{causal_node2_obj}]. Individuals are not of the specified class" +
                                "'CausalNode', they are specified as of the classes " +
-                              f"{possibly_existing_entity_cause.is_a} and " +
-                              f"{possibly_existing_entity_effect.is_a}.")
+                              f"{causal_node1_obj.is_a} and " +
+                              f"{causal_node2_obj.is_a}.")
             return False
         # Delete entity if both prerequisites are met, dedicated logging for each
-        edge_list = self._causal_edges_btw_nodes(causal_node1, causal_node2)
+        edge_list = self._causal_edges_btw_nodes(causal_node1_name, causal_node2_name)
         if not edge_list:
-            self.logger.error(f"No edges were deleted between {causal_node1} and {causal_node2}.")
+            self.logger.error(f"No edges were deleted between '{causal_node1_name}' and '{causal_node2_name}'.")
             return True
         for edge in edge_list:
             edge = (str(edge).replace(f'[{self.individuals_onto_prefix}.','').replace(']',''))
             self.delete_individual_of_type(edge, 'CausalEdge')
         return True
 
 
-    def causal_edges_from_node(self, causal_node: str) -> bool:
+    @strict_types
+    def causal_edges_from_node(self, causal_node: Union[str, owlready2.Thing]) -> bool:
         """Deletes all CausalEdges which are connected with 'causal_node'
 
-        :param causalNode: class name/type of individual
+        :param causalNode: Object or name of the affected CausalNode
         :type causalNode: str
         :return: 'True' if delete successful
         :rtype: bool
         """
-        # return false if individual does not exist
-        if entity_exists(causal_node, self.store) is False:
-            self.logger.error(f"Individual '{causal_node}' does not exist.")
+        causal_node_name, causal_node_obj = owlutils.get_name_and_object(causal_node, self.store)
+        # Return false if individual does not exist
+        if causal_node_obj is None:
+            self.logger.error(f"Individual '[{causal_node_name}|{causal_node_obj}]' does not exist.")
             return False
-        # return false if individual is no CausalNode
-        entity_of_right_class = is_instance_of_class(causal_node, 'CausalNode', self.store, logger= self.logger)
+        # Return false if individual is no CausalNode
+        entity_of_right_class = owlutils.is_instance_of_type(causal_node_name, 'CausalNode', self.store, logger=self.logger, include_subtypes=True)
         if entity_of_right_class is False:
-            self.logger.error(f"Individual '{causal_node}' is not of the class 'CausalNode'")
+            self.logger.error(f"Individual '{causal_node_name}' is not of the class 'CausalNode'")
             return False
         # Delete edges if both prerequisites are met
-        edge_list = self._list_of_all_causal_edges_from_one_node(causal_node)
+        edge_list = self._list_of_all_causal_edges_from_one_node(causal_node_name)
         if not edge_list:
-            self.logger.warning(f"No edges were deleted at '{causal_node}'.")
+            self.logger.warning(f"No edges were deleted at '{causal_node_name}'.")
             return True
         for edge in edge_list:
-            edge = (str(edge).replace(f'[{self.individuals_onto_prefix}.','').replace(']',''))
-            self.delete_individual_of_type(edge, 'CausalEdge')
+            self.delete_individual_of_type(edge[0], 'CausalEdge')
         return True
 
 
-    def delete_individual_of_type(self, individual_name: str, class_of_individual: str) -> bool:
+    @strict_types
+    def delete_individual_of_type(self, individual: Union[str, owlready2.Thing], type_of_individual: Union[str, owlready2.EntityClass], include_subtypes = False) -> bool:
         """Deletes an individual of the specified class/type.
 
-        :param class_of_individual: class name/type of individual
-        :type class_of_individual: str
-        :param name_for_individual: name for individual
-        :type name_for_individual: str
+        :param individual: The object to be deleted or its name.
+        :type individual: Union[str, owlready2.Thing],
+        :param type_of_individual: Class name or owlready EntityClass object of individual class.
+        :type type_of_individual: Union[str, owlready2.EntityClass]
+        :param include_subtypes: Switch to also include subtypes of typename in check, defaults to False
+        :type include_subtypes: bool
         :return: 'True' if delete successful
         :rtype: bool
         """
-        # return false if individual does not exist
-        if entity_exists(individual_name, self.store) is False:
+        individual_name, individual_obj = owlutils.get_name_and_object(individual, self.store)
+        # Check if individual (still) exists
+        if individual_obj is None:
             self.logger.error(f"Did not delete {individual_name} because it does not exist")
             return False
         # return false if individual is not of the right class
-        entity_of_right_class = is_instance_of_class(individual_name, class_of_individual, self.store, logger= self.logger)
+        type_name, type_obj = owlutils.get_name_and_object(type_of_individual, self.store)
+        entity_of_right_class = owlutils.is_instance_of_type(individual_name, type_obj, self.store, include_subtypes=include_subtypes, logger=self.logger)
         if entity_of_right_class is False:
-            self.logger.error("Could not delete individual. Individual not of specified class." +
-                             f"{individual_name} is of class '{class_of_individual}")
+            subclasses = owlutils.get_subclasses(type_obj, self.store, self.logger)
+            if include_subtypes == True:
+                error_msg = f"""Could not delete individual. Individual not of specified class or any of its subtypes.
+                          '{individual_name}' is of class(es) '{individual_obj.is_a}'. Passed Class '{type_name}' or any of it's subclasses '{subclasses}'."""
+            else:
+                error_msg = f"""Could not delete individual. Individual not of specified class.
+                          '{individual_name}' is of class(es) '{individual_obj.is_a}'. Passed Class '{type_name}'. Use option 'include_subtypes=True' if you also want to allow removal for subclasses of '{type_name}' """
+            self.logger.error(error_msg)
             return False
-        # Delete entity if both prerequisites are met
-        entity = get_entity_by_name(individual_name, self.store, self.logger)
-        owlready2.destroy_entity(entity)
-        self.logger.info(f"Deleted individual {individual_name} of class {class_of_individual}")
+        # Delete entity if both prerequisites are met based on type
+        owlready2.destroy_entity(individual_obj)
+        self.logger.info(f"Deleted entity '{individual_name}' of class '{individual_obj.is_a}'")
         self.store.save()
         return True
 
 
-    def _causal_edges_btw_nodes(self, causal_node1: str, causal_node2: str) -> list:
+    @strict_types
+    def entity(self, entity: Union[str, owlready2.Thing]) -> bool:
+        """Removes entity from store. Entity can be provided as object or as string identifer.
+
+        :param entity: Entity to remove
+        :type entity: owlready2.Thing | str
+        :return: deletion successful
+        :rtype: bool
+        """
+        # Check Inputs and if entity exists in store
+        if type(entity)==str:
+            entity_str = entity
+            entity = owlutils.get_entity_by_name(entity, self.store, self.logger, suppress_warn=True)
+        elif type(entity) in list(self.store.classes()):
+            entity_str = entity.get_name()
+        else:
+            self.logger.error(f"Did not delete '{entity}' because it was not found in store.")
+            return False
+        # Check Type of entity in case special treatment necessary
+        if owlutils.is_instance_of_type(entity_str, 'CausalNode', self.store, include_subtypes=True, logger=self.logger):
+            return self.causal_node(entity_str)
+        elif owlutils.is_instance_of_type(entity_str, 'CausalEdge', self.store, include_subtypes=True, logger=self.logger):
+            return self.causal_edge(entity_str)
+        else:
+            owlready2.destroy_entity(entity)
+            self.logger.info(f"Deleted entity '{entity_str}' of class '{entity.is_a}'")
+            self.store.save()
+            return True
+
+
+    def _causal_edges_btw_nodes(self, causal_node1: Union[str, owlready2.Thing], causal_node2: Union[str, owlready2.Thing]) -> list:
         """ Returns a list of all CausalEdges between 'causal_node1' and 'causal_node2'
 
-        :param causal_node1: name for individual 'hasCause' or 'hasEffect'
-        :type causal_node1: str
-        :param causal_node2: name for individual 'hasCause' or 'hasEffect'
-        :type causal_node2: str
+        :param causal_node1: First Node individual object of 'hasCause' or 'hasEffect'. Can also be just the name of it.
+        :type causal_node1: Union[str, owlready2.Thing]
+        :param causal_node2: Second Node individual object of 'hasCause' or 'hasEffect'. Can also be just the name of it.
+        :type causal_node2: Union[str, owlready2.Thing]
         :return: a list of all edges between 'hasCause' and 'hasEffect'
         :rtype: list of all causal_edges
         """
-        causal_node1_iri = get_entity_by_name(causal_node1, self.store, self.logger).iri
-        causal_node2_iri = get_entity_by_name(causal_node2, self.store, self.logger).iri
+        causal_node1_iri = owlutils.get_entity_by_name(causal_node1, self.store, self.logger).iri
+        causal_node2_iri = owlutils.get_entity_by_name(causal_node2, self.store, self.logger).iri
         list_causal_edges = list(self.store.sparql("""
             SELECT ?CausalEdge
             WHERE {
             """ + f"""
             <{causal_node1_iri}> ^{self.classes_onto_prefix}:hasCause ?CausalEdge .
             <{causal_node2_iri}> ^{self.classes_onto_prefix}:hasEffect ?CausalEdge 
             """ + "}"
@@ -197,15 +245,15 @@
 
         :param causal_node: class name/type of individual
         :type causal_node: str
         :return: a list of all edges on 'causalNode'
         :rtype: list
         """
         # get nodes that are connected to the specified node via incoming or outgoing edges
-        causal_node_iri = get_entity_by_name(causal_node, self.store, self.logger).iri
+        causal_node_iri = owlutils.get_entity_by_name(causal_node, self.store, self.logger).iri
         list_nodes_has_cause = list(self.store.sparql ("""
             SELECT ?CausalEdge
             WHERE {
             """ + f"""
             <{causal_node_iri}> ^{self.classes_onto_prefix}:hasCause ?CausalEdge . 
             """ + "}"
             ))
```

### Comparing `causalgraph-0.0.6/causalgraph/utils/logging_utils.py` & `causalgraph-0.1.0/causalgraph/utils/logging_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 # general imports
 import os
 import logging
 import ecs_logging
 # causalgraph imports
-from causalgraph.utils.path_utils import get_project_root
+from causalgraph.utils.misc_utils import get_project_root
 
 
 def init_logger(logger_name: str,
                 file_handler_level= logging.DEBUG,
                 console_handler_level= logging.WARNING,
                 file_handler= False,
                 elastic_style_json= True,
```

### Comparing `causalgraph-0.0.6/causalgraph/utils/mapping.py` & `causalgraph-0.1.0/causalgraph/utils/mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 # SPDX-License-Identifier: MIT
 
 """ Contains functionalities to map a cg graph to and from a dictionary.
 """
 # general imports
 import owlready2
 from logging import Logger
-# causalgraph imports
-from causalgraph.utils.logging_utils import init_logger
-from causalgraph.utils.owlready2_utils import get_entity_by_name
-from causalgraph.utils.owlready2_utils import create_individual_of_type
-from causalgraph.utils.owlready2_utils import validate_prop_for_type
-from causalgraph.utils.owlready2_utils import validate_data_type_for_property
 import networkx as nx
 import numpy as np
+
+from typing import Union
+# causalgraph imports
+from causalgraph.utils.logging_utils import init_logger
 import causalgraph.utils.owlready2_utils as owlutils
 
 
 class Mapping():
     def __init__(self, graph, logger: Logger = None) -> None:
         self.graph = graph
+        self.validate_domain_range = graph.validate_domain_range
         if logger is not None:
             self.logger = logger
         else:
             self.logger = init_logger("Mapping")
         self.logger.info("Initialized the 'mapping' functionalities.")
         self.causalgraph_object_properties = [prop.name for prop in list(self.graph.classes_onto.object_properties())] + ["comment"]
         self.causalgraph_data_properties = [prop.name for prop in list(self.graph.classes_onto.data_properties())]
@@ -57,39 +56,39 @@
         # Get all CausalNodes and their subclasses
         causalnodes_list = owlutils.get_all_causalnodes(self.graph.store)
         # Get all CausalEdges
         causaledges_list = owlutils.get_all_causaledges(self.graph.store)
         # Handling all CausalNodes
         for causalnode in causalnodes_list:
             # Append the dict for single individuals to the dict of the whole graph
-            causalnode_prop_dict = self.__add_properties_to_dict(individual=causalnode[0], indi_type='CausalNode')
+            causalnode_prop_dict = self.__create_prop_dict_from_individual(individual=causalnode[0])
             if len(causalnode_prop_dict) > 0:
                 dict_graph[causalnode[0].name] = causalnode_prop_dict
         # Handling all CausalEdge
         for causaledge in causaledges_list:
             # Append the dict for single individuals to the dict of the whole graph
-            causaledge_prop_dict = self.__add_properties_to_dict(individual=causaledge[0], indi_type='CausalEdge')
+            causaledge_prop_dict = self.__create_prop_dict_from_individual(individual=causaledge[0])
             if len(causaledge_prop_dict) > 0:
                 dict_graph[causaledge[0].name] = causaledge_prop_dict
         return dict_graph
 
 
-    def __add_properties_to_dict(self, individual: object, indi_type: str) -> dict:
-        """Creates a properties dict of a single individual and returns it. Type of individual must be
-        passed due to possible multi class inheritance.
+    def __create_prop_dict_from_individual(self, individual: owlready2.Thing) -> dict:
+        """Creates a properties dict of a single individual and returns it. 
+        Multiple types of an individual are supported and will be added to the dict (e.G. [CausalNode, Error])
 
         :param individual: Individual object
-        :type individual: object
+        :type individual: owlready2.Thing
         :param type: Object type (e. g. CausalNode, CausalEdge)
         :type type: str
         :raises ValueError: Unvalid property Error
         :return: Properties dict of single individual
         :rtype: dict
         """
-        prop_dict = {'type': indi_type, 'iri': individual.iri}
+        prop_dict = {'type': [type_.name for type_ in individual.is_a], 'iri': individual.iri}
         # Iteratively fill the property dictionary
         possible_props = self.causalgraph_object_properties + self.causalgraph_data_properties + self.third_party_data_properties + self.third_party_object_properties
         for prop in individual.get_properties():
             # Validate that the property is in valid
             if prop.name not in possible_props:
                 raise ValueError(f'{prop.name} is not a valid property since it is not contained in the mapping_dict!')
             # Get value of the property
@@ -161,15 +160,15 @@
 
         # Compare number of nodes in link_matrix with the number of node_names
         if len(link_matrix) != len(node_names):
             self.logger.error("Too few nodes in the link matrix or the list of node names.")
             return False
         # Add nodes without their properties to graph_dict
         for nodes in node_names:
-            graph_dict[nodes] = {"type": "CausalNode"}
+            graph_dict[nodes] = {"type": ['CausalNode']}
         # Handle all edges, also add missing node properties
         for node_ind, matrix in enumerate(link_matrix):
             # Get indices of cause/effect pair and timelag
             possibly_edge = np.argwhere(matrix)
             # Only handle matrices with edges and timelags
             for edge in possibly_edge:
                 cause = node_names[node_ind]
@@ -186,21 +185,21 @@
                     # To do so, pop the current one so the other edge is accessible in the next iteration.
                     edge_names.pop(edge_name)
                 except ValueError:
                     self.logger.error(f"There is no edge with cause {cause} and effect {effect}")
                     return False
                 # Add edge with its cause, effect, confidence and timelag to graph_dict
                 graph_dict[edge_name] = {}
-                graph_dict[edge_name].update({"hasCause": [cause]})
+                graph_dict[edge_name].update({"hasCause": cause})
                 if confidence != 0.0:
                     graph_dict[edge_name].update({"hasConfidence": float(confidence)})
-                graph_dict[edge_name].update({"hasEffect": [effect]})
+                graph_dict[edge_name].update({"hasEffect": effect})
                 if time_lag != 0.0:
                     graph_dict[edge_name].update({"hasTimeLag": float(time_lag)})
-                graph_dict[edge_name].update({"type": "CausalEdge"})
+                graph_dict[edge_name].update({"type": ['CausalEdge']})
                 # Add node properties "affected_by" and "causing"
                 graph_dict[cause].setdefault("isCausing", []).append(edge_name)
                 graph_dict[effect].setdefault("isAffectedBy", []).append(edge_name)
         return graph_dict
 
 
     def fill_empty_graph_from_dict(self, graph_dict: dict):
@@ -208,143 +207,156 @@
 
         :param graph_dict: A causalgraph properties dict of a whole graph
         :type graph_dict: dict
         :return: The filled causalgraph object
         :rtype: causalgraph.Graph()
         """
         if type(graph_dict) not in [dict] or graph_dict == {}:
-            self.logger.error("Filling graph with individuals from graph_dict wasn't successful. Passed graph_dict not valid.")
+            self.logger.error(f"Filling graph with individuals from graph_dict wasn't successful. Passed graph_dict not valid. Got graph dict: {graph_dict}")
             return self.graph
         # Check if Graph is empty
         causalnodes_list = owlutils.get_all_causalnodes(self.graph.store)
         causaledges_list = owlutils.get_all_causaledges(self.graph.store)
         if causaledges_list or causalnodes_list:
             self.logger.error("Filling graph with individuals from graph_dict wasn't successful. Graph is not empty.")
             return self.graph
 
-        # Iterate over all individuals in graph_dict
-        # Handling CausalNode first
-        for individual in graph_dict:
-            individual_type = graph_dict[individual]['type']
-            # Handling CausalNodes
-            if individual_type == 'CausalNode':
-                # Create props for later usage as kwargs in G.add.causal_node()
-                individual_prop_dict = self.__create_individual_kwargs_props(graph_dict=graph_dict, individual=individual, type_class=individual_type)
-                # Create CausalNode with props kwargs
-                self.graph.add.causal_node(individual, **individual_prop_dict)      
-
-        # Iterate over individuals over graph_dict
-        # Handling CausalEdges after CausalNodes
-        for individual in graph_dict:
-            individual_type = graph_dict[individual]['type']
-            # Handling CausalEdges
-            if individual_type == 'CausalEdge':
-                # Create props for later usage as kwargs in G.add.causal_edge()
-                individual_prop_dict = self.__create_individual_kwargs_props(graph_dict=graph_dict, individual=individual, type_class=individual_type)
-                # Create CausalEdge with props kwargs
-                cause = graph_dict[individual]['hasCause'][0]
-                effect = graph_dict[individual]['hasEffect'][0]
-                edge_name = individual
-                self.graph.add.causal_edge(cause_node_name=cause, effect_node_name=effect, name_for_edge=edge_name, **individual_prop_dict)
-
+        ### Iterate over all individuals in graph_dict
+        # 1) Check which types can be retrieved and sort into Causal Nodes and Causal Edges
+        causal_node_dict = {}
+        causal_edge_dict = {}
+        for individual, props in graph_dict.items():
+            type_dict = {type_str: self.graph.get_entity(type_str, suppress_warn=True) for type_str in props['type']}
+            # First remove all types, which can not be found in causal knowledge graph
+            for type_str, type_obj in type_dict.items():
+                if type_obj == None:
+                    self.logger.warning(f"TypeDefinition '{type_str}' of individual '{individual}' could not be found in causalgraph-store. Please import the right ontologies first. Type of individual removed from graph_dict.")
+                    props['type'].remove(type_str)
+            # Sort into causal_node_dict, causal_edge_dict or display error
+            if any(owlutils.is_subclass_of(type_, "CausalNode", self.graph.store) for type_ in props['type']):
+                causal_node_dict[individual] = props
+            elif any(owlutils.is_subclass_of(type_, "CausalEdge", self.graph.store) for type_ in props['type']):
+                causal_edge_dict[individual] = props
+            else:
+                raise ValueError(f"Individual '{individual}' in dict is neither 'CausalNode' nor 'CausalEdge'. Only Causal entities supported")
+        # 2) Create causalNodes first
+        for individual_name, props_dict in causal_node_dict.items():
+            individual_prop_dict = self.__create_individual_kwargs_props(props_dict)
+            # Create CausalNode with props kwargs
+            # 2A) Validate domain and range of properties first (if validate_domain_range is True), as adding causal_node will fail otherwise
+            pre_validation = owlutils.validate_property_target_pairs_for_classes(props_dict["type"], individual_prop_dict,
+                                                                                 self.graph.store, logger=self.logger,
+                                                                                 validate_domain_range=self.validate_domain_range)
+            if pre_validation is False:
+                raise ValueError(f"Individual '{individual_name}' with props {individual_prop_dict} could not be created. Property validation failed.")
+            # 2B) Create CausaLNode, with disabled internal validation, only if pre_validation succeeded 
+            # >> This is needed to allow creation first as "CausalNode" and then in 2C change to other derived types
+            causal_node = self.graph.add.causal_node(individual_name, validate_domain_range = False, **individual_prop_dict)
+            if causal_node == None:
+                raise RuntimeError(f"Causal Node '{individual_name}' with props {individual_prop_dict} could not be created. Please check graph_dict: {graph_dict}.")
+            # 2C) Add other potential types as well (e.g. [Pizza, CausalGraph])
+            individual_types_str = props_dict['type']
+            types_list = [self.graph.get_entity(type_str, suppress_warn=True) for type_str in individual_types_str]
+            causal_node.is_a = types_list
+        # 3) Create causalEdges after causalNodes
+        for individual_name, props_dict in causal_edge_dict.items():
+            # Create props for later usage as kwargs in G.add.causal_edge()
+            individual_prop_dict = self.__create_individual_kwargs_props(props_dict)
+            # Create CausalEdge with props kwargs
+            cause = props_dict['hasCause']
+            effect = props_dict['hasEffect']
+            causal_edge = self.graph.add.causal_edge(cause_node=cause, effect_node=effect, name_for_edge=individual_name, **individual_prop_dict)
+            if causal_edge == None:
+                raise RuntimeError(f"Causal Edge '{individual_name}' with props {individual_prop_dict} could not be created. Please check graph_dict: {graph_dict}.")
+            # Add other potential alias or additonals types as well 
+            individual_types_str = props_dict['type']
+            types_list = [self.graph.get_entity(type_str, suppress_warn=True) for type_str in individual_types_str]
+            causal_edge.is_a = types_list
         # Return filled Graph() object
         return self.graph
 
 
-    def __create_individual_kwargs_props(self, graph_dict: dict, individual: str, type_class: str) -> dict:
+    def __create_individual_kwargs_props(self, props_dict: dict) -> dict:
         """This method returns a props dict that can be used to passed as kwargs to the functions add.causal_node()
         or add.causal_edge(). The prop dict will not be containing the properties ["isCausing", "isAffectedBy", "hasCause", "hasEffect"].
-
-        :param graph_dict: A causalgraph properties dict of a whole graph
-        :type graph_dict: dict
-        :param individual: Name of the individual
-        :type individual: str
-        :param type_class: Type of the individual (e. g. CausalEdge or CausalNode)
-        :type type_class: str
+        
+        :param props_dict: The properties dict of the individual
+        :type props_dict: dict
         :return: A properties dict that can be passed as kwargs to add.causal_node() or add.causal_edge()
         :rtype: dict
         """
-        individual_prop_dict = {}
-
-        limiter = []
-        if type_class == "CausalNode":
+        # Remove properties that are not needed for creation
+        types = props_dict['type']
+        if any(owlutils.is_subclass_of(type_, "CausalNode", self.graph.store) for type_ in types):
             limiter = ['isCausing', 'isAffectedBy']
-        elif type_class == "CausalEdge":
+        elif any(owlutils.is_subclass_of(type_, "CausalEdge", self.graph.store) for type_ in types):
             limiter = ['hasCause', 'hasEffect']
         else:
-            self.logger.error(f"Type class '{type_class}' not supported. Empty dict will be returned.")
+            self.logger.error(f"Type classes '{types}' not supported. Empty dict will be returned.")
             return {}
 
-        for prop in graph_dict[individual]:
+        # Create individual_prop_dict
+        individual_prop_dict = {}
+        for prop in props_dict:
             if prop not in ['iri', 'type']:
                 # if prop is object property
                 if prop in (self.causalgraph_object_properties + self.third_party_object_properties) and prop not in limiter:
-                    prop_value = graph_dict[individual][prop]
+                    prop_value = props_dict[prop]
                     if prop == 'comment':
                         comments = list(prop_value)
                         individual_prop_dict[prop] = comments
                     else:
                         if type(prop_value) is list:
                             for value in prop_value:
-                                exists = owlutils.entity_exists(entity_name=value, store=self.graph.store)
+                                exists = owlutils.entity_exists(entity=value, store=self.graph.store)
                                 if not exists:
-                                    range = owlutils.get_range_of_property(store=self.graph.store, property_name=prop)
-                                    new_indi_name = owlutils.create_individual_of_type(
+                                    prop_obj = owlutils.get_entity_by_name(prop, self.graph.store, logger=self.logger)
+                                    range = prop_obj.range
+                                    new_indi = owlutils.create_individual_of_type(
                                         class_of_individual=range[0].name,
                                         store=self.graph.store,
                                         name_for_individual=value,
+                                        validate_domain_range=self.validate_domain_range,
                                         logger=self.logger
                                     )
-                                    new_indi = owlutils.get_entity_by_name(name_of_entity=new_indi_name, store=self.graph.store, logger=self.logger)
+                                    new_indi_name = new_indi.name
                                     try:
                                         individual_prop_dict[prop].append(new_indi)
                                     except:
                                         individual_prop_dict[prop] = [new_indi]
                                 else:
                                     old_indi = owlutils.get_entity_by_name(name_of_entity=value, store=self.graph.store, logger=self.logger)
                                     try:
                                         individual_prop_dict[prop].append(old_indi)
                                     except:
                                         individual_prop_dict[prop] = [old_indi]
                         else:
-                            exists = owlutils.entity_exists(entity_name=prop_value, store=self.graph.store)
+                            exists = owlutils.entity_exists(entity=prop_value, store=self.graph.store)
                             if not exists:
-                                range = owlutils.get_range_of_property(store=self.graph.store, property_name=prop)
-                                new_indi_name = owlutils.create_individual_of_type(
+                                prop_obj = owlutils.get_entity_by_name(prop, self.graph.store, logger=self.logger)
+                                range = prop_obj.range
+                                new_indi = owlutils.create_individual_of_type(
                                     class_of_individual=range[0].name,
                                     store=self.graph.store,
                                     name_for_individual=prop_value,
+                                    validate_domain_range=self.validate_domain_range,
                                     logger=self.logger
                                 )
-                                new_indi = owlutils.get_entity_by_name(name_of_entity=new_indi_name, store=self.graph.store, logger=self.logger)
+                                new_indi_name = new_indi.name
                                 individual_prop_dict[prop] = new_indi
                             else:
                                 old_indi = owlutils.get_entity_by_name(name_of_entity=prop_value, store=self.graph.store, logger=self.logger)
                                 individual_prop_dict[prop] = old_indi
                 # if prop is data property
                 elif prop in (self.causalgraph_data_properties + self.third_party_data_properties):
-                    prop_value = graph_dict[individual][prop]  
+                    prop_value = props_dict[prop]  
                     individual_prop_dict[prop] = prop_value
                 # property unknown
                 else:
                     if prop not in limiter:
                         self.logger.warning(f"Property {prop} unknown. Will be skipped. For creation please import the right ontologies.")
                     
         return individual_prop_dict
 
 
     def update_graph_from_dict(self, graph_dict: dict=None):
         raise NotImplementedError
-
-
-    def __validate_property(self, property: str) -> bool:
-        """Checks if property is valid and therefore within the causalgraph_object_properties, causalgraph_data_properties or third_party_properties list.
-        Returns True if valid, otherwise False.
-
-        :param property: Name of property
-        :type property: str
-        :return: True if valid, otherwise False.
-        :rtype: bool
-        """
-        possible_props = self.causalgraph_object_properties + self.causalgraph_data_properties + self.third_party_data_properties + self.third_party_object_properties
-        return property in possible_props
-
```

### Comparing `causalgraph-0.0.6/causalgraph.egg-info/PKG-INFO` & `causalgraph-0.1.0/causalgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalgraph
-Version: 0.0.6
+Version: 0.1.0
 Summary: A python package for modeling, persisting and visualizing causal graphs embedded in knowledge graphs.
 Author: Fraunhofer IWU
 Author-email: causalgraph@iwu.fraunhofer.de
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: causalgraph Version: 0.0.6 Summary: A python
+Metadata-Version: 2.1 Name: causalgraph Version: 0.1.0 Summary: A python
 package for modeling, persisting and visualizing causal graphs embedded in
 knowledge graphs. Author: Fraunhofer IWU Author-email:
 causalgraph@iwu.fraunhofer.de License: MIT Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
 Content-Type: text/markdown License-File: LICENSE  [![IWU][iwu-shield]](https:/
 /www.iwu.fraunhofer.de/) [![Tests][pytest-shield]](https://github.com/
 causalgraph/causalgraph/actions) [![License][mit-licence]](https://
```

### Comparing `causalgraph-0.0.6/causalgraph.egg-info/SOURCES.txt` & `causalgraph-0.1.0/causalgraph.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,12 +14,14 @@
 causalgraph/store/export.py
 causalgraph/store/load.py
 causalgraph/store/remove.py
 causalgraph/utils/__init__.py
 causalgraph/utils/draw.py
 causalgraph/utils/logging_utils.py
 causalgraph/utils/mapping.py
+causalgraph/utils/misc_utils.py
 causalgraph/utils/owlready2_utils.py
-causalgraph/utils/path_utils.py
 data/__init__.py
 data/causalgraph.owl
-data/logs/__init__.py
+data/logs/__init__.py
+data/logs/cg.json
+tests/test_graph.py
```

### Comparing `causalgraph-0.0.6/data/causalgraph.owl` & `causalgraph-0.1.0/data/causalgraph.owl`

 * *Files 6% similar despite different names*

#### Comparing `causalgraph-0.0.6/data/causalgraph.owl` & `causalgraph-0.1.0/data/causalgraph.owl`

```diff
@@ -13,15 +13,15 @@
   </Annotation>
   <Annotation>
     <AnnotationProperty abbreviatedIRI="rdfs:label"/>
     <Literal xml:lang="en">causalgraph-ontology</Literal>
   </Annotation>
   <Annotation>
     <AnnotationProperty abbreviatedIRI="owl:versionInfo"/>
-    <Literal xml:lang="en">0.1.2</Literal>
+    <Literal xml:lang="en">0.15</Literal>
   </Annotation>
   <Declaration>
     <Class IRI="#CausalEdge"/>
   </Declaration>
   <Declaration>
     <Class IRI="#CausalGraph"/>
   </Declaration>
@@ -214,32 +214,34 @@
     <ObjectProperty IRI="#hasCause"/>
     <ObjectProperty IRI="#isCausing"/>
   </InverseObjectProperties>
   <InverseObjectProperties>
     <ObjectProperty IRI="#hasEffect"/>
     <ObjectProperty IRI="#isAffectedBy"/>
   </InverseObjectProperties>
+  <FunctionalObjectProperty>
+    <ObjectProperty IRI="#hasCause"/>
+  </FunctionalObjectProperty>
+  <FunctionalObjectProperty>
+    <ObjectProperty IRI="#hasEffect"/>
+  </FunctionalObjectProperty>
   <SymmetricObjectProperty>
     <ObjectProperty IRI="#hasCausalConnection"/>
   </SymmetricObjectProperty>
   <ObjectPropertyDomain>
     <ObjectProperty IRI="#created"/>
     <Class IRI="#Creator"/>
   </ObjectPropertyDomain>
   <ObjectPropertyDomain>
     <ObjectProperty IRI="#hasCause"/>
     <Class IRI="#CausalEdge"/>
   </ObjectPropertyDomain>
   <ObjectPropertyDomain>
     <ObjectProperty IRI="#hasCreator"/>
-    <Class IRI="#CausalEdge"/>
-  </ObjectPropertyDomain>
-  <ObjectPropertyDomain>
-    <ObjectProperty IRI="#hasCreator"/>
-    <Class IRI="#CausalNode"/>
+    <Class abbreviatedIRI="owl:Thing"/>
   </ObjectPropertyDomain>
   <ObjectPropertyDomain>
     <ObjectProperty IRI="#hasEffect"/>
     <Class IRI="#CausalEdge"/>
   </ObjectPropertyDomain>
   <ObjectPropertyDomain>
     <ObjectProperty IRI="#isAffectedBy"/>
@@ -247,19 +249,15 @@
   </ObjectPropertyDomain>
   <ObjectPropertyDomain>
     <ObjectProperty IRI="#isCausing"/>
     <Class IRI="#CausalNode"/>
   </ObjectPropertyDomain>
   <ObjectPropertyRange>
     <ObjectProperty IRI="#created"/>
-    <Class IRI="#CausalEdge"/>
-  </ObjectPropertyRange>
-  <ObjectPropertyRange>
-    <ObjectProperty IRI="#created"/>
-    <Class IRI="#CausalNode"/>
+    <Class abbreviatedIRI="owl:Thing"/>
   </ObjectPropertyRange>
   <ObjectPropertyRange>
     <ObjectProperty IRI="#hasCause"/>
     <Class IRI="#CausalNode"/>
   </ObjectPropertyRange>
   <ObjectPropertyRange>
     <ObjectProperty IRI="#hasCreator"/>
@@ -321,21 +319,34 @@
   </DataPropertyRange>
   <DataPropertyRange>
     <DataProperty IRI="#hasTimeLag"/>
     <Datatype abbreviatedIRI="xsd:double"/>
   </DataPropertyRange>
   <DataPropertyRange>
     <DataProperty IRI="#hasTimeLag"/>
+    <Datatype abbreviatedIRI="xsd:int"/>
+  </DataPropertyRange>
+  <DataPropertyRange>
+    <DataProperty IRI="#hasTimeLag"/>
     <DatatypeRestriction>
       <Datatype abbreviatedIRI="xsd:double"/>
       <FacetRestriction facet="http://www.w3.org/2001/XMLSchema#minInclusive">
         <Literal datatypeIRI="http://www.w3.org/2001/XMLSchema#double">0.0</Literal>
       </FacetRestriction>
     </DatatypeRestriction>
   </DataPropertyRange>
+  <DataPropertyRange>
+    <DataProperty IRI="#hasTimeLag"/>
+    <DatatypeRestriction>
+      <Datatype abbreviatedIRI="xsd:int"/>
+      <FacetRestriction facet="http://www.w3.org/2001/XMLSchema#minInclusive">
+        <Literal datatypeIRI="http://www.w3.org/2001/XMLSchema#int">0</Literal>
+      </FacetRestriction>
+    </DatatypeRestriction>
+  </DataPropertyRange>
   <DisjointDataProperties>
     <DataProperty IRI="#hasConfidence"/>
     <DataProperty IRI="#hasTimeLag"/>
   </DisjointDataProperties>
   <AnnotationAssertion>
     <AnnotationProperty abbreviatedIRI="rdfs:comment"/>
     <IRI>#CausalEdge</IRI>
@@ -505,17 +516,37 @@
   <AnnotationAssertion>
     <AnnotationProperty abbreviatedIRI="rdfs:label"/>
     <IRI>#Variable</IRI>
     <Literal xml:lang="en">Variable</Literal>
   </AnnotationAssertion>
   <AnnotationAssertion>
     <AnnotationProperty abbreviatedIRI="rdfs:comment"/>
+    <IRI>#hasCause</IRI>
+    <Literal xml:lang="en">A CausalEdge can only have a single 'cause' indicated via the functional 'hasCause' property.</Literal>
+  </AnnotationAssertion>
+  <AnnotationAssertion>
+    <AnnotationProperty abbreviatedIRI="rdfs:comment"/>
     <IRI>#hasConfidence</IRI>
     <Literal xml:lang="en">Functional property of a CausalEdge. Measures the Creator's confidence (e.g., a learning algorithm) in the presence of this CausalEdge. A value of  1.0 represents complete confidence in the edge's existence, while 0.0 means that this particular edge is not present.</Literal>
   </AnnotationAssertion>
   <AnnotationAssertion>
     <AnnotationProperty abbreviatedIRI="rdfs:comment"/>
+    <IRI>#hasEffect</IRI>
+    <Literal xml:lang="en">A CausalEdge can only have a single 'effect' indicated via the functional 'hasEffect' property.</Literal>
+  </AnnotationAssertion>
+  <AnnotationAssertion>
+    <AnnotationProperty abbreviatedIRI="rdfs:comment"/>
     <IRI>#hasTimeLag</IRI>
     <Literal xml:lang="en">Functional property of a CausalEdge. Measures in SECONDS,  the time lag between cause and the effect to take place. Only positive values are allowed, which means that the effect always occurs after the effect.</Literal>
   </AnnotationAssertion>
+  <AnnotationAssertion>
+    <AnnotationProperty abbreviatedIRI="rdfs:comment"/>
+    <IRI>#isAffectedBy</IRI>
+    <Literal xml:lang="en">A CausalNode can be influenced by many  'causes'  indicated via different CausalEdges pointing toward a CausalNode. All Edges influencing the CausalNode are gathered via the 'isAffectedBy' property.</Literal>
+  </AnnotationAssertion>
+  <AnnotationAssertion>
+    <AnnotationProperty abbreviatedIRI="rdfs:comment"/>
+    <IRI>#isCausing</IRI>
+    <Literal xml:lang="en">A CausalNode can influence many  'effects'  indicated via different CausalEdges being caused by a CausalNode. All Edges influenced from the CausalNode are gathered via the 'isCausing' property.</Literal>
+  </AnnotationAssertion>
 </Ontology>
 <!-- Generated by the OWL API (version 4.5.9.2019-02-01T07:24:44Z) https://github.com/owlcs/owlapi -->
```

### Comparing `causalgraph-0.0.6/setup.py` & `causalgraph-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 with open("README_PIP.md", "r", encoding="utf-8") as fh:
     # variable will be filled with the README content and used
     # as the long description of the package
     long_description = fh.read()
 
 setup(
     name="causalgraph",
-    #name='causalgraph-dev',
-    version="0.0.6",
+    version="0.1.0",
     author="Fraunhofer IWU",
     author_email="causalgraph@iwu.fraunhofer.de",
     description="A python package for modeling, persisting and visualizing causal graphs embedded in knowledge graphs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(exclude=[
@@ -26,19 +25,20 @@
         'data.logs': ['*','*/*','*/*/*'],
         'data': ['*','*/*','*/*/*'],
         'config': ['*','*/*','*/*/*']
     },
     include_package_data=True,
     exclude_package_data={'': ['*__pycache__*']},
     install_requires=[
-        'owlready2==0.35',
-        'networkx==2.6.3',
+        'owlready2==0.43',
+        'networkx==2.8.4',
         'matplotlib==3.5.1',
         'ecs_logging==1.1.0',
-        'numpy==1.22.1',
-        'pandas==1.2.3'
+        'numpy==1.23.5',
+        'pandas==1.5.1',
+        'deprecated==1.2.14'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ]
 )
```

