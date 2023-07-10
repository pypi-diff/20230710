# Comparing `tmp/robotcode_debugger-0.46.0.tar.gz` & `tmp/robotcode_debugger-0.47.0.tar.gz`

## Comparing `robotcode_debugger-0.46.0.tar` & `robotcode_debugger-0.47.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    52858 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13755 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/README.md
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    25779 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    65073 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15579 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/README.md
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.47.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from .__version__ import __version__
 from .run import run_debugger
 
 DEBUGGER_DEFAULT_PORT = 6612
 DEBUGPY_DEFAULT_PORT = 5678
 
 
+# mypy: disable-error-code="misc, arg-type, attr-defined"
+
+
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
 )
```

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/dap_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1088,7 +1088,71 @@
 class SetExceptionBreakpointsResponseBody(Model):
     breakpoints: Optional[List[Breakpoint]] = None
 
 
 @dataclass
 class SetExceptionBreakpointsResponse(Response):
     body: Optional[SetExceptionBreakpointsResponseBody] = None
+
+
+@dataclass
+class _CompletionsRequest:
+    arguments: CompletionsArguments
+
+
+@dataclass
+class CompletionsRequest(Request, _CompletionsRequest):
+    arguments: CompletionsArguments = field()
+    command: str = "completions"
+
+
+@dataclass
+class CompletionsArguments(Model):
+    text: str
+    column: int
+    line: Optional[int] = None
+    frame_id: Optional[int] = None
+
+
+class CompletionItemType(Enum):
+    METHOD = "method"
+    FUNCTION = "function"
+    CONSTRUCTOR = "constructor"
+    FIELD = "field"
+    VARIABLE = "variable"
+    CLASS = "class"
+    INTERFACE = "interface"
+    MODULE = "module"
+    PROPERTY = "property"
+    UNIT = "unit"
+    VALUE = "value"
+    ENUM = "enum"
+    KEYWORD = "keyword"
+    SNIPPET = "snippet"
+    TEXT = "text"
+    COLOR = "color"
+    FILE = "file"
+    REFERENCE = "reference"
+    CUSTOMCOLOR = "customcolor"
+
+
+@dataclass
+class CompletionItem(Model):
+    label: str
+    text: Optional[str] = None
+    sort_text: Optional[str] = None
+    detail: Optional[str] = None
+    type: Optional[CompletionItemType] = None
+    start: Optional[int] = None
+    length: Optional[int] = None
+    selection_start: Optional[int] = None
+    selection_length: Optional[int] = None
+
+
+@dataclass
+class CompletionsResponseBody(Model):
+    targets: List[CompletionItem]
+
+
+@dataclass
+class CompletionsResponse(Response):
+    body: Optional[CompletionsResponseBody] = None
```

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/debugger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from __future__ import annotations
 
 import asyncio
 import itertools
 import os
 import pathlib
 import re
+import reprlib
 import threading
+import time
 import weakref
 from collections import deque
 from enum import Enum
 from pathlib import Path, PurePath
 from typing import (
     Any,
     Callable,
     ClassVar,
     Deque,
     Dict,
     Iterator,
     List,
     Literal,
+    Mapping,
     NamedTuple,
     Optional,
+    Sequence,
     Set,
     Tuple,
     Union,
 )
 
 from robot.api.parsing import get_model
 from robot.errors import VariableError
@@ -35,14 +39,16 @@
 from robot.variables import evaluate_expression
 from robotcode.core.event import event
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.robot.utils import get_robot_version
 
 from .dap_types import (
     Breakpoint,
+    CompletionItem,
+    CompletionItemType,
     ContinuedEvent,
     ContinuedEventBody,
     EvaluateArgumentContext,
     Event,
     ExceptionFilterOptions,
     ExceptionOptions,
     OutputCategory,
@@ -113,14 +119,15 @@
 
 class RequestedState(Enum):
     Nothing = 0
     Pause = 1
     Next = 2
     StepIn = 3
     StepOut = 4
+    Running = 5
 
 
 class BreakpointsEntry(NamedTuple):
     breakpoints: Tuple[SourceBreakpoint, ...]
     lines: Tuple[int, ...]
 
 
@@ -208,14 +215,25 @@
 
 
 class PathMapping(NamedTuple):
     local_root: Optional[str]
     remote_root: Optional[str]
 
 
+class DebugLogger:
+    def __init__(self) -> None:
+        self.steps: List[Any] = []
+
+    def start_keyword(self, kw: Any) -> None:
+        self.steps.append(kw)
+
+    def end_keyword(self, kw: Any) -> None:
+        self.steps.pop()
+
+
 class Debugger:
     __instance: ClassVar[Optional[Debugger]] = None
     __lock: ClassVar = threading.RLock()
     __inside_instance: ClassVar = False
 
     _logger = LoggingDescriptor()
 
@@ -249,15 +267,15 @@
             ExceptionBreakpointsEntry((), (ExceptionFilterOptions("uncaught_failed_keyword"),), ())
         )
 
         self.main_thread: Optional[threading.Thread] = None
         self.full_stack_frames: Deque[StackFrameEntry] = deque()
         self.stack_frames: Deque[StackFrameEntry] = deque()
         self.condition = threading.Condition()
-        self.state: State = State.Stopped
+        self._state: State = State.Stopped
         self.requested_state: RequestedState = RequestedState.Nothing
         self.stop_stack_len = 0
         self._robot_report_file: Optional[str] = None
         self._robot_log_file: Optional[str] = None
         self._robot_output_file: Optional[str] = None
         self.output_messages: bool = False
         self.output_log: bool = False
