# Comparing `tmp/signe-0.1.7.tar.gz` & `tmp/signe-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signe-0.1.7.tar", last modified: Mon Jul 10 06:58:28 2023, max compression
+gzip compressed data, was "signe-0.1.8.tar", last modified: Mon Jul 10 10:30:31 2023, max compression
```

## Comparing `signe-0.1.7.tar` & `signe-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.213555 signe-0.1.7/
--rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      469 2023-07-10 06:58:28.194279 signe-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 06:58:28.213555 signe-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.168317 signe-0.1.7/signe/
--rw-rw-rw-   0        0        0      225 2023-07-10 06:58:13.000000 signe-0.1.7/signe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.188277 signe-0.1.7/signe/core/
--rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.7/signe/core/__init__.py
--rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.7/signe/core/collections.py
--rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.7/signe/core/consts.py
--rw-rw-rw-   0        0        0     5939 2023-07-08 17:46:06.000000 signe-0.1.7/signe/core/effect.py
--rw-rw-rw-   0        0        0     2840 2023-07-08 17:46:06.000000 signe-0.1.7/signe/core/runtime.py
--rw-rw-rw-   0        0        0     2818 2023-07-08 17:46:06.000000 signe-0.1.7/signe/core/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.192290 signe-0.1.7/signe/reactive/
--rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.7/signe/reactive/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.7/signe/reactive/proxy.py
--rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.7/signe/types.py
--rw-rw-rw-   0        0        0     5319 2023-07-10 06:58:11.000000 signe-0.1.7/signe/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.178293 signe-0.1.7/signe.egg-info/
--rw-rw-rw-   0        0        0      469 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 10:30:31.957951 signe-0.1.8/
+-rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      469 2023-07-10 10:30:31.956953 signe-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 10:30:31.957951 signe-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:30:31.912771 signe-0.1.8/signe/
+-rw-rw-rw-   0        0        0      225 2023-07-10 10:30:23.000000 signe-0.1.8/signe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:30:31.934015 signe-0.1.8/signe/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.8/signe/core/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.8/signe/core/collections.py
+-rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.8/signe/core/consts.py
+-rw-rw-rw-   0        0        0     6531 2023-07-10 10:30:13.000000 signe-0.1.8/signe/core/effect.py
+-rw-rw-rw-   0        0        0     2840 2023-07-08 17:46:06.000000 signe-0.1.8/signe/core/runtime.py
+-rw-rw-rw-   0        0        0     3033 2023-07-10 10:30:13.000000 signe-0.1.8/signe/core/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:30:31.938004 signe-0.1.8/signe/reactive/
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.8/signe/reactive/__init__.py
+-rw-rw-rw-   0        0        0     7500 2023-07-10 10:30:13.000000 signe-0.1.8/signe/reactive/proxy.py
+-rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.8/signe/types.py
+-rw-rw-rw-   0        0        0     5989 2023-07-10 10:30:13.000000 signe-0.1.8/signe/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:30:31.923044 signe-0.1.8/signe.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-07-10 10:30:31.000000 signe-0.1.8/signe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-10 10:30:31.000000 signe-0.1.8/signe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 10:30:31.000000 signe-0.1.8/signe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 10:30:31.000000 signe-0.1.8/signe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-10 10:30:31.000000 signe-0.1.8/signe.egg-info/top_level.txt
```

### Comparing `signe-0.1.7/LICENSE` & `signe-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `signe-0.1.7/README.md` & `signe-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `signe-0.1.7/setup.py` & `signe-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.7/signe/core/collections.py` & `signe-0.1.8/signe/core/collections.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.7/signe/core/effect.py` & `signe-0.1.8/signe/core/effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,27 @@
 
     def __init__(
         self,
         executor: Executor,
         fn: Callable[[], T],
         debug_trigger: Optional[Callable] = None,
         priority_level=1,
+        debug_name: Optional[str] = None,
+        capture_parent_effect=True,
     ) -> None:
         Effect._g_id += 1
         self.id = Effect._g_id
         self.__executor = executor
         self.value: Optional[T] = None
         self.fn = fn
         self._age = 0
         self._state = EffectState.CURRENT
         self.__dep_signals: Set[Signal] = set()
         self.__priority_level = priority_level
