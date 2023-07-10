# Comparing `tmp/eons-2.6.5.tar.gz` & `tmp/eons-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.6.5.tar", last modified: Sun Jun 25 22:38:26 2023, max compression
+gzip compressed data, was "eons-2.6.6.tar", last modified: Mon Jul 10 02:32:36 2023, max compression
```

## Comparing `eons-2.6.5.tar` & `eons-2.6.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-25 22:38:26.756589 eons-2.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-25 22:38:08.000000 eons-2.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.752589 eons-2.6.5/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92334 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-25 22:38:17.000000 eons-2.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-25 22:38:26.760589 eons-2.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-07-10 02:32:36.257643 eons-2.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-10 02:32:20.000000 eons-2.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.253643 eons-2.6.6/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.253643 eons-2.6.6/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93216 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 02:32:28.000000 eons-2.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-10 02:32:36.261643 eons-2.6.6/setup.cfg
```

### Comparing `eons-2.6.5/PKG-INFO` & `eons-2.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.5
+Version: 2.6.6
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.5/README.md` & `eons-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.6.5/pkg/eons/eons.py` & `eons-2.6.6/pkg/eons/eons.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
 import inspect
 import shutil
 import builtins
+import re
 from pathlib import Path
 from subprocess import Popen
 from subprocess import PIPE
 from subprocess import STDOUT
 import argparse
 import requests
 import yaml
 from requests_futures.sessions import FuturesSession
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
 from eot import EOT
-import re
 
 ######## START CONTENT ########
+def INVALID_NAME():
+	return "INVALID_NAME"
+
 class ActualType(type):
 	def __repr__(self):
 		return self.__name__
 
 class GlobalError(Exception, metaclass=ActualType): pass
 
 class NotInstantiableError(Exception, metaclass=ActualType): pass
@@ -200,17 +203,14 @@
 		setattr(logging, levelName, value)
 		setattr(logging.getLogger(), methodName, logForLevel)
 		setattr(logging, methodName, logToRoot)
 
 
 jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
 
-def INVALID_NAME():
-	return "INVALID_NAME"
-
 
 #Self registration for use with json loading.
 #Any class that derives from SelfRegistering can be instantiated with:
 #   SelfRegistering("ClassName")
 #Based on: https://stackoverflow.com/questions/55973284/how-to-create-this-registering-factory-in-python/55973426
 class SelfRegistering(object):
 
@@ -518,14 +518,64 @@
 			pass
 		tracker.functors.reverse()
 
 	@staticmethod
 	def GetCount():
 		return len(FunctorTracker.Instance().functors)
 
+
+# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
+# This can be abused quite a bit, so please try to restrict usage of this to only:
+# * Ease of use global functions
+#
+# Thanks! 
+class ExecutorTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in ExecutorTracker.__dict__:
+			logging.debug(f"Creating new ExecutorTracker: {this}")
+			ExecutorTracker.instance = this
+		else:
+			return None
+
+		this.executors = [None]
+
+	@staticmethod
+	def Instance():
+		if "instance" not in ExecutorTracker.__dict__:
+			ExecutorTracker()
+		return ExecutorTracker.instance
+
+	@staticmethod
+	def Push(executor):
+		ExecutorTracker.Instance().executors.append(executor)
+
+		# Adding the executor to our list here increases its reference count.
+		# Executors are supposed to remove themselves from this list when they are deleted.
+		# A python object cannot be deleted if it has references.
+		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
+		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
+		# If you want your executor to stop being tracked, do it yourself. :(
+		#
+		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+
+		logging.debug(f"Now tracking Executor: {executor}")
+
+	@staticmethod
+	def Pop(executor):
+		try:
+			ExecutorTracker.Instance().executors.remove(executor)
+			logging.debug(f"No longer tracking Executor: {executor}")
+		except:
+			pass
+
+	@staticmethod
+	def GetLatest():
+		return ExecutorTracker.Instance().executors[-1]
+
 # Don't import Method or Executor, even though they are required: it will cause a circular dependency.
 # Instead, pretend there's a forward declaration here and don't think too hard about it ;)
 ################################################################################
 
 # Functor is a base class for any function-oriented class structure or operation.
 # This class derives from Datum, primarily, to give it a name but also to allow it to be stored and manipulated, should you so desire.
 # Functors will automatically Fetch any ...Args specified.
