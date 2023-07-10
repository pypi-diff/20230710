# Comparing `tmp/Perfole-0.0.1.tar.gz` & `tmp/Perfole-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Perfole-0.0.1.tar", last modified: Mon Jul 10 11:05:00 2023, max compression
+gzip compressed data, was "Perfole-0.0.2.tar", last modified: Mon Jul 10 12:01:57 2023, max compression
```

## Comparing `Perfole-0.0.1.tar` & `Perfole-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 11:05:00.317318 Perfole-0.0.1/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1368 2023-07-10 11:05:00.317193 Perfole-0.0.1/PKG-INFO
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 11:05:00.316526 Perfole-0.0.1/Perfole/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    17442 2023-07-09 21:19:26.000000 Perfole-0.0.1/Perfole/Perfole.py
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.1/Perfole/__init__.py
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 11:05:00.316998 Perfole-0.0.1/Perfole.egg-info/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1368 2023-07-10 11:05:00.000000 Perfole-0.0.1/Perfole.egg-info/PKG-INFO
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      193 2023-07-10 11:05:00.000000 Perfole-0.0.1/Perfole.egg-info/SOURCES.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-10 11:05:00.000000 Perfole-0.0.1/Perfole.egg-info/dependency_links.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-10 11:05:00.000000 Perfole-0.0.1/Perfole.egg-info/top_level.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1177 2023-07-10 11:02:15.000000 Perfole-0.0.1/README.md
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.1/license.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-10 11:05:00.317358 Perfole-0.0.1/setup.cfg
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      433 2023-07-10 11:04:24.000000 Perfole-0.0.1/setup.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:01:57.797309 Perfole-0.0.2/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:01:57.797170 Perfole-0.0.2/PKG-INFO
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:01:57.796251 Perfole-0.0.2/Perfole/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12927 2023-07-10 11:40:47.000000 Perfole-0.0.2/Perfole/Perfole.py
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.2/Perfole/__init__.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:01:57.796977 Perfole-0.0.2/Perfole.egg-info/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/PKG-INFO
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/SOURCES.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/dependency_links.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/requires.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/top_level.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1183 2023-07-10 11:07:54.000000 Perfole-0.0.2/README.md
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.2/license.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-10 12:01:57.797355 Perfole-0.0.2/setup.cfg
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      469 2023-07-10 11:30:25.000000 Perfole-0.0.2/setup.py
```

### Comparing `Perfole-0.0.1/PKG-INFO` & `Perfole-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.1
+Version: 0.0.2
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 
@@ -45,19 +45,19 @@
 
 ## Results
 Stop() method will return list of caught actions. For cloud reporting functionality visit https://perfole.com
 
 
 ## UniqueIdentifier parameter
 UniqueIdentifier parameter must be given when start/end points are in different threads:
-
+```
 PERFORMANCE_TEST.StartAction(name="myAction", uniqueIdentifier= "myIdentifier")
 ...
 PERFORMANCE_TEST.EndAction(name="myAction", uniqueIdentifier= "myIdentifier")
-
+```
```

### Comparing `Perfole-0.0.1/Perfole/Perfole.py` & `Perfole-0.0.2/Perfole/Perfole.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,24 +9,27 @@
     actionsBeforeCalculation ={}
     calculatedActions ={}
     calculatedActionsPublish =[]
     execution_start_time=0
     execution_end_time=0#time.time()
     uniqueRandom = "224335oho"
     actionPoints = 0
+    lock=threading.Lock()
 
     @staticmethod
     def Start(measure):
             if(measure):
                 try:
                     PERFORMANCE_TEST.clearResult()
                     PERFORMANCE_TEST.resolveArguments(measure)
                     PERFORMANCE_TEST.execution_start_time = round(time.time() * 1000)
                 except:
                     PERFORMANCE_TEST.clearResult()
+            else:
+                PERFORMANCE_TEST.argumentsValue = {'shouldMeasure':False}
     
     @staticmethod
     def Stop(publish=False,apiKey = "",version = "",machineName = ""):
         try:
             if (PERFORMANCE_TEST.argumentsValue['shouldMeasure']):
                 if (len(PERFORMANCE_TEST.actionsBeforeCalculation) == 0):
                     PERFORMANCE_TEST.clearResult()