@@ -277,14 +295,37 @@
         self._evaluated_keyword_result: Any = None
         self._evaluate_keyword_event = threading.Event()
         self._evaluate_keyword_event.set()
         self._after_evaluate_keyword_event = threading.Event()
         self._after_evaluate_keyword_event.set()
         self.expression_mode = False
 
+        self.debug_logger: Optional[DebugLogger] = None
+        self.run_started = False
+        self._evaluate_cache: List[Any] = []
+        self._variables_cache: Dict[int, Any] = {}
+        self._variables_object_cache: List[Any] = []
+
+    @property
+    def state(self) -> State:
+        return self._state
+
+    @state.setter
+    def state(self, value: State) -> None:
+        # if state is changed, do nothing and wait a little bit to avoid busy loop
+
+        if self._state == State.Paused and value not in [State.Paused, State.CallKeyword]:
+            self._variables_cache.clear()
+            self._variables_object_cache.clear()
+            self._evaluate_cache.clear()
+
+        time.sleep(0.01)
+
+        self._state = value
+
     @property
     def debug(self) -> bool:
         return self._debug
 
     @debug.setter
     def debug(self, value: bool) -> None:
         self._debug = value
@@ -334,52 +375,40 @@
                     ContinuedEvent(
                         body=ContinuedEventBody(thread_id=self.main_thread.ident, all_threads_continued=True)
                     ),
                 )
 
             self.condition.notify_all()
 
-    def continue_all(self, send_event: bool = True) -> None:
+    def continue_all(self) -> None:
         if self.main_thread is not None and self.main_thread.ident is not None:
-            self.continue_thread(self.main_thread.ident, send_event)
+            self.continue_thread(self.main_thread.ident)
 
-    def continue_thread(self, thread_id: int, send_event: bool = False) -> None:
+    def continue_thread(self, thread_id: int) -> None:
         if self.main_thread is None or thread_id != self.main_thread.ident:
             raise InvalidThreadIdError(thread_id)
 
         with self.condition:
-            if send_event:
-                self.send_event(
-                    self,
-                    ContinuedEvent(
-                        body=ContinuedEventBody(thread_id=self.main_thread.ident, all_threads_continued=True)
-                    ),
-                )
-
-            self.requested_state = RequestedState.Nothing
-            self.state = State.Running
+            self.requested_state = RequestedState.Running
             self.condition.notify_all()
 
     def pause_thread(self, thread_id: int) -> None:
         if self.main_thread is None or thread_id != self.main_thread.ident:
             raise InvalidThreadIdError(thread_id)
 
         with self.condition:
             self.requested_state = RequestedState.Pause
-            self.state = State.Paused
 
             self.condition.notify_all()
 
     def next(self, thread_id: int, granularity: Optional[SteppingGranularity] = None) -> None:
         if self.main_thread is None or thread_id != self.main_thread.ident:
             raise InvalidThreadIdError(thread_id)
 
         with self.condition:
-            self.state = State.Running
-
             if self.full_stack_frames and self.full_stack_frames[0].type in ["TEST", "SUITE"]:
                 self.requested_state = RequestedState.StepIn
             else:
                 self.requested_state = RequestedState.Next
 
                 self.stop_stack_len = len(self.full_stack_frames)
                 if self.full_stack_frames and self.full_stack_frames[0].type in [
@@ -402,25 +431,23 @@
         self, thread_id: int, target_id: Optional[int] = None, granularity: Optional[SteppingGranularity] = None
     ) -> None:
         if self.main_thread is None or thread_id != self.main_thread.ident:
             raise InvalidThreadIdError(thread_id)
 
         with self.condition:
             self.requested_state = RequestedState.StepIn
-            self.state = State.Running
 
             self.condition.notify_all()
 
     def step_out(self, thread_id: int, granularity: Optional[SteppingGranularity] = None) -> None:
         if self.main_thread is None or thread_id != self.main_thread.ident:
             raise InvalidThreadIdError(thread_id)
 
         with self.condition:
             self.requested_state = RequestedState.StepOut