@@ -610,18 +660,25 @@
 		# For converting config value names.
 		# e.g. "type": "projectType" makes it so that when calling Set("projectType", ...),  this.type is changed.
 		this.configNameOverrides = {}
 
 		# Rolling back can be disabled by setting this to False.
 		this.enableRollback = True
 
-		# Numerical result indication the success or failure of *this.
-		# Set automatically.
+		# Automatically return the result.data object if the function returns None
+		this.enableAutoReturn = True
+
+		# this.result encompasses the return value of *this.
+		# The code is a numerical result indication the success or failure of *this and is set automatically.
 		# 0 is success; 1 is no change; higher numbers are some kind of error.
-		this.result = 0
+		# this.result.data should be set manuallly.
+		# It is highly recommended that you check result.data in DidFunctionSucceed().
+		this.result = util.DotDict()
+		this.result.code = 0
+		this.result.data = util.DotDict()
 
 		# Whether or not we should pass on exceptions when calls fail.
 		this.raiseExceptions = True
 
 		# Ease of use members
 		# These can be calculated in Function and Rollback, respectively.
 		this.functionSucceeded = False
@@ -1057,14 +1114,16 @@
 			return this.GetExecutor().Execute(next, precursor=this, next=this.next)
 
 
 	def WarmUp(this, *args, **kwargs):
 
 		this.args = args
 		this.kwargs = kwargs
+		this.result.code = 0
+		this.result.data = util.DotDict()
 		
 		try:
 			this.PopulatePrecursor()
 			if (this.executor):
 				this.executor.BeginPlacing(this.name)
 			this.Initialize() # nop on call 2+
 			this.PopulateMethods() # Doesn't require Fetch; depends on precursor
@@ -1096,46 +1155,49 @@
 			this.WarmUp(*args, **kwargs)
 			logging.debug(f"{this.name}({this.args}, {this.kwargs})")
 
 			getattr(this, f"Before{this.callMethod}")()
 			ret = getattr(this, this.callMethod)()
 
 			if (getattr(this, f"Did{this.callMethod}Succeed")()):
-					this.result = 0
+					this.result.code = 0
 					# logging.info(f"{this.name} successful!")
 					nextRet = this.CallNext()
 			elif (this.enableRollback):
 				logging.warning(f"{this.name} failed. Attempting Rollback...")
 				ret = getattr(this, this.rollbackMethod)()
 				if (getattr(this, f"Did{this.rollbackMethod}Succeed")()):
-					this.result = 1
+					this.result.code = 1
 					# logging.info(f"Rollback succeeded. All is well.")
 					nextRet = this.CallNext()
 				else:
-					this.result = 2
+					this.result.code = 2
 					logging.error(f"ROLLBACK FAILED! SYSTEM STATE UNKNOWN!!!")
 			else:
-				this.result = 3
+				this.result.code = 3
 				logging.error(f"{this.name} failed.")
 
 			getattr(this, f"After{this.callMethod}")()
 
 		except Exception as e:
 			if (this.raiseExceptions):
 				raise e
 			else:
 				logging.error(f"ERROR: {e}")
 				util.LogStack()
 
-		if (this.raiseExceptions and this.result > 1):
-			raise FunctorError(f"{this.name} failed with result {this.result}")
+		if (this.raiseExceptions and this.result.code > 1):
+			raise FunctorError(f"{this.name} failed with result {this.result.code}: {this.result}")
 
 		if (nextRet is not None):
 			ret = nextRet
 
+		if (this.enableAutoReturn and len(this.result.data) and ret is None):
+			ret = this.result.data
+
 		logging.info(f"return {ret}")
 		FunctorTracker.Pop(this)
 		logging.info(f"}} ({this.name})")
 
 		return ret
 
 
@@ -1403,72 +1465,113 @@
 		if (not this.next):
 			return None
 
 		for next in this.next:
 			next(precursor=this)
 
 
-# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
-# This can be abused quite a bit, so please try to restrict usage of this to only:
-# * Ease of use global functions
-#
-# Thanks! 
-class ExecutorTracker:
-	def __init__(this):
-		# Singletons man...
-		if "instance" not in ExecutorTracker.__dict__:
-			logging.debug(f"Creating new ExecutorTracker: {this}")
-			ExecutorTracker.instance = this
-		else:
-			return None
-
-		this.executors = [None]
-
-	@staticmethod
-	def Instance():
-		if "instance" not in ExecutorTracker.__dict__:
-			ExecutorTracker()
-		return ExecutorTracker.instance
-
-	@staticmethod
-	def Push(executor):
-		ExecutorTracker.Instance().executors.append(executor)
-
-		# Adding the executor to our list here increases its reference count.
-		# Executors are supposed to remove themselves from this list when they are deleted.
-		# A python object cannot be deleted if it has references.
-		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
-		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
-		# If you want your executor to stop being tracked, do it yourself. :(
-		#
-		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
-
-		logging.debug(f"Now tracking Executor: {executor}")
+class FetchCallbackFunctor(Functor):
 
-	@staticmethod
-	def Pop(executor):
-		try:
-			ExecutorTracker.Instance().executors.remove(executor)
-			logging.debug(f"No longer tracking Executor: {executor}")
-		except:
-			pass
+	def __init__(this, name = "FetchCallbackFunctor"):
+		super().__init__(name)
 
-	@staticmethod
-	def GetLatest():
-		return ExecutorTracker.Instance().executors[-1]
+		this.requiredKWArgs.append('varName')
+		this.requiredKWArgs.append('location')
+		this.requiredKWArgs.append('value')
 
+		this.functionSucceeded = True
+		this.enableRollback = False
 
 # Global Fetch() function.
 # Uses the latest registered Executor
 def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
     return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
 
 # Ease-of-use wrapper for the global Fetch()
 def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
     Fetch(varName, default, fetchFrom, start, attempted)
+#from .Executor import Executor # don't import this, it'll be circular!
+
+# @recoverable
+# Decorating another function with this method will engage the error recovery system provided by *this.
+# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
+# For more info, see Executor.ResolveError and the README.md
+def recoverable(function):
+	def RecoverableDecorator(obj, *args, **kwargs):
+		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
+	return RecoverableDecorator
+
+
+# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
+def RecoverableImplementation(obj, executor, function, *args, **kwargs):
+	try:
+		return function(obj, *args, **kwargs)
+	except FailedErrorResolution as fatal:
+		raise fatal
+	except Exception as e:
+		if (not executor.resolveErrors):
+			raise e
+		return Recover(e, obj, executor, function, *args, **kwargs)
+
+
+def Recover(error, obj, executor, function, *args, **kwargs):
+	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
+	util.LogStack()
+
+	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
+	if (str(error) not in executor.errorResolutionStack.keys()):
+		executor.errorResolutionStack.update({str(error):[]})
+
+	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
+	# ResolveError is itself @recoverable.
+	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
+	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
+	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
+
+	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
+		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
+
+	successfullyRecovered = False
+	ret = None
+	resolvedBy = None
+	for i, res in enumerate(executor.resolveErrorsWith):
+
+		logging.debug(f"Checking if {res} can fix '{error}'.")
+		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
+			# if no resolution was attempted, there's no need to re-run the function.
+			continue
+		try:
+			logging.debug(f"Trying function ({function}) again after applying {res}.")
+			resolvedBy = res
+			ret = function(obj, *args, **kwargs)
+			successfullyRecovered = True
+			break
+
+		except Exception as e2:
+			if (str(error) == str(e2)):
+				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
+				# Resolution failed. That's okay. Let's try the next.
+				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
+				continue
+			else:
+				# The error changed, maybe we're making progress.
+				ret = Recover(e2, obj, executor, function, *args, **kwargs)
+				successfullyRecovered = True
+				break
+
+	if (successfullyRecovered):
+		executor.ClearErrorResolutionStack(str(error)) # success!
+		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
+		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
+		return ret
+
+	#  We failed to resolve the error. Die
+	sys.tracebacklimit = 0 # traceback is NOT helpful here.
+	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
+
 
 # The standard Functor extends Functor to add a set of standard members and methods.
 # This is similar to the standard library in C and C++
 # You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
 class StandardFunctor(Functor):
 	def __init__(this, name="Standard Functor"):
 		super().__init__(name)
