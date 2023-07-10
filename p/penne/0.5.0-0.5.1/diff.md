# Comparing `tmp/penne-0.5.0.tar.gz` & `tmp/penne-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penne-0.5.0.tar", last modified: Wed Jun  7 21:24:46 2023, max compression
+gzip compressed data, was "penne-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `penne-0.5.0.tar` & `penne-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,7 @@
--rw-r--r--   0        0        0     2854 2023-06-01 20:08:41.865752 penne-0.5.0/.github/workflows/continuous_integration.yml
--rw-r--r--   0        0        0     1421 2023-06-01 20:08:41.866554 penne-0.5.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1047 2023-06-01 20:08:41.867485 penne-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1084 2023-06-01 20:08:41.868117 penne-0.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3190 2023-06-01 20:08:41.868765 penne-0.5.0/.gitignore
--rw-r--r--   0        0        0     1101 2022-07-26 21:32:06.694759 penne-0.5.0/LICENSE
--rw-r--r--   0        0        0     7539 2023-06-07 18:52:37.200651 penne-0.5.0/README.md
--rw-r--r--   0        0        0      564 2023-06-07 21:24:43.063336 penne-0.5.0/penne/__init__.py
--rw-r--r--   0        0        0    12279 2023-06-07 21:14:41.758639 penne-0.5.0/penne/core.py
--rw-r--r--   0        0        0    29166 2023-06-07 18:06:30.561762 penne-0.5.0/penne/delegates.py
--rw-r--r--   0        0        0     4575 2023-06-07 21:14:41.735989 penne-0.5.0/penne/handlers.py
--rw-r--r--   0        0        0      737 2023-06-01 20:08:41.873575 penne-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-06 00:39:00.685439 penne-0.5.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-04-28 16:49:33.574552 penne-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     6590 2023-06-07 18:44:56.624565 penne-0.5.0/tests/clients.py
--rw-r--r--   0        0        0     2562 2023-06-07 17:29:34.352182 penne-0.5.0/tests/plottyn_integration.py
--rw-r--r--   0        0        0      393 2023-06-01 20:08:41.878884 penne-0.5.0/tests/server_conformance.py
--rw-r--r--   0        0        0     9951 2023-06-06 18:39:21.774324 penne-0.5.0/tests/servers.py
--rw-r--r--   0        0        0     5600 2023-06-07 21:14:41.753887 penne-0.5.0/tests/test_core.py
--rw-r--r--   0        0        0     9994 2023-06-07 20:52:06.090169 penne-0.5.0/tests/test_delegates.py
--rw-r--r--   0        0        0     2117 2023-06-07 15:49:58.585778 penne-0.5.0/tests/test_handlers.py
--rw-r--r--   0        0        0     8274 1970-01-01 00:00:00.000000 penne-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1550 2023-07-10 17:15:24.171165 penne-0.5.1/README.md
+-rw-r--r--   0        0        0      564 2023-07-10 17:15:24.347167 penne-0.5.1/penne/__init__.py
+-rw-r--r--   0        0        0    12998 2023-07-10 17:15:24.347167 penne-0.5.1/penne/core.py
+-rw-r--r--   0        0        0    44214 2023-07-10 17:15:24.347167 penne-0.5.1/penne/delegates.py
+-rw-r--r--   0        0        0     4581 2023-07-10 17:15:24.351167 penne-0.5.1/penne/handlers.py
+-rw-r--r--   0        0        0      893 2023-07-10 17:15:24.351167 penne-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 penne-0.5.1/PKG-INFO
```

### Comparing `penne-0.5.0/penne/__init__.py` & `penne-0.5.1/penne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 Modules:
     core.py
     test_delegates.py
     handlers.py
     messages.py
 """
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 # Imports for easier user access
 from .core import Client
 from .delegates import *
```

### Comparing `penne-0.5.0/penne/core.py` & `penne-0.5.1/penne/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,40 +52,40 @@
         _current_invoke (str):
             id for next method invoke
         callback_map (dict):
             mapping invoke_id to callback function
     """
 
     def __init__(self, url: str, custom_delegate_hash: dict[Type[delegates.Delegate], Type[delegates.Delegate]] = None,
-                 on_connected=None, strict=False, json=False):
+                 on_connected=None, strict=False, json=None):
         """Constructor for the Client Class
 
         Args:
             url (string):
                 address used to connect to server
             custom_delegate_hash (dict):
                 map for new delegates to be used on client
             on_connected (Callable):
                 callback function to run once client is set up
             strict (bool):
                 flag for strict data validation and throwing hard exceptions
-            json (bool):
-                flag for outputting json log of messages
+            json (str):
+                path for outputting json log of messages
         """
 
         if not custom_delegate_hash:
             custom_delegate_hash = {}
 
         self._url = url
         self._loop = asyncio.new_event_loop()
         self.on_connected = on_connected
         self.delegates = delegates.default_delegates.copy()
         self.strict = strict
         self.json = json