-            self.state = State.Running
             self.stop_stack_len = len(self.full_stack_frames) - 1
 
             i = 1
 
             while i < len(self.full_stack_frames) and self.full_stack_frames[i].type in [
                 "FOR",
                 "FOR ITERATION",
@@ -470,62 +497,69 @@
         return []
 
     def process_start_state(self, source: str, line_no: int, type: str, status: str) -> None:
         if self.state == State.Stopped:
             return
 
         if self.requested_state == RequestedState.Pause:
+            self.requested_state = RequestedState.Nothing
             self.state = State.Paused
+
             self.send_event(
                 self,
                 StoppedEvent(
                     body=StoppedEventBody(
                         reason=StoppedReason.PAUSE,
                         thread_id=threading.current_thread().ident,
                     )
                 ),
             )
-            self.requested_state = RequestedState.Nothing
+
         elif self.requested_state == RequestedState.Next:
             if len(self.full_stack_frames) <= self.stop_stack_len:
+                self.requested_state = RequestedState.Nothing
                 self.state = State.Paused
+
                 self.send_event(
                     self,
                     StoppedEvent(
                         body=StoppedEventBody(
                             reason=StoppedReason.STEP,
                             thread_id=threading.current_thread().ident,
                         )
                     ),
                 )
-                self.requested_state = RequestedState.Nothing
+
         elif self.requested_state == RequestedState.StepIn:
+            self.requested_state = RequestedState.Nothing
             self.state = State.Paused
+
             self.send_event(
                 self,
                 StoppedEvent(
                     body=StoppedEventBody(
                         reason=StoppedReason.STEP,
                         thread_id=threading.current_thread().ident,
                     )
                 ),
             )
-            self.requested_state = RequestedState.Nothing
+
         elif self.requested_state == RequestedState.StepOut and len(self.full_stack_frames) <= self.stop_stack_len:
+            self.requested_state = RequestedState.Nothing
             self.state = State.Paused
+
             self.send_event(
                 self,
                 StoppedEvent(
                     body=StoppedEventBody(
                         reason=StoppedReason.STEP,
                         thread_id=threading.current_thread().ident,
                     )
                 ),
             )
-            self.requested_state = RequestedState.Nothing
 
         if source is not None:
             source_path = self.map_path_to_client(str(Path(source).absolute()))
             if source_path in self.breakpoints:
                 breakpoints = [v for v in self.breakpoints[source_path].breakpoints if v.line == line_no]
                 if len(breakpoints) > 0:
                     for point in breakpoints:
@@ -574,56 +608,64 @@
                                     )
                                 ),
                             )
                             return
 
                         self.requested_state = RequestedState.Nothing
                         self.state = State.Paused
+
                         self.send_event(
                             self,
                             StoppedEvent(
                                 body=StoppedEventBody(
                                     reason=StoppedReason.BREAKPOINT,
                                     thread_id=threading.current_thread().ident,
                                     hit_breakpoint_ids=[id(v) for v in breakpoints],
                                 )
                             ),
                         )
 
     def process_end_state(self, status: str, filter_id: Set[str], description: str, text: Optional[str]) -> None:
+        if self.state == State.Stopped:
+            return
+
         if (
             not self.terminated
             and status == "FAIL"
             and any(
                 v
                 for v in self.exception_breakpoints
                 if v.filter_options and any(o for o in v.filter_options if o.filter_id in filter_id)
             )
         ):
+            reason = StoppedReason.EXCEPTION
+
             self.requested_state = RequestedState.Nothing
             self.state = State.Paused
 
             self.send_event(
                 self,
                 StoppedEvent(
                     body=StoppedEventBody(
-                        description=description,
-                        reason=StoppedReason.EXCEPTION,
+                        reason=reason,
                         thread_id=threading.current_thread().ident,
-                        all_threads_stopped=True,
+                        description=description,
                         text=text,
                     )
                 ),
             )
 
     def wait_for_running(self) -> None:
         if self.attached:
             while True:
                 with self.condition:
-                    self.condition.wait_for(lambda: self.state in [State.Running, State.Stopped, State.CallKeyword])
+                    self.condition.wait_for(
+                        lambda: self.state in [State.Running, State.Stopped, State.CallKeyword]
+                        or self.requested_state != RequestedState.Nothing
+                    )
 
                 if self.state == State.CallKeyword:
                     self._evaluated_keyword_result = None
                     try:
                         if self._keyword_to_evaluate is not None:
                             self._evaluated_keyword_result = self._keyword_to_evaluate()
                             self._keyword_to_evaluate = None
@@ -633,14 +675,26 @@
                         self._evaluated_keyword_result = e
                     finally:
                         self._evaluate_keyword_event.set()
                         self._after_evaluate_keyword_event.wait(120)
 
                     continue
 
+                if self.requested_state == RequestedState.Running:
+                    self.requested_state = RequestedState.Nothing
+                    self.state = State.Running
+                    if self.main_thread is not None and self.main_thread.ident is not None:
+                        self.send_event(
+                            self,
+                            ContinuedEvent(
+                                body=ContinuedEventBody(thread_id=self.main_thread.ident, all_threads_continued=True)
+                            ),
+                        )
+                    continue
+
                 break
 
     def start_output_group(self, name: str, attributes: Dict[str, Any], type: Optional[str] = None) -> None:
         if self.group_output:
             source = attributes.get("source", None)
             line_no = attributes.get("lineno", None)
 
@@ -753,26 +807,32 @@
             if self.stack_frames:
                 self.stack_frames[0].stack_frames.popleft()
         else:
             if self.stack_frames:
                 self.stack_frames[0].stack_frames.popleft()
 
     def start_suite(self, name: str, attributes: Dict[str, Any]) -> None:
+        if not self.run_started:
+            self.run_started = True
+            self.debug_logger = DebugLogger()
+            LOGGER.register_logger(self.debug_logger)
+
         source = attributes.get("source", None)
         line_no = attributes.get("lineno", 1)
         longname = attributes.get("longname", "")
         status = attributes.get("status", "")
         type = "SUITE"
 
         entry = self.add_stackframe_entry(name, type, source, line_no, longname=longname)
 
         if self.debug:
             if self.stop_on_entry:
                 self.stop_on_entry = False
 
