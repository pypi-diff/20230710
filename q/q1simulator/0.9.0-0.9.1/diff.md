# Comparing `tmp/q1simulator-0.9.0.tar.gz` & `tmp/q1simulator-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\q1simulator-0.9.0.tar", last modified: Mon Mar 13 17:17:16 2023, max compression
+gzip compressed data, was "dist\q1simulator-0.9.1.tar", last modified: Mon Jul 10 09:36:19 2023, max compression
```

## Comparing `q1simulator-0.9.0.tar` & `q1simulator-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 17:17:16.000000 q1simulator-0.9.0/
--rw-rw-rw-   0        0        0     1092 2021-12-09 11:11:44.000000 q1simulator-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      209 2023-03-13 17:17:16.000000 q1simulator-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     8071 2023-03-13 17:10:43.000000 q1simulator-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 17:17:16.000000 q1simulator-0.9.0/q1simulator/
--rw-rw-rw-   0        0        0      178 2023-03-13 17:17:02.000000 q1simulator-0.9.0/q1simulator/__init__.py
--rw-rw-rw-   0        0        0     4843 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/cluster.py
--rw-rw-rw-   0        0        0    11159 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/q1core.py
--rw-rw-rw-   0        0        0     6250 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/q1parser.py
--rw-rw-rw-   0        0        0    15408 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/q1sequencer.py
--rw-rw-rw-   0        0        0     8967 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/q1simulator.py
--rw-rw-rw-   0        0        0     2102 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/q1viewer.py
--rw-rw-rw-   0        0        0      613 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/qblox_version.py
--rw-rw-rw-   0        0        0    20102 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/rt_renderer.py
--rw-rw-rw-   0        0        0     2004 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/trigger_sorting.py
--rw-rw-rw-   0        0        0     1213 2023-03-13 17:10:43.000000 q1simulator-0.9.0/q1simulator/triggers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:17:16.000000 q1simulator-0.9.0/q1simulator.egg-info/
--rw-rw-rw-   0        0        0      209 2023-03-13 17:17:15.000000 q1simulator-0.9.0/q1simulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-03-13 17:17:15.000000 q1simulator-0.9.0/q1simulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 17:17:15.000000 q1simulator-0.9.0/q1simulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-13 17:17:15.000000 q1simulator-0.9.0/q1simulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-13 17:17:15.000000 q1simulator-0.9.0/q1simulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-03-13 17:17:16.000000 q1simulator-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      377 2023-03-13 17:17:02.000000 q1simulator-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:17:16.000000 q1simulator-0.9.0/test/
--rw-rw-rw-   0        0        0     4585 2023-03-13 17:10:43.000000 q1simulator-0.9.0/test/test_conditional.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/
+-rw-rw-rw-   0        0        0     1092 2021-12-09 11:11:44.000000 q1simulator-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-07-10 09:36:19.000000 q1simulator-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8162 2023-07-10 09:33:00.000000 q1simulator-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator/
+-rw-rw-rw-   0        0        0      178 2023-07-10 09:35:50.000000 q1simulator-0.9.1/q1simulator/__init__.py
+-rw-rw-rw-   0        0        0     4843 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/cluster.py
+-rw-rw-rw-   0        0        0    11391 2023-05-02 14:09:38.000000 q1simulator-0.9.1/q1simulator/q1core.py
+-rw-rw-rw-   0        0        0     6365 2023-06-30 08:34:39.000000 q1simulator-0.9.1/q1simulator/q1parser.py
+-rw-rw-rw-   0        0        0    15504 2023-04-28 13:04:44.000000 q1simulator-0.9.1/q1simulator/q1sequencer.py
+-rw-rw-rw-   0        0        0     9060 2023-07-10 09:20:17.000000 q1simulator-0.9.1/q1simulator/q1simulator.py
+-rw-rw-rw-   0        0        0     2102 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/q1viewer.py
+-rw-rw-rw-   0        0        0      613 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/qblox_version.py
+-rw-rw-rw-   0        0        0    20159 2023-07-10 09:26:54.000000 q1simulator-0.9.1/q1simulator/rt_renderer.py
+-rw-rw-rw-   0        0        0     2004 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/trigger_sorting.py
+-rw-rw-rw-   0        0        0     1213 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/triggers.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/
+-rw-rw-rw-   0        0        0      209 2023-07-10 09:36:18.000000 q1simulator-0.9.1/q1simulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:36:18.000000 q1simulator-0.9.1/q1simulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-10 09:36:19.000000 q1simulator-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      377 2023-07-10 09:35:50.000000 q1simulator-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/test/
+-rw-rw-rw-   0        0        0     4585 2023-03-13 17:18:47.000000 q1simulator-0.9.1/test/test_conditional.py
```

### Comparing `q1simulator-0.9.0/LICENSE` & `q1simulator-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.0/README.md` & `q1simulator-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 The simulator takes the trigger network latency into account, but does not
 check whether triggers overlap. 
 
 
 # Simulator output
 The simulator has some methods to show the simulator output.
 - `plot()` shows pyplot charts with the rendered output.