@@ -1583,92 +1686,166 @@
 		logging.debug(f"================ Completed command: {command} ================")
 		if (saveout):
 			return process.returncode, output
 		
 		return process.returncode
 	######## END: UTILITIES ########
 
-#from .Executor import Executor # don't import this, it'll be circular!
 
-# @recoverable
-# Decorating another function with this method will engage the error recovery system provided by *this.
-# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
-# For more info, see Executor.ResolveError and the README.md
-def recoverable(function):
-	def RecoverableDecorator(obj, *args, **kwargs):
-		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
-	return RecoverableDecorator
+# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
+# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
+# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
+# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
+#
+# startPosition is always positive
+# endPosition is always negative
+class ErrorStringParser:
 
+	def __init__(this, applicableError, startPosition, endPosition):
+		this.applicableError = applicableError
+		this.startPosition = startPosition
+		this.endPosition = endPosition
 
-# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
-def RecoverableImplementation(obj, executor, function, *args, **kwargs):
-	try:
-		return function(obj, *args, **kwargs)
-	except FailedErrorResolution as fatal:
-		raise fatal
-	except Exception as e:
-		if (not executor.resolveErrors):
-			raise e
-		return Recover(e, obj, executor, function, *args, **kwargs)
+	def Parse(this, errorString):
+		end = this.endPosition
+		if (not end):
+			end = len(errorString)
+		return errorString[this.startPosition:end]
 
 
-def Recover(error, obj, executor, function, *args, **kwargs):
-	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
-	util.LogStack()
+# ErrorResolution is a Functor which can be executed when an Exception is raised.
+# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
+class ErrorResolution(StandardFunctor):
 
-	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
-	if (str(error) not in executor.errorResolutionStack.keys()):
-		executor.errorResolutionStack.update({str(error):[]})
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
 
-	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
-	# ResolveError is itself @recoverable.
-	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
-	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
-	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
+		# What errors, as ErrorStringParser objects, is *this prepared to handle?
+		this.parsers = []
 
-	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
-		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
+		this.error = None
+		this.errorType = ""
+		this.errorString = ""
+		this.errorObject = ""
+		this.errorResolutionStack = {}
 
-	successfullyRecovered = False
-	ret = None
-	resolvedBy = None
-	for i, res in enumerate(executor.resolveErrorsWith):
+		# Provided directly from the recoverable decorator.
+		this.optionalKWArgs["obj"] = None
+		this.optionalKWArgs["function"] = None
 
-		logging.debug(f"Checking if {res} can fix '{error}'.")
-		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
-			# if no resolution was attempted, there's no need to re-run the function.
-			continue
-		try:
-			logging.debug(f"Trying function ({function}) again after applying {res}.")
-			resolvedBy = res
-			ret = function(obj, *args, **kwargs)
-			successfullyRecovered = True
-			break
+		# We do want to know whether or not we should attempt to run whatever failed again.
+		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
+		# No rollback, by default and definitely don't throw Exceptions.
+		this.enableRollback = False
+		this.functionSucceeded = True
+		this.raiseExceptions = False
 
-		except Exception as e2:
-			if (str(error) == str(e2)):
-				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
-				# Resolution failed. That's okay. Let's try the next.
-				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
+		this.errorShouldBeResolved = False
+
+
+
+	# Put your logic here!
+	def Resolve(this):
+		# You get the following members:
+		# this.error (an Exception)
+		# this.errorString (a string cast of the Exception)
+		# this.errorType (a string)
+		# this.errorObjet (a string or whatever you return from GetObjectFromError())
+
+		# You get the following guarantees:
+		# *this has not been called on this particular error before.
+		# the error given is applicable to *this per this.parsers
+
+		###############################################
+		# Please throw errors if something goes wrong #
+		# Otherwise, set this.errorShouldBeResolved   #
+		###############################################
+		
+		pass
+
+
+
+	# Helper method for creating ErrorStringParsers
+	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
+	def ApplyTo(this, error, exampleString):
+		match = re.search('OBJECT', exampleString)
+		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
+
+
+	# Get the type of this.error as a string.
+	def GetErrorType(this):
+		return type(this.error).__name__
+
+
+	# Get an actionable object from the error.
+	# For example, if the error is 'ModuleNotFoundError', what is the module?
+	def GetObjectFromError(this):
+		for parser in this.parsers:
+			if (parser.applicableError != this.errorType):
 				continue