+                self.requested_state = RequestedState.Nothing
                 self.state = State.Paused
                 self.send_event(
                     self,
                     StoppedEvent(
                         body=StoppedEventBody(
                             reason=StoppedReason.ENTRY,
                             thread_id=threading.current_thread().ident,
@@ -876,34 +936,91 @@
         "BuiltIn.Run Keyword And Expect Error",
         "BuiltIn.Run Keyword And Ignore Error",
         "BuiltIn.Run Keyword And Warn On Failure",
         "BuiltIn.Wait Until Keyword Succeeds",
         "BuiltIn.Run Keyword And Continue On Failure",
     ]
 
-    def in_caughted_keyword(self) -> bool:
+    def is_not_caughted_by_keyword(self) -> bool:
         r = next(
             (
                 v
                 for v in itertools.islice(self.full_stack_frames, 1, None)
                 if v.type == "KEYWORD" and v.longname in self.CAUGHTED_KEYWORDS
             ),
             None,
         )
         return r is None
 
+    __matchers: Optional[Dict[str, Callable[[str, str], bool]]] = None
+
+    def _get_matcher(self, pattern_type: str) -> Optional[Callable[[str, str], bool]]:
+        from robot.utils import Matcher
+
+        if self.__matchers is None:
+            self.__matchers: Dict[str, Callable[[str, str], bool]] = {
+                "GLOB": lambda m, p: bool(Matcher(p, spaceless=False, caseless=False).match(m)),
+                "LITERAL": lambda m, p: m == p,
+                "REGEXP": lambda m, p: re.match(rf"{p}\Z", m) is not None,
+                "START": lambda m, p: m.startswith(p),
+            }
+
+        return self.__matchers.get(pattern_type.upper(), None)
+
+    def _should_run_except(self, branch: Any, error: str) -> bool:
+        if not branch.patterns:
+            return True
+
+        if branch.pattern_type:
+            pattern_type = EXECUTION_CONTEXTS.current.variables.replace_string(branch.pattern_type)
+        else:
+            pattern_type = "LITERAL"
+
+        matcher = self._get_matcher(pattern_type)
+
+        if not matcher:
+            return False
+
+        for pattern in branch.patterns:
+            if matcher(error, EXECUTION_CONTEXTS.current.variables.replace_string(pattern)):
+                return True
+
+        return False
+
+    def is_not_caugthed_by_except(self, message: Optional[str]) -> bool:
+        if not message:
+            return True
+
+        if get_robot_version() >= (5, 0) and self.debug_logger:
+            from robot.running.model import Try
+
+            if self.debug_logger.steps:
+                for branch in [f.data for f in reversed(self.debug_logger.steps) if isinstance(f.data, Try)]:
+                    for except_branch in branch.except_branches:
+                        if self._should_run_except(except_branch, message):
+                            return False
+        return True
+
     def end_keyword(self, name: str, attributes: Dict[str, Any]) -> None:
         type = attributes.get("type", None)
         if self.debug:
             status = attributes.get("status", "")
 
             if status == "FAIL" and type in ["KEYWORD", "SETUP", "TEARDOWN"]:
                 self.process_end_state(
                     status,
-                    {"failed_keyword", *({"uncaught_failed_keyword"} if self.in_caughted_keyword() else {})},
+                    {
+                        "failed_keyword",
+                        *(
+                            {"uncaught_failed_keyword"}
+                            if self.is_not_caughted_by_keyword()
+                            and self.is_not_caugthed_by_except(self.last_fail_message)
+                            else {}
+                        ),
+                    },
                     "Keyword failed.",
                     f"Keyword failed: {self.last_fail_message}" if self.last_fail_message else "Keyword failed.",
                 )
 
                 self.wait_for_running()
 
         source = attributes.get("source", None)
@@ -1118,94 +1235,162 @@
                             presentation_hint="global",
                             variables_reference=entry.global_id(),
                         )
                     )
 
         return result
 
+    def _new_cache_id(self) -> int:
+        o = object()
+        self._variables_object_cache.append(o)
+        return id(o)
+
+    def _create_variable(self, name: str, value: Any) -> Variable:
+        if isinstance(value, Mapping):
+            v_id = self._new_cache_id()
+            self._variables_cache[v_id] = value
+            return Variable(
+                name=name,
+                value=reprlib.repr(value),
+                type=repr(type(value)),
+                variables_reference=v_id,
+                named_variables=len(value) + 1,
+                indexed_variables=0,
+            )
+
+        if isinstance(value, Sequence) and not isinstance(value, str):
+            v_id = self._new_cache_id()
+            self._variables_cache[v_id] = value
+            return Variable(
+                name=name,
+                value=reprlib.repr(value),
+                type=repr(type(value)),
+                variables_reference=v_id,
+                named_variables=1,
+                indexed_variables=len(value),
+            )
+
+        return Variable(name=name, value=repr(value), type=repr(type(value)))
+
     def get_variables(
         self,
         variables_reference: int,
         filter: Optional[Literal["indexed", "named"]] = None,
         start: Optional[int] = None,
         count: Optional[int] = None,
         format: Optional[ValueFormat] = None,
     ) -> List[Variable]:
         result = NormalizedDict(ignore="_")
 
