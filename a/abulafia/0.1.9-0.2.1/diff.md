# Comparing `tmp/abulafia-0.1.9.tar.gz` & `tmp/abulafia-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abulafia-0.1.9.tar", last modified: Thu Jan 19 11:45:29 2023, max compression
+gzip compressed data, was "abulafia-0.2.1.tar", last modified: Mon Jul 10 19:27:54 2023, max compression
```

## Comparing `abulafia-0.1.9.tar` & `abulafia-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.228820 abulafia-0.1.9/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)     1073 2022-09-21 10:53:07.000000 abulafia-0.1.9/LICENSE
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    13023 2023-01-19 11:45:29.228364 abulafia-0.1.9/PKG-INFO
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    12761 2022-11-18 08:02:32.000000 abulafia-0.1.9/README.md
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)      503 2023-01-19 11:45:06.000000 abulafia-0.1.9/pyproject.toml
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       38 2023-01-19 11:45:29.228919 abulafia-0.1.9/setup.cfg
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       37 2022-08-23 07:22:48.000000 abulafia-0.1.9/setup.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.216377 abulafia-0.1.9/src/
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.218973 abulafia-0.1.9/src/abulafia/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       22 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/__init__.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.222590 abulafia-0.1.9/src/abulafia/actions/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       64 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/actions/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    23580 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/actions/actions.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.224424 abulafia-0.1.9/src/abulafia/functions/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       31 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/functions/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    24719 2022-12-02 11:46:39.000000 abulafia-0.1.9/src/abulafia/functions/core_functions.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.225536 abulafia-0.1.9/src/abulafia/observers/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       25 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/observers/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)     4601 2022-09-21 13:16:09.000000 abulafia-0.1.9/src/abulafia/observers/observers.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.227755 abulafia-0.1.9/src/abulafia/task_specs/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       75 2022-08-23 07:22:48.000000 abulafia-0.1.9/src/abulafia/task_specs/__init__.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    46063 2023-01-19 11:42:16.000000 abulafia-0.1.9/src/abulafia/task_specs/core_task.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    15826 2022-09-21 10:53:07.000000 abulafia-0.1.9/src/abulafia/task_specs/pipeline.py
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    51668 2023-01-19 11:42:16.000000 abulafia-0.1.9/src/abulafia/task_specs/task_specs.py
-drwxr-xr-x   0 thiippal (1057415414) ATKK\hyad-all (984178727)        0 2023-01-19 11:45:29.220773 abulafia-0.1.9/src/abulafia.egg-info/
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)    13023 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/PKG-INFO
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)      604 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/SOURCES.txt
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)        1 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/dependency_links.txt
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)       76 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/requires.txt
--rw-r--r--   0 thiippal (1057415414) ATKK\hyad-all (984178727)        9 2023-01-19 11:45:29.000000 abulafia-0.1.9/src/abulafia.egg-info/top_level.txt
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.791179 abulafia-0.2.1/
+-rw-r--r--   0 thiippal (1057415414) 984178727     1073 2022-09-21 10:53:07.000000 abulafia-0.2.1/LICENSE
+-rw-r--r--   0 thiippal (1057415414) 984178727     3715 2023-07-10 19:27:54.791062 abulafia-0.2.1/PKG-INFO
+-rw-r--r--   0 thiippal (1057415414) 984178727     3453 2023-07-10 19:21:03.000000 abulafia-0.2.1/README.md
+-rw-r--r--   0 thiippal (1057415414) 984178727      525 2023-07-10 19:21:03.000000 abulafia-0.2.1/pyproject.toml
+-rw-r--r--   0 thiippal (1057415414) 984178727       38 2023-07-10 19:27:54.791220 abulafia-0.2.1/setup.cfg
+-rw-r--r--   0 thiippal (1057415414) 984178727       37 2022-08-23 07:22:48.000000 abulafia-0.2.1/setup.py
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.786808 abulafia-0.2.1/src/
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.787063 abulafia-0.2.1/src/abulafia/
+-rw-r--r--   0 thiippal (1057415414) 984178727       22 2022-08-23 07:22:48.000000 abulafia-0.2.1/src/abulafia/__init__.py
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.788062 abulafia-0.2.1/src/abulafia/actions/
+-rw-r--r--   0 thiippal (1057415414) 984178727       79 2023-03-20 13:59:15.000000 abulafia-0.2.1/src/abulafia/actions/__init__.py
+-rw-r--r--   0 thiippal (1057415414) 984178727    29355 2023-07-10 19:21:03.000000 abulafia-0.2.1/src/abulafia/actions/actions.py
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.788969 abulafia-0.2.1/src/abulafia/functions/
+-rw-r--r--   0 thiippal (1057415414) 984178727       31 2022-08-23 07:22:48.000000 abulafia-0.2.1/src/abulafia/functions/__init__.py
+-rw-r--r--   0 thiippal (1057415414) 984178727    25299 2023-07-10 19:21:03.000000 abulafia-0.2.1/src/abulafia/functions/core_functions.py
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.789575 abulafia-0.2.1/src/abulafia/observers/
+-rw-r--r--   0 thiippal (1057415414) 984178727       25 2022-08-23 07:22:48.000000 abulafia-0.2.1/src/abulafia/observers/__init__.py
+-rw-r--r--   0 thiippal (1057415414) 984178727     4801 2023-07-10 19:21:00.000000 abulafia-0.2.1/src/abulafia/observers/observers.py
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.790466 abulafia-0.2.1/src/abulafia/task_specs/
+-rw-r--r--   0 thiippal (1057415414) 984178727       75 2022-08-23 07:22:48.000000 abulafia-0.2.1/src/abulafia/task_specs/__init__.py
+-rw-r--r--   0 thiippal (1057415414) 984178727    46297 2023-07-10 19:21:03.000000 abulafia-0.2.1/src/abulafia/task_specs/core_task.py
+-rw-r--r--   0 thiippal (1057415414) 984178727    15560 2023-07-10 19:21:03.000000 abulafia-0.2.1/src/abulafia/task_specs/pipeline.py
+-rw-r--r--   0 thiippal (1057415414) 984178727    31556 2023-07-10 19:21:03.000000 abulafia-0.2.1/src/abulafia/task_specs/task_specs.py
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.787724 abulafia-0.2.1/src/abulafia.egg-info/
+-rw-r--r--   0 thiippal (1057415414) 984178727     3715 2023-07-10 19:27:54.000000 abulafia-0.2.1/src/abulafia.egg-info/PKG-INFO
+-rw-r--r--   0 thiippal (1057415414) 984178727      664 2023-07-10 19:27:54.000000 abulafia-0.2.1/src/abulafia.egg-info/SOURCES.txt
+-rw-r--r--   0 thiippal (1057415414) 984178727        1 2023-07-10 19:27:54.000000 abulafia-0.2.1/src/abulafia.egg-info/dependency_links.txt
+-rw-r--r--   0 thiippal (1057415414) 984178727       91 2023-07-10 19:27:54.000000 abulafia-0.2.1/src/abulafia.egg-info/requires.txt
+-rw-r--r--   0 thiippal (1057415414) 984178727       18 2023-07-10 19:27:54.000000 abulafia-0.2.1/src/abulafia.egg-info/top_level.txt
+-rw-r--r--   0 thiippal (1057415414) 984178727      678 2023-04-24 18:45:55.000000 abulafia-0.2.1/src/outtakes.py
+drwxr-xr-x   0 thiippal (1057415414) 984178727        0 2023-07-10 19:27:54.790895 abulafia-0.2.1/tests/
+-rw-r--r--   0 thiippal (1057415414) 984178727     1870 2022-08-23 07:22:48.000000 abulafia-0.2.1/tests/test_functions.py
+-rw-r--r--   0 thiippal (1057415414) 984178727    11200 2023-07-10 19:21:03.000000 abulafia-0.2.1/tests/test_tasks.py
```

### Comparing `abulafia-0.1.9/LICENSE` & `abulafia-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abulafia-0.1.9/src/abulafia/actions/actions.py` & `abulafia-0.2.1/src/abulafia/actions/actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Import libraries
 from ..functions.core_functions import *
 from wasabi import Printer