-			else:
-				# The error changed, maybe we're making progress.
-				ret = Recover(e2, obj, executor, function, *args, **kwargs)
-				successfullyRecovered = True
-				break
 
-	if (successfullyRecovered):
-		executor.ClearErrorResolutionStack(str(error)) # success!
-		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
-		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
-		return ret
+			this.errorObject = parser.Parse(this.errorString)
+			return
 
-	#  We failed to resolve the error. Die
-	sys.tracebacklimit = 0 # traceback is NOT helpful here.
-	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
+		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
+
+
+	# Determine if this resolution method is applicable.
+	def CanProcess(this):
+		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def ParseInitialArgs(this):
+		super().ParseInitialArgs()
+		if ('error' in this.kwargs):
+			this.error = this.kwargs.pop('error')
+			# Just assume the error is an actual Exception object.
+		else:
+			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
+
+		this.errorString = str(this.error)
+		this.errorType = this.GetErrorType()
+
+		# Internal member to avoid processing duplicates
+		this.errorResolutionStack = this.executor.errorResolutionStack
+
+
+	# Error resolution is unchained.
+	def PopulateNext(this):
+		this.next = []
+
+
+	# Override of Functor method.
+	# We'll keep calling this until an error is raised.
+	def Function(this):
+		this.functionSucceeded = True
+		this.errorShouldBeResolved = True
+		
+		if (not this.CanProcess()):
+			this.errorShouldBeResolved = False
+			return this.errorResolutionStack, this.errorShouldBeResolved
+
+		if (not this.errorString in this.errorResolutionStack.keys()):
+			this.errorResolutionStack.update({this.errorString:[]})
+		
+		if (this.name in this.errorResolutionStack[this.errorString]):
+			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
+
+		this.GetObjectFromError()
+
+		try:
+			this.Resolve()
+		except Exception as e:
+			logging.error(f"Error resolution with {this.name} failed: {e}")
+			util.LogStack()
+			this.functionSucceeded = False
+		
+		this.errorResolutionStack[this.errorString].append(this.name)
+		return this.errorResolutionStack, this.errorShouldBeResolved
 
 
 # Executor: a base class for user interfaces.
 # An Executor is a functor and can be executed as such.
 # For example
 #	class MyExecutor(Executor):
 #		def __init__(this):
@@ -1686,14 +1863,17 @@
 
 		this.optionalKWArgs['log_time_stardate'] = True
 		this.optionalKWArgs['log_indentation'] = True
 		this.optionalKWArgs['log_tab_width'] = 2
 		this.optionalKWArgs['log_aggregate'] = True
 		this.optionalKWArgs['log_aggregate_url'] = "https://eons.sh/log"
 
