# Comparing `tmp/dynamicpy-1.0.1.tar.gz` & `tmp/dynamicpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicpy-1.0.1.tar", max compression
+gzip compressed data, was "dynamicpy-1.1.0.tar", max compression
```

## Comparing `dynamicpy-1.0.1.tar` & `dynamicpy-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      631 2023-06-12 22:26:31.466444 dynamicpy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2071 2023-06-11 16:07:04.241129 dynamicpy-1.0.1/README.md
--rw-r--r--   0        0        0      932 2023-06-11 16:56:21.650424 dynamicpy-1.0.1/src/dynamicpy/__init__.py
--rw-r--r--   0        0        0     4053 2023-06-11 16:12:16.780891 dynamicpy-1.0.1/src/dynamicpy/dependencies.py
--rw-r--r--   0        0        0     1091 2023-06-11 14:18:34.657264 dynamicpy-1.0.1/src/dynamicpy/errors.py
--rw-r--r--   0        0        0     4037 2023-06-11 15:15:30.094095 dynamicpy-1.0.1/src/dynamicpy/loader.py
--rw-r--r--   0        0        0     5070 2023-06-11 17:19:59.134633 dynamicpy-1.0.1/src/dynamicpy/utils.py
--rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 dynamicpy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2008 2023-07-10 17:05:28.972821 dynamicpy-1.1.0/README.md
+-rw-r--r--   0        0        0      627 2023-07-10 17:05:28.976821 dynamicpy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      893 2023-07-10 17:05:28.976821 dynamicpy-1.1.0/src/dynamicpy/__init__.py
+-rw-r--r--   0        0        0     3932 2023-07-10 17:05:28.976821 dynamicpy-1.1.0/src/dynamicpy/dependencies.py
+-rw-r--r--   0        0        0     1056 2023-07-10 17:05:28.976821 dynamicpy-1.1.0/src/dynamicpy/errors.py
+-rw-r--r--   0        0        0     5553 2023-07-10 17:05:28.976821 dynamicpy-1.1.0/src/dynamicpy/loader.py
+-rw-r--r--   0        0        0     4884 2023-07-10 17:05:28.976821 dynamicpy-1.1.0/src/dynamicpy/utils.py
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 dynamicpy-1.1.0/PKG-INFO
```

### Comparing `dynamicpy-1.0.1/pyproject.toml` & `dynamicpy-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-[tool.poetry]
-name = "dynamicpy"
-version = "1.0.1"
-description = "A python module for dynamically interacting with objects to improve expandability."
-authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
-repository = "https://github.com/NimajnebEC/dynamicpy"
-packages = [{ include = "dynamicpy", from = "src" }]
-readme = "README.md"
-license = "MIT"
-
-[tool.poetry.dependencies]
-typeguard = "^4.0.0"
-python = "^3.8.1"
-
-[tool.poetry.group.dev.dependencies]
-flake8-length = "^0.3.1"
-pytest = "^7.3.1"
-flake8 = "^6.0.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "dynamicpy"
+version = "1.1.0"
+description = "A python module for dynamically interacting with objects to improve expandability."
+authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
+repository = "https://github.com/NimajnebEC/dynamicpy"
+packages = [{ include = "dynamicpy", from = "src" }]
+readme = "README.md"
+license = "MIT"
+
+[tool.poetry.dependencies]
+typeguard = "^4.0.0"
+python = "^3.8.1"
+
+[tool.poetry.group.dev.dependencies]
+flake8-length = "^0.3.1"
+pytest = "^7.3.1"
+flake8 = "^6.0.0"
+isort = "^5.12.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `dynamicpy-1.0.1/README.md` & `dynamicpy-1.1.0/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# DynamicPy
-
-A python module for dynamically interacting with objects to improve expandability.
-
-## DynamicLoader
-
-The `DynamicLoader` class allows for the dynamic import of modules and the scraping of their globals.
-
-To provide functionality with the scraped globals you must register a handler using the `register_handler` method or the `handler` decorator. Both methods take an optional `selector` parameter which is a predicate to determine wether the handler should be called.
-
-### Example:
-
-```py
-from dynamicpy import DynamicLoader
-
-loader = DynamicLoader()
-
-@loader.handler()
-def handler(name: str, value: object):
-    print(name) # Prints the name of every global imported
-
-loader.load_module("package.module")
-```
-
-Dynamicpy provides a handful of utility functions to traverse modules in the stack which can be useful for streamlining this process.
-
-## DependencyLibrary
-
-The `DependencyLibrary` class allows you to create a library of objects which can then be injected into function parameters using type annotations.
-
-Dependencies are added using the `add` method, only a single dependency per type can be added to the library. Dependencies can be retrived using square brackets. You can check if an object has been added to the library using the `in` operator which can also be used to check if there are any dependencies of a certain type in the library.
-
-### Example
-
-```py
-from dynamicpy import DependencyLibrary
-
-library = DependencyLibrary()
-library.add("Hello World!")
-
-print(library[str]) # Hello World!
-
-print(str in library) # True
-print("Hello World!" in library) # True
-print("Lorem Ipsum" in library) # False
-print(int in library) # False
-```
-
-The `DependencyLibrary` class also allows for dependencies to be injected into function parameters using the `inject` method.
-
-### Example
-
-```py
-from dynamicpy import DependencyLibrary
-
-library = DependencyLibrary()
-library.add("Hello World!")
-
-def injected(message: str):
-    print(message) # Hello World!
-
-library.inject(injected)
-```
+# DynamicPy
+
+A python module for dynamically interacting with objects to improve expandability.
+
+## DynamicLoader
+
+The `DynamicLoader` class allows for the dynamic import of modules and the scraping of their globals.
+
+To provide functionality with the scraped globals you must register a handler using the `register_handler` method or the `handler` decorator. Both methods take an optional `selector` parameter which is a predicate to determine wether the handler should be called.
+
+### Example:
+
+```py
+from dynamicpy import DynamicLoader
+
+loader = DynamicLoader()
+
+@loader.handler()
+def handler(name: str, value: object):
+    print(name) # Prints the name of every global imported
+
+loader.load_module("package.module")
+```
+
+Dynamicpy provides a handful of utility functions to traverse modules in the stack which can be useful for streamlining this process.
+
+## DependencyLibrary
+
+The `DependencyLibrary` class allows you to create a library of objects which can then be injected into function parameters using type annotations.
+
+Dependencies are added using the `add` method, only a single dependency per type can be added to the library. Dependencies can be retrived using square brackets. You can check if an object has been added to the library using the `in` operator which can also be used to check if there are any dependencies of a certain type in the library.
+
+### Example
+
+```py
+from dynamicpy import DependencyLibrary
+
+library = DependencyLibrary()
+library.add("Hello World!")
+
+print(library[str]) # Hello World!
+
+print(str in library) # True
+print("Hello World!" in library) # True
+print("Lorem Ipsum" in library) # False
+print(int in library) # False
+```
+
+The `DependencyLibrary` class also allows for dependencies to be injected into function parameters using the `inject` method.
+
+### Example
+
+```py
+from dynamicpy import DependencyLibrary
+
+library = DependencyLibrary()
+library.add("Hello World!")
+
+def injected(message: str):
+    print(message) # Hello World!
+
+library.inject(injected)
+```
```

### Comparing `dynamicpy-1.0.1/src/dynamicpy/__init__.py` & `dynamicpy-1.1.0/src/dynamicpy/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-A python module for dynamically interacting with objects to improve expandability.
-
-https://github.com/NimajnebEC/dynamicpy
-"""
-
-from dynamicpy.dependencies import DependencyLibrary
-from dynamicpy.loader import DynamicLoader
-from dynamicpy.errors import (
-    DynamicPyError,
-    NoForeignModulesError,
-    NoParentError,
-    DependencyNotFoundError,
-    DuplicateDependencyError,
-    InjectDependenciesError,
-)
-from dynamicpy.utils import (
-    get_foreign_module,
-    get_module_parent,
-    is_package,
-    get_module,
-    get_stack_module_up,
-)
-
-__all__ = (
-    "DynamicLoader",
-    "DependencyLibrary",
-    "DynamicPyError",
-    "NoForeignModulesError",
-    "NoParentError",
-    "get_foreign_module",
-    "get_module_parent",
-    "get_stack_module_up",
-    "get_module",
-    "is_package",
-    "DependencyNotFoundError",
-    "DuplicateDependencyError",
-    "InjectDependenciesError",
-)
+"""
+A python module for dynamically interacting with objects to improve expandability.
+
+https://github.com/NimajnebEC/dynamicpy
+"""
+
+from dynamicpy.dependencies import DependencyLibrary
+from dynamicpy.errors import (
+    DependencyNotFoundError,
+    DuplicateDependencyError,
+    DynamicPyError,
+    InjectDependenciesError,
+    NoForeignModulesError,
+    NoParentError,
+)
+from dynamicpy.loader import DynamicLoader
+from dynamicpy.utils import (
+    get_foreign_module,
+    get_module,
+    get_module_parent,
+    get_stack_module_up,
+    is_package,
+)
+
+__all__ = (
+    "DynamicLoader",
+    "DependencyLibrary",
+    "DynamicPyError",
+    "NoForeignModulesError",
+    "NoParentError",
+    "get_foreign_module",
+    "get_module_parent",
+    "get_stack_module_up",
+    "get_module",
+    "is_package",
+    "DependencyNotFoundError",
+    "DuplicateDependencyError",
+    "InjectDependenciesError",
+)
```

### Comparing `dynamicpy-1.0.1/src/dynamicpy/dependencies.py` & `dynamicpy-1.1.0/src/dynamicpy/dependencies.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,118 @@
-from typing import Union, TypeVar, Type, Callable
-from typeguard import check_type, TypeCheckError
-from dynamicpy import errors
-import inspect
-import logging
-
-__all__ = ("DependencyLibrary",)
-
-_log = logging.getLogger(__name__)
-
-T = TypeVar("T")
-
-
-class DependencyLibrary:
-    """An instance of `DependencyLibrary` can be used to build up a library of objects that can be injected into functions by type."""
-
-    def __init__(self) -> None:
-        """An instance of `DependencyLibrary` can be used to build up a library of objects that can be injected into functions by type."""
-        self._library: list[object] = []
-
-    def add(self, dependency: object):
-        """Adds a dependency to the library.
-
-        Parameters
-        ----------
-        dependency : object
-            The dependency to add to the library,
-
-        Raises
-        ------
-        TypeError
-            Raised when attempting to add a type to the library.
-        DuplicateDependencyError
-            Raised when another dependency with that type already exists in the library.
-        """
-        if isinstance(dependency, type):
-            raise TypeError("Dependencies cannot be types.")
-        if type(dependency) in self:
-            raise errors.DuplicateDependencyError(
-                f"Instance of '{type(dependency)}' already in library."
-            )
-        self._library.append(dependency)
-
-    def inject(self, func: Callable[..., T]) -> T:
-        """Calls the specified function, injecting dependencies from the library into parameters by type annotations.
-
-        Parameters
-        ----------
-        func : Callable
-            The function to call.
-
-        Returns
-        -------
-            The return value of the `func` parameter.
-
-        Raises
-        ------
-        InjectDependenciesError
-            Raised when there is an error injecting dependencies.
-        DependencyNotFoundError
-            Raised when a requested dependency could not be found.
-        """
-        signature = inspect.signature(func)
-
-        args = []
-        kwargs = {}
-        # Iterate through function parameters
-        for parameter in signature.parameters.values():
-            # Raise error if parameter has no type annotations
-            if parameter.annotation is inspect._empty:
-                raise errors.InjectDependenciesError(
-                    f"Parameter '{parameter.name}' is missing type annotations."
-                )
-
-            try:
-                # Attempt to find dependency in library
-                value = self[parameter.annotation]
-            except errors.DependencyNotFoundError:
-                # Ignore missing dependency if parameter has default value
-                if parameter.default is inspect._empty:
-                    raise
-                continue
-            # Add value to the appropriate collection
-            if parameter.kind is parameter.POSITIONAL_ONLY:
-                args.append(value)
-            else:
-                kwargs[parameter.name] = value
-
-        try:
-            # Attempt to bind parameters
-            signature.bind(*args, **kwargs)
-        except TypeError as e:
-            raise errors.InjectDependenciesError(
-                "Could not bind dependencies to function."
-            ) from e
-
-        return func(*args, **kwargs)
-
-    def __contains__(self, item: Union[type, object]) -> bool:
-        if isinstance(item, type):
-            try:
-                self[item]
-            except errors.DependencyNotFoundError:
-                return False
-            else:
-                return True
-        else:
-            return item in self._library
-
-    def __getitem__(self, type: Type[T]) -> T:
-        for dependency in self._library:
-            try:
-                return check_type(dependency, type)
-            except TypeCheckError:
-                continue
-        raise errors.DependencyNotFoundError(f"No dependency of type '{type}' found.")
+import inspect
+import logging
+from typing import Any, Callable, Type, TypeVar, Union
+
+from typeguard import TypeCheckError, check_type
+
+from dynamicpy import errors
+
+__all__ = ("DependencyLibrary",)
+
+_log = logging.getLogger(__name__)
+
+T = TypeVar("T")
+
+
+class DependencyLibrary:
+    """An instance of `DependencyLibrary` can be used to build up a library of objects that can be injected into functions by type."""
+
+    def __init__(self) -> None:
+        """An instance of `DependencyLibrary` can be used to build up a library of objects that can be injected into functions by type."""
+        self._library: list[Any] = []
+
+    def add(self, dependency: Any):
+        """Adds a dependency to the library.
+
+        Parameters
+        ----------
+        dependency : Any
+            The dependency to add to the library,
+
+        Raises
+        ------
+        TypeError
+            Raised when attempting to add a type to the library.
+        DuplicateDependencyError
+            Raised when another dependency with that type already exists in the library.
+        """
+        if isinstance(dependency, type):
+            raise TypeError("Dependencies cannot be types.")
+        if type(dependency) in self:
+            raise errors.DuplicateDependencyError(
+                f"Instance of '{type(dependency)}' already in library."
+            )
+        self._library.append(dependency)
+
+    def inject(self, func: Callable[..., T]) -> T:
+        """Calls the specified function, injecting dependencies from the library into parameters by type annotations.
+
+        Parameters
+        ----------
+        func : Callable
+            The function to call.
+
+        Returns
+        -------
+            The return value of the `func` parameter.
+
+        Raises
+        ------
+        InjectDependenciesError
+            Raised when there is an error injecting dependencies.
+        DependencyNotFoundError
+            Raised when a requested dependency could not be found.
+        """
+        signature = inspect.signature(func)
+
+        args = []
+        kwargs = {}
+        # Iterate through function parameters
+        for parameter in signature.parameters.values():
+            # Raise error if parameter has no type annotations
+            if parameter.annotation is inspect._empty:
+                raise errors.InjectDependenciesError(
+                    f"Parameter '{parameter.name}' is missing type annotations."
+                )
+
+            try:
+                # Attempt to find dependency in library
+                value = self[parameter.annotation]
+            except errors.DependencyNotFoundError:
+                # Ignore missing dependency if parameter has default value
+                if parameter.default is inspect._empty:
+                    raise
+                continue
+            # Add value to the appropriate collection
+            if parameter.kind is parameter.POSITIONAL_ONLY:
+                args.append(value)
+            else:
+                kwargs[parameter.name] = value
+
+        try:
+            # Attempt to bind parameters
+            signature.bind(*args, **kwargs)
+        except TypeError as e:
+            raise errors.InjectDependenciesError(
+                "Could not bind dependencies to function."
+            ) from e
+
+        return func(*args, **kwargs)
+
+    def __contains__(self, item: Union[type, Any]) -> bool:
+        if isinstance(item, type):
+            try:
+                self[item]
+            except errors.DependencyNotFoundError:
+                return False
+            else:
+                return True
+        else:
+            return item in self._library
+
+    def __getitem__(self, type: Type[T]) -> T:
+        for dependency in self._library:
+            try:
+                return check_type(dependency, type)
+            except TypeCheckError:
+                continue
+        raise errors.DependencyNotFoundError(f"No dependency of type '{type}' found.")
```

### Comparing `dynamicpy-1.0.1/src/dynamicpy/utils.py` & `dynamicpy-1.1.0/src/dynamicpy/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,187 +1,188 @@
-import dynamicpy.errors as errors
-from typing import Iterator, Union
-from types import ModuleType
-import importlib.machinery
-import importlib.util
-import importlib.abc
-import importlib
-import pkgutil
-import sys
-
-__all__ = (
-    "iter_stack_modules",
-    "iter_submodules",
-    "get_stack_module_up",
-    "get_foreign_module",
-    "get_module_parent",
-    "is_package",
-    "get_module",
-)
-
-
-def iter_stack_modules(offset: int = 1) -> Iterator[str]:
-    """Yields the containing module name for every frame in the stack.
-
-    Parameters
-    ----------
-    offset : int
-        Offset up the stack to start iterating from.
-
-    Yields
-    ------
-    str
-        The name of the frame's containing module.
-    """
-    frame = sys._getframe(offset)
-    while frame is not None:
-        yield frame.f_globals.get("__name__", "")
-        frame = frame.f_back
-
-
-def get_stack_module_up(amount: int) -> str:
-    """Get the module name of the frame `amount` steps up the stack.
-
-    If `amount` = 0 then the name of the module this function is called from will be returned.
-
-    Parameters
-    ----------
-    amount : int
-        Number of steps up stack to get the module name of.
-
-    Returns
-    -------
-    str
-        The module name of the frame.
-    """
-    return next(iter_stack_modules(amount + 2))
-
-
-def get_foreign_module(just_module: bool = False) -> str:
-    """Gets the name of the first module with a different top-level package found in the stack.
-
-    Parameters
-    ----------
-    just_module : bool, optional
-        If `True` will also look for sibling modules in the same package, `False` by default.
-
-    Returns
-    -------
-    str
-        The name of the foreign module.
-
-    Raises
-    ------
-    NoForeignModulesError
-        Raised when no foreign module could be found.
-    """
-    # get module name of caller
-    location = get_stack_module_up(1)
-    if not just_module:
-        location = location.split(".")[0]
-
-    # iterate through stack unil foreign module found
-    for module in iter_stack_modules(2):
-        if module != location and (just_module or not module.startswith(location + ".")):
-            return module
-    raise errors.NoForeignModulesError("Could not find any foreign modules in the stack.")
-
-
-def iter_submodules(package: ModuleType) -> Iterator[importlib.machinery.ModuleSpec]:
-    """Yields ModuleSpec for all submodules of the provided package.
-
-    Parameters
-    ----------
-    module : ModuleType
-        The package to iterate through.
-
-    Yields
-    ------
-    ModuleSpec
-        The spec for a submodule of the package.
-
-    Raises
-    ------
-    ExpectedPackageError
-        Raised when the provided module is not a package.
-    """
-    if not is_package(package):
-        raise errors.NotPackageError("Provided module is not a package.")
-    for finder, name, _ in pkgutil.iter_modules(package.__path__, package.__name__ + "."):
-        spec = None
-        if isinstance(finder, importlib.abc.MetaPathFinder):
-            spec = finder.find_spec(name, package.__path__)
-        elif isinstance(finder, importlib.abc.PathEntryFinder):
-            spec = finder.find_spec(name, package)
-
-        if spec is not None:
-            yield spec
-
-
-def is_package(module: Union[str, ModuleType]) -> bool:
-    """Checks if the given module is a package.
-
-    Parameters
-    ----------
-    module : ModuleType
-        The module to check.
-
-    Returns
-    -------
-    bool
-        True if the provided module is a package.
-    """
-    if isinstance(module, str):
-        module = get_module(module)
-    return hasattr(module, "__path__")
-
-
-def get_module(name: str, package: Union[str, ModuleType, None] = None) -> ModuleType:
-    """Gets a module from its name.
-
-    Parameters
-    ----------
-    name : str
-        The absolute name of the module.
-    package : Union[str, ModuleType], optional
-        If present, will perform a relative import from the specified package.
-
-    Returns
-    -------
-    ModuleType
-        The imported module.
-
-    Raises
-    ------
-    ImportError
-        Raised when there is an error importing the module.
-    """
-    if isinstance(package, ModuleType):
-        package = package.__name__
-    return importlib.import_module(name, package)
-
-
-def get_module_parent(module: Union[ModuleType, str]) -> str:
-    """Gets the parent package of the specified module.
-
-    Parameters
-    ----------
-    module : str
-        The module to get the parent of.
-
-    Returns
-    -------
-    str
-        The parent package of the specified module.
-
-    Raises
-    ------
-    NoParentError
-        Raised when the specified module has no parent.
-    """
-    if isinstance(module, ModuleType):
-        module = module.__name__
-    try:
-        resolved = importlib.util.resolve_name("..", module)
-    except ImportError:
-        raise errors.NoParentError(f"'{module}' does not have a parent.")
-    return resolved
+import importlib
+import importlib.abc
+import importlib.machinery
+import importlib.util
+import pkgutil
+import sys
+from types import ModuleType
+from typing import Iterator, Union
+
+import dynamicpy.errors as errors
+
+__all__ = (
+    "iter_stack_modules",
+    "iter_submodules",
+    "get_stack_module_up",
+    "get_foreign_module",
+    "get_module_parent",
+    "is_package",
+    "get_module",
+)
+
+
+def iter_stack_modules(offset: int = 1) -> Iterator[str]:
+    """Yields the containing module name for every frame in the stack.
+
+    Parameters
+    ----------
+    offset : int
+        Offset up the stack to start iterating from.
+
+    Yields
+    ------
+    str
+        The name of the frame's containing module.
+    """
+    frame = sys._getframe(offset)
+    while frame is not None:
+        yield frame.f_globals.get("__name__", "")
+        frame = frame.f_back
+
+
+def get_stack_module_up(amount: int) -> str:
+    """Get the module name of the frame `amount` steps up the stack.
+
+    If `amount` = 0 then the name of the module this function is called from will be returned.
+
+    Parameters
+    ----------
+    amount : int
+        Number of steps up stack to get the module name of.
+
+    Returns
+    -------
+    str
+        The module name of the frame.
+    """
+    return next(iter_stack_modules(amount + 2))
+
+
+def get_foreign_module(just_module: bool = False) -> str:
+    """Gets the name of the first module with a different top-level package found in the stack.
+
+    Parameters
+    ----------
+    just_module : bool, optional
+        If `True` will also look for sibling modules in the same package, `False` by default.
+
+    Returns
+    -------
+    str
+        The name of the foreign module.
+
+    Raises
+    ------
+    NoForeignModulesError
+        Raised when no foreign module could be found.
+    """
+    # get module name of caller
+    location = get_stack_module_up(1)
+    if not just_module:
+        location = location.split(".")[0]
+
+    # iterate through stack unil foreign module found
+    for module in iter_stack_modules(2):
+        if module != location and (just_module or not module.startswith(location + ".")):
+            return module
+    raise errors.NoForeignModulesError("Could not find any foreign modules in the stack.")
+
+
+def iter_submodules(package: ModuleType) -> Iterator[importlib.machinery.ModuleSpec]:
+    """Yields ModuleSpec for all submodules of the provided package.
+
+    Parameters
+    ----------
+    module : ModuleType
+        The package to iterate through.
+
+    Yields
+    ------
+    ModuleSpec
+        The spec for a submodule of the package.
+
+    Raises
+    ------
+    ExpectedPackageError
+        Raised when the provided module is not a package.
+    """
+    if not is_package(package):
+        raise errors.NotPackageError("Provided module is not a package.")
+    for finder, name, _ in pkgutil.iter_modules(package.__path__, package.__name__ + "."):
+        spec = None
+        if isinstance(finder, importlib.abc.MetaPathFinder):
+            spec = finder.find_spec(name, package.__path__)
+        elif isinstance(finder, importlib.abc.PathEntryFinder):
+            spec = finder.find_spec(name, package)
+
+        if spec is not None:
+            yield spec
+
+
+def is_package(module: Union[str, ModuleType]) -> bool:
+    """Checks if the given module is a package.
+
+    Parameters
+    ----------
+    module : ModuleType
+        The module to check.
+
+    Returns
+    -------
+    bool
+        True if the provided module is a package.
+    """
+    if isinstance(module, str):
+        module = get_module(module)
+    return hasattr(module, "__path__")
+
+
+def get_module(name: str, package: Union[str, ModuleType, None] = None) -> ModuleType:
+    """Gets a module from its name.
+
+    Parameters
+    ----------
+    name : str
+        The absolute name of the module.
+    package : Union[str, ModuleType], optional
+        If present, will perform a relative import from the specified package.
+
+    Returns
+    -------
+    ModuleType
+        The imported module.
+
+    Raises
+    ------
+    ImportError
+        Raised when there is an error importing the module.
+    """
+    if isinstance(package, ModuleType):
+        package = package.__name__
+    return importlib.import_module(name, package)
+
+
+def get_module_parent(module: Union[ModuleType, str]) -> str:
+    """Gets the parent package of the specified module.
+
+    Parameters
+    ----------
+    module : str
+        The module to get the parent of.
+
+    Returns
+    -------
+    str
+        The parent package of the specified module.
+
+    Raises
+    ------
+    NoParentError
+        Raised when the specified module has no parent.
+    """
+    if isinstance(module, ModuleType):
+        module = module.__name__
+    try:
+        resolved = importlib.util.resolve_name("..", module)
+    except ImportError:
+        raise errors.NoParentError(f"'{module}' does not have a parent.")
+    return resolved
```

### Comparing `dynamicpy-1.0.1/PKG-INFO` & `dynamicpy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python module for dynamically interacting with objects to improve expandability.
 Home-page: https://github.com/NimajnebEC/dynamicpy
 License: MIT
 Author: NimajnebEC
 Author-email: nimajnebec@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

