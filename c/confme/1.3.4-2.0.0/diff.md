# Comparing `tmp/confme-1.3.4.tar.gz` & `tmp/confme-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confme-1.3.4.tar", max compression
+gzip compressed data, was "confme-2.0.0.tar", max compression
```

## Comparing `confme-1.3.4.tar` & `confme-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1085 2023-06-02 10:57:07.714049 confme-1.3.4/LICENSE
--rw-r--r--   0        0        0     8192 2023-06-02 10:57:07.714049 confme-1.3.4/README.md
--rw-r--r--   0        0        0      238 2023-06-02 10:57:07.714049 confme-1.3.4/confme/__init__.py
--rw-r--r--   0        0        0      550 2023-06-02 10:57:07.714049 confme-1.3.4/confme/annotation.py
--rw-r--r--   0        0        0        0 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/__init__.py
--rw-r--r--   0        0        0     1076 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/argument_overwrite.py
--rw-r--r--   0        0        0     6810 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/base_config.py
--rw-r--r--   0        0        0      728 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/env_overwrite.py
--rw-r--r--   0        0        0     2262 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/global_config.py
--rw-r--r--   0        0        0    18170 2023-06-02 10:57:07.714049 confme-1.3.4/confme/pylintrc
--rw-r--r--   0        0        0      841 2023-06-02 10:57:07.714049 confme-1.3.4/confme/source_backend/__init__.py
--rw-r--r--   0        0        0      728 2023-06-02 10:57:07.714049 confme-1.3.4/confme/source_backend/backend_base.py
--rw-r--r--   0        0        0      847 2023-06-02 10:57:07.714049 confme-1.3.4/confme/source_backend/backend_yaml.py
--rw-r--r--   0        0        0        0 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/base_exception.py
--rw-r--r--   0        0        0      974 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/deprecated.py
--rw-r--r--   0        0        0     1099 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/dict_util.py
--rw-r--r--   0        0        0      832 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/typing.py
--rw-r--r--   0        0        0     1353 2023-06-02 10:57:07.714049 confme-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     9443 1970-01-01 00:00:00.000000 confme-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-10 14:20:04.523162 confme-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9849 2023-07-10 14:20:04.523162 confme-2.0.0/README.md
+-rw-r--r--   0        0        0      173 2023-07-10 14:20:04.523162 confme-2.0.0/confme/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-10 14:20:04.523162 confme-2.0.0/confme/annotation.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/__init__.py
+-rw-r--r--   0        0        0     1091 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/argument_overwrite.py
+-rw-r--r--   0        0        0     6814 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/base_config.py
+-rw-r--r--   0        0        0      743 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/env_overwrite.py
+-rw-r--r--   0        0        0    18170 2023-07-10 14:20:04.523162 confme-2.0.0/confme/pylintrc
+-rw-r--r--   0        0        0      841 2023-07-10 14:20:04.523162 confme-2.0.0/confme/source_backend/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-10 14:20:04.523162 confme-2.0.0/confme/source_backend/backend_base.py
+-rw-r--r--   0        0        0      847 2023-07-10 14:20:04.523162 confme-2.0.0/confme/source_backend/backend_yaml.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/base_exception.py
+-rw-r--r--   0        0        0      974 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/deprecated.py
+-rw-r--r--   0        0        0     1099 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/dict_util.py
+-rw-r--r--   0        0        0      763 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/typing.py
+-rw-r--r--   0        0        0     1353 2023-07-10 14:20:04.523162 confme-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11100 1970-01-01 00:00:00.000000 confme-2.0.0/PKG-INFO
```

### Comparing `confme-1.3.4/LICENSE` & `confme-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `confme-1.3.4/README.md` & `confme-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -217,11 +217,35 @@
 ### Overwrite Parameters with Environment Variables
 Likewise to overwriting parameters from the commandline you can also overwrite by passing environment variables. Therefore, simply set the environment variable in the same format as it would be passed as command line arguments and run your application:
 ```shell
 $ export database.host=localhost
 $ python my_programm.py
 ```
 
+## Breaking Changes in v2
+Pydantic is the underlying library powering ConfMe and with the update to pydantic v2 some breaking changes where
+introduced. However, we tried our best to minimize the impact on your project and only passed a selection of changes
+to you. Please find these documented bellow:
+
+### Required, optional and nullable fields
+Pydantic V2 changes some of the logic for specifying whether a field annotated as Optional is required (i.e., has no 
+default value) or not (i.e., has a default value of None or any other value of the corresponding type), and now more 
+closely matches the behavior of dataclasses. Similarly, fields annotated as Any no longer have a default value of None.
+
+The following table describes the behavior of field annotations in V2:
+
+| State                                                 | Field Definition            |
+|-------------------------------------------------------|-----------------------------|
+| Required, cannot be `None`                            | `f1: str`                   |
+| Not required, cannot be `None`, is `'abc'` by default | `f3: str = 'abc'`           |
+| Required, can be `None`                               | `f2: Optional[str]`         |
+| Not required, can be `None`, is `None` by default     | `f3: Optional[str] = None`  |
+| Not required, can be `None`, is `'abc'` by default    | `f3: Optional[str] = 'abc'` |
+| Not required, cannot be `None`                        | `f4: str = 'Foobar'`        |
+| Required, can be any type (including `None`)          | `f5: Any`                   |
+| Not required, can be any type (including `None`)      | `f6: Any = None`            |
+
+
 ## LICENSE
 
 ConfMe is released under the [MIT](LICENSE) license.
```