+        self.__debug_name = debug_name
 
         """
         When one effect is triggered by another effect, 
         the former belongs to a pre dependency 
         and the latter belongs to a next dependency.
 
         @effect
@@ -59,24 +62,39 @@
 
         self._sub_effects: list[Effect] = []
 
         self._cleanup_callbacks: list[Callable] = []
 
         self._debug_trigger = debug_trigger
 
+        """
+        This method must be executed before Method __run_fn. 
+        If an effect object is created 
+        during the execution of a parent effect object, 
+        it is considered as its child object.
+        """
+        if capture_parent_effect:
+            self.__try_add_self_to_parent_sub_effect()
+
         self.__run_fn()
         self.__init_no_deps = (
             len(self.__pre_dep_effects)
             + len(self.__next_dep_effects)
             + len(self.__dep_signals)
         ) <= 0
 
     def __get_all_dep_effects(self):
         return chain(self.__pre_dep_effects, self.__next_dep_effects)
 
+    def __try_add_self_to_parent_sub_effect(self):
+        current_effect = self.__executor.effect_running_stack.get_current()
+
+        if current_effect is not None and current_effect is not self:
+            current_effect._add_sub_effect(self)
+
     @property
     def priority_level(self):
         return self.__priority_level
 
     def _get_pre_dep_effects(self):
         return list(self.__pre_dep_effects)
 
@@ -119,15 +137,15 @@
             return
 
         self._age = tick
         self._state = EffectState.STALE
 
         self.__executor.current_execution_scheduler.add_effect(self)
 
-        for effect in self.__get_all_dep_effects():
+        for effect in self.__next_dep_effects:
             effect._push_scheduler()
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         return self.getValue()
 
     def update(self):
         if self._state != EffectState.STALE:
@@ -137,19 +155,14 @@
 
     def add_cleanup_callback(self, callback: Callable):
         self._cleanup_callbacks.append(callback)
 
     def __run_fn(self):
         self._cleanup_source_before_update()
 
-        current_effect = self.__executor.effect_running_stack.get_current()
-
-        if current_effect is not None and current_effect is not self:
-            current_effect._add_sub_effect(self)
-
         try:
             self.__executor.effect_running_stack.set_current(self)
 
             self._state = EffectState.RUNNING
 
             self.cleanup_deps()
 
@@ -195,19 +208,22 @@
 
         for cb in self._cleanup_callbacks:
             cb()
 
         self._cleanup_callbacks.clear()
 
     def _cleanup_sub_effects(self):
-        # for effect in self._sub_effects:
-        #     effect.dispose()
+        for effect in self._sub_effects:
+            effect.dispose()
 
         self._sub_effects.clear()
 
     def dispose(self):
         self._cleanup_sub_effects()
         self.cleanup_deps()
         # self.fn = None
 
     def _reset_age(self):
         self._age = 0
+
+    def __repr__(self) -> str:
+        return f"Effect(id ={self.id}, name={self.__debug_name})"
```

### Comparing `signe-0.1.7/signe/core/runtime.py` & `signe-0.1.8/signe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.7/signe/core/signal.py` & `signe-0.1.8/signe/core/signal.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,23 +36,28 @@
         self.comp: TSignalOptionComp = comp  # type: ignore
 
 
 class Signal(Generic[T]):
     _g_id = 0
 
     def __init__(
-        self, executor: Executor, value: T, option: Optional[SignalOption[T]] = None
+        self,
+        executor: Executor,
+        value: T,
+        option: Optional[SignalOption[T]] = None,
+        debug_name: Optional[str] = None,
     ) -> None:
         Signal._g_id += 1
         self.id = Signal._g_id
         self.__executor = executor
         self.value = value
         self.__dep_effects: Set[Effect] = set()
         self.option = option or SignalOption[T]()
         self._pending = NOT_PENDING
+        self.__debug_name = debug_name
 
         self._option_comp = cast(Callable[[T, T], bool], self.option.comp)
 
     def getValue(self) -> T:
         current_effect = self.__executor.effect_running_stack.get_current()
 
         if current_effect:
@@ -93,7 +98,10 @@
         return hash(self.id)
 
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, self.__class__):
             return self.__hash__() == __value.__hash__()
 
         return False
+
+    def __repr__(self) -> str:
+        return f"Signal(id= {self.id} , name = {self.__debug_name})"
```

### Comparing `signe-0.1.7/signe/reactive/proxy.py` & `signe-0.1.8/signe/reactive/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def __init__(self, obj) -> None:
         super().__init__(obj)
         self._keySignalMap: TKeySignalMap = {}
 
     def _create_signal(self, key: TKeySignalMapKey, value):
         signal = None
         if key not in self._keySignalMap:
-            signal = createSignal(value)
+            signal = createSignal(value,debug_name=str(key))
             self._keySignalMap[key] = signal
         else:
             signal = self._keySignalMap[key]
 
         return signal
 
     def _try_get_signal(self, key: TKeySignalMapKey):
```

### Comparing `signe-0.1.7/signe/utils.py` & `signe-0.1.8/signe/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,50 +21,61 @@
 
 TGetter = Callable[[], T]
 
 TSetterParme = Union[T, Callable[[T], T]]
 TSetter = Callable[[TSetterParme[T]], T]
 
 
-def createSignal(value: T, comp: TSignalOptionInitComp[T] = None):
-    s = Signal(exec, value, SignalOption(comp))
+def createSignal(
+    value: T,
+    comp: TSignalOptionInitComp[T] = None,
+    debug_name: Optional[str] = None,
+):
+    s = Signal(exec, value, SignalOption(comp), debug_name)
 
     return s.getValue, s.setValue
 
 
 _TEffect_Fn = Callable[[Callable[..., T]], Effect[T]]
 
 
 @overload
 def effect(
     fn: None = ...,
     *,
     priority_level=1,
     debug_trigger: Optional[Callable] = None,
+    debug_name: Optional[str] = None,
 ) -> _TEffect_Fn[None]:
     ...
 
 
 @overload
 def effect(
     fn: Callable[..., None],
     *,
     priority_level=1,
     debug_trigger: Optional[Callable] = None,
+    debug_name: Optional[str] = None,
 ) -> Effect[None]:
     ...
 
 
 def effect(
     fn: Optional[Callable[..., None]] = None,
     *,
     priority_level=1,
     debug_trigger: Optional[Callable] = None,
+    debug_name: Optional[str] = None,
 ) -> Union[_TEffect_Fn[None], Effect[None]]:
-    kws = {"priority_level": priority_level, "debug_trigger": debug_trigger}
+    kws = {
+        "priority_level": priority_level,
+        "debug_trigger": debug_trigger,
+        "debug_name": debug_name,
+    }
 
     if fn:
         return Effect(exec, fn, **kws)
     else:
 
         def wrap(fn: Callable[..., None]):
             return Effect(exec, fn, **kws)
@@ -74,41 +85,55 @@
 
 @overload
 def computed(
     fn: None = ...,
     *,
     priority_level=1,
     debug_trigger: Optional[Callable] = None,
+    debug_name: Optional[str] = None,
 ) -> Callable[[Callable[..., T]], Callable[..., T]]:
     ...
 
 
 @overload
 def computed(
     fn: Callable[..., T],
     *,
     priority_level=1,
     debug_trigger: Optional[Callable] = None,
+    debug_name: Optional[str] = None,
 ) -> Callable[..., T]:
     ...
 
 
 def computed(
     fn: Optional[Callable[[], T]] = None,
     *,
     priority_level=1,
     debug_trigger: Optional[Callable] = None,
+    debug_name: Optional[str] = None,
 ) -> Union[Callable[[Callable[..., T]], Callable[..., T]], Callable[..., T]]:
-    kws = {"priority_level": priority_level, "debug_trigger": debug_trigger}
+    kws = {
+        "priority_level": priority_level,
+        "debug_trigger": debug_trigger,
+        "debug_name": debug_name,
+    }
 
     if fn:
+        current_effect = exec.effect_running_stack.get_current()
 
         def first():
-            nonlocal real_fn
-            effect = Effect(exec, fn, **kws)
+            nonlocal real_fn, current_effect
+            effect = Effect(exec, fn, **kws, capture_parent_effect=False)
+
+            if current_effect is not None:
+                current_effect._add_sub_effect(effect)
+
+            del current_effect
+
             real_fn = effect
             return effect.getValue()
 
         real_fn = first
 
         def wrap():
             return real_fn()
```