+- `config(render_repetitions=False)` stops rendering when main sequence is executed once.
 - `print_acquisitions()` prints the path0 and path1 data and average counts.
 - `print_registers()` prints the contents of the Q1 registers.
 
 # Simulator logging
 Q1Simulator has a logging feature to help with code debugging.
 It uses of special comment line in the Q1ASM code.
 The comment line should start with `#Q1Sim:` and is followed by the
```

### Comparing `q1simulator-0.9.0/q1simulator/cluster.py` & `q1simulator-0.9.1/q1simulator/cluster.py`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.0/q1simulator/q1core.py` & `q1simulator-0.9.1/q1simulator/q1core.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 class Q1Core:
     def __init__(self, name, renderer, is_qrm):
         self.name = name
         self.renderer = renderer
         self._is_qrm = is_qrm
         self.max_core_cycles= 10_000_000
+        self.render_repetitions = True
         self.R = [0]*64
         self.lines = []
         self.instructions = []
         self.iptr = 0
         self.errors = set()
 
     def load(self, program):
@@ -149,14 +150,18 @@
         self.clock.add_ticks(4)
         if value >= n:
             self.iptr = label
 
     def _loop(self, register, label):
         self.clock.add_ticks(5)
         self._set_register(register, self.R[register] - 1)
+        instr = self.instructions[self.iptr-1]
+        if not self.render_repetitions and instr.arglist[1] == '@_start':
+            logger.info('Skipping repetitions')
+            return
         if self.R[register] != 0:
             self.iptr = label
 
     def _move(self, source, destination):
         self.clock.add_ticks(1)
         self._set_register(destination, source)
```

### Comparing `q1simulator-0.9.0/q1simulator/q1parser.py` & `q1simulator-0.9.1/q1simulator/q1parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import re
 
 from dataclasses import dataclass
-from typing import Optional, Tuple, Any, List
+from typing import Optional, Tuple, Any, List, Union
 
 @dataclass
 class Instruction:
     text_line_nr: int
     mnemonic: str
-    args: Optional[Tuple[str]] = None
+    arglist: Optional[Tuple[str]] = None
     label: Optional[str] = None
+    args: List[Union[int,str]] = None
     reg_args: List[int] = None
     func_name: Optional[str] = None
     func: Any = None
 
 
 class AsmSyntaxError(Exception):
     pass
@@ -81,21 +82,23 @@
 
         for instr in instructions:
             mnemonic = instr.mnemonic
             func_name = '_' + mnemonic
             instr.func_name = func_name
             if mnemonic in mnemonic_args:
                 try:
-                    args,reg_args = self._evaluate_args(mnemonic_args[mnemonic], instr.args)
+                    args,reg_args = self._evaluate_args(mnemonic_args[mnemonic], instr.arglist)
                     instr.args = args
                     instr.reg_args = reg_args
                 except AsmSyntaxError as ex:
                     print(ex)
                     print(lines[instr.text_line_nr])
                     raise
+            else:
+                instr.args = instr.arglist
 
         return lines,instructions
 
     def _parseline(self, line):
         org_line = line
         label_pattern = r'(\w+:)'
         instr_pattern = r'(\w+:)?\s*(\w+)\s*(.*)'
```

### Comparing `q1simulator-0.9.0/q1simulator/q1sequencer.py` & `q1simulator-0.9.1/q1simulator/q1sequencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
         elif name == 'max_render_time':
             self.rt_renderer.max_render_time = value
         elif name == 'max_core_cycles':
             self.q1core.max_core_cycles = value
         elif name == 'trace':
             self._trace = value
             self.rt_renderer.trace_enabled = value