@@ -42,71 +45,49 @@
 
                     if (machineName != ""):
                         PERFORMANCE_TEST.argumentsValue['machineName'] = machineName
                     else:
                         try:
                             import os
                             PERFORMANCE_TEST.argumentsValue['machineName'] = os.uname()[1]#Environment.MachineName
-                        except:# InvalidOperationException:
+                        except:
                             PERFORMANCE_TEST.argumentsValue['machineName'] = "Unknown"
                     pub = PERFORMANCE_TEST.publishResult(apiKey)
                     if (pub):
                         return PERFORMANCE_TEST.calculatedActions
                     else:
                         return []
                 else:
                     PERFORMANCE_TEST.argumentsValue['shouldMeasure'] = False
                     return PERFORMANCE_TEST.calculatedActions
         except Exception as e:
-            print(e)
             PERFORMANCE_TEST.clearResult()
         return []
 
     @staticmethod
     def ActionStart(name, additionalInfo = "", uniqueIdentifier = ""):
         try:
             if(PERFORMANCE_TEST.argumentsValue['shouldMeasure'] and PERFORMANCE_TEST.actionPoints < 200):
-                #if (uniqueIdentifier == ""):
-                    # if (Thread.CurrentThread.Name != null):
-                    #     if (Thread.CurrentThread.Name.Contains("Worker")):
-                    #         uniqueIdentifier = uniqueRandom
-                    #     else:
-                    #         uniqueIdentifier = Thread.CurrentThread.ManagedThreadId.ToString()
-                    # else:
-                    #     uniqueIdentifier = Thread.CurrentThread.ManagedThreadId.ToString()
                 if(uniqueIdentifier==""):
-                    uniqueIdentifier=threading.current_thread().name#os.getpid()
-                print('uniqueispod')
-                print(uniqueIdentifier)
+                    uniqueIdentifier=threading.current_thread().name
                 PERFORMANCE_TEST.writeToActionsBeforeCalculation(
                     "start",
                     name,
                     additionalInfo,
                     uniqueIdentifier
                 )
         except Exception as e:
-            print(e)
             PERFORMANCE_TEST.clearResult()
     
     @staticmethod
     def ActionEnd(name, additionalInfo = "", uniqueIdentifier = ""):
         try:
             if (PERFORMANCE_TEST.argumentsValue['shouldMeasure'] and PERFORMANCE_TEST.actionPoints < 200):
-                #if (uniqueIdentifier == ""):
-                    # if (Thread.CurrentThread.Name != null):
-                    #     if (Thread.CurrentThread.Name.Contains("Worker")):
-                    #         uniqueIdentifier = uniqueRandom
-                    #     else:
-                    #         uniqueIdentifier = Thread.CurrentThread.ManagedThreadId.ToString()
-                    # else:
-                    #     uniqueIdentifier = Thread.CurrentThread.ManagedThreadId.ToString()
                 if(uniqueIdentifier==""):
                     uniqueIdentifier=threading.current_thread().name
-                print('uniqueispod')
-                print(uniqueIdentifier)
                 PERFORMANCE_TEST.writeToActionsBeforeCalculation("end", name, additionalInfo, uniqueIdentifier)
         except:
             PERFORMANCE_TEST.clearResult()
     
     @staticmethod
     def publishResult(apiKey):
         url = 'https://xwycqvx020.execute-api.us-east-1.amazonaws.com/library/execution'
@@ -144,41 +125,36 @@
 
         return PERFORMANCE_TEST.argumentsValue['shouldMeasure']
 
     @staticmethod
     def writeToActionsBeforeCalculation(type, actionName, additional_info, unique_identifier):
         currentTime = round(time.time() * 1000)
         actionInfo = Event( tip = type,actionName = actionName,timeVreme = currentTime,unique_identifier = unique_identifier,additional_info = additional_info)
