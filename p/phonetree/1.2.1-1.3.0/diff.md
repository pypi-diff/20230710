# Comparing `tmp/phonetree-1.2.1.tar.gz` & `tmp/phonetree-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonetree-1.2.1.tar", last modified: Wed Jun 14 21:00:45 2023, max compression
+gzip compressed data, was "phonetree-1.3.0.tar", last modified: Mon Jul 10 02:11:34 2023, max compression
```

## Comparing `phonetree-1.2.1.tar` & `phonetree-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 21:00:45.023933 phonetree-1.2.1/
--rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.2.1/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 21:00:45.023830 phonetree-1.2.1/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.2.1/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 21:00:45.023015 phonetree-1.2.1/phonetree/
--rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.2.1/phonetree/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)    11806 2023-06-14 20:59:32.000000 phonetree-1.2.1/phonetree/phonetree.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 21:00:45.023693 phonetree-1.2.1/phonetree.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      241 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       18 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       10 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)      944 2023-06-14 21:00:22.000000 phonetree-1.2.1/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-14 21:00:45.023961 phonetree-1.2.1/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-10 02:11:34.119609 phonetree-1.3.0/
+-rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.3.0/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-07-10 02:11:34.119511 phonetree-1.3.0/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.3.0/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-10 02:11:34.118810 phonetree-1.3.0/phonetree/
+-rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.3.0/phonetree/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)    11373 2023-07-10 02:11:04.000000 phonetree-1.3.0/phonetree/phonetree.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-10 02:11:34.119391 phonetree-1.3.0/phonetree.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      241 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       18 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       10 2023-07-10 02:11:34.000000 phonetree-1.3.0/phonetree.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)      944 2023-07-10 01:37:54.000000 phonetree-1.3.0/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-07-10 02:11:34.119634 phonetree-1.3.0/setup.cfg
```

### Comparing `phonetree-1.2.1/LICENSE` & `phonetree-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phonetree-1.2.1/PKG-INFO` & `phonetree-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.2.1
+Version: 1.3.0
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.2.1/README.md` & `phonetree-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `phonetree-1.2.1/phonetree/phonetree.py` & `phonetree-1.3.0/phonetree/phonetree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from __future__ import annotations
 
 import inspect
 from typing import Any, Callable, Iterator, Protocol, Sequence
 
 from rapidfuzz.distance import Indel
 
-__all__ = ["menu", "Ask", "Tell"]
+__all__ = ["menu", "Ask", "Tell", "Flow"]
 
 Ask = Callable[[str], str | None]
 
 Tell = Callable[[str], None]
 
 ActionCallback = Callable[..., Any]
 
 
 class NormalizedActionCallback(Protocol):
-    def __call__(self, state: Any, ask: Ask, tell: Tell) -> Any:
+    def __call__(self, state: Any, ask: Ask, tell: Tell, flow: Flow) -> Any:
         """
         Represents a callback function with a normalized action.
 
         The method should implement a specific action to be executed given the input state and
         the methods ask and tell. The method should return any object representing the resulting
         state after the action has been taken.
 
         :param state: The current state of the application or system.
         :param ask: The method to ask questions or make requests to the user.
         :param tell: The method to send messages or information to the user.
+        :param flow: The flow object controlling the flow of the application.
         :return: The resulting state after the specific action has been taken.
         """
         ...
 
 
 def similarity(s1: str, s2: str) -> float:
     """
@@ -45,14 +46,24 @@
 
 
 class NextProtocol(Protocol):
     def next(self, state: Any, ask: Ask, tell: Tell) -> tuple[Menu | Action | None, Any]:
         ...
 
 
+class Flow:
+    """Controls the flow of the menu system."""
+
+    __slots__ = ("next",)
+
+    # noinspection PyShadowingBuiltins
+    def __init__(self, next: Menu | Action) -> None:
+        self.next = next
+
+
 class Menu(NextProtocol):
     def __init__(
         self,
         parent: Menu | None = None,
         include_exit: bool = False,
         include_exit_on_submenus: bool = False,
     ) -> None:
@@ -178,15 +189,15 @@
         :param state: The state object from previous interaction
         :param ask: The `ask` function for getting user input
         :param tell: The `tell` function for providing information to the user
         :return: A tuple with the next Menu or Action object and the updated state
         """
         # Trigger the callback if it's set
         if (callback := self.callback) is not None:
-            state = callback(state, ask, tell)
+            state = callback(state, ask, tell, Flow(self))
 
         # Display the menu options to the user
         question = "Please select an option:\n" + "\n".join(self._menu)
 
         while True:
             question_answer = ask(question)
 
@@ -239,27 +250,28 @@
         self.callback: NormalizedActionCallback | None = None
 
     def next(
         self,
         state: Any,
         ask: Ask,
         tell: Tell,
-    ) -> tuple[Menu, Any]:
+    ) -> tuple[Menu | Action, Any]:
         """
         Executes the action callback and provides a next menu and updated state.
 
         :param state: The current state of the menu system.
         :param ask: An instance of the Ask object used for questions to the user.
         :param tell: An instance of the Tell object used to communicate information to
             the user.
         :return: A tuple containing the next menu object and the updated state.
         """
+        flow = Flow(self.parent)
         if (callback := self.callback) is not None:
-            state = callback(state, ask=ask, tell=tell)
-        return self.parent, state
+            state = callback(state, ask=ask, tell=tell, flow=flow)
+        return flow.next, state
 
     def __call__(self, callback: ActionCallback) -> Action:
         """
         Sets the action callback for this action.
 
         :param callback: The function to be called during action execution.
         :return: The updated action with the new callback.
@@ -267,49 +279,44 @@
         # Normalize the callback if it is not None, otherwise set it to None
         self.callback = normalize_callback(callback) if callback is not None else None
         return self
 
 
 def normalize_callback(callback: ActionCallback) -> NormalizedActionCallback:
     """
-    Normalize a given callback function to have `state`, `ask`, and `tell` as parameters. The
-    given callback may have fewer parameters (e.g. only `state`, only `ask`, etc.).
+    Normalize a given callback function to have `state`, `ask`, `tell`, and `flow` as arguments. The
+    given callback may have only `state` as positional argument and `ask`, `tell` and `action` as keyword arguments.
 
     :param callback: The callback function to normalize.
-    :return: The normalized callback function, accepting `state`, `ask`, and `tell` as parameters.
-    :raises ValueError: If the given callback function has an unsupported number of parameters or
+    :return: The normalized callback function, accepting `state`, `ask`, `tell`, and 'action' as arguments.
+    :raises ValueError: If the given callback function has unsupported number of arguments or
         an invalid signature.
     """
     signature = inspect.signature(callback)
     parameters = signature.parameters
-    if len(parameters) == 3:
-        # Case when the callback already has the correct signature
-        return callback
-    elif len(parameters) == 2:
-        # Case when the callback has 2 parameters, we need to find which parameters are present
-        if "ask" in parameters and "tell" not in parameters:
-            # def callback(state: Any, ask: Ask) -> Any:
-            return lambda state, ask, tell: callback(state, ask=ask)
-        elif "ask" not in parameters and "tell" in parameters:
-            # def callback(state: Any, tell: Tell) -> Any:
-            return lambda state, ask, tell: callback(state, tell=tell)
-        elif "ask" in parameters and "tell" in parameters:
-            # def callback(ask: Ask, tell: Tell) -> Any:
-            return lambda state, ask, tell: callback(ask=ask, tell=tell)
-        else:
-            raise ValueError("wrong callback signature")
-    elif len(parameters) == 1:
-        # Case when the callback has 1 parameter, we need to find which parameter is present
-        if "ask" in parameters:
-            # def callback(ask: Ask) -> Any:
-            return lambda state, ask, tell: callback(ask=ask)
-        elif "tell" in parameters:
-            # def callback(tell: Tell) -> Any:
-            return lambda state, ask, tell: callback(tell=tell)
-        else:
-            # def callback(state: Any) -> Any:
-            return lambda state, ask, tell: callback(state)
-    elif len(parameters) == 0:
-        # Case when the callback has no parameters, we provide a lambda version with parameters
-        return lambda state, ask, tell: callback()
+    kwargs = []
+
+    params = list(parameters.keys())
+
+    if len(params) > 0 and params[0] not in ("ask", "tell", "flow"):
+        params.pop(0)
+        hasState = True
     else:
-        raise ValueError("wrong callback signature")
+        hasState = False
+
+    while params:
+        param = params.pop(0)
+        if param not in ("ask", "tell", "flow"):
+            raise ValueError("Unsupported argument in callback function: {}".format(param))
+        kwargs.append(param)
+
+    def normalized_callback(state: Any, ask: Ask, tell: Tell, flow: Flow) -> Any:
+        callbackLocals = locals()
+        return callback(
+            *((state,) if hasState else ()),
+            **{k: callbackLocals[k] for k in kwargs},
+        )
+
+    normalized_callback.__name__ = callback.__name__
+    normalized_callback.__doc__ = callback.__doc__
+
+    return normalized_callback
```

### Comparing `phonetree-1.2.1/phonetree.egg-info/PKG-INFO` & `phonetree-1.3.0/phonetree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.2.1
+Version: 1.3.0
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.2.1/pyproject.toml` & `phonetree-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phonetree"
-version = "1.2.1"
+version = "1.3.0"
 authors = [
   { name="Leandro Lima", email="leandro@lls-software.com" },
 ]
 description = "A phone-tree like menu system for text-based interfaces"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