+from shapely.geometry import Polygon
 import contextlib
 import io
 import toloka.client as toloka
 from toloka.streaming.event import AssignmentEvent
 from toloka.client.exceptions import IncorrectActionsApiError
 from typing import List, Union
 import collections
@@ -24,115 +25,38 @@
     from crowdkit.aggregation.classification.m_msr import MMSR
     from crowdkit.aggregation.classification.wawa import Wawa
     from crowdkit.aggregation.classification.zero_based_skill import ZeroBasedSkill
     from crowdkit.aggregation.classification.glad import GLAD
 warn = f.getvalue()
 
 if warn.startswith("None of PyTorch"):
-    msg.warn(f"Could not find a working installation of PyTorch or TensorFlow, one of which is "
+    msg.fail(f"Could not find a working installation of PyTorch or TensorFlow, one of which is "
              f"needed for the crowd-kit aggregators to function. Cancelling pipeline.", exits=1)
 
 
-class Verify:
-    """
-    This class defines an action for manually verifying crowdsourcing descriptions using other crowdsourced workers.
-
-    To add this action to a TaskSequence, register this object with AssignmentObserver using the 'on_accepted' method.
-    """
-    def __init__(self, configuration, task):
-        """
-        This function initialises the manual verification mechanism.
-
-        Parameters:
-            configuration: A string object that defines a path to a YAML file with configuration.
-            task: An object that inherits from the CrowdsourcingTask class.
-
-        Returns:
-            None
-        """
-        self.conf = read_configuration(configuration)
-        self.name = self.conf['name']
-        self.task = task
-        self.client = self.task.client
-        self.queue = collections.defaultdict(list)
-        self.aggregator = None
-
-    def __call__(self, events: List[AssignmentEvent]) -> None:
-
-        # Loop over the list of incoming AssignmentEvent objects
-        for event in events:
-
-            # Zip and iterate over tasks and solutions in each event
-            for task, solution in zip(event.assignment.tasks, event.assignment.solutions):
-
-                # Retrieve the answer
-                answer = solution.output_values[self.conf['data']['output']]
-
-                # Add the answer to the queue under assignment id
-                self.queue[task.input_values['assignment_id']].append(answer)
-
-        # Set up a placeholder for processed task suites
-        processed = []
-
-        # Loop over the assignments in the queue
-        for assignment_id, results in self.queue.items():
-
-            try:
-
-                # Accept the task suite if all assignments in the suite have been verified as correct
-                if all(results) is True:
-
-                    self.client.accept_assignment(assignment_id=assignment_id,
-                                                  public_comment=self.conf['messages']['accepted'])
-
-                    msg.good(f'Accepted assignment {assignment_id}')
-
-                # Reject the task suite if all assignments in the suite have not been verified as correct
-                if all(results) is not True:
-
-                    self.client.reject_assignment(assignment_id=assignment_id,
-                                                  public_comment=self.conf['messages']['rejected'])
-
-                    msg.warn(f'Rejected assignment {assignment_id}')
-
-            # Catch the error that might be raised by manually accepting/rejecting tasks in
-            # the web interface
-            except IncorrectActionsApiError:
-
-                msg.warn(f'Could not {"accept" if all(results) == True else "reject"} assignment {assignment_id}')
-
-            # Append the task suite to the list of processed suites
-            processed.append(assignment_id)
-
-        # Delete the assignment from the list of processed task suites
-        for assignment_id in processed:
-
-            processed.remove(assignment_id)
-
-
 class Aggregate:
     """
-    This class can be used to aggregate crowdsourced answers.
+    This class can be used to aggregate crowdsourced answers using various algorithms.
 
     Parameters:
         configuration: A string object that defines a path to a YAML file with configuration.
-        task: Crowdsourcing Task of which results will be aggregated.
-        forward: Forward object with which the aggregated tasks will be forwarded to the next pool or accepted/rejected.
+        task: The CrowdsourcingTask object whose results should be aggregated.
+        forward: The Forward object that will be used to forward, accept or reject the aggregated tasks.
 
     Returns:
         None
-    
     """
     def __init__(self, configuration, task, forward=None):
 
         self.task = task
         self.conf = read_configuration(configuration)
         self.name = self.conf['name']
 
         self.forward = forward
+        self.messages = self.conf['messages'] if 'messages' in self.conf else None
 
         self.majority_vote = True if self.conf['method'] == 'majority_vote' else False
         self.dawid_skene = True if self.conf['method'] == 'dawid_skene' else False
         self.gold_majority_vote = True if self.conf['method'] == 'gold_majority_vote' else False
         self.mmsr = True if self.conf['method'] == 'mmsr' else False
         self.wawa = True if self.conf['method'] == 'wawa' else False
         self.zero_based_skill = True if self.conf['method'] == 'zero_based_skill' else False
@@ -141,17 +65,20 @@
         self.result = None
         self.prev_assignments = set()
 
         self.complete = False
 
     def __call__(self, pool: toloka.Pool) -> None:
 
-        assignments = list(self.task.client.get_assignments(pool_id=pool.id, status=[toloka.Assignment.SUBMITTED, toloka.Assignment.ACCEPTED]))
+        assignments = list(self.task.client.get_assignments(pool_id=pool.id,
+                                                            status=[toloka.Assignment.SUBMITTED,
+                                                                    toloka.Assignment.ACCEPTED]))
 
         if assignments:
+
             a_dict = {"task": [], "inputs": [], "label": [], "worker": [], "id": []}
 
             input_data = list(self.task.data_conf['input'].keys())[0]
             output_data = list(self.task.data_conf['output'].keys())[0]
 
             for a in assignments:
                 if a.id not in self.prev_assignments:
@@ -191,52 +118,56 @@
 
             elif self.glad:
 
                 self.result = GLAD().fit_predict(df)
 
             assert self.result is not None, raise_error("Aggregation did not produce a result!")
 
-            forward_data = [{"id": df.loc[df["task"] == task, "id"].iloc[0], 
-                             "input_data": df.loc[df["task"] == task, "inputs"].iloc[0], 
-                             "label": self.result[task]} 
+            forward_data = [{'id': df.loc[df['task'] == task, 'id'].iloc[0],
+                             'input_data': df.loc[df['task'] == task, 'inputs'].iloc[0],
+                             'label': self.result[task],
+                             'message': self.messages[self.result[task]] if self.messages is not None
+                             else "No reason was provided."}
                             for task in self.result.index]
 
-            msg.good(f"Finished aggregating {len(forward_data)} submitted tasks from {self.task.name}")
+            msg.good(f"Finished aggregating {len(forward_data)} submitted assignments from {self.task.name}")
             self.complete = True
 
             if self.forward:
+
                 self.forward(forward_data)
 
 
 class Forward:
     """
     This class defines an action for forwarding completed tasks to specific pools based on values.
 
-    For example, if a task receives the value True, it can be forwarded to Pool 1, whereas tasks with value False
-    will be forwarded to Pool 2.
+    For example, if a task receives the value True, it can be forwarded to Pool 1, whereas tasks
+    with value False will be forwarded to Pool 2.
 
     Parameters:
         configuration: A string object that defines a path to a YAML file with configuration.
-        client: Toloka client object.
-        targets: Pools where tasks will be forwarded.
+        client: A Toloka client object.
+        targets: A list of objects that inherit from the CrowdsourcingTask class to which the tasks
+                 will be forwarded to.
 
     Returns:
         None
     """
     def __init__(self, configuration, client, targets=None):
 
         self.conf = read_configuration(configuration)
         self.name = self.conf['name']
         self.client = client
         self.reject = []
         self.accept = []
         self.dont_forward = []
 
         # Possible outputs for the task (e.g. true and false) and their forward pools
-        self.outputs = self.conf['actions']['on_result']
+        self.outputs = self.conf['on_result']
 
         # Check if some outputs should be accepted or rejected (these are not forwarded like other tasks,
         # but accepted or rejected based on the output) and remove these from outputs
         self.reject.extend([k for k, v in self.outputs.items() if v == 'reject'])
         [self.outputs.pop(k) for k in self.reject]
 
         self.accept.extend([k for k, v in self.outputs.items() if v == 'accept'])
@@ -246,64 +177,86 @@
         self.dont_forward.extend([k for k, v in self.outputs.items() if v == None])
         [self.outputs.pop(k) for k in self.dont_forward]
 
         # Deal with outputs that have several actions (both accepting/rejecting and forwarding)
         multi_action = {k: v for (k, v) in self.outputs.items() if type(v) == list}
         self.reject.extend([k for k, v in multi_action.items() if 'reject' in v])
         self.accept.extend([k for k, v in multi_action.items() if 'accept' in v])
-        multi_action = {k: [i for i in v if i not in ["accept", "reject"]][0] for (k, v) in multi_action.items()}
+        multi_action = {k: [i for i in v if i not in ['accept', 'reject']][0] for (k, v) in multi_action.items()}
+
+        # Check that messages for accepting and rejecting assignments have been defined
+        if len(self.accept) or len(self.reject) > 0:
+
+            try:
+
+                self.conf['messages']
+
+            except KeyError:
+
+                msg.fail("Please use the top-level key 'messages' to define messages associated with outputs that "
+                         "accept or reject assignments. Define a message for each output value defined under "
+                         "'on_result' that leads to acceptance or rejection. These messages will be added to "
+                         "assignments and shown to the workers.", exits=1)
+
+            # Get the difference between the outputs defined under 'on_result' and 'messages'
+            diff = set(self.reject + self.accept).difference(self.conf['messages'])
+
+            if len(diff) > 0:
+
+                msg.fail(f"Please define messages associated with the following outputs under the top-level key "
+                         f"'messages': {', '.join(list(diff))}.", exits=True)
 
         self.outputs = {**self.outputs, **multi_action}
 
         # Create mapping for output and the configured CrowdsourcingTask object of the forward pool
         self.name_mapping = {pool.name: pool for pool in targets}
         self.forward_pools = {output: self.name_mapping[name] for (output, name) in self.outputs.items()}
 
         # Initialize dictionary of key-list pairs. Keys are possible outputs for the task
         # and the lists are tasks to be forwarded.
         self.tasks_to_forward = collections.defaultdict(list)
 
     def __call__(self, events: Union[List[AssignmentEvent], List[dict]]) -> None:
 
-        # Process tasks that come from an observer call
+        # Begin by processing incoming events that originate from observers (AssignmentEvent)
         if all(isinstance(x, AssignmentEvent) for x in events):
 
             # Loop over the list of incoming AssignmentEvent objects
             for event in events:
 
                 for i in range(len(event.assignment.tasks)):
 
-                    solution = event.assignment.solutions[i].output_values[self.conf['data']['output']]
+                    solution = event.assignment.solutions[i].output_values[self.conf['data']]
 
                     # If performer verified the task as incorrect, reject the original assignment
                     # and, if configured in source pool under "on_reject", re-add the task to the pool
                     if solution in self.reject:
 
                         self.client.reject_assignment(assignment_id=event.assignment.tasks[i].input_values['assignment_id'],
-                                                      public_comment="Assignment was verified as incorrect by another user.")
-                        msg.warn(f'Rejected assignment {event.assignment.tasks[i].input_values["assignment_id"]}')
+                                                      public_comment=self.conf['messages']['solution'])
+                        msg.warn(f"Rejected assignment {event.assignment.tasks[i].input_values['assignment_id']}")
 
                     # If performer verified the task as correct, accept original assignment and don't forward task
                     if solution in self.accept:
 
                         self.client.accept_assignment(assignment_id=event.assignment.tasks[i].input_values['assignment_id'],
-                                                    public_comment="Assignment was verified correct by another user.")
-                        msg.good(f'Accepted assignment {event.assignment.tasks[i].input_values["assignment_id"]}')
+                                                      public_comment=self.conf['messages']['solution'])
+                        msg.warn(f"Accepted assignment {event.assignment.tasks[i].input_values['assignment_id']}")
 
                     # If no forward pool was configured, submit task without forwarding/accepting/rejecting
                     if solution in self.dont_forward:
 
                         msg.good(f'Received a submitted assignment with output "{solution}"')
 
                     # Else, forward task according to configuration
                     if solution in self.forward_pools:
 
                         try:
                             task = toloka.Task(
-                                pool_id = self.forward_pools[solution].pool.id,
+                                pool_id=self.forward_pools[solution].pool.id,
                                 input_values=event.assignment.tasks[i].input_values,
                                 unavailable_for=self.forward_pools[solution].blocklist
                             )
                             self.tasks_to_forward[solution].append(task)
 
                         # Catch errors
                         except toloka.exceptions.ValidationApiError:
@@ -321,54 +274,56 @@
 
             if tasks_list:
                 
                 # Add tasks to defined pools
                 self.client.create_tasks(tasks_list, allow_defaults=True, open_pool=True)
 
                 # Print status if any tasks were forwarded on this call
-                msg.good(f"Successfully forwarded {len(tasks_list)} {'tasks' if len(tasks_list) > 1 else 'task'}")
+                msg.good(f"Successfully forwarded {len(tasks_list)} "
+                         f"{'tasks' if len(tasks_list) > 1 else 'task'}")
 
             # Tasks currently in lists have been forwarded, so reset lists
             self.tasks_to_forward = collections.defaultdict(list)
             tasks_list = []
 
-        # Process tasks that come from aggregation
+        # Continue by processing results from Aggregate or VerifyPolygon actions, in which case
+        # the list of incoming objects named "events" consists of dictionaries.
         if all(isinstance(x, dict) for x in events):
 
-            # Loop over the list of incoming AssignmentEvent objects
+            # Loop over the list of incoming dictionaries
             for event in events:
 
                 solution = event['label']
 
                 # If performer verified the task as incorrect, reject the original assignment
                 # and, if configured in source pool under "on_reject", re-add the task to the pool
                 if solution in self.reject:
 
-                    self.client.reject_assignment(assignment_id=event["input_data"]["assignment_id"],
-                                                  public_comment="Assignment was verified incorrect by another user.")
-                    msg.warn(f'Rejected assignment {event["input_data"]["assignment_id"]}')
+                    self.client.reject_assignment(assignment_id=event['input_data']['assignment_id'],
+                                                  public_comment=event['message'])
+                    msg.warn(f"Rejected assignment {event['input_data']['assignment_id']}")
 
                 # If performer verified the task as correct, accept original assignment and don't forward task
                 if solution in self.accept:
 