-        self.thread = threading.Thread(target=self.start_communication_thread)
+        self.thread = threading.Thread(target=self._start_communication_thread)
         self.connection_established = threading.Event()
         self._socket = None
         self.name = "Python Client"
         self.state = {}
         self.client_message_map = {
             "intro": 0,
             "invoke": 1
@@ -153,70 +153,83 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Exit method for context manager"""
         self.shutdown()
         self.is_active = False
 
-    def start_communication_thread(self):
+    def _start_communication_thread(self):
         """Starts the communication thread for the client"""
         try:
             asyncio.set_event_loop(self._loop)
-            self._loop.run_until_complete(self.run())
+            self._loop.run_until_complete(self._run())
         except Exception as e:
             self.is_active = False
             logging.warning(f"Connection terminated in communication thread: {e}")
 
     def get_delegate_id(self, name: str) -> Type[delegates.ID]:
-        """Get a delegate's id from its name
+        """Get a delegate's id from its name. Assumes names are unique, or returns the first match
 
         Args:
             name (str): name of method
 
         Returns:
-            ID group attached to the method, note this is just the first match if names are not unique
+            ID (ID): ID for the delegate
 
         Raises:
-            Couldn't find method exception
+            KeyError: if no match is found
         """
         if name == "document":
             return name
 
         state_delegates = self.state.values()
         for delegate in state_delegates:
             if delegate.name == name:
                 return delegate.id
         raise KeyError(f"Couldn't find object '{name}' in state")
 
     def get_delegate(self, identifier: Union[delegates.ID, str, Dict[str, delegates.ID]]) -> Type[delegates.Delegate]:
         """Getter to easily retrieve components from state
 
+        Accepts multiple types of identifiers for flexibility
+
         Args:
-            identifier (ID | Name | Context): id, name, or context for the component
+            identifier (ID | str | dict): id, name, or context for the component
 
         Returns:
-            Component delegate from state
+            Delegate (Delegate): delegate object from state
+
+        Raises:
+            TypeError: if identifier is not a valid type
+            KeyError: if id or name is not found in state
+            ValueError: if context is not found in state
         """
         if isinstance(identifier, delegates.ID):
             return self.state[identifier]
         elif isinstance(identifier, str):
             return self.state[self.get_delegate_id(identifier)]
         elif isinstance(identifier, dict):
             return self.get_delegate_by_context(identifier)
         else:
             raise TypeError(f"Invalid type for identifier: {type(identifier)}")
 
     def get_delegate_by_context(self, context: dict = None) -> delegates.Delegate:
-        """Get delegate object from a context message object
+        """Get delegate object from a context object
+
+        Contexts are of the form {"table": TableID}, {"entity": EntityID}, or {"plot": PlotID}.
+        They are only applicable for tables, entities, and plots
 
         Args:
-            context (Message): object containing context
+            context (dict): dict containing context
+
+        Returns:
+            Delegate (Delegate): delegate object from state
 
         Raises:
-            Exception: Couldn't get delegate from context
+            ValueError: Couldn't get delegate from context
         """
 
         if not context:
             target_delegate = self.state["document"]
             return target_delegate
 
         table = context.get("table")
@@ -226,41 +239,44 @@
         if table:
             target_delegate = self.state[delegates.TableID(*table)]
         elif entity:
             target_delegate = self.state[delegates.EntityID(*entity)]
         elif plot:
             target_delegate = self.state[delegates.PlotID(*plot)]
         else:
-            raise Exception("Couldn't get delegate from context")
+            raise ValueError("Couldn't get delegate from context")
 
         return target_delegate
 
-    def invoke_method(self, method: delegates.MethodID | str, args: list = None,
+    def invoke_method(self, method: Union[delegates.MethodID, str], args: list = None,
                       context: dict[str, tuple] = None, on_done=None):
         """Invoke method on server
 
         Constructs a dictionary of arguments to use in send_message. The
         Dictionary follows the structure of an InvokeMethodMessage, but
         using a dictionary prevents from converting back and forth just
         before sending.
 
         Also implements callback functions attached to each invocation. By
         default, each invocation will store a None object in the callback
         map, and the handler responsible for reply messages will delete pop
         it from the map and call the method if there is one
 
         Args:
-            method (list or str):
+            method (ID | str):
                 id or name for method
             args (list): 
                 arguments for method
             context (dict): 
                 optional, target context for method call
-            on_done (function):
+            on_done (Callable):
                 function to be called upon response
+
+        Returns:
+            message (list): message to be sent to server in the form of [tag, {content}]
         """
 
         # Handle default args
         if not args:
             args = []
         
         # Get proper ID
@@ -298,15 +314,15 @@
         # Construct message with ID from map and converted message object
         message = [self.client_message_map[kind], message_dict]
         logging.debug(f"Sending Message: {message}")
         
         asyncio.run_coroutine_threadsafe(self._socket.send(dumps(message)), self._loop)
         return message
 
-    def process_message(self, message):
+    def _process_message(self, message):
         """Prep message for handling
 
         Messages here are of form: [tag, {content}, tag, {content}, ...]
         """
 
         content = iter(message)
         for tag in content:
@@ -314,15 +330,15 @@
                 handlers.handle(self, tag, next(content))
             except Exception as e:
                 if self.strict:
                     raise e
                 else:
                     logging.error(f"Exception: {e} for message {message}")
 
-    async def run(self):
+    async def _run(self):
         """Network thread for managing websocket connection"""  
 
         async with websockets.connect(self._url) as websocket:
 
             # update class
             self._socket = websocket
             self.name = f"Python Client @ {self._url}"
@@ -331,21 +347,24 @@
             # send intro message
             intro = {"client_name": self.name}
             self.send_message(intro, "intro")
 
             # decode and handle all incoming messages
             async for message in self._socket:
                 message = loads(message)
-                self.process_message(message)
+                self._process_message(message)
 
     def show_methods(self):
-        """Displays Available Methods to the User"""
+        """Displays Available Methods to the User on the document
+
+        Uses the document delegate's show_methods function to display
+        """
         self.state["document"].show_methods()
 
     def shutdown(self):
         """Method for shutting down the client
         
-        Closes websocket connection then blocks to finish all callbacks
+        Closes websocket connection then blocks to finish all callbacks, joins thread as well
         """
         asyncio.run_coroutine_threadsafe(self._socket.close(), self._loop)
         self.is_active = False
         self.thread.join()
```

### Comparing `penne-0.5.0/penne/delegates.py` & `penne-0.5.1/penne/delegates.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,46 +3,49 @@
 Follows the specification in the cddl document, and
 implements strict validation
 """
 
 from __future__ import annotations
 
 import logging
-from typing import Optional, Any, Union, Callable, List, Tuple, NamedTuple
+from typing import Optional, Any, Callable, List, Tuple, NamedTuple
 from enum import Enum
 from math import pi
 
-from pydantic import BaseModel, root_validator, Extra, validator, Field
-from pydantic.color import Color
+from pydantic import ConfigDict, BaseModel, model_validator, field_validator
+from pydantic_extra_types.color import Color
 
 
 class InjectedMethod(object):
-    """Class for representing injected method in delegate, context automatically set
+    """Class for representing injected method in delegate
+
+    The context is automatically set when invoked. This object is callable and is what is actually called when the
+    injected method is called.
 
     Attributes:
-        method (method): method to be called
-        injected (bool): attribute marking method as injected
+        method (Callable): method to be called
+        injected (bool): attribute marking method as injected, useful for clearing out old injected methods
     """
 
     def __init__(self, method_obj) -> None:
         self.method = method_obj
         self.injected = True
 
     def __call__(self, *args, **kwargs):
         self.method(*args, **kwargs)
 
 
 class LinkedMethod(object):
     """Class linking target delegate and method's delegate
 
-    make a cleaner function call in injected method, it's like setting the context automatically
+    Make a cleaner function call in injected method, it's like setting the context automatically
     This is what actually gets called for the injected method
 
     Attributes:
-        _obj_delegate (delegate):
+        _obj_delegate (Delegate):
             delegate method is being linked to
         _method_delegate (MethodDelegate):
             the method's delegate
     """
 
     def __init__(self, object_delegate: Delegate, method_delegate: Method):
         self._obj_delegate = object_delegate
@@ -51,31 +54,38 @@
     def __call__(self, on_done=None, *arguments):
         self._method_delegate.invoke(self._obj_delegate, list(arguments), callback=on_done)
 
 
 def inject_methods(delegate: Delegate, methods: List[MethodID]):
     """Inject methods into a delegate class
 
-    Idea is to inject a method that is from the server to put int into a delegate.
+    Idea is to inject a method that is from the server to put into a delegate.
     Now it looks like the delegate has an instance method that actually calls what
-    is on the server. Context, is automatically taken care of by the linked method
+    is on the server. Context, is automatically taken care of. This should mostly be
+    called on_new or on_update for delegates that have methods. This method clears out any
+    old injected methods if present.
 
     Args:
         delegate (Delegate):
             identifier for delegate to be modified
         methods (list):
             list of method id's to inject
     """
 
     # Clear out old injected methods
     to_remove = []
     for field, value in delegate:
         if hasattr(value, "injected"):
             logging.debug(f"Deleting: {field} in inject methods")
             to_remove.append(field)
+    # Hack for now: waiting on https://github.com/pydantic/pydantic/issues/6560
+    for field, value in delegate.__pydantic_extra__.items():
+        if hasattr(value, "injected"):
+            logging.debug(f"Deleting: {field} in inject methods")
+            to_remove.append(field)
     for field in to_remove:
         delattr(delegate, field)
 
     for method_id in methods:
 
         # Get method delegate and manipulate name to exclude noo::
         method = delegate.client.get_delegate(method_id)
@@ -90,28 +100,39 @@
 
         setattr(delegate, name, injected)
 
 
 def inject_signals(delegate: Delegate, signals: List[SignalID]):
     """Method to inject signals into delegate
 
+    Idea is to inject a signal that is from the server to put into a delegate. These signals are stored in a dict
+    that can be used to map the signal name to a callable response that handles the signal and its args.
+
     Args:
-        delegate (delegate):
+        delegate (Delegate):
             delegate object to be injected
         signals (list):
             list of signal id's to be injected
     """
 
     for signal_id in signals:
         signal = delegate.client.state[signal_id]  # refactored state
         delegate.signals[signal.name] = None
 
 
-def get_context(delegate):
-    """Helper to get context from delegate"""
+def get_context(delegate: Delegate):
+    """Helper to get context from delegate
+
+    Args:
+        delegate (Delegate): delegate to get context for, can be Entity, Table, or Plot
+
+    Returns:
+        context (dict): context for delegate, None if not found indicating document
+
+    """
 
     if isinstance(delegate, Entity):
         return {"entity": delegate.id}
     elif isinstance(delegate, Table):
         return {"table": delegate.id}
     elif isinstance(delegate, Plot):
         return {"plot": delegate.id}
@@ -119,14 +140,26 @@
         return None
 
 
 """ =============================== ID's ============================= """
 
 
 class ID(NamedTuple):
+    """Base class for all ID's
+
+    Each ID is composed of a slot and a generation, resulting in a tuple like id ex. (0, 0). Both are positive
+    integers that are filled in increasing order. Slots are taken first, but once the slot is freed, it can be used
+    with a new generation. For example, a method is created -> (0, 0), then another is created -> (1, 0), then method
+    (0, 0) is deleted. Now, the next method created will be (0, 1).
+
+    Attributes:
+        slot (int): Slot of the ID
+        gen (int): Generation of the ID
+    """
+
     slot: int
     gen: int
 
     def compact_str(self):
         return f"|{self.slot}/{self.gen}|"
 
     def __str__(self):
@@ -145,87 +178,94 @@
         return not self.__eq__(other)
 
     def __hash__(self):
         return hash(self.__key())
 
 
 class MethodID(ID):
+    """ID specific to methods"""
     pass
 
 
 class SignalID(ID):
+    """ID specific to signals"""
     pass
 
 
 class EntityID(ID):
+    """ID specific to entities"""
     pass
 
 
 class PlotID(ID):
+    """ID specific to plots"""
     pass
 
 
 class BufferID(ID):
+    """ID specific to buffers"""
     pass
 
 
 class BufferViewID(ID):
+    """ID specific to buffer views"""
     pass
 
 
 class MaterialID(ID):
+    """ID specific to materials"""
     pass
 
 
 class ImageID(ID):
+    """ID specific to images"""
     pass
 
 
 class TextureID(ID):
+    """ID specific to textures"""
     pass
 
 
 class SamplerID(ID):
+    """ID specific to samplers"""
     pass
 
 
 class LightID(ID):
+    """ID specific to lights"""
     pass
 
 
 class GeometryID(ID):
+    """ID specific to geometries"""
     pass
 
 
 class TableID(ID):
+    """ID specific to tables"""
     pass
 
 
 """ ====================== Generic Parent Class ====================== """
 
 
 class NoodleObject(BaseModel):
     """Parent Class for all noodle objects"""
-
-    class Config:
-        """Configuration for Validation"""
-
-        arbitrary_types_allowed = True
-        use_enum_values = True
-        extra = Extra.allow  # Allow injected methods
+    model_config = ConfigDict(arbitrary_types_allowed=True, use_enum_values=True, extra="allow", frozen=False)
 
 
 class Delegate(NoodleObject):
     """Parent class for all delegates
     
     Defines general methods that should be available for all delegates
     
     Attributes:
         client (Client): Client delegate is attached to
-        id: (ID): Unique identifier for delegate
+        id (ID): Unique identifier for delegate
         name (str): Name of delegate
         signals (dict): Signals that can be called on delegate, method name to callable
     """
 
     client: object = None
     id: ID = None
     name: Optional[str] = "No-Name"
@@ -245,268 +285,455 @@
     # For all except Document Delegate
     def on_remove(self, message: dict):
         pass
 
 
 """ ====================== Common Definitions ====================== """
 
-Vec3 = Tuple[float, float, float]
-Vec4 = Tuple[float, float, float, float]
-Mat3 = Tuple[float, float, float,
-             float, float, float,
-             float, float, float]
-Mat4 = Tuple[float, float, float, float,
-             float, float, float, float,
-             float, float, float, float,
-             float, float, float, float]
+Vec3 = List[float]  # Length 3
+Vec4 = List[float]  # Length 4
+Mat3 = List[float]  # Length 9
+Mat4 = List[float]  # Length 16
 
 
 class AttributeSemantic(Enum):
+    """String indicating type of attribute, used in Attribute inside of geometry patch
+
+    Takes value of either POSITION, NORMAL, TANGENT, TEXTURE, or COLOR
+    """
     position = "POSITION"
     normal = "NORMAL"
     tangent = "TANGENT"
     texture = "TEXTURE"
     color = "COLOR"
 
 
 class Format(Enum):
+    """String indicating format of byte data for an attribute
+
+    Used in Attribute inside of geometry patch. Takes value of either U8, U16, U32, U8VEC4, U16VEC2,
+    VEC2, VEC3, VEC4, MAT3, or MAT4
+    """
+
     u8 = "U8"
     u16 = "U16"
     u32 = "U32"
     u8vec4 = "U8VEC4"
     u16vec2 = "U16VEC2"
     vec2 = "VEC2"
     vec3 = "VEC3"
     vec4 = "VEC4"
     mat3 = "MAT3"
     mat4 = "MAT4"
 
 
 class IndexFormat(str, Enum):
+    """String indicating format of byte data for an index
+
+   Used in Index inside of geometry patch. Takes value of either U8, U16, or U32
+   """
     u8 = "U8"
     u16 = "U16"
     u32 = "U32"
 
 
 class PrimitiveType(Enum):
+    """String indicating type of primitive used in a geometry patch
+
+    Takes value of either POINTS, LINES, LINE_LOOP, LINE_STRIP, TRIANGLES, or TRIANGLE_STRIP
+    """
     points = "POINTS"
     lines = "LINES"
     line_loop = "LINE_LOOP"
     line_strip = "LINE_STRIP"
     triangles = "TRIANGLES"
     triangle_strip = "TRIANGLE_STRIP"
 
 
 class ColumnType(str, Enum):
+    """String indicating type of data stored in a column in a table
+
+    Used in TableColumnInfo inside TableInitData. Takes value of either TEXT, REAL, or INTEGER
+    """
     text = "TEXT"
     real = "REAL"
     integer = "INTEGER"
 
 
 class BufferType(str, Enum):
+    """String indicating type of data stored in a buffer
+
+    Used in BufferView. Takes value of either UNK, GEOMETRY, or IMAGE
+    """
     unknown = "UNK"
     geometry = "GEOMETRY"
     image = "IMAGE"
 
 
 class SamplerMode(Enum):
+    """String options for sampler mode
+
+    Used in Sampler. Takes value of either CLAMP_TO_EDGE, MIRRORED_REPEAT, or REPEAT
+    """
     clamp_to_edge = "CLAMP_TO_EDGE"
     mirrored_repeat = "MIRRORED_REPEAT"
     repeat = "REPEAT"
 
 
 class MagFilterTypes(Enum):
+    """Options for magnification filter type
+
+    Used in Sampler. Takes value of either NEAREST or LINEAR
+    """
     nearest = "NEAREST"
     linear = "LINEAR"
 
 
 class MinFilterTypes(Enum):
+    """Options for minification filter type
+
+    Used in Sampler. Takes value of either NEAREST, LINEAR, or LINEAR_MIPMAP_LINEAR
+    """
     nearest = "NEAREST"
     linear = "LINEAR"
     linear_mipmap_linear = "LINEAR_MIPMAP_LINEAR"
 
 
 class SelectionRange(NoodleObject):
+    """Range of rows to select in a table
+
+    Attributes:
+        key_from_inclusive (int): First row to select
+        key_to_exclusive (int): Where to end selection, exclusive
+    """
     key_from_inclusive: int
     key_to_exclusive: int
 
 
 class Selection(NoodleObject):
+    """Selection of rows in a table
+
+    Attributes:
+        name (str): Name of selection
+        rows (List[int]): List of rows to select
+        row_ranges (List[SelectionRange]): List of ranges of rows to select
+    """
     name: str
     rows: Optional[List[int]] = None
     row_ranges: Optional[List[SelectionRange]] = None
 
 
 class MethodArg(NoodleObject):
+    """Argument for a method
+
+    Attributes:
+        name (str): Name of argument
+        doc (str): Documentation for argument
+        editor_hint (str): Hint for editor, refer to message spec for hint options
+    """
     name: str
     doc: Optional[str] = None
     editor_hint: Optional[str] = None
 
 
 class BoundingBox(NoodleObject):
+    """Axis-aligned bounding box
+
+    Attributes:
+        min (Vec3): Minimum point of bounding box
+        max (Vec3): Maximum point of bounding box
+    """
     min: Vec3
     max: Vec3
 
 
 class TextRepresentation(NoodleObject):
+    """Text representation for an entity
+
+    Attributes:
+        txt (str): Text to display
+        font (str): Font to use
+        height (Optional[float]): Height of text
+        width (Optional[float]): Width of text
+    """
     txt: str
     font: Optional[str] = "Arial"
     height: Optional[float] = .25
     width: Optional[float] = -1.0
 
 
 class WebRepresentation(NoodleObject):
+    """Web page with a given URL rendered as a plane
+
+    Attributes:
+        source (str): URL for entity
+        height (Optional[float]): Height of plane
+        width (Optional[float]): Width of plane
+    """
     source: str
     height: Optional[float] = .5
     width: Optional[float] = .5
 
 
 class InstanceSource(NoodleObject):
-    view: BufferViewID  # view of mat4
+    """Source of instances for a geometry patch
+
+    Attributes:
+        view (BufferViewID): View of mat4
+        stride (int): Stride for buffer
+        bb (BoundingBox): Bounding box of instances
+    """
+    view: BufferViewID
     stride: int
     bb: Optional[BoundingBox] = None
 
 
 class RenderRepresentation(NoodleObject):
+    """Render representation for an entity
+
+   Attributes:
+       mesh (GeometryID): Mesh to render
+       instances (Optional[InstanceSource]): Source of instances for mesh
+   """
     mesh: GeometryID
     instances: Optional[InstanceSource] = None
 
 
 class TextureRef(NoodleObject):
+    """Reference to a texture
+
+    Attributes:
+        texture (TextureID): Texture to reference
+        transform (Optional[Mat3]): Transform to apply to texture
+        texture_coord_slot (Optional[int]): Texture coordinate slot to use
+    """
     texture: TextureID
     transform: Optional[Mat3] = [1.0, 0.0, 0.0,
                                  0.0, 1.0, 0.0,
                                  0.0, 0.0, 1.0]
     texture_coord_slot: Optional[int] = 0.0
 
 
 class PBRInfo(NoodleObject):
+    """Physically based rendering information for a material
+
+   Attributes:
+       base_color (Optional[RGBA]): Base color of material
+       base_color_texture (Optional[TextureRef]): Texture to use for base color
+       metallic (Optional[float]): Metallic value of material
+       roughness (Optional[float]): Roughness value of material
+       metal_rough_texture (Optional[TextureRef]): Texture to use for metallic and roughness
+   """
     base_color: Optional[Color] = Color('white')
     base_color_texture: Optional[TextureRef] = None  # assume SRGB, no premult alpha
 
     metallic: Optional[float] = 1.0
     roughness: Optional[float] = 1.0
     metal_rough_texture: Optional[TextureRef] = None  # assume linear, ONLY RG used
 
-    @validator("base_color", pre=True, allow_reuse=True)
+    @field_validator("base_color", mode='before')
     def check_color_rgba(cls, value):
 
         # Raise warning if format is wrong from server
         if len(value) != 4:
             logging.warning(f"Base Color is Wrong Color Format: {value}")
         return value
 
 
 class PointLight(NoodleObject):
+    """Point light information for a light delegate
+
+    Attributes:
+        range (float): Range of light, -1 defaults to infinite
+    """
     range: float = -1.0
 
 
 class SpotLight(NoodleObject):
+    """Spotlight information for a light delegate
+
+    Attributes:
+        range (float): Range of light, -1 defaults to infinite
+        inner_cone_angle_rad (float): Inner cone angle of light
+        outer_cone_angle_rad (float): Outer cone angle of light
+    """
     range: float = -1.0
     inner_cone_angle_rad: float = 0.0
     outer_cone_angle_rad: float = pi/4
 
 
 class DirectionalLight(NoodleObject):
+    """Directional light information for a light delegate
+
+    Attributes:
+        range (float): Range of light, -1 defaults to infinite
+    """
     range: float = -1.0
 
 
 class Attribute(NoodleObject):
+    """Attribute for a geometry patch
+
+    Each attribute is a view into a buffer that corresponds to a specific element of the mesh
+    (e.g. position, normal, etc.). Attributes allow information for the vertices to be extracted from buffers
+
+    Attributes:
+        view (BufferViewID): View of the buffer storing the data
+        semantic (AttributeSemantic): String describing the type of attribute
+        channel (Optional[int]): Channel of attribute, if applicable
+        offset (Optional[int]): Offset into buffer
+        stride (Optional[int]): Distance, in bytes, between data for two vertices in the buffer
+        format (Format): How many bytes per element, how to decode the bytes
+        minimum_value (Optional[List[float]]): Minimum value for attribute data
+        maximum_value (Optional[List[float]]): Maximum value for attribute data
+        normalized (Optional[bool]): Whether to normalize the attribute data
+    """
     view: BufferViewID
     semantic: AttributeSemantic
     channel: Optional[int] = None
     offset: Optional[int] = 0
     stride: Optional[int] = 0
     format: Format
     minimum_value: Optional[List[float]] = None
     maximum_value: Optional[List[float]] = None
     normalized: Optional[bool] = False
 
 
 class Index(NoodleObject):
+    """Index for a geometry patch
+
+    The index is a view into a buffer that corresponds to the indices of the mesh. The index allows the mesh to
+    connect vertices and render triangles, lines, or points.
+
+    Attributes:
+        view (BufferViewID): View of the buffer storing the data
+        count (int): Number of indices
+        offset (Optional[int]): Offset into buffer
+        stride (Optional[int]): Distance, in bytes, between data for two elements in the buffer
+        format (IndexFormat): How many bytes per element, how to decode the bytes
+    """
     view: BufferViewID
     count: int
     offset: Optional[int] = 0
     stride: Optional[int] = 0
     format: IndexFormat
 
 
 class GeometryPatch(NoodleObject):
+    """Geometry patch for a mesh
+
+   Principle object used in geometry delegates. A geometry patch combines vertex data from attributes and index data
+   from indices.
+
+   Attributes:
+       attributes (List[Attribute]): List of attributes storing vertex data for the mesh
+       vertex_count (int): Number of vertices in the mesh
+       indices (Optional[Index]): Indices for the mesh
+       type (PrimitiveType): Type of primitive to render
+       material (MaterialID): Material to use for rendering
+   """
     attributes: List[Attribute]
     vertex_count: int
     indices: Optional[Index] = None
     type: PrimitiveType
     material: MaterialID  # Material ID
 
 
 class InvokeIDType(NoodleObject):
+    """Context for invoking a signal
+
+    Attributes:
+        entity (Optional[EntityID]): Entity to invoke signal on
+        table (Optional[TableID]): Table to invoke signal on
+        plot (Optional[PlotID]): Plot to invoke signal on
+    """
     entity: Optional[EntityID] = None
     table: Optional[TableID] = None
     plot: Optional[PlotID] = None
 
-    @root_validator
-    def one_of_three(cls, values):
-        already_found = False
-        for field in values:
-            if values[field] and already_found:
-                raise ValueError("More than one field entered")
-            elif values[field]:
-                already_found = True
-
-        if not already_found:
-            raise ValueError("No field provided")
-        else:
-            return values
+    @model_validator(mode="after")
+    def one_of_three(cls, model):
+        num_set = bool(model.entity) + bool(model.table) + bool(model.plot)
+        if num_set != 1:
+            raise ValueError("Must set exactly one of entity, table, or plot")
+        return model
 
 
 class TableColumnInfo(NoodleObject):
+    """Information about a column in a table
+
+    Attributes:
+        name (str): Name of column
+        type (ColumnType): Type data in the column
+    """
     name: str
     type: ColumnType
 
 
 class TableInitData(NoodleObject):
+    """Init data to create a table
+
+    Attributes:
+        columns (List[TableColumnInfo]): List of column information
+        keys (List[int]): List of column indices that are keys
+        data (List[List[Any]]): List of rows of data
+        selections (Optional[List[Selection]]): List of selections to apply to table
+    """
     columns: List[TableColumnInfo]
     keys: List[int]
     data: List[List[Any]]  # Originally tried union, but currently order is used to coerce by pydantic
     selections: Optional[List[Selection]] = None
 
     # too much overhead? - strict mode
-    @root_validator
-    def types_match(cls, values):
-        for row in values['data']:
-            for col, i in zip(values['columns'], range(len(row))):
+    @model_validator(mode="after")
+    def types_match(cls, model):
+        for row in model.data:
+            for col, i in zip(model.columns, range(len(row))):
                 text_mismatch = isinstance(row[i], str) and col.type != "TEXT"
                 real_mismatch = isinstance(row[i], float) and col.type != "REAL"
                 int_mismatch = isinstance(row[i], int) and col.type != "INTEGER"
                 if text_mismatch or real_mismatch or int_mismatch:
                     raise ValueError(f"Column Info doesn't match type in data: {col, row[i]}")
-        return values
+        return model
 
 
 """ ====================== NOODLE COMPONENTS ====================== """
 
 
 class Method(Delegate):
+    """A method that clients can request the server to call.
+
+    Attributes:
+        id: ID for the method
+        name: Name of the method
+        doc: Documentation for the method
+        return_doc: Documentation for the return value
+        arg_doc: Documentation for the arguments
+    """
+
     id: MethodID
     name: str
     doc: Optional[str] = None
     return_doc: Optional[str] = None
     arg_doc: List[MethodArg] = []
 
     def invoke(self, on_delegate: Delegate, args=None, callback=None):
         """Invoke this delegate's method
 
         Args:
-            on_delegate (delegate):
+            on_delegate (Delegate):
                 delegate method is being invoked on 
                 used to get context
             args (list, optional):
                 args for the method
             callback (function):
                 function to be called when complete
+
+        Raises:
+            ValueError: Invalid delegate context
         """
 
         if isinstance(on_delegate, Table):
             kind = "table"
         elif isinstance(on_delegate, Plot):
             kind = "plot"
         elif isinstance(on_delegate, Entity):
@@ -523,21 +750,47 @@
         rep = f"{self.name}:\n\t{self.doc}\n\tReturns: {self.return_doc}\n\tArgs:"
         for arg in self.arg_doc:
             rep += f"\n\t\t{arg.name}: {arg.doc}"
         return rep
 
 
 class Signal(Delegate):
+    """A signal that the server can send to update clients.
+
+    Attributes:
+        id: ID for the signal
+        name: Name of the signal
+        doc: Documentation for the signal
+        arg_doc: Documentation for the arguments
+    """
     id: SignalID
     name: str
     doc: Optional[str] = None
     arg_doc: List[MethodArg] = None
 
 
 class Entity(Delegate):
+    """Container for other entities, possibly renderable, has associated methods and signals
+
+    Attributes:
+        id: ID for the entity
+        name: Name of the entity
+        parent: Parent entity
+        transform: Local transform for the entity
+        text_rep: Text representation for the entity
+        web_rep: Web representation for the entity
+        render_rep: Render representation for the entity
+        lights: List of lights attached to the entity
+        tables: List of tables attached to the entity
+        plots: List of plots attached to the entity
+        tags: List of tags for the entity
+        methods_list: List of methods attached to the entity
+        signals_list: List of signals attached to the entity
+        influence: Bounding box for the entity
+    """
     id: EntityID
     name: Optional[str] = "Unnamed Entity Delegate"
 
     parent: Optional[EntityID] = None
     transform: Optional[Mat4] = None
 
     null_rep: Optional[Any] = None
@@ -566,29 +819,40 @@
                 message += f">> {method}"
 
         print(message)
         return message
 
 
 class Plot(Delegate):
+    """An abstract plot object.
+
+    Attributes:
+        id: ID for the plot
+        name: Name of the plot
+        table: Table to plot
+        simple_plot: Simple plot to render
+        url_plot: URL for plot to render
+        methods_list: List of methods attached to the plot
+        signals_list: List of signals attached to the plot
+    """
     id: PlotID
     name: Optional[str] = "Unnamed Plot Delegate"
 
     table: Optional[TableID] = None
 
     simple_plot: Optional[str] = None
     url_plot: Optional[str] = None
 
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
-    @root_validator
-    def one_of(cls, values):
-        if bool(values['simple_plot']) != bool(values['url_plot']):
-            return values
+    @model_validator(mode="after")
+    def one_of(cls, model):
+        if bool(model.simple_plot) != bool(model.url_plot):
+            return model
         else:
             raise ValueError("One plot type must be specified")
 
     def show_methods(self):
         """Show methods available on the entity"""
 
         if self.methods_list is None:
@@ -600,53 +864,89 @@
                 message += f">> {method}"
 
         print(message)
         return message
 
 
 class Buffer(Delegate):
+    """A buffer of bytes containing data for an image or a mesh.
+
+    Attributes:
+        id: ID for the buffer
+        name: Name of the buffer
+        size: Size of the buffer in bytes
+        inline_bytes: Bytes of the buffer
+        uri_bytes: URI for the bytes
+    """
     id: BufferID
     name: Optional[str] = "Unnamed Buffer Delegate"
     size: int = None
 
     inline_bytes: bytes = None
     uri_bytes: str = None
 
-    @root_validator
-    def one_of(cls, values):
-        if bool(values['inline_bytes']) != bool(values['uri_bytes']):
-            return values
+    @model_validator(mode="after")
+    def one_of(cls, model):
+        if bool(model.inline_bytes) != bool(model.uri_bytes):
+            return model
         else:
             raise ValueError("One plot type must be specified")
 
 
 class BufferView(Delegate):
+    """A view into a buffer, specifying a subset of the buffer and how to interpret it.
+
+    Attributes:
+        id: ID for the buffer view
+        name: Name of the buffer view
+        source_buffer: Buffer that the view is referring to
+        type: Type of the buffer view
+        offset: Offset into the buffer in bytes
+        length: Length of the buffer view in bytes
+    """
     id: BufferViewID
     name: Optional[str] = "Unnamed Buffer-View Delegate"
     source_buffer: BufferID
 
     type: BufferType = BufferType.unknown
     offset: int
     length: int
 
-    @validator("type", pre=True)
+    @field_validator("type", mode='before')
     def coerce_type(cls, value):
         if value in ["UNK", "GEOMETRY", "IMAGE"]:
             return value
 
-        logging.warning(f"Buffer View Type does not meet the specification: {value} coerced to 'UNK'")
         if "GEOMETRY" in value.upper():
+            logging.warning(f"Buffer View Type does not meet the specification: {value} coerced to 'GEOMETRY'")
             return "GEOMETRY"
         elif "IMAGE" in value.upper():
+            logging.warning(f"Buffer View Type does not meet the specification: {value} coerced to 'IMAGE'")
             return "IMAGE"
         else:
+            logging.warning(f"Buffer View Type does not meet the specification: {value} coerced to 'UNK'")
             return "UNK"
 
 
 class Material(Delegate):
+    """A material that can be applied to a mesh.
+
+    Attributes:
+        id: ID for the material
+        name: Name of the material
+        pbr_info: Information for physically based rendering
+        normal_texture: Texture for normals
+        occlusion_texture: Texture for occlusion
+        occlusion_texture_factor: Factor for occlusion
+        emissive_texture: Texture for emissive
+        emissive_factor: Factor for emissive
+        use_alpha: Whether to use alpha
+        alpha_cutoff: Alpha cutoff
+        double_sided: Whether the material is double-sided
+    """
     id: MaterialID
     name: Optional[str] = "Unnamed Material Delegate"
 
     pbr_info: Optional[PBRInfo] = PBRInfo()
     normal_texture: Optional[TextureRef] = None
 
     occlusion_texture: Optional[TextureRef] = None  # assumed to be linear, ONLY R used
@@ -658,111 +958,155 @@
     use_alpha: Optional[bool] = False
     alpha_cutoff: Optional[float] = .5
 
     double_sided: Optional[bool] = False
 
 
 class Image(Delegate):
+    """An image, can be used for a texture
+
+    Attributes:
+        id: ID for the image
+        name: Name of the image
+        buffer_source: Buffer that the image is stored in
+        uri_source: URI for the bytes if they are hosted externally
+    """
     id: ImageID
     name: Optional[str] = "Unnamed Image Delegate"
 
     buffer_source: BufferID = None
     uri_source: str = None
 
-    @root_validator
-    def one_of(cls, values):
-        if bool(values['buffer_source']) != bool(values['uri_source']):
-            return values
+    @model_validator(mode="after")
+    def one_of(cls, model):
+        if bool(model.buffer_source) != bool(model.uri_source):
+            return model
         else:
             raise ValueError("One plot type must be specified")
 
 
 class Texture(Delegate):
+    """A texture, can be used for a material
+
+    Attributes:
+        id: ID for the texture
+        name: Name of the texture
+        image: Image to use for the texture
+        sampler: Sampler to use for the texture
+    """
     id: TextureID
     name: Optional[str] = "Unnamed Texture Delegate"
     image: ImageID
     sampler: Optional[SamplerID] = None
 
 
 class Sampler(Delegate):
+    """A sampler to use for a texture
+
+   Attributes:
+       id: ID for the sampler
+       name: Name of the sampler
+       mag_filter: Magnification filter
+       min_filter: Minification filter
+       wrap_s: Wrap mode for S
+       wrap_t: Wrap mode for T
+   """
     id: SamplerID
     name: Optional[str] = "Unnamed Sampler Delegate"
 
     mag_filter: Optional[MagFilterTypes] = MagFilterTypes.linear
     min_filter: Optional[MinFilterTypes] = MinFilterTypes.linear_mipmap_linear
 
     wrap_s: Optional[SamplerMode] = "REPEAT"
     wrap_t: Optional[SamplerMode] = "REPEAT"
 
 
 class Light(Delegate):
+    """Represents a light in the scene
+
+    Attributes:
+        id: ID for the light
+        name: Name of the light
+        color: Color of the light
+        intensity: Intensity of the light
+        point: Point light information
+        spot: Spotlight information
+        directional: Directional light information
+    """
     id: LightID
     name: Optional[str] = "Unnamed Light Delegate"
 
     color: Optional[Color] = Color('white')
     intensity: Optional[float] = 1.0
 
     point: PointLight = None
     spot: SpotLight = None
     directional: DirectionalLight = None
 
-    @validator("color", pre=True, allow_reuse=True)
+    @field_validator("color", mode='before')
     def check_color_rgb(cls, value):
 
         # Raise warning if format is wrong
         if len(value) != 3:
             logging.warning(f"Color is not RGB in Light: {value}")
-
         return value
 
-    @root_validator
-    def one_of(cls, values):
-        already_found = False
-        for field in ['point', 'spot', 'directional']:
-            if values[field] and already_found:
-                raise ValueError("More than one field entered")
-            elif values[field]:
-                already_found = True
-
-        if not already_found:
-            raise ValueError("No field provided")
+    @model_validator(mode="after")
+    def one_of(cls, model):
+        num_selected = bool(model.point) + bool(model.spot) + bool(model.directional)
+        if num_selected > 1:
+            raise ValueError("Only one light type can be selected")
+        elif num_selected == 0:
+            raise ValueError("No light type selected")
         else:
-            return values
+            return model
 
 
 class Geometry(Delegate):
+    """Represents geometry in the scene and can be used for meshes
+
+    Attributes:
+        id: ID for the geometry
+        name: Name of the geometry
+        patches: Patches that make up the geometry
+    """
     id: GeometryID
     name: Optional[str] = "Unnamed Geometry Delegate"
     patches: List[GeometryPatch]
 
 
 class Table(Delegate):
+    """Object to store tabular data.
+
+    Attributes:
+        id: ID for the table
+        name: Name of the table
+        meta: Metadata for the table
+        methods_list: List of methods for the table
+        signals_list: List of signals for the table
+        tbl_subscribe: Injected method to subscribe to the table
+        tbl_insert: Injected method to insert rows into the table
+        tbl_update: Injected method to update rows in the table
+        tbl_remove: Injected method to remove rows from the table
+        tbl_clear: Injected method to clear the table
+        tbl_update_selection: Injected method to update the selection
+    """
     id: TableID
     name: Optional[str] = f"Unnamed Table Delegate"
 
     meta: Optional[str] = None
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
-    methods: List[str] = [
-        "subscribe",
-        "request_clear",
-        "request_insert",
-        "request_remove",
-        "request_update",
-        "request_update_selection",
-        "plot"
-    ]
-
-    tbl_subscribe: InjectedMethod = None
-    tbl_insert: InjectedMethod = None
-    tbl_update: InjectedMethod = None
-    tbl_remove: InjectedMethod = None
-    tbl_clear: InjectedMethod = None
-    tbl_update_selection: InjectedMethod = None
+    tbl_subscribe: Optional[InjectedMethod] = None
+    tbl_insert: Optional[InjectedMethod] = None
+    tbl_update: Optional[InjectedMethod] = None
+    tbl_remove: Optional[InjectedMethod] = None
+    tbl_clear: Optional[InjectedMethod] = None
+    tbl_update_selection: Optional[InjectedMethod] = None
 
     def __init__(self, **kwargs):
         """Override init to link default values with methods"""
         super().__init__(**kwargs)
         self.signals = {
             "noo::tbl_reset": self._reset_table,
             "noo::tbl_rows_removed": self._remove_rows,
@@ -832,35 +1176,35 @@
 
         self.selections.setdefault(selection["name"], selection)
         logging.info(f"Made selection {selection['name']} = {selection}")
 
     def relink_signals(self):
         """Relink the signals for built-in methods
 
-        These should always be linked, along with whatever is injected,
-        so relink on new and on update messages
+        Injecting signals adds them as keys which map to None. The signals must be relinked after injecting.
+        These should always be linked, along with whatever is injected.
         """
 
         self.signals["noo::tbl_reset"] = self._reset_table
         self.signals["noo::tbl_rows_removed"] = self._remove_rows
         self.signals["noo::tbl_updated"] = self._update_rows
         self.signals["noo::tbl_selection_updated"] = self._update_selection
 
     def on_new(self, message: dict):
         """Handler when create message is received
 
         Args:
             message (Message): create message with the table's info
         """
 
-        # Set name
+        # Check contents
         methods = self.methods_list
         signals = self.signals_list
 
-        # Inject methods and signals
+        # Inject methods and signals if applicable
         if methods:
             inject_methods(self, methods)
         if signals:
             inject_signals(self, signals)
 
         # Reset
         self._reset_table()
@@ -868,25 +1212,33 @@
 
     def on_update(self, message: dict):
         """Handler when update message is received
         
         Args:
             message (Message): update message with the new table's info
         """
+        # Check contents
+        methods = message.get("methods_list")
+        signals = message.get("signals_list")
 
+        # Inject methods and signals
+        if methods:
+            inject_methods(self, methods)
+        if signals:
+            inject_signals(self, signals)
         self.relink_signals()
 
-    def on_remove(self, message: dict):
-        pass
-
     def subscribe(self, on_done: Callable = None):
         """Subscribe to this delegate's table
 
         Calls on_table_init as callback
-        
+
+        Args:
+              on_done (Callable): function to be called after table is subscribed to and initialized
+
         Raises:
             Exception: Could not subscribe to table
         """
 
         try:
             # Allow for callback after table init
             self.tbl_subscribe(on_done=lambda data: self._on_table_init(data, on_done))
@@ -904,29 +1256,27 @@
         sx, sy, sz -> scaling factors, default size is 1 meter
 
         Row_list: [[1, 2, 3, 4, 5, 6, 7, 8, 9]]
 
         Args:
             row_list (list, optional): add rows using list of rows
             on_done (function, optional): callback function
-        Raises:
-            Invalid input for request insert exception
         """
 
         self.tbl_insert(on_done, row_list)
 
     def request_update(self, keys: List[int], rows: List[List[int]], on_done=None):
         """Update the table using a DataFrame
 
         User endpoint for interacting with table and invoking method
 
         Args:
             keys (list[int]):
                 list of keys to update
-            rows (list[list[int]])
+            rows (list[list[int]]):
                 list of new rows to update with
             on_done (function, optional): 
                 callback function called when complete
         """
 
         self.tbl_update(on_done, keys, rows)
 
@@ -964,15 +1314,15 @@
                 name of the selection object to be updated
             keys (list):
                 list of keys to be in new selection
             on_done (function, optional): 
                 callback function called when complete
         """
         selection = Selection(name=name, rows=keys)
-        self.tbl_update_selection(on_done, selection.dict())
+        self.tbl_update_selection(on_done, selection.model_dump())
 
     def show_methods(self):
         """Show methods available on the table"""
 
         if self.methods_list is None:
             message = "No methods available"
         else:
@@ -982,26 +1332,45 @@
                 message += f">> {method}"
 
         print(message)
         return message
 
 
 class Document(Delegate):
+    """Delegate for document
+
+    Attributes:
+        name (str): name will be "Document"
+        methods_list (list[MethodID]): list of methods available on the document
+        signals_list (list[SignalID]): list of signals available on the document
+    """
+
     name: str = "Document"
 
     methods_list: List[MethodID] = []  # Server usually sends as an update
     signals_list: List[SignalID] = []
 
     def on_update(self, message: dict):
+        """Handler when update message is received
+
+        Should update methods_list and signals_list
+
+        Args:
+            message (Message): update message with the new document's info
+        """
         if "methods_list" in message:
             self.methods_list = [MethodID(*element) for element in message["methods_list"]]
         if "signals_list" in message:
             self.signals_list = [SignalID(*element) for element in message["signals_list"]]
 
     def reset(self):
+        """Reset the document
+
+        Called when document reset message is received. Will reset state, and clear methods and signals on document
+        """
         self.client.state = {"document": self}
         self.methods_list = []
         self.signals_list = []
 
     def show_methods(self):
         """Show methods available on the document"""
 
@@ -1025,20 +1394,38 @@
     context: Optional[InvokeIDType] = None  # if empty - document
     signal_data: List[Any]
 
 
 # Note: this isn't technically an exception
 # for now this uses a model so that it can be validated / sent as message easier
 class MethodException(NoodleObject):
+    """Exception raised when invoking a method
+
+    Will be sent as part of a reply message
+
+    Attributes:
+        code (int): error code
+        message (str): error message
+        data (Any): data associated with the error
+    """
     code: int
     message: Optional[str] = None
     data: Optional[Any] = None
 
 
 class Reply(NoodleObject):
+    """Reply message sent from server in response to method invocation
+
+    Will either contain resulting data, or an exception
+
+    Attributes:
+        invoke_id (str): id of the invoke message that this is a reply to
+        result (Any): result of the method invocation
+        method_exception (MethodException): exception raised when invoking method
+    """
     invoke_id: str
     result: Optional[Any] = None
     method_exception: Optional[MethodException] = None
 
 
 """ ====================== Miscellaneous Objects ====================== """
```

### Comparing `penne-0.5.0/penne/handlers.py` & `penne-0.5.1/penne/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         message (Message): 
             message containing updates
         component_id (ID):
             ID of the component to be updated
     """
 
     delegate = client.get_delegate(component_id)
-    current_state = delegate.dict()
+    current_state = delegate.model_dump()
     current_state.update(message)
 
     delegate_type = type(delegate)
     client.state[component_id] = delegate_type(**current_state)
 
 
 def handle(client, message_id, message: dict[str, Any]):
```

### Comparing `penne-0.5.0/pyproject.toml` & `penne-0.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,31 +6,37 @@
 [project]
 name = "penne"
 authors = [
     {name = "Alex Racapé"},
 ]
 dynamic = ["version", "description"]
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 keywords = ["noodles", "cbor", "Websockets", "client", "NOODLES"]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Visualization"
 ]
 dependencies = [
     "websockets",
     "cbor2",
-    "pydantic"
+    "pydantic",
+    "pydantic-extra-types"
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "rigatoni",
     "pandas",
     "matplotlib"
 ]
 
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+log_cli = true
+
 [project.urls]
-Source = "https://github.com/InsightCenterNoodles/Penne"
+Source = "https://github.com/InsightCenterNoodles/Penne"
+Documentation = "https://insightcenternoodles.github.io/Penne/"
```