-        entry = next(
-            (
-                v
-                for v in self.stack_frames
-                if variables_reference in [v.global_id(), v.suite_id(), v.test_id(), v.local_id()]
-            ),
-            None,
-        )
-        if entry is not None:
-            context = entry.context()
-            if context is not None:
-                if entry.global_id() == variables_reference:
-                    result.update(
-                        {
-                            k: Variable(name=k, value=repr(v), type=repr(type(v)))
-                            for k, v in context.variables._global.as_dict().items()
-                        }
-                    )
-                elif entry.suite_id() == variables_reference:
-                    globals = context.variables._global.as_dict()
-                    result.update(
-                        {
-                            k: Variable(name=k, value=repr(v), type=repr(type(v)))
-                            for k, v in context.variables._suite.as_dict().items()
-                            if k not in globals or globals[k] != v
-                        }
-                    )
-                elif entry.test_id() == variables_reference:
-                    globals = context.variables._suite.as_dict()
-                    result.update(
-                        {
-                            k: Variable(name=k, value=repr(v), type=repr(type(v)))
-                            for k, v in context.variables._test.as_dict().items()
-                            if k not in globals or globals[k] != v
-                        }
-                    )
-                elif entry.local_id() == variables_reference:
-                    vars = entry.get_first_or_self().variables()
-                    if vars is not None:
-                        p = entry.parent() if entry.parent else None
-
-                        globals = (
-                            (p.get_first_or_self().variables() if p is not None else None)
-                            or context.variables._test
-                            or context.variables._suite
-                            or context.variables._global
-                        ).as_dict()
-
-                        suite_vars = (context.variables._suite or context.variables._global).as_dict()
-
+        if filter is None:
+            entry = next(
+                (
+                    v
+                    for v in self.stack_frames
+                    if variables_reference in [v.global_id(), v.suite_id(), v.test_id(), v.local_id()]
+                ),
+                None,
+            )
+            if entry is not None:
+                context = entry.context()
+                if context is not None:
+                    if entry.global_id() == variables_reference:
+                        result.update(
+                            {k: self._create_variable(k, v) for k, v in context.variables._global.as_dict().items()}
+                        )
+                    elif entry.suite_id() == variables_reference:
+                        globals = context.variables._global.as_dict()
                         result.update(
                             {
-                                k: Variable(name=k, value=repr(v), type=repr(type(v)))
-                                for k, v in vars.as_dict().items()
-                                if (k not in globals or globals[k] != v)
-                                and (entry.handler is None or k not in suite_vars or suite_vars[k] != v)
+                                k: self._create_variable(k, v)
+                                for k, v in context.variables._suite.as_dict().items()
+                                if k not in globals or globals[k] != v
                             }
                         )
+                    elif entry.test_id() == variables_reference:
+                        globals = context.variables._suite.as_dict()
+                        result.update(
+                            {
+                                k: self._create_variable(k, v)
+                                for k, v in context.variables._test.as_dict().items()
+                                if k not in globals or globals[k] != v
+                            }
+                        )
+                    elif entry.local_id() == variables_reference:
+                        vars = entry.get_first_or_self().variables()
+                        if vars is not None:
+                            p = entry.parent() if entry.parent else None
+
+                            globals = (
+                                (p.get_first_or_self().variables() if p is not None else None)
+                                or context.variables._test
+                                or context.variables._suite
+                                or context.variables._global
+                            ).as_dict()
+
+                            suite_vars = (context.variables._suite or context.variables._global).as_dict()
+
+                            result.update(
+                                {
+                                    k: self._create_variable(k, v)
+                                    for k, v in vars.as_dict().items()
+                                    if (k not in globals or globals[k] != v)
+                                    and (entry.handler is None or k not in suite_vars or suite_vars[k] != v)
+                                }
+                            )
+
+                            if entry.handler is not None and entry.handler.arguments:
+                                for argument in entry.handler.arguments.argument_names:
+                                    name = f"${{{argument}}}"
+                                    try:
+                                        value = vars[name]
+                                    except (SystemExit, KeyboardInterrupt):
+                                        raise
+                                    except BaseException as e:
+                                        value = str(e)
+
+                                    result[name] = self._create_variable(name, value)
+            else:
+                value = self._variables_cache.get(variables_reference, None)
+
+                if value is not None and isinstance(value, Mapping):
+                    result.update({"len()": self._create_variable("len()", len(value))})
 
-                        if entry.handler is not None and entry.handler.arguments:
-                            for argument in entry.handler.arguments.argument_names:
-                                name = f"${{{argument}}}"
-                                try:
-                                    value = vars[name]
-                                except (SystemExit, KeyboardInterrupt):
-                                    raise
-                                except BaseException as e:
-                                    value = str(e)
+                    for i, (k, v) in enumerate(value.items(), start or 0):
+                        result[repr(i)] = self._create_variable(repr(k), v)
+                        if i >= 500:
+                            result["Unable to handle"] = self._create_variable(
+                                "Unable to handle", "Maximum number of items (500) reached."
+                            )
+                            break
+
+                elif value is not None and isinstance(value, Sequence) and not isinstance(value, str):
+                    result.update({"len()": self._create_variable("len()", len(value))})
+
+        elif filter == "indexed":
+            value = self._variables_cache.get(variables_reference, None)
 
-                                result[name] = Variable(name=name, value=repr(value), type=repr(type(value)))
+            if value is not None:
+                c = 0
+                for i, v in enumerate(value, start or 0):
+                    result[str(i)] = self._create_variable(str(i), v)
+                    c += 1
+                    if count is not None and c >= count:
+                        break
+
+        elif filter == "named":
+            value = self._variables_cache.get(variables_reference, None)
+
+            if value is not None and isinstance(value, Mapping):
+                for i, (k, v) in enumerate(value.items(), start or 0):
+                    result[repr(i)] = self._create_variable(repr(k), v)
+                    if count is not None and i >= count:
+                        break
+            elif value is not None and isinstance(value, Sequence) and not isinstance(value, str):
+                result.update({"len()": self._create_variable("len()", len(value))})
 
         return list(result.values())
 
     IS_VARIABLE_RE: ClassVar = re.compile(r"^[$@&%]\{.*\}(\[[^\]]*\])?$")
     IS_VARIABLE_ASSIGNMENT_RE: ClassVar = re.compile(r"^[$@&%]\{.*\}=?$")
     SPLIT_LINE: ClassVar = re.compile(r"(?= {2,}| ?\t)\s*")
     CURRDIR: ClassVar = re.compile(r"(?i)\$\{CURDIR\}")