-                    self.client.accept_assignment(assignment_id=event["input_data"]["assignment_id"],
-                                                  public_comment="Assignment was verified correct by another user.")
-                    msg.good(f'Accepted assignment {event["input_data"]["assignment_id"]}')
+                    self.client.accept_assignment(assignment_id=event['input_data']['assignment_id'],
+                                                  public_comment=event['message'])
+                    msg.warn(f"Accepted assignment {event['input_data']['assignment_id']}")
 
                 # If no forward pool was configured, submit task without forwarding/accepting/rejecting
                 if solution in self.dont_forward:
 
                     msg.good(f'Received a submitted assignment with output "{solution}"')
 
                 # Else, forward task according to configuration
                 if solution in self.forward_pools:
 
                     try:
                         task = toloka.Task(
-                            pool_id = self.forward_pools[solution].pool.id,
+                            pool_id=self.forward_pools[solution].pool.id,
                             input_values=event['input_data'],
                             unavailable_for=self.forward_pools[solution].blocklist
                         )
                         self.tasks_to_forward[solution].append(task)
 
                     # Catch errors
                     except toloka.exceptions.ValidationApiError:
@@ -386,144 +341,303 @@
 
             if tasks_list:
                 
                 # Add tasks to defined pools
                 self.client.create_tasks(tasks_list, allow_defaults=True, open_pool=True)
 
                 # Print status if any tasks were forwarded on this call
-                msg.good(f"Successfully forwarded {len(tasks_list)} {'tasks' if len(tasks_list) > 1 else 'task'}")
+                msg.good(f"Successfully forwarded {len(tasks_list)} "
+                         f"{'tasks' if len(tasks_list) > 1 else 'task'}")
 
             # Tasks currently in lists have been forwarded, so reset lists
             self.tasks_to_forward = collections.defaultdict(list)
             tasks_list = []
 
 
 class SeparateBBoxes:
     """
-    This class defines an action for separating an image with several bounding boxes to several tasks with one
-    bounding box per image.
+    This class defines an action for separating an image with several bounding boxes to several
+    tasks with one bounding box per image.
 
     Parameters:
         target: CrowdsourcingTask to which the new tasks will be created
         configuration: A string object that defines a path to a YAML file with configuration.
-        add_label: A string object of a label that will be given to the created bounding boxes. Optional parameter.
+        add_label: A string object of a label that will be given to the created bounding boxes.
+                   Optional parameter.
 
     Returns:
         None
     """
 
     def __init__(self, target, configuration, add_label=False):
         self.target = target
         self.client = self.target.client
         self.conf = read_configuration(configuration)
-        self.name = self.conf["name"]
+        self.name = self.conf['name']
         self.add_label = add_label
 
-        if "input_file" in self.conf["data"]:
-            self.input_file = self.conf["data"]["input_file"]
+        try:
+
+            image = self.conf['data']['image']
+            outlines = self.conf['data']['bboxes']
+
+        except KeyError:
+
+            msg.fail(f"The configuration file for the SeparateBboxes Action named {self.name} does not contain "
+                     f"the names of the variables that contain the images and bounding boxes. Please ensure that "
+                     f"the top-level key 'data' contains keys 'image' and 'bboxes', whose values provide the "
+                     f"variable names.", exits=1)
 
-    def __call__(self, event: Union[AssignmentEvent, dict, List[AssignmentEvent]]=None) -> None:
+        if 'file' in self.conf['data']:
 