+		# Executors should have control over their returns, if they have any.
+		this.enableAutoReturn = False
+
 		this.resolveErrors = True
 		this.errorRecursionDepth = 0
 		this.errorResolutionStack = {}
 		this.resolveErrorsWith = [ # order matters: FIFO (first is first).
 			'find_by_fetch',
 			'install_from_repo_with_default_package_type',
 			'install_from_repo',
@@ -2015,15 +2195,15 @@
 		pass
 
 
 	# Register all classes in each directory in this.registerDirectories
 	def RegisterAllClasses(this):
 		for d in this.registerDirectories:
 			this.RegisterAllClassesInDirectory(os.path.join(os.getcwd(), d))
-		this.RegisterAllClassesInDirectory(this.repo.store)
+		this.RegisterAllClassesInDirectory(this.repo.registry)
 
 
 	# Grok the configFile and populate this.config
 	def ParseConfigFile(this, configFile):
 		if (this.configType in ['py']):
 			this.RegisterAllClassesInDirectory(Path('./').joinpath('/'.join(this.parsedArgs.config.split('/')[:-1])))
 			functor = SelfRegistering(this.parsedArgs.config.split('/')[-1].split('.')[0])
@@ -2064,14 +2244,15 @@
 
 
 	#  Get information for how to download packages.
 	def PopulateRepoDetails(this):
 		details = {
 			"online": not this.Fetch('no_repo', False, ['this', 'args', 'config']),
 			"store": this.defaultRepoDirectory,
+			"registry": str(Path(this.defaultRepoDirectory).joinpath('registry').resolve()),
 			"url": "https://api.infrastructure.tech/v1/package",
 			"username": None,
 			"password": None
 		}
 		for key, default in details.items():
 			this.repo[key] = this.Fetch(f"repo_{key}", default=default)
 
@@ -2219,17 +2400,19 @@
 
 		if (not this.repo.online):
 			logging.debug(f"Refusing to download {packageName}; we were told not to use a repository.")
 			return False
 
 		logging.debug(f"Trying to download {packageName} from repository ({this.repo.url})")
 
-		if (not os.path.exists(this.repo.store)):
-			logging.debug(f"Creating directory {this.repo.store}")
-			mkpath(this.repo.store)
+		for path in ['store', 'registry']:
+			if (Path(this.repo[path]).is_dir()):
+				continue
+			logging.debug(f"Creating directory {this.repo[path]}")
+			mkpath(this.repo[path])
 
 		packageZipPath = os.path.join(this.repo.store, f"{packageName}.zip")
 
 		url = f"{this.repo.url}/download?package_name={packageName}"
 
 		auth = None
 		if this.repo.username and this.repo.password:
@@ -2269,25 +2452,27 @@
 		packageZipContents.close()
 
 		if (not os.path.exists(packageZipPath)):
 			raise PackageError(f"Failed to create {packageZipPath}")
 
 		openArchive = ZipFile(packageZipPath, 'r')
 		extractLoc = this.repo.store
+		if (registerClasses):
+			extractLoc = this.repo.registry
 		if (createSubDirectory):
 			extractLoc = os.path.join(extractLoc, packageName)
 		elif (this.placement.session.active):
 			extractLoc = os.path.join(extractLoc, str(this.placement.session.level))
 		logging.debug(f"Extracting {packageZipPath} to {extractLoc}")
 		openArchive.extractall(f"{extractLoc}")
 		openArchive.close()
 		os.remove(packageZipPath)
 
 		if (registerClasses):
-			this.RegisterAllClassesInDirectory(this.repo.store)
+			this.RegisterAllClassesInDirectory(this.repo.registry)
 
 		return True
 
 	# RETURNS and instance of a Datum, Functor, etc. (aka modules) which has been discovered by a prior call of RegisterAllClassesInDirectory()
 	# Will attempt to register existing modules if one of the given name is not found. Failing that, the given package will be downloaded if it can be found online.
 	# Both python modules and other eons modules of the same packageType will be installed automatically in order to meet all required dependencies of the given module.
 	@recoverable
@@ -2442,172 +2627,7 @@
 		for key, val in this.extraArgs.items():
 			if (key == varName):
 				return val, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
-
-# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
-# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
-# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
-# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
-#
-# startPosition is always positive
-# endPosition is always negative
-class ErrorStringParser:
-
-	def __init__(this, applicableError, startPosition, endPosition):
-		this.applicableError = applicableError
-		this.startPosition = startPosition
-		this.endPosition = endPosition
-
-	def Parse(this, errorString):
-		end = this.endPosition
-		if (not end):
-			end = len(errorString)
-		return errorString[this.startPosition:end]
-
-
-# ErrorResolution is a Functor which can be executed when an Exception is raised.
-# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
-class ErrorResolution(StandardFunctor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# What errors, as ErrorStringParser objects, is *this prepared to handle?
-		this.parsers = []
-
-		this.error = None
-		this.errorType = ""
-		this.errorString = ""
-		this.errorObject = ""
-		this.errorResolutionStack = {}
-
-		# Provided directly from the recoverable decorator.
-		this.optionalKWArgs["obj"] = None
-		this.optionalKWArgs["function"] = None
-
-		# We do want to know whether or not we should attempt to run whatever failed again.
-		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
-		# No rollback, by default and definitely don't throw Exceptions.
-		this.enableRollback = False
-		this.functionSucceeded = True
-		this.raiseExceptions = False
-
-		this.errorShouldBeResolved = False
-
-
-
-	# Put your logic here!
-	def Resolve(this):
-		# You get the following members:
-		# this.error (an Exception)
-		# this.errorString (a string cast of the Exception)
-		# this.errorType (a string)
-		# this.errorObjet (a string or whatever you return from GetObjectFromError())
-
-		# You get the following guarantees:
-		# *this has not been called on this particular error before.
-		# the error given is applicable to *this per this.parsers
-
-		###############################################
-		# Please throw errors if something goes wrong #
-		# Otherwise, set this.errorShouldBeResolved   #
-		###############################################
-		
-		pass
-
-
-
-	# Helper method for creating ErrorStringParsers
-	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
-	def ApplyTo(this, error, exampleString):
-		match = re.search('OBJECT', exampleString)
-		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
-
-
-	# Get the type of this.error as a string.
-	def GetErrorType(this):
-		return type(this.error).__name__
-
-
-	# Get an actionable object from the error.
-	# For example, if the error is 'ModuleNotFoundError', what is the module?
-	def GetObjectFromError(this):
-		for parser in this.parsers:
-			if (parser.applicableError != this.errorType):
-				continue
-
-			this.errorObject = parser.Parse(this.errorString)
-			return
-
-		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
-
-
-	# Determine if this resolution method is applicable.
-	def CanProcess(this):
-		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def ParseInitialArgs(this):
-		super().ParseInitialArgs()
-		if ('error' in this.kwargs):
-			this.error = this.kwargs.pop('error')
-			# Just assume the error is an actual Exception object.
-		else:
-			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
-
-		this.errorString = str(this.error)
-		this.errorType = this.GetErrorType()
-
-		# Internal member to avoid processing duplicates
-		this.errorResolutionStack = this.executor.errorResolutionStack
-
-
-	# Error resolution is unchained.
-	def PopulateNext(this):
-		this.next = []
-
-
-	# Override of Functor method.
-	# We'll keep calling this until an error is raised.
-	def Function(this):
-		this.functionSucceeded = True
-		this.errorShouldBeResolved = True
-		
-		if (not this.CanProcess()):
-			this.errorShouldBeResolved = False
-			return this.errorResolutionStack, this.errorShouldBeResolved
-
-		if (not this.errorString in this.errorResolutionStack.keys()):
-			this.errorResolutionStack.update({this.errorString:[]})
-		
-		if (this.name in this.errorResolutionStack[this.errorString]):
-			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
-
-		this.GetObjectFromError()
-
-		try:
-			this.Resolve()
-		except Exception as e:
-			logging.error(f"Error resolution with {this.name} failed: {e}")
-			util.LogStack()
-			this.functionSucceeded = False
-		
-		this.errorResolutionStack[this.errorString].append(this.name)
-		return this.errorResolutionStack, this.errorShouldBeResolved
-
-
-class FetchCallbackFunctor(Functor):
-
-	def __init__(this, name = "FetchCallbackFunctor"):
-		super().__init__(name)
-
-		this.requiredKWArgs.append('varName')
-		this.requiredKWArgs.append('location')
-		this.requiredKWArgs.append('value')
-
-		this.functionSucceeded = True
-		this.enableRollback = False
```

### Comparing `eons-2.6.5/pkg/eons/method/External.py` & `eons-2.6.6/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.5/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.6.6/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.5/pkg/eons/resolve/resolve_import_module.py` & `eons-2.6.6/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.6.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.5/pkg/eons.egg-info/PKG-INFO` & `eons-2.6.6/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.5
+Version: 2.6.6
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.5/pkg/eons.egg-info/SOURCES.txt` & `eons-2.6.6/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.6.5/setup.cfg` & `eons-2.6.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.6.5
+version = 2.6.6
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -21,17 +21,17 @@
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	pyyaml
 	requests_futures
 	requests
-	jsonpickle
 	eot
 	tqdm
+	jsonpickle
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