-     #   lock (actionsBeforeCalculation):
-        if(not actionName in PERFORMANCE_TEST.actionsBeforeCalculation):
-            PERFORMANCE_TEST.actionsBeforeCalculation[actionName] = StartEndList([],[])
-        if (type == "start"):
-            editedStartAction = PERFORMANCE_TEST.actionsBeforeCalculation[actionName].startAction
-            editedStartAction.append(actionInfo)
-            PERFORMANCE_TEST.actionPoints+=1
-        else:
-            editedEndAction = PERFORMANCE_TEST.actionsBeforeCalculation[actionName].endAction
-            editedEndAction.append(actionInfo)
-            PERFORMANCE_TEST.actionPoints+=1
+        with PERFORMANCE_TEST.lock:
+            if(not actionName in PERFORMANCE_TEST.actionsBeforeCalculation):
+                PERFORMANCE_TEST.actionsBeforeCalculation[actionName] = StartEndList([],[])
+            if (type == "start"):
+                editedStartAction = PERFORMANCE_TEST.actionsBeforeCalculation[actionName].startAction
+                editedStartAction.append(actionInfo)
+                PERFORMANCE_TEST.actionPoints+=1
+            else:
+                editedEndAction = PERFORMANCE_TEST.actionsBeforeCalculation[actionName].endAction
+                editedEndAction.append(actionInfo)
+                PERFORMANCE_TEST.actionPoints+=1
 
     @staticmethod
     def calculateActions():
         finalLogData = []
  
         for attr, value in PERFORMANCE_TEST.actionsBeforeCalculation.items():
-            print(attr)
-            print(value.startAction)
-            #  foreach (KeyValuePair<string, StartEndList> actionKey in actionsBeforeCalculation):
             startActionList = value.startAction
             endActionList = value.endAction
 
             startActionList.sort(key=lambda x: x.timeVreme, reverse=True)
             endActionList.sort(key=lambda x: x.timeVreme)
-            # HelperFunctions.sortByDate(startActionList)
-            # HelperFunctions.sortByDateReverse(endActionList)
 
             stIdsToRemove = []
             etIdsToRemove = []
 
             #spajam sa istim ui
             for  eti in endActionList:
                 for stId in startActionList:
@@ -217,17 +193,14 @@
             for stime in startActionList:
                # if (not stime.isThreadId):
                 PERFORMANCE_TEST.addRemaining(finalLogData, stime, attr)
 
             for etime in endActionList:
                # if (not etime.isThreadId):
                 PERFORMANCE_TEST.addRemaining(finalLogData, etime, attr)
-
-            sMergedId = []
-            eMergedId = []
    
         PERFORMANCE_TEST.sortFinalLog(finalLogData)
 
         PERFORMANCE_TEST.calculatedActions = finalLogData[0:100] if len(finalLogData)>100 else finalLogData
     
     @staticmethod
     def createadditional_info(first, addInfo = ""):
@@ -255,69 +228,28 @@
             help.additionalInfo = "start event not caught"
         whereToAdd.append(help)
         return whereToAdd
 
     @staticmethod
     def sortFinalLog(actions):
         actions.sort(key=lambda x: x.startTime if x.startTime>0 else x.endTime)
-        # actions.Sort(
-                #     (x, y) =>
-                #     {
-                #         int nz;
-                #         long prvi;
-                #         long drugi;
-                #         if (x.startTime == 0)
-                #         {
-                #             prvi = x.endTime;
-                #         }
-                #         else
-                #         {
-                #             prvi = x.startTime;
-                #         }
-
-                #         if (y.startTime == 0)
-                #         {
-                #             drugi = y.endTime;
-                #         }
-                #         else
-                #         {
-                #             drugi = y.startTime;
-                #         }
-                #         if (prvi < drugi)
-                #         {
-                #             nz = -1;
-                #         }
-                #         else if (prvi > y.startTime)
-                #         {
-                #             nz = 1;
-                #         }
-                #         else
-                #         {
-                #             nz = 0;
-                #         }
-                #         return nz;
-                #     }
-                # );
 
 class Event:
     tip =""
     actionName=""
     timeVreme=0
     unique_identifier=""
     additional_info =""
-    #isThreadId =False
  
-    # parameterized constructor
     def __init__(self, tip, actionName, timeVreme, unique_identifier, additional_info):
         self.tip = tip
         self.actionName = actionName
         self.timeVreme=timeVreme
         self.unique_identifier=unique_identifier
         self.additional_info=additional_info
-     #   self.isThreadId=isThreadId
 
 
 class StartEndList:
 
     startAction=[]
     endAction=[]
     def __init__(self, startAction, endAction):