-        # If the object is registered with an observer, use data from AssignmentEvents or the incoming dict to create new tasks
+            self.input_file = self.conf['data']['file']
+
+    def __call__(self, event: Union[AssignmentEvent, dict, List[AssignmentEvent]] = None) -> None:
+
+        # If the object is registered with an observer, use data from AssignmentEvents or the incoming dict to create
+        # new tasks
         if event:
 
             if type(event) == AssignmentEvent:
 
                 msg.info(f"Creating new tasks in pool {self.target.name} with action {self.name}")
 
                 if self.add_label:
 
                     for i in range(len(event.assignment.tasks)):
 
                         new_tasks = [toloka.Task(pool_id=self.target.pool.id,
-                                                input_values={"image": event.assignment.tasks[i].input_values["image"], "outlines": [bbox]},
-                                                unavailable_for=self.target.blocklist) 
-                                        for bbox in [dict(x, **{'label': self.add_label}) for x in event.assignment.solutions[i].output_values["outlines"]] ]
+                                                 input_values={image: event.assignment.tasks[i].input_values[image],
+                                                               outlines: [bbox]},
+                                                 unavailable_for=self.target.blocklist)
+                                     for bbox in [dict(x, **{'label': self.add_label})
+                                                  for x in event.assignment.solutions[i].output_values[outlines]]]
 
                         self.client.create_tasks(new_tasks, allow_defaults=True, open_pool=True)
 
                 else:
 
                     for i in range(len(event.assignment.tasks)):
 
                         new_tasks = [toloka.Task(pool_id=self.target.pool.id,
-                                                input_values={"image": event.assignment.tasks[i].input_values["image"], "outlines": [bbox]},
-                                                unavailable_for=self.target.blocklist) 
-                                        for bbox in event.assignment.solutions[i].output_values["outlines"] ]
+                                                 input_values={image: event.assignment.tasks[i].input_values[image],
+                                                               outlines: [bbox]},
+                                                 unavailable_for=self.target.blocklist)
+                                     for bbox in event.assignment.solutions[i].output_values[outlines]]
 
                         self.client.create_tasks(new_tasks, allow_defaults=True, open_pool=True)
 
             elif type(event) == List[AssignmentEvent]:
 
                 msg.info(f"Creating new tasks in pool {self.target.name} with action {self.name}")
 
                 if self.add_label:
 
                     for e in event:
 
                         for i in range(len(e.assignment.tasks)):
 
                             new_tasks = [toloka.Task(pool_id=self.target.pool.id,
-                                                    input_values={"image": e.assignment.tasks[i].input_values["image"], "outlines": [bbox]},
-                                                    unavailable_for=self.target.blocklist) 
-                                            for bbox in [dict(x, **{'label': self.add_label}) for x in e.assignment.solutions[i].output_values["outlines"]] ]
+                                                     input_values={image: e.assignment.tasks[i].input_values[image],
+                                                                   outlines: [bbox]},
+                                                     unavailable_for=self.target.blocklist)
+                                         for bbox in [dict(x, **{'label': self.add_label})
+                                                      for x in e.assignment.solutions[i].output_values[outlines]]]
 
                             self.client.create_tasks(new_tasks, allow_defaults=True, open_pool=True)
 
                 else:
 
                     for e in event:
 
                         for i in range(len(e.assignment.tasks)):
 
                             new_tasks = [toloka.Task(pool_id=self.target.pool.id,
-                                                    input_values={"image": e.assignment.tasks[i].input_values["image"], "outlines": [bbox]},
-                                                    unavailable_for=self.target.blocklist) 
-                                            for bbox in e.assignment.solutions[i].output_values["outlines"] ]
+                                                     input_values={image: e.assignment.tasks[i].input_values[image],
+                                                                   outlines: [bbox]},
+                                                     unavailable_for=self.target.blocklist)
+                                         for bbox in e.assignment.solutions[i].output_values[outlines]]
 
                             self.client.create_tasks(new_tasks, allow_defaults=True, open_pool=True)
 
             # If input comes from a forward action, it is in the form of a dictionary:
             elif type(event) == dict:
 
                 msg.info(f"Creating new tasks in pool {self.target.name} with action {self.name}")
 
                 if self.add_label:
 
                     new_tasks = [toloka.Task(pool_id=self.target.pool.id,
-                                            input_values={"image": event["input_data"]["image"], "outlines": [bbox]},
-                                            unavailable_for=self.target.blocklist) 
-                                        for bbox in [dict(x, **{'label': self.add_label}) for x in event['input_data']['outlines']] ]
+                                             input_values={image: event['input_data'][image],
+                                                           outlines: [bbox]},
+                                             unavailable_for=self.target.blocklist)
+                                 for bbox in [dict(x, **{'label': self.add_label})
+                                              for x in event['input_data'][outlines]]]
 
                     self.client.create_tasks(new_tasks, allow_defaults=True, open_pool=True)
 
                 else:
 
                     new_tasks = [toloka.Task(pool_id=self.target.pool.id,
-                                            input_values={"image": event["input_data"]["image"], "outlines": [bbox]},
-                                            unavailable_for=self.target.blocklist) 
-                                        for bbox in event['input_data']['outlines'] ]
+                                             input_values={image: event['input_data'][image],
+                                                           outlines: [bbox]},
+                                             unavailable_for=self.target.blocklist)
+                                 for bbox in event['input_data'][outlines]]
 
                     self.client.create_tasks(new_tasks, allow_defaults=True, open_pool=True)
 
         # If the object is called without AssignmentEvents, the action starts the pipeline and
         # input data should be read from a file 
         else:
         
             input_df = pd.read_csv(self.input_file, sep="\t", index_col=False)
 
             msg.info(f"Creating new tasks in pool {self.target.name} with action {self.name}")
 
             if self.add_label:
 
-                input_df["outlines"] = input_df["outlines"].apply(lambda x: json.loads(x))
-                input_df["outlines"] = input_df["outlines"].apply(lambda x: [dict(y, **{'label': self.add_label}) for y in x])
+                input_df[outlines] = input_df[outlines].apply(lambda x: json.loads(x))
+                input_df[outlines] = input_df[outlines].apply(lambda x:
+                                                              [dict(y, **{'label': self.add_label}) for y in x])
 
             for i, task in input_df.iterrows():
 
                 new_tasks = [toloka.Task(pool_id=self.target.pool.id,
-                                        input_values={"image": task["image"], "outlines": [bbox]},
-                                        unavailable_for=self.target.blocklist)
-                            for bbox in task["outlines"]
-                ]
+                                         input_values={image: task[image], outlines: [bbox]},
+                                         unavailable_for=self.target.blocklist)
+                             for bbox in task[outlines]]
                 
                 self.client.create_tasks(new_tasks, allow_defaults=True, open_pool=True)