+        elif name == 'render_repetitions':
+            self.q1core.render_repetitions = value
 
     def reset(self):
         self.waveforms = {}
         self.weights = {}
         self.acquisition_bins = {}
         self._mock_data = {}
         self._trigger_events = []
```

### Comparing `q1simulator-0.9.0/q1simulator/q1simulator.py` & `q1simulator-0.9.1/q1simulator/q1simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,17 @@
 
     def config(self, name, value):
         for seq in self.sequencers:
             seq.config(name, value)
 
     def plot(self, **kwargs):
         for seq in self.sequencers:
-            seq.plot()
+            # assume only sequencers in sync mode have executed.
+            if seq.sync_en():
+                seq.plot()
 
     def print_acquisitions(self):
         for i,seq in enumerate(self.sequencers):
             data = self.get_acquisitions(i)
             if not len(data):
                 continue
             for name, datadict in data.items():
@@ -222,15 +224,15 @@
         self.sequencers[seq_nr].print_registers(reg_nrs)
 
 
 class Q1Simulator(qc.Instrument, Q1Module):
     _pulsar_parameters = [
         'reference_source',
         ]
-        
+
     def __init__(self, name, n_sequencers=6, sim_type=None):
         super().__init__(name)
         super().init_module(n_sequencers, sim_type)
 
         for par_name in self._pulsar_parameters:
             self.add_parameter(par_name, set_cmd=partial(self._set, par_name))
```

### Comparing `q1simulator-0.9.0/q1simulator/q1viewer.py` & `q1simulator-0.9.1/q1simulator/q1viewer.py`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.0/q1simulator/qblox_version.py` & `q1simulator-0.9.1/q1simulator/qblox_version.py`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.0/q1simulator/rt_renderer.py` & `q1simulator-0.9.1/q1simulator/rt_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,28 +344,31 @@
             new_phase_offset = phase - (self.time * new.frequency * 1e-9) % 1
             self.nco_phase_offset = new_phase_offset
             self.nco_frequency = new.frequency
             new.frequency = None
         self.delta_phase += new.phase_shift
         new.phase_shift = 0.0
         if new.marker != old.marker:
-            for i in range(4):
-                m = 1 << i
-                m_old = old.marker & m
-                m_new = new.marker & m
-                if (new.marker & m) != (m_old):
-                    l = self.marker_out[i]
-                    if self.time < self.max_render_time:
-                        l += [[self.time, m_old], [self.time, m_new]]
-                    elif l[-1][0] < self.max_render_time:
-                        # add final marker step
-                        l += [[self.max_render_time, m_old], [self.max_render_time, 0]]
+            self._render_marker(old.marker, new.marker)
         # copy marker, offset and gain
         self.settings = copy(self.next_settings)
 
+    def _render_marker(self, old_marker, new_marker):
+        for i in range(4):
+            m = 1 << i
+            m_old = old_marker & m
+            m_new = new_marker & m
+            if m_new != m_old:
+                l = self.marker_out[i]
+                if self.time < self.max_render_time:
+                    l += [[self.time, m_old], [self.time, m_new]]
+                elif l[-1][0] < self.max_render_time:
+                    # add final marker step
+                    l += [[self.max_render_time, m_old], [self.max_render_time, 0]]
+
     def _render(self, time):
         if time & 0x0003:
             logger.error(f'{self.name}: wait time not aligned on '
                           f'4 ns boundary: {time} ns (offset={time&0x03} ns)')
             self._error('TIME NOT ALIGNED')
 
         # 16 bits, 4 ns resolution
```

### Comparing `q1simulator-0.9.0/q1simulator/trigger_sorting.py` & `q1simulator-0.9.1/q1simulator/trigger_sorting.py`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.0/q1simulator/triggers.py` & `q1simulator-0.9.1/q1simulator/triggers.py`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.0/q1simulator.egg-info/SOURCES.txt` & `q1simulator-0.9.1/q1simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.0/test/test_conditional.py` & `q1simulator-0.9.1/test/test_conditional.py`

 * *Files identical despite different names*