@@ -1216,14 +1401,22 @@
         frame_id: Optional[int] = None,
         context: Union[EvaluateArgumentContext, str, None] = None,
         format: Optional[ValueFormat] = None,
     ) -> EvaluateResult:
         if not expression:
             return EvaluateResult(result="")
 
+        if (
+            (context == EvaluateArgumentContext.REPL or context == EvaluateArgumentContext.REPL.value)
+            and expression.startswith("#")
+            and expression[1:].strip() == "exprmode"
+        ):
+            self.expression_mode = not self.expression_mode
+            return EvaluateResult(result="# Expression mode is now " + ("on" if self.expression_mode else "off"))
+
         stack_frame = next((v for v in self.full_stack_frames if v.id == frame_id), None)
 
         evaluate_context = stack_frame.context() if stack_frame else None
 
         if evaluate_context is None:
             evaluate_context = EXECUTION_CONTEXTS.current
 
@@ -1262,14 +1455,17 @@
 
                             def run_kw() -> Any:
                                 kw = Keyword(name=splitted[0], args=tuple(splitted[1:]), assign=tuple(variables))
                                 return kw.run(evaluate_context)
 
                             result = self.run_in_robot_thread(run_kw)
 
+                            if isinstance(result, BaseException):
+                                raise result
+
                 elif self.IS_VARIABLE_RE.match(expression.strip()):
                     try:
                         result = vars.replace_scalar(expression)
                     except VariableError:
                         if context is not None and (
                             isinstance(context, EvaluateArgumentContext)
                             and (
@@ -1287,64 +1483,100 @@
                         ):
                             result = UNDEFINED
                         else:
                             raise
                 else:
                     result = internal_evaluate_expression(vars.replace_string(expression), vars)
             else:
+                if self.IS_VARIABLE_RE.match(expression.strip()):
+                    result = vars[expression.strip()]
+                else:
 
-                def get_test_body_from_string(command: str) -> TestCase:
-                    suite_str = (
-                        "*** Test Cases ***\nDummyTestCase423141592653589793\n  "
-                        + ("\n  ".join(command.split("\n")) if "\n" in command else command)
-                    ) + "\n"
-
-                    model = get_model(suite_str)
-                    suite: TestSuite = TestSuite.from_model(model)
-                    return suite.tests[0]
-
-                def run_kw() -> Any:
-                    test = get_test_body_from_string(expression)
-                    result = None
-
-                    if len(test.body):
-                        for kw in test.body:
-                            with LOGGER.delayed_logging:
-                                try:
-                                    result = kw.run(evaluate_context)
-                                    if kw.assign:
+                    def get_test_body_from_string(command: str) -> TestCase:
+                        suite_str = (
+                            "*** Test Cases ***\nDummyTestCase423141592653589793\n  "
+                            + ("\n  ".join(command.split("\n")) if "\n" in command else command)
+                        ) + "\n"
+
+                        model = get_model(suite_str)
+                        suite: TestSuite = TestSuite.from_model(model)
+                        return suite.tests[0]
+
+                    def run_kw() -> Any:
+                        test = get_test_body_from_string(expression)
+                        result = None
+
+                        if len(test.body):
+                            for kw in test.body:
+                                with LOGGER.delayed_logging:
+                                    try:
+                                        result = kw.run(evaluate_context)
+                                        if kw.assign:
+                                            result = None
+                                    except (SystemExit, KeyboardInterrupt):
+                                        raise
+                                    except BaseException:
                                         result = None
-                                except (SystemExit, KeyboardInterrupt):
-                                    raise
-                                except BaseException:
-                                    result = None
-                                    break
-                                finally:
-                                    messages = LOGGER._log_message_cache or []
-                                    for msg in messages or ():
-                                        # hack to get and evaluate log level
-                                        listener: Any = next(iter(LOGGER), None)
-                                        if listener is None or listener._is_logged(msg.level):
-                                            self.log_message(
-                                                {"level": msg.level, "message": msg.message, "timestamp": msg.timestamp}
-                                            )
-                    return result
+                                        break
+                                    finally:
+                                        messages = LOGGER._log_message_cache or []
+                                        for msg in messages or ():
+                                            # hack to get and evaluate log level
+                                            listener: Any = next(iter(LOGGER), None)
+                                            if listener is None or listener._is_logged(msg.level):
+                                                self.log_message(
+                                                    {
+                                                        "level": msg.level,
+                                                        "message": msg.message,
+                                                        "timestamp": msg.timestamp,
+                                                    }
+                                                )
+                        return result
 
-                result = self.run_in_robot_thread(run_kw)
+                    result = self.run_in_robot_thread(run_kw)
 
-                if isinstance(result, BaseException):
-                    raise result
+                    if isinstance(result, BaseException):
+                        raise result
 
         except (SystemExit, KeyboardInterrupt):
             raise
         except BaseException as e:
             self._logger.exception(e)
             raise
 
-        return EvaluateResult(repr(result) if result is not None else "", repr(type(result)))
+        return self._create_evaluate_result(result)
+
+    def _create_evaluate_result(self, value: Any) -> EvaluateResult:
+        self._evaluate_cache.insert(0, value)
+        if len(self._evaluate_cache) > 50:
+            self._evaluate_cache.pop()
+
+        if isinstance(value, Mapping):
+            v_id = self._new_cache_id()
+            self._variables_cache[v_id] = value
+            return EvaluateResult(
+                result=reprlib.repr(value),
+                type=repr(type(value)),
+                variables_reference=v_id,
+                named_variables=len(value) + 1,
+                indexed_variables=0,
+            )
+
+        if isinstance(value, Sequence) and not isinstance(value, str):
+            v_id = self._new_cache_id()
+            self._variables_cache[v_id] = value
+            return EvaluateResult(
+                result=reprlib.repr(value),
+                type=repr(type(value)),
+                variables_reference=v_id,
+                named_variables=1,
+                indexed_variables=len(value),
+            )
+
+        return EvaluateResult(result=repr(value), type=repr(type(value)))
 
     def run_in_robot_thread(self, kw: Callable[[], Any]) -> Any:
         with self.condition:
             self._keyword_to_evaluate = kw
             self._evaluated_keyword_result = None
 
             self._evaluate_keyword_event.clear()
@@ -1366,14 +1598,43 @@
                 self.state = old_state
                 self.condition.notify_all()
 
                 self._after_evaluate_keyword_event.set()
 
             return result
 
+    def _create_set_variable_result(self, value: Any) -> SetVariableResult:
+        self._evaluate_cache.insert(0, value)
+        if len(self._evaluate_cache) > 50:
+            self._evaluate_cache.pop()
+
+        if isinstance(value, Mapping):
+            v_id = self._new_cache_id()
+            self._variables_cache[v_id] = value
+            return SetVariableResult(
+                value=reprlib.repr(value),
+                type=repr(type(value)),
+                variables_reference=v_id,
+                named_variables=len(value) + 1,
+                indexed_variables=0,
+            )
+
+        if isinstance(value, Sequence) and not isinstance(value, str):
+            v_id = self._new_cache_id()
+            self._variables_cache[v_id] = value
+            return SetVariableResult(
+                value=reprlib.repr(value),
+                type=repr(type(value)),
+                variables_reference=v_id,
+                named_variables=1,
+                indexed_variables=len(value),
+            )
+
+        return SetVariableResult(value=repr(value), type=repr(type(value)))
+
     def set_variable(
         self, variables_reference: int, name: str, value: str, format: Optional[ValueFormat] = None
     ) -> SetVariableResult:
         entry = next(
             (
                 v
                 for v in self.full_stack_frames
@@ -1389,15 +1650,15 @@
 
                 if (name[2:-1] if self.IS_VARIABLE_RE.match(name) else name) not in variables:
                     raise NameError(f"Variable '{name}' not found.")
 
                 evaluated_value = internal_evaluate_expression(variables.replace_string(value), variables)
                 variables[name] = evaluated_value
 
-                return SetVariableResult(repr(evaluated_value), repr(type(value)))
+                return self._create_set_variable_result(evaluated_value)
 
         raise ReferenceError("Invalid variable reference.")
 
     def set_exception_breakpoints(
         self,
         filters: List[str],
         filter_options: Optional[List[ExceptionFilterOptions]] = None,
@@ -1418,7 +1679,76 @@
 
                     self.exception_breakpoints.add(entry)
                     result.append(Breakpoint(verified=True))
                 else:
                     result.append(Breakpoint(verified=False))
 
         return result or None
+
+    def completions(
+        self, text: str, column: int, line: Optional[int] = None, frame_id: Optional[int] = None
+    ) -> List[CompletionItem]:
+        if self.expression_mode:
+            return []
+
+        stack_frame = next((v for v in self.full_stack_frames if v.id == frame_id), None)
+
+        evaluate_context = stack_frame.context() if stack_frame else None
+
+        if evaluate_context is None:
+            evaluate_context = EXECUTION_CONTEXTS.current
+
+        if evaluate_context is None:
+            return []
+
+        result = []
+
+        for library in evaluate_context.namespace._kw_store.libraries.values():
+            result.append(
+                CompletionItem(
+                    label=library.name,
+                    text=library.name,
+                    sort_text=f"020_{library.name}",
+                    type=CompletionItemType.MODULE,
+                )
+            )
+            for kw in library.handlers:
+                result.append(
+                    CompletionItem(
+                        label=kw.name,
+                        text=kw.name,
+                        sort_text=f"001_{kw.name}",
+                        type=CompletionItemType.FUNCTION,
+                        detail=kw.shortdoc,
+                    )
+                )
+
+        for resource in evaluate_context.namespace._kw_store.resources.values():
+            result.append(
+                CompletionItem(
+                    label=resource.name,
+                    text=resource.name,
+                    sort_text=f"020_{resource.name}",
+                    type=CompletionItemType.MODULE,
+                )
+            )
+            for kw in resource.handlers:
+                result.append(
+                    CompletionItem(
+                        label=kw.name,
+                        text=kw.name,
+                        sort_text=f"001_{kw.name}",
+                        type=CompletionItemType.FUNCTION,
+                        detail=kw.shortdoc,
+                    )
+                )
+
+        for var in evaluate_context.variables.as_dict().keys():
+            result.append(
+                CompletionItem(
+                    label=var,
+                    text=var,
+                    sort_text=f"010_{var}",
+                    type=CompletionItemType.VARIABLE,
+                )
+            )
+        return result
```

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/run.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from robotcode.core.types import ServerMode, TcpParams
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.jsonrpc2.server import JsonRPCServer
 
 from .dap_types import (
     AttachRequestArguments,
     Capabilities,
+    CompletionsArguments,
+    CompletionsResponseBody,
     ConfigurationDoneArguments,
     ContinueArguments,
     ContinueResponseBody,
     DisconnectArguments,
     EvaluateArgumentContext,
     EvaluateArguments,
     EvaluateResponseBody,
@@ -174,14 +176,15 @@
                     label="Failed Suite",
                     description="Breaks on failed suite",
                     default=False,
                 ),
             ],
             supports_exception_options=True,
             supports_exception_filter_options=True,
+            supports_completions_request=True,
         )
 
     @rpc_method(name="attach", param_type=AttachRequestArguments)
     async def _attach(
         self,
         arguments: AttachRequestArguments,
         request: Optional[str] = None,
@@ -240,15 +243,15 @@
             and arguments is not None
             and arguments.terminate_debuggee
         ):
             os._exit(-1)
         else:
             await self.send_event_async(Event("disconnectRequested"))
             Debugger.instance().attached = False
-            Debugger.instance().continue_all(False)
+            Debugger.instance().continue_all()
 
     @rpc_method(name="setBreakpoints", param_type=SetBreakpointsArguments)
     async def _set_breakpoints(
         self, arguments: SetBreakpointsArguments, *args: Any, **kwargs: Any
     ) -> SetBreakpointsResponseBody:
         return SetBreakpointsResponseBody(
             breakpoints=Debugger.instance().set_breakpoints(
@@ -372,14 +375,28 @@
         self, arguments: SetExceptionBreakpointsArguments, *args: Any, **kwargs: Any
     ) -> Optional[SetExceptionBreakpointsResponseBody]:
         result = Debugger.instance().set_exception_breakpoints(
             arguments.filters, arguments.filter_options, arguments.exception_options
         )
         return SetExceptionBreakpointsResponseBody(breakpoints=result) if result else None
 
+    @rpc_method(name="completions", param_type=CompletionsArguments)
+    async def _completions(
+        self,
+        arguments: CompletionsArguments,
+        text: str,
+        column: int,
+        line: Optional[int] = None,
+        frame_id: Optional[int] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> CompletionsResponseBody:
+        result = Debugger.instance().completions(text, column, line, frame_id)
+        return CompletionsResponseBody(targets=result)
+
 
 class DebugAdapterServer(JsonRPCServer[DebugAdapterServerProtocol]):
     def __init__(
         self,
         mode: ServerMode = ServerMode.TCP,
         tcp_params: TcpParams = TcpParams(None, TCP_DEFAULT_PORT),
         pipe_name: Optional[str] = None,
```

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 )
 
 from ..__version__ import __version__
 from .run import run_launcher
 
 LAUNCHER_DEFAULT_PORT = 6611
 
+# mypy: disable-error-code="misc, arg-type, attr-defined"
+
 
 @click.command(
     add_help_option=True,
     hidden=True,
 )
 @add_options(*server_options(ServerMode.STDIO, default_port=LAUNCHER_DEFAULT_PORT))
 @click.version_option(version=__version__, prog_name="RobotCode Launcher")
```

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.47.0/src/robotcode/debugger/launcher/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
                     label="Failed Suite",
                     description="Breaks on failed suite",
                     default=False,
                 ),
             ],
             supports_exception_options=True,
             supports_exception_filter_options=True,
+            supports_completions_request=True,
         )
 
     @rpc_method(name="launch", param_type=LaunchRequestArguments)
     async def _launch(
         self,
         request: str,
         python: Optional[str] = None,
@@ -148,15 +149,15 @@
         name: Optional[str] = None,
         no_debug: Optional[bool] = None,
         robotPythonPath: Optional[List[str]] = None,  # noqa: N803
         launcherArgs: Optional[List[str]] = None,  # noqa: N803
         launcherTimeout: Optional[int] = None,  # noqa: N803
         debuggerArgs: Optional[List[str]] = None,  # noqa: N803
         debuggerTimeout: Optional[int] = None,  # noqa: N803
-        attachPython: Optional[bool] = True,  # noqa: N803
+        attachPython: Optional[bool] = False,  # noqa: N803
         attachPythonPort: Optional[int] = None,  # noqa: N803
         variables: Optional[Dict[str, Any]] = None,
         outputDir: Optional[str] = None,  # noqa: N803
         outputMessages: Optional[bool] = False,  # noqa: N803
         outputLog: Optional[bool] = False,  # noqa: N803
         outputTimestamps: Optional[bool] = False,  # noqa: N803
         groupOutput: Optional[bool] = False,  # noqa: N803
```

### Comparing `robotcode_debugger-0.46.0/.gitignore` & `robotcode_debugger-0.47.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/LICENSE.txt` & `robotcode_debugger-0.47.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/README.md` & `robotcode_debugger-0.47.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.46.0/pyproject.toml` & `robotcode_debugger-0.47.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.46.0",
-  "robotcode-runner==0.46.0",
+  "robotcode-jsonrpc2==0.47.0",
+  "robotcode-runner==0.47.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.46.0/PKG-INFO` & `robotcode_debugger-0.47.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.46.0
+Version: 0.47.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.46.0
-Requires-Dist: robotcode-runner==0.46.0
+Requires-Dist: robotcode-jsonrpc2==0.47.0
+Requires-Dist: robotcode-runner==0.47.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