+
+
+class VerifyPolygon:
+    """
+    This class defines an action for verifying that the polygons created by crowdsourced workers
+    are valid, that is, they do not contain self-intersecting edges. This means that the lines of a
+    polygon should not cross each other at any point.
+
+    """
+    def __init__(self, configuration, task, forward=None):
+        """
+        This function initialises the polygon verification mechanism.
+
+        Parameters:
+            configuration: A string object that defines a path to a YAML file with configuration.
+            task: The CrowdsourcingTask object whose results should be validated.
+
+        Returns:
+             None
+        """
+        self.conf = read_configuration(configuration)
+        self.name = self.conf['name']
+        self.labels = True if 'labels' in self.conf else False
+        self.task = task
+        self.client = self.task.client
+        self.forward = forward
+
+    def __call__(self, events: List[AssignmentEvent]) -> None:
+
+        # Create a placeholder list for data to be forwarded
+        forward_data = []
+
+        # Loop over the list of incoming AssignmentEvent objects. These consist of task suites
+        # completed by the crowdsourced workers.
+        for event in events:
+
+            # Set up a flag for tracking the presence of invalid polygons
+            valid = True
+            message = "The outlines you submitted were evaluated as valid. Thank you!"
+
+            # Zip and iterate over tasks and solutions in each event
+            for task, solution in zip(event.assignment.tasks, event.assignment.solutions):
+
+                # Retrieve the answer (the bounding box)
+                answer = solution.output_values[self.conf['data']]
+
+                # Retrieve all polygons
+                polygons = [p for p in answer if p['shape'] == 'polygon']
+
+                # Loop over the polygons
+                for p in polygons:
+
+                    # Retrieve coordinate pairs for each point of the polygon
+                    coords = [(c['left'], c['top']) for c in p['points']]
+
+                    # Create a Polygon using shapely and check if the polygon contains
+                    # self-intersecting edges using the is_valid attribute
+                    polygon = Polygon(coords).is_valid
+
+                    # If a polygon is not valid, set the flag tracking invalid polygons to True
+                    if not polygon:
+
+                        valid = False
+                        message = "Your task was rejected, because it contained polygons " \
+                                  "with lines that cross each other."
+
+                # Check if the labels of polygons and rectangles should be checked
+                if self.labels:
+
+                    # Retrieve all rectangles, combine them with polygons and count labels
+                    rectangles = [p for p in answer if p['shape'] == 'rectangle']
+                    labels = collections.Counter([o['label'] for o in rectangles + polygons])
+
+                    # Loop over the criteria defined for the labels
+                    for label in self.conf['labels']:
+
+                        # Check if the label is a string, which means the label must be present
+                        if type(label) == str:
+
+                            if label not in labels:
+
+                                valid = False
+                                message = f"Your task was rejected, because it did not contain " \
+                                          f"any bounding boxes with the label {label}."
+
+                        # Next, check if the label is a dictionary, which defines a number of labels
+                        if type(label) == dict:
+
+                            # Loop over the dictionary to ensure that the labels are present and
+                            # their number is correct.
+                            for k, v in label.items():
+
+                                # Check the labels against the Counter object 'labels'
+                                if k not in labels:
+
+                                    valid = False
+                                    message = f"Your task was rejected, because it did not " \
+                                              f"contain any bounding boxes with the label {k}."
+
+                                if k in labels:
+
+                                    if labels[k] > v:
+
+                                        valid = False
+                                        message = f"Your task was rejected, because it contained " \
+                                                  f"too many bounding boxes for the label {k} " \
+                                                  f"(max. {v})."
+
+                                    if labels[k] < v:
+
+                                        valid = False
+                                        message = f"Your task was rejected, because it did not " \
+                                                  f"contain enough bounding boxes for the label " \
+                                                  f"{k} ({v} were expected)."
+
+                # Create a dictionary containing the data to be forwarded
+                result = {'input_data': task.input_values,
+                          'label': valid,
+                          'message': message}
+
+                # Add the assignment ID into the input data dictionary. This information is required
+                # by the Forward action for rejection/acceptance.
+                result['input_data'].update({'assignment_id': event.assignment.id})
+
+                # Add the bounding boxes stored under the variable to the input data, in case they
+                # are forwarded further. Store them under the key data/output defined in the YAML
+                # configuration for this Action.
+                result['input_data'].update({self.conf['data']: answer})
+
+                # Append the event dictionary to the list to be forwarded
+                forward_data.append(result)
+
+        # Forward the tasks to the Forward object
+        self.forward(forward_data)
```

### Comparing `abulafia-0.1.9/src/abulafia/functions/core_functions.py` & `abulafia-0.2.1/src/abulafia/functions/core_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,35 +216,48 @@
         # Print status message
         raise_error(f'Failed to create tasks on Toloka due to a validation error. Check '
                     f'the input data, configuration file and see the error message above! '
                     f'Note that this error was raised by {kind} tasks, so see the relevant '
                     f'section of the configuration file.')
 
 
-def check_io(configuration: dict, expected_input: set, expected_output: set):
+def check_io(configuration: dict,
+             expected_input: set,
+             expected_output: set):
+    """
+    This function checks the inputs and outputs defined in the YAML configuration against those allowed in the
+    crowdsourcing task specification.
+
+    configuration: A dictionary containing the configuration for a crowdsourcing task.
+    expected_input: A set of input data types defined in the crowdsourcing task specification.
+    expected_output: A set of output data types defined in the crowdsourcing task specification.
+
+    Returns:
+         Four dictionaries mapping the input variables to Toloka data specifications.
+    """
 
     # Read input and output data and create data specifications
     data_in = {k: data_spec[v] for k, v in configuration['data']['input'].items()}
     data_out = {k: data_spec[v] for k, v in configuration['data']['output'].items()}
 
     # Create a dictionary mapping input data types to variable names.
     input_data = {v: k for k, v in configuration['data']['input'].items()}
 
     # Raise error if the expected input data types have been provided
-    if not set(input_data.keys()) == expected_input:
+    if not set(input_data.keys()).issubset(expected_input):
 
         raise_error(f'Could not find the expected input types ({", ".join(expected_input)}) for '
                     f'{configuration["name"]}. Please check the configuration under the '
                     f'key data/input.')
 
     # Create a dictionary mapping output data types to variable names.
     output_data = {v: k for k, v in configuration['data']['output'].items()}
 
     # Raise error if the expected input data types have been provided
-    if not set(output_data.keys()) == expected_output:
+    if not set(output_data.keys()).issubset(expected_output):
 
         raise_error(f'Could not find the expected output types ({", ".join(expected_output)}) for '
                     f'{configuration["name"]}. Please check the configuration under the '
                     f'key data/output.')
 
     return data_in, data_out, input_data, output_data
 