### Comparing `confme-1.3.4/confme/core/argument_overwrite.py` & `confme-2.0.0/confme/core/argument_overwrite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import argparse
+from typing import Type
 
-from pydantic.main import ModelMetaclass
+from pydantic import BaseModel
 
 from confme.utils.dict_util import flatten, InfiniteDict
 from confme.utils.typing import get_schema
 
 
-def argument_overwrite(config_cls: ModelMetaclass):
+def argument_overwrite(config_cls: Type[BaseModel]):
     # extract possible parameters
     config_dict = get_schema(config_cls)
     parameters, _ = flatten(config_dict)
 
     # get arguments from command line
     parser = argparse.ArgumentParser(prefix_chars='+/')
     group = parser.add_argument_group('Configuration Parameters',
```

### Comparing `confme-1.3.4/confme/core/base_config.py` & `confme-2.0.0/confme/core/base_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 import os
 from pathlib import Path
 from typing import Union, Any, List, Tuple, Callable, TypeVar, Dict
 
-from pydantic import BaseSettings
+from pydantic import BaseModel
 from tabulate import tabulate
 
 from confme import source_backend
 from confme.core.argument_overwrite import argument_overwrite
 from confme.core.env_overwrite import env_overwrite
 from confme.utils.base_exception import ConfmeException
 from confme.utils.dict_util import recursive_update, flatten
 
 T = TypeVar('T', bound='BaseConfig')
 
 
-class BaseConfig(BaseSettings):
+class BaseConfig(BaseModel):
     _KEY_LOOKUP = ['env', 'environment', 'environ', 'stage']
     _config_path: Path = None
     _default_env: str = None
     _cache: Dict[str, T] = {}
 
     @classmethod
     def load(cls, path: Union[Path, str]) -> 'BaseConfig':
@@ -28,22 +28,22 @@
         :param path: path to configuration file
         :return: instance of config_class with all values added from the config file
         """
         config_content = source_backend.parse_file(Path(path))
         config_content = recursive_update(config_content, env_overwrite(cls))
         config_content = recursive_update(config_content, argument_overwrite(cls))
 
-        return cls.parse_obj(config_content)
+        return cls.model_validate(config_content)
 
     @classmethod
     def load_from_dict(cls, config_content: Dict) -> 'BaseConfig':
         config_content = recursive_update(config_content, env_overwrite(cls))
         config_content = recursive_update(config_content, argument_overwrite(cls))
 
-        return cls.parse_obj(config_content)
+        return cls.model_validate(config_content)
 
     @classmethod
     def register_folder(cls, config_folder: Path, default_env: str = None, strict: bool = False):
         """Register a folder where configuration files are drawn based on the environment.
         :param config_folder: Path to the folder with configuration files per environment
         :param default_env: Default environment that should be used if none is specified via environment variable
         :param strict: If True, an exception is raised if no configuration file is found that exactly matches env name.
```

### Comparing `confme-1.3.4/confme/core/env_overwrite.py` & `confme-2.0.0/confme/core/env_overwrite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
+from typing import Type
 
-from pydantic.main import ModelMetaclass
+from pydantic import BaseModel
 
 from confme.utils.dict_util import flatten, InfiniteDict
 from confme.utils.typing import get_schema
 
 
-def env_overwrite(config_cls: ModelMetaclass):
+def env_overwrite(config_cls: Type[BaseModel]):
     # extract possible parameters
     config_dict = get_schema(config_cls)
     parameters, _ = flatten(config_dict)
 
     # make env variables case insensitive
     keys, values = zip(*os.environ.items())
     keys = [k.casefold() for k in keys]
```

### Comparing `confme-1.3.4/confme/pylintrc` & `confme-2.0.0/confme/pylintrc`

 * *Files identical despite different names*

### Comparing `confme-1.3.4/confme/source_backend/__init__.py` & `confme-2.0.0/confme/source_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.4/confme/source_backend/backend_base.py` & `confme-2.0.0/confme/source_backend/backend_base.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.4/confme/source_backend/backend_yaml.py` & `confme-2.0.0/confme/source_backend/backend_yaml.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.4/confme/utils/deprecated.py` & `confme-2.0.0/confme/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.4/confme/utils/dict_util.py` & `confme-2.0.0/confme/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.4/confme/utils/typing.py` & `confme-2.0.0/confme/utils/typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from typing import Dict
+from typing import Dict, Type
 
-from pydantic.main import ModelMetaclass
-from pydantic.schema import model_schema
+from pydantic import BaseModel
 
 
 def _create_dict(schema_head: Dict, definitions: Dict):
     schema_dict = {}
     if 'type' in schema_head and schema_head['type'] == 'object':
         for key, value in schema_head['properties'].items():
-            if 'allOf' in value:
-                sub_schema = value['allOf'][0]['$ref'].replace('#/definitions/', '')
+            if '$ref' in value:
+                sub_schema = value['$ref'].replace('#/$defs/', '')
                 schema_dict[key] = _create_dict(definitions[sub_schema], definitions)
             else:
                 schema_dict[key] = None
     else:
         return None
     return schema_dict
 
 
-def get_schema(config_cls: ModelMetaclass):
-    schema = model_schema(config_cls)
-    definitions = schema['definitions'] if 'definitions' in schema else {}
+def get_schema(config_cls: Type[BaseModel]):
+    schema = config_cls.model_json_schema()
+    definitions = schema['$defs'] if '$defs' in schema else {}
     return _create_dict(schema, definitions)
```

### Comparing `confme-1.3.4/pyproject.toml` & `confme-2.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confme"
-version = "1.3.4"
+version = "2.0.0"
 description = "Easy configuration management in python"
 authors = ["Iwan Silvan Bolzern <iwan.bolzern@roche.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/iwanbolzern/confme"
 repository = "https://github.com/iwanbolzern/confme"
 classifiers = [
@@ -27,15 +27,15 @@
     { include = "confme" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 pyyaml = "^5.3"
-pydantic = "^1.4"
+pydantic = "^2.0"
 tabulate = "^0.8.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1.2"
 pylint = "^2.17.4"
 sphinx = "^3.2.1"
 recommonmark = "^0.6.0"
```

### Comparing `confme-1.3.4/PKG-INFO` & `confme-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confme
-Version: 1.3.4
+Version: 2.0.0
 Summary: Easy configuration management in python
 Home-page: https://github.com/iwanbolzern/confme
 License: LICENSE
 Author: Iwan Silvan Bolzern
 Author-email: iwan.bolzern@roche.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: pydantic (>=1.4,<2.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyyaml (>=5.3,<6.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Project-URL: Repository, https://github.com/iwanbolzern/confme
 Description-Content-Type: text/markdown
 
 # ConfMe: Configuration Made Easy 💖
 
@@ -247,12 +247,36 @@
 ### Overwrite Parameters with Environment Variables
 Likewise to overwriting parameters from the commandline you can also overwrite by passing environment variables. Therefore, simply set the environment variable in the same format as it would be passed as command line arguments and run your application:
 ```shell
 $ export database.host=localhost
 $ python my_programm.py
 ```
 
+## Breaking Changes in v2
+Pydantic is the underlying library powering ConfMe and with the update to pydantic v2 some breaking changes where
+introduced. However, we tried our best to minimize the impact on your project and only passed a selection of changes
+to you. Please find these documented bellow:
+
+### Required, optional and nullable fields
+Pydantic V2 changes some of the logic for specifying whether a field annotated as Optional is required (i.e., has no 
+default value) or not (i.e., has a default value of None or any other value of the corresponding type), and now more 
+closely matches the behavior of dataclasses. Similarly, fields annotated as Any no longer have a default value of None.
+
+The following table describes the behavior of field annotations in V2:
+
+| State                                                 | Field Definition            |
+|-------------------------------------------------------|-----------------------------|
+| Required, cannot be `None`                            | `f1: str`                   |
+| Not required, cannot be `None`, is `'abc'` by default | `f3: str = 'abc'`           |
+| Required, can be `None`                               | `f2: Optional[str]`         |
+| Not required, can be `None`, is `None` by default     | `f3: Optional[str] = None`  |
+| Not required, can be `None`, is `'abc'` by default    | `f3: Optional[str] = 'abc'` |
+| Not required, cannot be `None`                        | `f4: str = 'Foobar'`        |
+| Required, can be any type (including `None`)          | `f5: Any`                   |
+| Not required, can be any type (including `None`)      | `f6: Any = None`            |
+
+
 ## LICENSE
 
 ConfMe is released under the [MIT](LICENSE) license.
```