@@ -377,58 +309,7 @@
 
 class MyEncoder(json.JSONEncoder):
     def default(self, o):
         if hasattr(o, "reprJson"):
             return o.reprJson()
         else:
             return super().default(o)
-k=1
-
-def _prva():
-        PERFORMANCE_TEST.ActionStart(name= "calculatePlus")
-        numberOfSeconds = 0
-        while (numberOfSeconds < 3):
-            time.sleep(1)
-            numberOfSeconds+=1
-        PERFORMANCE_TEST.ActionEnd(name= "calculatePlus")
-
-def _druga():
-    time.sleep(1)
-    PERFORMANCE_TEST.ActionStart(name= "calculatePlus")
-    time.sleep(1)
-    PERFORMANCE_TEST.ActionEnd(name= "calculatePlus")
-
-async def job1(seconds):
-    print(f"job1 start {time.strftime('%X')}")
-    PERFORMANCE_TEST.ActionStart("calculatePlus")
-    await asyncio.sleep(2)
-    print(f"job1 end {time.strftime('%X')}")
-    PERFORMANCE_TEST.ActionEnd("calculatePlus")
-
-async def job2(seconds):
-    await asyncio.sleep(1)
-    print(f"job2 start {time.strftime('%X')}")
-    PERFORMANCE_TEST.ActionStart("calculatePlus")
-
-async def asyncJobMultiple(delay, uid):
-    #  cid = Task.CurrentId.ToString()
-    print(f"start {time.strftime('%X')}")
-    PERFORMANCE_TEST.ActionStart(name= "calculatePlus")
-    await asyncio.sleep(delay)
-    print(f"end {time.strftime('%X')}")
-    PERFORMANCE_TEST.ActionEnd("calculatePlus")
-
-# PERFORMANCE_TEST.Start(measure= True)
-# PERFORMANCE_TEST.ActionStart("calculatePlus")
-# time.sleep(1)
-# PERFORMANCE_TEST.ActionEnd("calculatePlus")
-# time.sleep(1)
-PERFORMANCE_TEST.Start(measure= True)
-PERFORMANCE_TEST.ActionStart("calculatePluss", uniqueIdentifier="1")
-PERFORMANCE_TEST.ActionStart("calculatePluss", uniqueIdentifier="2")
-time.sleep(2)
-PERFORMANCE_TEST.ActionEnd("calculatePluss", uniqueIdentifier="1")
-PERFORMANCE_TEST.ActionEnd("calculatePluss", uniqueIdentifier="2")
-time.sleep(1)
-exe = PERFORMANCE_TEST.Stop(publish= True, version= "sfds1", apiKey= "CCrEhMf7b7b8uKDiks6jgZWx3kYovoPWgLoD_EejJE0")#, 
-print(exe)
-
```

### Comparing `Perfole-0.0.1/Perfole.egg-info/PKG-INFO` & `Perfole-0.0.2/Perfole.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.1
+Version: 0.0.2
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 
@@ -45,19 +45,19 @@
 
 ## Results
 Stop() method will return list of caught actions. For cloud reporting functionality visit https://perfole.com
 
 
 ## UniqueIdentifier parameter
 UniqueIdentifier parameter must be given when start/end points are in different threads:
-
+```
 PERFORMANCE_TEST.StartAction(name="myAction", uniqueIdentifier= "myIdentifier")
 ...
 PERFORMANCE_TEST.EndAction(name="myAction", uniqueIdentifier= "myIdentifier")
-
+```
```

### Comparing `Perfole-0.0.1/README.md` & `Perfole-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 
 ## Results
 Stop() method will return list of caught actions. For cloud reporting functionality visit https://perfole.com
 
 
 ## UniqueIdentifier parameter
 UniqueIdentifier parameter must be given when start/end points are in different threads:
-
+```
 PERFORMANCE_TEST.StartAction(name="myAction", uniqueIdentifier= "myIdentifier")
 ...
 PERFORMANCE_TEST.EndAction(name="myAction", uniqueIdentifier= "myIdentifier")
-
+```
```

### Comparing `Perfole-0.0.1/license.txt` & `Perfole-0.0.2/license.txt`

 * *Files identical despite different names*