@@ -533,15 +546,15 @@
         task_sequence: a list of CrowdsourcingTask objects and/or actions.
 
     Returns:
          Prints a table with information on all pools/actions to standard output.
     """
 
     # Set up headers and a placeholder for data
-    header = ('Name', 'Input', 'Output', 'Pool ID', 'Project ID', 'Pool type')
+    header = ('Name', 'Input', 'Output', 'Pool ID', 'Project ID', 'Type')
     data = []
 
     # Loop over the tasks
     for task in task_sequence:
 
         # Check if training has been defined
         try:
```

### Comparing `abulafia-0.1.9/src/abulafia/observers/observers.py` & `abulafia-0.2.1/src/abulafia/observers/observers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Import libraries
 from wasabi import Printer
 from toloka.streaming.observer import BaseObserver
 from toloka.client.analytics_request import UniqueWorkersCountPoolAnalytics, ActiveWorkersByFilterCountPoolAnalytics, \
     SubmittedAssignmentsCountPoolAnalytics
 from toloka.client.operations import Operation
-from toloka.client.exceptions import DoesNotExistApiError
+from toloka.client.exceptions import DoesNotExistApiError, IncorrectActionsApiError
 
 
 # Set up Printer
 msg = Printer(pretty=True, timestamp=True, hide_animation=True)
 
 
 class AnalyticsObserver(BaseObserver):
@@ -71,14 +71,19 @@
                                 pass
 
                             except DoesNotExistApiError:
 
                                 # If a training is found, but it cannot be closed, raise warning
                                 msg.warn(f"Attempted to close a training for pool {self.pool.id} that does not exist")
 
+                            # TODO Possible hotfix for crashing pipelines
+                            except IncorrectActionsApiError:
+
+                                pass
+
                     if response['request']['name'] == 'unique_workers_count' and not self.limit_reached:
 
                         # Check if number of submissions has changed: only print update 
                         # if there has been a change.
                         if response['result'] != self.prev_result:
                             
                             msg.info(f'{response["result"]} workers submitted to pool {self.pool.id}')
```

### Comparing `abulafia-0.1.9/src/abulafia/task_specs/core_task.py` & `abulafia-0.2.1/src/abulafia/task_specs/core_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,24 +57,29 @@
         self.train_tasks = None  # Placeholder for training tasks
         self.tasks = None  # Placeholder for main tasks
         self.results = None  # Placeholder for results
         self.is_complete = False  # Is the Task complete or not?
         self.skill = False  # Does the Task provide or require a skill?
         self.exam = False  # Is this Task an exam?
         self.test = True if kwargs and kwargs['test'] else False  # Are we running a test?
+        self.verify = True if 'verify' in self.data_conf and self.data_conf['verify'] else False
 
         # See if users should be banned from the pool and check that blocklist is configured correctly
         try:
 
-            self.blocklist = list(pd.read_csv(self.pool_conf['blocklist'], sep="\t")["user_id"]) \
+            self.blocklist = list(pd.read_csv(self.pool_conf['blocklist'], sep='\t')['user_id'].dropna()) \
                 if 'blocklist' in self.pool_conf.keys() else []
 
+            if len(self.blocklist) > 0:
+
+                msg.info(f'Successfully loaded a blocklist with {len(self.blocklist)} user IDs.')
+
         except KeyError:
 
-            msg.warn(f"Could not find the column 'user_id' in the blocklist.", exits=1)
+            msg.fail(f"Could not find the column 'user_id' in the blocklist.", exits=1)
 
         # Print status message
         msg.info(f'The unique ID for this object ({self.name}) is {self.task_id}')
 
         # Get requester information unless we're running a test
         if not self.test:
 
@@ -112,47 +117,52 @@
             # Create tasks and add them to the pool
             self.tasks = create_tasks(self, data)
 
             if not self.test:
 
                 add_tasks(self, self.tasks)
 
-    def __call__(self, in_obj, **options):
+    def __call__(self, in_obj):
 
         # Check that the input object is a list of AssignmentEvent objects
         if type(in_obj) == list and all(isinstance(item, AssignmentEvent) for item in in_obj):
 
             # Check the status of AssignmentEvent objects. These AssignmentEvent objects correspond
             # to task suites on Toloka. Their status may be accepted, rejected, submitted, etc.
             for event in in_obj:
 
                 # If the event type is accepted or submitted, create new tasks in current pool
                 if event.event_type.value in ['ACCEPTED', 'SUBMITTED']:
 
-                    # Create new Task objects
-                    new_tasks = [Task(pool_id=self.pool.id,
-                                      overlap=self.pool_conf['defaults']['default_overlap_for_new_tasks'],
-                                      input_values={k: v for k, v in task.input_values.items()},
-                                      unavailable_for=self.blocklist
-                                      )
-                                 for task, solution
-                                 in zip(event.assignment.tasks,
-                                        event.assignment.solutions)]
-
-                    # If the assignments are for a verification pool, add the output values to the input of
-                    # the new task and make the verification task unavailable for the performer
-                    if options and 'verify' in options:
-
-                        new_tasks = [Task(pool_id=self.pool.id,
-                                          overlap=self.pool_conf['defaults']['default_overlap_for_new_tasks'],
-                                          input_values={**task.input_values,
-                                                        **solution.output_values,
-                                                        'assignment_id': event.assignment.id},
-                                          unavailable_for=[*self.blocklist, event.assignment.user_id])
-                                     for task, solution in zip(event.assignment.tasks, event.assignment.solutions)]
+                    # If the assignments are intended to be verified by other users, add the output
+                    # values to the input of the new task and make the verification task unavailable
+                    # for the worker who originally submitted it.
+                    if self.verify:
+
+                        new_tasks = [Task(
+                            pool_id=self.pool.id,
+                            overlap=self.pool_conf['defaults']['default_overlap_for_new_tasks'],
+                            input_values={**task.input_values,
+                                          **solution.output_values,
+                                          'assignment_id': event.assignment.id},
+                            unavailable_for=[*self.blocklist, event.assignment.user_id])
+                            for task, solution in
+                            zip(event.assignment.tasks, event.assignment.solutions)]
+
+                    else:
+
+                        # Create new Task objects
+                        new_tasks = [Task(
+                            pool_id=self.pool.id,
+                            overlap=self.pool_conf['defaults']['default_overlap_for_new_tasks'],
+                            input_values={k: v for k, v in task.input_values.items()},
+                            unavailable_for=self.blocklist)
+                            for task, solution
+                            in zip(event.assignment.tasks,
+                                   event.assignment.solutions)]
 
                     # Add Tasks and open the pool
                     self.client.create_tasks(tasks=new_tasks, open_pool=True)
 
                     # Print status messages
                     msg.good(f'Received {len(new_tasks)} {event.event_type.value.lower()} tasks '
                              f'from pool {event.assignment.pool_id}')
@@ -372,15 +382,15 @@
 
                     # Link training pool and retrieve minimum performance value
                     self.pool.set_training_requirement(training_pool_id=self.training.id,
                                                        **self.pool_conf['training'])
 
                 except KeyError:
 
-                    msg.warn(f"Could not find the key 'training' under the main pool configuration. "
+                    msg.fail(f"Could not find the key 'training' under the main pool configuration. "
                              f"Define the key 'training' and place a key/value pair with the key "
                              f"'training_passing_skill_value' under 'training' to link the training "
                              f"and main pools. This key is used to set the criteria for passing "
                              f"the training, e.g. training_passing_skill_value: 70", exits=1)
 
             # Print status message
             msg.good(f'Successfully configured a new main pool')
@@ -641,15 +651,15 @@
                 if 'user_agent_type' in self.pool_conf['filter'].keys():
 
                     # Check if only one agent type has been defined
                     if len(self.pool_conf['filter']['user_agent_type']) == 1:
 
                         # Create filter
                         agent = (toloka.filter.UserAgentType ==
-                                   self.pool_conf['filter']['user_agent_type'][0].upper())
+                                 self.pool_conf['filter']['user_agent_type'][0].upper())
 
                         # Check for existing filters and set
                         self.pool.filter = set_filter(filters=self.pool.filter,
                                                       new_filters=agent)
 
                     # Check if more than one user agent has been defined
                     if len(self.pool_conf['filter']['user_agent_type']) > 1:
```

### Comparing `abulafia-0.1.9/src/abulafia/task_specs/pipeline.py` & `abulafia-0.2.1/src/abulafia/task_specs/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,29 @@
 
 
 class TaskSequence:
     """
     This class allows defining a sequence of crowdsourcing tasks on Toloka.
 
     """
-    def __init__(self, sequence, client):
+    def __init__(self, sequence, client, **kwargs):
         """
         This function initialises the TaskSequence class.
 
         Parameters:
             sequence: A list of objects that inherit from the CrowdsourcingTask class.
             client: A TolokaClient object with valid credentials.
+            kwargs: Keywords and arguments for additional settings.
         """
         # Set up attributes
         self.complete = False       # Tracks if all tasks have been completed
         self.sequence = sequence    # A list of CrowdsourcingTask objects
         self.client = client        # A Toloka Client object
         self.pipeline = None        # Placeholder for a Toloka Pipeline object
+        self.no_exit = True if 'no_exit' in kwargs and kwargs['no_exit'] else False     # Do not exit after finishing
 
         msg.info(f'Creating a task sequence')
 
         # Verify that connections between tasks have been specified in the configuration
         verify_connections(self.sequence)
 
         msg.info(f'Printing tasks, inputs and outputs')
@@ -97,75 +99,65 @@
 
                     if self.client.get_pool(pool_id=task.pool.id).is_closed():
 
                         status.append(True)
 
                     else:
 
-                        self.client.close_pool(pool_id=task.pool.id)
+                        # Check pool status again
+                        if not self.client.get_pool(pool_id=task.pool.id).is_closed():
 
-                        msg.info(f'Closed pool with ID {task.pool.id}')
+                            self.client.close_pool(pool_id=task.pool.id)
+
+                            msg.info(f'Closed pool with ID {task.pool.id}')
 
                 # Check if there is a training pool that should be closed
                 if hasattr(task, 'training') and task.training is not None:
 
                     if self.client.get_pool(pool_id=task.training.id).is_closed():
 
                         status.append(True)
 
                     else:
 
-                        self.client.close_pool(pool_id=task.training.id)
+                        # Check status again
+                        if not self.client.get_pool(pool_id=task.training.id).is_closed():
+
+                            self.client.close_pool(pool_id=task.training.id)
 
-                        msg.info(f'Closed pool with ID {task.training.id}')
+                            msg.info(f'Closed pool with ID {task.training.id}')
 
             for action in (a for a in self.sequence if hasattr(a, 'aggregator')):
 
-                if action.complete == True:
+                if action.complete:
                     
                     status.append(True)
 
             if all(status):
 
-                # Wait for a minute to ensure that no new tasks are added to pools in the pipeline
+                # Wait for 3 minutes to ensure that no new tasks are added to pools in the pipeline
                 # before ending the task sequence
-                time.sleep(60)
+                time.sleep(90)
 
                 if all(status):
 
                     self.complete = True
 
                     msg.good(f'Successfully completed the task sequence')
 
         # Check the outputs
         if self.complete:
 
-            exit()
-
-            # Check if tasks are supposed to output the results
-            for task in self.sequence:
-
-                if hasattr(task, 'pool'):
-
-                    # Get the output DataFrame for each task; assign under 'output_data'
-                    task.output_data = self.client.get_assignments_df(pool_id=task.pool.id)
-
-                    # Check if the output should be written to disk
-                    try:
-
-                        if task.conf['actions'] is not None and 'output' in task.conf['actions']:
-
-                            # Write the DataFrame to disk
-                            task.output_data.to_csv(f'{task.name}_{task.pool.id}.csv')
+            if not self.no_exit:
 
-                            msg.good(f'Wrote data for task {task.name} ({task.pool.id}) to disk.')
+                exit()
 
-                    except KeyError:
+            if self.no_exit:
 
-                        pass
+                pass
 
     def create_pipeline(self):
 
         # Create an asyncronous client
         async_client = AsyncMultithreadWrapper(self.client)
 
         # Loop over the tasks and create an AssignmentsObserver object for each task. Exam tasks
```

### Comparing `abulafia-0.1.9/src/abulafia.egg-info/SOURCES.txt` & `abulafia-0.2.1/src/abulafia.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+src/outtakes.py
 src/abulafia/__init__.py
 src/abulafia.egg-info/PKG-INFO
 src/abulafia.egg-info/SOURCES.txt
 src/abulafia.egg-info/dependency_links.txt
 src/abulafia.egg-info/requires.txt
 src/abulafia.egg-info/top_level.txt
 src/abulafia/actions/__init__.py
@@ -13,8 +14,10 @@
 src/abulafia/functions/__init__.py
 src/abulafia/functions/core_functions.py
 src/abulafia/observers/__init__.py
 src/abulafia/observers/observers.py
 src/abulafia/task_specs/__init__.py
 src/abulafia/task_specs/core_task.py
 src/abulafia/task_specs/pipeline.py
-src/abulafia/task_specs/task_specs.py
+src/abulafia/task_specs/task_specs.py
+tests/test_functions.py
+tests/test_tasks.py
```

