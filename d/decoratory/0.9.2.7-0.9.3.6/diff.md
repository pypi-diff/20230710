# Comparing `tmp/decoratory-0.9.2.7.tar.gz` & `tmp/decoratory-0.9.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.9.2.7.tar", last modified: Tue Jul  4 07:14:53 2023, max compression
+gzip compressed data, was "decoratory-0.9.3.6.tar", last modified: Mon Jul 10 12:10:22 2023, max compression
```

## Comparing `decoratory-0.9.2.7.tar` & `decoratory-0.9.3.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 07:14:53.763277 decoratory-0.9.2.7/
--rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.2.7/License.txt
--rw-rw-rw-   0        0        0    47399 2023-07-04 07:14:53.763277 decoratory-0.9.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    45672 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.2.7/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 07:14:53.208483 decoratory-0.9.2.7/Sources/
-drwxrwxrwx   0        0        0        0 2023-07-04 07:14:53.462446 decoratory-0.9.2.7/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.2.7/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     7623 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5889 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14162 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12426 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    36916 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     8007 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10867 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:14:53.524955 decoratory-0.9.2.7/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    47399 2023-07-04 07:14:53.000000 decoratory-0.9.2.7/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-04 07:14:53.000000 decoratory-0.9.2.7/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 07:14:53.000000 decoratory-0.9.2.7/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-04 07:14:53.000000 decoratory-0.9.2.7/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 07:14:53.725510 decoratory-0.9.2.7/Unittest/
--rw-rw-rw-   0        0        0    24047 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23868 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40117 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10739 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10203 2023-07-04 07:14:18.000000 decoratory-0.9.2.7/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-07-04 07:14:53.763277 decoratory-0.9.2.7/setup.cfg
--rw-rw-rw-   0        0        0     4608 2023-07-04 07:14:19.000000 decoratory-0.9.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/
+-rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.3.6/License.txt
+-rw-rw-rw-   0        0        0    48657 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    46898 2023-07-10 12:03:21.000000 decoratory-0.9.3.6/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.3.6/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.053933 decoratory-0.9.3.6/Sources/
+drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.100801 decoratory-0.9.3.6/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.3.6/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7623 2023-07-10 12:09:45.000000 decoratory-0.9.3.6/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5889 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14162 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12426 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36916 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     8007 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10867 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.100801 decoratory-0.9.3.6/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    48657 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/Unittest/
+-rw-rw-rw-   0        0        0    24047 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23868 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40117 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10739 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10203 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     4678 2023-07-10 12:09:45.000000 decoratory-0.9.3.6/setup.py
```

### Comparing `decoratory-0.9.2.7/License.txt` & `decoratory-0.9.3.6/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.2.7/PKG-INFO` & `decoratory-0.9.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.2.7
+Version: 0.9.3.6
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu/decoratory
-Download-URL: http://evation.eu/decoratory\section\download.html
+Home-page: http://evation.eu/decoratory/index.html
+Download-URL: http://evation.eu/decoratory/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
-Project-URL: Projekt, http://evation.eu/decoratory
-Project-URL: Release Notes, http://evation.eu/decoratory\section\releasenotes.html
-Project-URL: Download, http://evation.eu/decoratory\section\download.html
+Project-URL: Projekt, http://evation.eu/decoratory/index.html
+Project-URL: Release Notes, http://evation.eu/decoratory/Section/ReleaseNotes.html
+Project-URL: Download, http://evation.eu/decoratory/Section/Download.html
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -49,17 +49,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu/decoratory"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.2.4"
-    __date__ = "2023-07-04"
-    __time__ = "09:14:18"
+    __version__ = "0.9.3.2"
+    __date__ = "2023-07-10"
+    __time__ = "14:03:21"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -106,15 +106,15 @@
 This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, simple as well as
 more complex examples are presented. Even if only one particular module
-is needed, it is recommended to view the preceding examples as well. For even
+is needed, it is recommended to view the preceding examples as well. For
 more examples of the full range of possibilities, please refer to
 `Decorator Implementations`_ on the `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
@@ -299,25 +299,25 @@
     # Case 1: decoration @Multiton(key=lambda spec, name: name)
     print(a)                        # Animal('dog', 'Teddy')
     print(b)                        # Animal('cat', 'Molly')
     print(c)                        # Animal('dog', 'Roxie')
 
 With three different names, a separate instance is created in each case.
 In contrast, the following variant distinguishes only two types (equivalence
-classes): animals with a character 'a' in their name and those without and
+classes): animals with a character 'y' in their name and those without and
 thus the key values can only be ``True`` or ``False``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per equivalence class
 
-    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'y' in name)
     print(a)                        # Animal('dog', 'Teddy')
-    print(b)                        # Animal('cat', 'Molly')
-    print(c)                        # Animal('cat', 'Molly')
+    print(b)                        # Animal('dog', 'Teddy')
+    print(c)                        # Animal('dog', 'Roxie')
 
 The initial parameter values of the initializer can also be accessed by their
 ``args``-index or ``kwargs``-name. So the following decorations are also
 possible:
 
 .. code-block:: python
 
@@ -341,15 +341,15 @@
     # Case 6: One unique instance from a @staticmethod or @classmethod
     @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
     class Animal:
         pass                        # Some code ...
 
         @classmethod
         def my_key(cls, spec, name):
-            return 'a' in name
+            return 'y' in name
 
 To actively control access to new equivalence classes, ``Multiton`` provides
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
 and checking the sealing state of the ``Multiton``. By default, the sealing
 state is set ``False``, so for every new key a new (unique) object is
 instantiated. When sealed (e.g. later in the process) is set ``True`` the
 dictionary has completed, i.e. restricted to the current object set and
@@ -396,14 +396,23 @@
         print(f"Sorry {ex.args[1]}, {ex.args[0]}")
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
     Animal.unseal()                 # Unseal the multiton!
     print(Animal.issealed())        # False
     Animal('cat', name='Molly')     # Now, Molly is added
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'),
                                     #  'Molly': Animal('cat', 'Molly')}
+    Animal.get_instances().pop('Teddy')
+    print(Animal.get_instances())   # {'Molly': Animal('cat', 'Molly')}
+    Animal.get_instances().clear()  # Same as Animal.reset()
+    print(Animal.get_instances())   # {}
+
+The last two lines show the functional equivalence of
+``Animal.get_instances().clear()`` with ``Animal.reset()``, but the ``reset``
+option is more transparent because it does not require going
+"behind the stage".
 
 
 ******************************************************************************
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
@@ -441,19 +450,26 @@
         print(f"value = '{value}'")
 
     # Function call with default parameters
     some_function()                 # value = 'original'
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
-The functionality of ``some_function()`` itself remains unchanged. A typical
-scenario for a wrapper is, of course, the execution of additional functionality
-before and/or after a given functionality, which itself remains unchanged,
-such as ``enter/leave`` markers, call data caches, runtime measurements, etc.
-Here is a typical example:
+The functionality of ``some_function()`` itself remains unchanged.
+For the sake of clarity, the principle of *all or nothing* is applied, i.e.
+defaults must be defined for all parameters and they are only used if no
+current parameters at all are transmitted. There is no mixing of current and
+default parameters. Thus, even a call of the decorated function with an
+incomplete parameter set is explicitly not supported and will throw a
+``TypeError``.
+
+A typical scenario for a wrapper is, of course, the execution of additional
+functionality before and/or after a given functionality, which itself remains
+unchanged, such as ``enter/leave`` markers, call data caches, runtime
+measurements, etc. Here is a typical example:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
@@ -697,14 +713,22 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
+Person is an observer, but not an observable, so the call to ``person()``
+reflects only personâ€™s own activity.
+Cat is an observable that is observed by person and therefore the activity
+``cat()`` triggers a follow-up activity by person.
+Calling ``dog()`` results in three activities at the observers, because
+``dog()`` is observed by the *observed cat*, which informs the person about
+its own activity.
+
 The order of reactions is determined by the order in the list in which
 the cat observes the dog prior to the person. If this order is reversed:
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
@@ -715,17 +739,19 @@
     # Case 3: Stacked observable decoration
     #    ---> Cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
 
-Calling ``dog()`` results in three activities at the observers, because
-``dog()`` observes the *observed cat*, which informs the person about its own
-action. If this behavior is not desired, ``dog()`` can instead address the
+Again, calling ``dog()`` results in three activities at the observers,
+but here person reacts first as an observer to dog and later again as an
+observer to cat.
+
+If this behavior is not desired, ``dog()`` can instead address the
 *original cat* using the ``cat.substitute.callee``, i.e.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
@@ -735,31 +761,34 @@
 
     # Case 4: Stacked observable decoration
     #    ---> Original cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Again, cat acts before person because of the order of the observer list and
-because the *original cat* observes dog the ``Hey, cat!`` statement of person
-is missing.
+In this case, cat acts before person because of the order of the observer
+list and because and because the *original cat* observes dog the ``Hey, cat!``
+statement of person is missing.
 
 
 Observer Decoration
 -------------------
 
 In this reversed decoration scheme, the observer decorator collects its
 observables. This seems more elaborate at first glance, but some prefer to
 explicitly designate the ``Observer`` and ``Observable`` roles in their code.
 
 Because an observer decoration uses observable methods, all
-observable(s) must always be declared before their observer(s).
+observable(s) must always be *declared and decorated* before their
+observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
+    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
+
 Thus, the initial example ``Case 1`` from `Observable Decoration`_ translates to:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
     from decoratory.observer import Observer, Observable
@@ -779,19 +808,15 @@
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 The use of the *semantic cross-function* ``X`` from ``decoratory.basic``
 instead of ``F`` indicates that ``dog`` is the observable, but the ``X``
 arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is also relevant, again.
-Each observable must be decorated before it is used by an observer.
-
-    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
-
+For multiple decorations, the *order of decoration* is also relevant here.
 The situation ``Case 2`` from `Observable Decoration`_ with person,
 dog and cat would then look like:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
@@ -854,15 +879,15 @@
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Now, both dog and cat end up being observers, observed by the person. But the
 cat observing the dog is the *original cat*, which does not inform the person
-of its activities, and so its statement ``Hey, cat!`` is missing.
+of its activities, and so personâ€™s statement ``Hey, cat!`` is missing.
 
 
 Class Decoration
 ----------------
 
 Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
@@ -990,15 +1015,15 @@
             print(f"Dog {name} arrived.")
 
     # Case 3: Dog is an observable to actions of various person instances.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe says Hello?
                                     # John Doe says What's up?
 
-Here, *one action of the observable*, the instantiation of ``Dog``, triggers
+But here, *one action of the observable*, the instantiation of ``Dog``, triggers
 *one to many actions at each selected resp. instantiated observer*, ``Person``.
 In such situations, a late `dynamic decoration <#dynamic-decoration>`_
 could be a good idea.
 
 So far, instantiating ``Dog`` resulted in an information and induced
 action at ``Person``. If ``Dog`` has its own actions that need to be
 selectively monitored, each of the selected actions can of course be decorated
@@ -1065,15 +1090,15 @@
 ``unregister`` *interface methods that an observable exposes*. Information can
 be given to the right recipients at relevant places in the code. For this,
 the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_
 comes into play. Dynamic decoration is used often also in connection with
 getter/setter/property constructions since data changes take place
 meaningfully over these methods.
 
-Let's consider two simple classes:
+Consider the following two example classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoratory-0.9.2.7/Readme.rst` & `decoratory-0.9.3.6/Readme.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu/decoratory"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.2.4"
-    __date__ = "2023-07-04"
-    __time__ = "09:14:18"
+    __version__ = "0.9.3.2"
+    __date__ = "2023-07-10"
+    __time__ = "14:03:21"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -67,15 +67,15 @@
 This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, simple as well as
 more complex examples are presented. Even if only one particular module
-is needed, it is recommended to view the preceding examples as well. For even
+is needed, it is recommended to view the preceding examples as well. For
 more examples of the full range of possibilities, please refer to
 `Decorator Implementations`_ on the `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
@@ -260,25 +260,25 @@
     # Case 1: decoration @Multiton(key=lambda spec, name: name)
     print(a)                        # Animal('dog', 'Teddy')
     print(b)                        # Animal('cat', 'Molly')
     print(c)                        # Animal('dog', 'Roxie')
 
 With three different names, a separate instance is created in each case.
 In contrast, the following variant distinguishes only two types (equivalence
-classes): animals with a character 'a' in their name and those without and
+classes): animals with a character 'y' in their name and those without and
 thus the key values can only be ``True`` or ``False``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per equivalence class
 
-    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'y' in name)
     print(a)                        # Animal('dog', 'Teddy')
-    print(b)                        # Animal('cat', 'Molly')
-    print(c)                        # Animal('cat', 'Molly')
+    print(b)                        # Animal('dog', 'Teddy')
+    print(c)                        # Animal('dog', 'Roxie')
 
 The initial parameter values of the initializer can also be accessed by their
 ``args``-index or ``kwargs``-name. So the following decorations are also
 possible:
 
 .. code-block:: python
 
@@ -302,15 +302,15 @@
     # Case 6: One unique instance from a @staticmethod or @classmethod
     @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
     class Animal:
         pass                        # Some code ...
 
         @classmethod
         def my_key(cls, spec, name):
-            return 'a' in name
+            return 'y' in name
 
 To actively control access to new equivalence classes, ``Multiton`` provides
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
 and checking the sealing state of the ``Multiton``. By default, the sealing
 state is set ``False``, so for every new key a new (unique) object is
 instantiated. When sealed (e.g. later in the process) is set ``True`` the
 dictionary has completed, i.e. restricted to the current object set and
@@ -357,14 +357,23 @@
         print(f"Sorry {ex.args[1]}, {ex.args[0]}")
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
     Animal.unseal()                 # Unseal the multiton!
     print(Animal.issealed())        # False
     Animal('cat', name='Molly')     # Now, Molly is added
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'),
                                     #  'Molly': Animal('cat', 'Molly')}
+    Animal.get_instances().pop('Teddy')
+    print(Animal.get_instances())   # {'Molly': Animal('cat', 'Molly')}
+    Animal.get_instances().clear()  # Same as Animal.reset()
+    print(Animal.get_instances())   # {}
+
+The last two lines show the functional equivalence of
+``Animal.get_instances().clear()`` with ``Animal.reset()``, but the ``reset``
+option is more transparent because it does not require going
+"behind the stage".
 
 
 ******************************************************************************
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
@@ -402,19 +411,26 @@
         print(f"value = '{value}'")
 
     # Function call with default parameters
     some_function()                 # value = 'original'
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
-The functionality of ``some_function()`` itself remains unchanged. A typical
-scenario for a wrapper is, of course, the execution of additional functionality
-before and/or after a given functionality, which itself remains unchanged,
-such as ``enter/leave`` markers, call data caches, runtime measurements, etc.
-Here is a typical example:
+The functionality of ``some_function()`` itself remains unchanged.
+For the sake of clarity, the principle of *all or nothing* is applied, i.e.
+defaults must be defined for all parameters and they are only used if no
+current parameters at all are transmitted. There is no mixing of current and
+default parameters. Thus, even a call of the decorated function with an
+incomplete parameter set is explicitly not supported and will throw a
+``TypeError``.
+
+A typical scenario for a wrapper is, of course, the execution of additional
+functionality before and/or after a given functionality, which itself remains
+unchanged, such as ``enter/leave`` markers, call data caches, runtime
+measurements, etc. Here is a typical example:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
@@ -658,14 +674,22 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
+Person is an observer, but not an observable, so the call to ``person()``
+reflects only person’s own activity.
+Cat is an observable that is observed by person and therefore the activity
+``cat()`` triggers a follow-up activity by person.
+Calling ``dog()`` results in three activities at the observers, because
+``dog()`` is observed by the *observed cat*, which informs the person about
+its own activity.
+
 The order of reactions is determined by the order in the list in which
 the cat observes the dog prior to the person. If this order is reversed:
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
@@ -676,17 +700,19 @@
     # Case 3: Stacked observable decoration
     #    ---> Cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
 
-Calling ``dog()`` results in three activities at the observers, because
-``dog()`` observes the *observed cat*, which informs the person about its own
-action. If this behavior is not desired, ``dog()`` can instead address the
+Again, calling ``dog()`` results in three activities at the observers,
+but here person reacts first as an observer to dog and later again as an
+observer to cat.
+
+If this behavior is not desired, ``dog()`` can instead address the
 *original cat* using the ``cat.substitute.callee``, i.e.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
@@ -696,31 +722,34 @@
 
     # Case 4: Stacked observable decoration
     #    ---> Original cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Again, cat acts before person because of the order of the observer list and
-because the *original cat* observes dog the ``Hey, cat!`` statement of person
-is missing.
+In this case, cat acts before person because of the order of the observer
+list and because and because the *original cat* observes dog the ``Hey, cat!``
+statement of person is missing.
 
 
 Observer Decoration
 -------------------
 
 In this reversed decoration scheme, the observer decorator collects its
 observables. This seems more elaborate at first glance, but some prefer to
 explicitly designate the ``Observer`` and ``Observable`` roles in their code.
 
 Because an observer decoration uses observable methods, all
-observable(s) must always be declared before their observer(s).
+observable(s) must always be *declared and decorated* before their
+observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
+    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
+
 Thus, the initial example ``Case 1`` from `Observable Decoration`_ translates to:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
     from decoratory.observer import Observer, Observable
@@ -740,19 +769,15 @@
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 The use of the *semantic cross-function* ``X`` from ``decoratory.basic``
 instead of ``F`` indicates that ``dog`` is the observable, but the ``X``
 arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is also relevant, again.
-Each observable must be decorated before it is used by an observer.
-
-    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
-
+For multiple decorations, the *order of decoration* is also relevant here.
 The situation ``Case 2`` from `Observable Decoration`_ with person,
 dog and cat would then look like:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
@@ -815,15 +840,15 @@
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Now, both dog and cat end up being observers, observed by the person. But the
 cat observing the dog is the *original cat*, which does not inform the person
-of its activities, and so its statement ``Hey, cat!`` is missing.
+of its activities, and so person’s statement ``Hey, cat!`` is missing.
 
 
 Class Decoration
 ----------------
 
 Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
@@ -951,15 +976,15 @@
             print(f"Dog {name} arrived.")
 
     # Case 3: Dog is an observable to actions of various person instances.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe says Hello?
                                     # John Doe says What's up?
 
-Here, *one action of the observable*, the instantiation of ``Dog``, triggers
+But here, *one action of the observable*, the instantiation of ``Dog``, triggers
 *one to many actions at each selected resp. instantiated observer*, ``Person``.
 In such situations, a late `dynamic decoration <#dynamic-decoration>`_
 could be a good idea.
 
 So far, instantiating ``Dog`` resulted in an information and induced
 action at ``Person``. If ``Dog`` has its own actions that need to be
 selectively monitored, each of the selected actions can of course be decorated
@@ -1026,15 +1051,15 @@
 ``unregister`` *interface methods that an observable exposes*. Information can
 be given to the right recipients at relevant places in the code. For this,
 the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_
 comes into play. Dynamic decoration is used often also in connection with
 getter/setter/property constructions since data changes take place
 meaningfully over these methods.
 
-Let's consider two simple classes:
+Consider the following two example classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory/__main__.py` & `decoratory-0.9.3.6/Sources/decoratory/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.7"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.6"
+__date__ = "2023-07-10"
+__time__ = "14:09:45"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory/banner.py` & `decoratory-0.9.3.6/Sources/decoratory/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory/basic.py` & `decoratory-0.9.3.6/Sources/decoratory/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory/multiton.py` & `decoratory-0.9.3.6/Sources/decoratory/multiton.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,17 +125,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory/observer.py` & `decoratory-0.9.3.6/Sources/decoratory/observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,17 +407,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory/singleton.py` & `decoratory-0.9.3.6/Sources/decoratory/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory/wrapper.py` & `decoratory-0.9.3.6/Sources/decoratory/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.3.6/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.2.7
+Version: 0.9.3.6
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu/decoratory
-Download-URL: http://evation.eu/decoratory\section\download.html
+Home-page: http://evation.eu/decoratory/index.html
+Download-URL: http://evation.eu/decoratory/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
-Project-URL: Projekt, http://evation.eu/decoratory
-Project-URL: Release Notes, http://evation.eu/decoratory\section\releasenotes.html
-Project-URL: Download, http://evation.eu/decoratory\section\download.html
+Project-URL: Projekt, http://evation.eu/decoratory/index.html
+Project-URL: Release Notes, http://evation.eu/decoratory/Section/ReleaseNotes.html
+Project-URL: Download, http://evation.eu/decoratory/Section/Download.html
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -49,17 +49,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu/decoratory"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.2.4"
-    __date__ = "2023-07-04"
-    __time__ = "09:14:18"
+    __version__ = "0.9.3.2"
+    __date__ = "2023-07-10"
+    __time__ = "14:03:21"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -106,15 +106,15 @@
 This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, simple as well as
 more complex examples are presented. Even if only one particular module
-is needed, it is recommended to view the preceding examples as well. For even
+is needed, it is recommended to view the preceding examples as well. For
 more examples of the full range of possibilities, please refer to
 `Decorator Implementations`_ on the `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
@@ -299,25 +299,25 @@
     # Case 1: decoration @Multiton(key=lambda spec, name: name)
     print(a)                        # Animal('dog', 'Teddy')
     print(b)                        # Animal('cat', 'Molly')
     print(c)                        # Animal('dog', 'Roxie')
 
 With three different names, a separate instance is created in each case.
 In contrast, the following variant distinguishes only two types (equivalence
-classes): animals with a character 'a' in their name and those without and
+classes): animals with a character 'y' in their name and those without and
 thus the key values can only be ``True`` or ``False``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per equivalence class
 
-    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'y' in name)
     print(a)                        # Animal('dog', 'Teddy')
-    print(b)                        # Animal('cat', 'Molly')
-    print(c)                        # Animal('cat', 'Molly')
+    print(b)                        # Animal('dog', 'Teddy')
+    print(c)                        # Animal('dog', 'Roxie')
 
 The initial parameter values of the initializer can also be accessed by their
 ``args``-index or ``kwargs``-name. So the following decorations are also
 possible:
 
 .. code-block:: python
 
@@ -341,15 +341,15 @@
     # Case 6: One unique instance from a @staticmethod or @classmethod
     @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
     class Animal:
         pass                        # Some code ...
 
         @classmethod
         def my_key(cls, spec, name):
-            return 'a' in name
+            return 'y' in name
 
 To actively control access to new equivalence classes, ``Multiton`` provides
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
 and checking the sealing state of the ``Multiton``. By default, the sealing
 state is set ``False``, so for every new key a new (unique) object is
 instantiated. When sealed (e.g. later in the process) is set ``True`` the
 dictionary has completed, i.e. restricted to the current object set and
@@ -396,14 +396,23 @@
         print(f"Sorry {ex.args[1]}, {ex.args[0]}")
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
     Animal.unseal()                 # Unseal the multiton!
     print(Animal.issealed())        # False
     Animal('cat', name='Molly')     # Now, Molly is added
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'),
                                     #  'Molly': Animal('cat', 'Molly')}
+    Animal.get_instances().pop('Teddy')
+    print(Animal.get_instances())   # {'Molly': Animal('cat', 'Molly')}
+    Animal.get_instances().clear()  # Same as Animal.reset()
+    print(Animal.get_instances())   # {}
+
+The last two lines show the functional equivalence of
+``Animal.get_instances().clear()`` with ``Animal.reset()``, but the ``reset``
+option is more transparent because it does not require going
+"behind the stage".
 
 
 ******************************************************************************
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
@@ -441,19 +450,26 @@
         print(f"value = '{value}'")
 
     # Function call with default parameters
     some_function()                 # value = 'original'
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
-The functionality of ``some_function()`` itself remains unchanged. A typical
-scenario for a wrapper is, of course, the execution of additional functionality
-before and/or after a given functionality, which itself remains unchanged,
-such as ``enter/leave`` markers, call data caches, runtime measurements, etc.
-Here is a typical example:
+The functionality of ``some_function()`` itself remains unchanged.
+For the sake of clarity, the principle of *all or nothing* is applied, i.e.
+defaults must be defined for all parameters and they are only used if no
+current parameters at all are transmitted. There is no mixing of current and
+default parameters. Thus, even a call of the decorated function with an
+incomplete parameter set is explicitly not supported and will throw a
+``TypeError``.
+
+A typical scenario for a wrapper is, of course, the execution of additional
+functionality before and/or after a given functionality, which itself remains
+unchanged, such as ``enter/leave`` markers, call data caches, runtime
+measurements, etc. Here is a typical example:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
@@ -697,14 +713,22 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
+Person is an observer, but not an observable, so the call to ``person()``
+reflects only personâ€™s own activity.
+Cat is an observable that is observed by person and therefore the activity
+``cat()`` triggers a follow-up activity by person.
+Calling ``dog()`` results in three activities at the observers, because
+``dog()`` is observed by the *observed cat*, which informs the person about
+its own activity.
+
 The order of reactions is determined by the order in the list in which
 the cat observes the dog prior to the person. If this order is reversed:
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
@@ -715,17 +739,19 @@
     # Case 3: Stacked observable decoration
     #    ---> Cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
 
-Calling ``dog()`` results in three activities at the observers, because
-``dog()`` observes the *observed cat*, which informs the person about its own
-action. If this behavior is not desired, ``dog()`` can instead address the
+Again, calling ``dog()`` results in three activities at the observers,
+but here person reacts first as an observer to dog and later again as an
+observer to cat.
+
+If this behavior is not desired, ``dog()`` can instead address the
 *original cat* using the ``cat.substitute.callee``, i.e.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
@@ -735,31 +761,34 @@
 
     # Case 4: Stacked observable decoration
     #    ---> Original cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Again, cat acts before person because of the order of the observer list and
-because the *original cat* observes dog the ``Hey, cat!`` statement of person
-is missing.
+In this case, cat acts before person because of the order of the observer
+list and because and because the *original cat* observes dog the ``Hey, cat!``
+statement of person is missing.
 
 
 Observer Decoration
 -------------------
 
 In this reversed decoration scheme, the observer decorator collects its
 observables. This seems more elaborate at first glance, but some prefer to
 explicitly designate the ``Observer`` and ``Observable`` roles in their code.
 
 Because an observer decoration uses observable methods, all
-observable(s) must always be declared before their observer(s).
+observable(s) must always be *declared and decorated* before their
+observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
+    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
+
 Thus, the initial example ``Case 1`` from `Observable Decoration`_ translates to:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
     from decoratory.observer import Observer, Observable
@@ -779,19 +808,15 @@
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 The use of the *semantic cross-function* ``X`` from ``decoratory.basic``
 instead of ``F`` indicates that ``dog`` is the observable, but the ``X``
 arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is also relevant, again.
-Each observable must be decorated before it is used by an observer.
-
-    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
-
+For multiple decorations, the *order of decoration* is also relevant here.
 The situation ``Case 2`` from `Observable Decoration`_ with person,
 dog and cat would then look like:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
@@ -854,15 +879,15 @@
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Now, both dog and cat end up being observers, observed by the person. But the
 cat observing the dog is the *original cat*, which does not inform the person
-of its activities, and so its statement ``Hey, cat!`` is missing.
+of its activities, and so personâ€™s statement ``Hey, cat!`` is missing.
 
 
 Class Decoration
 ----------------
 
 Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
@@ -990,15 +1015,15 @@
             print(f"Dog {name} arrived.")
 
     # Case 3: Dog is an observable to actions of various person instances.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe says Hello?
                                     # John Doe says What's up?
 
-Here, *one action of the observable*, the instantiation of ``Dog``, triggers
+But here, *one action of the observable*, the instantiation of ``Dog``, triggers
 *one to many actions at each selected resp. instantiated observer*, ``Person``.
 In such situations, a late `dynamic decoration <#dynamic-decoration>`_
 could be a good idea.
 
 So far, instantiating ``Dog`` resulted in an information and induced
 action at ``Person``. If ``Dog`` has its own actions that need to be
 selectively monitored, each of the selected actions can of course be decorated
@@ -1065,15 +1090,15 @@
 ``unregister`` *interface methods that an observable exposes*. Information can
 be given to the right recipients at relevant places in the code. For this,
 the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_
 comes into play. Dynamic decoration is used often also in connection with
 getter/setter/property constructions since data changes take place
 meaningfully over these methods.
 
-Let's consider two simple classes:
+Consider the following two example classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoratory-0.9.2.7/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.3.6/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.2.7/Unittest/test_basic.py` & `decoratory-0.9.3.6/Unittest/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.2.7/Unittest/test_multiton.py` & `decoratory-0.9.3.6/Unittest/test_multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.2.7/Unittest/test_observer.py` & `decoratory-0.9.3.6/Unittest/test_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.2.7/Unittest/test_singleton.py` & `decoratory-0.9.3.6/Unittest/test_singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.2.7/Unittest/test_wrapper.py` & `decoratory-0.9.3.6/Unittest/test_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.3"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.1"
+__date__ = "2023-07-10"
+__time__ = "13:27:32"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.2.7/setup.py` & `decoratory-0.9.3.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.2.7"
-__date__ = "2023-07-04"
-__time__ = "09:14:18"
+__version__ = "0.9.3.6"
+__date__ = "2023-07-10"
+__time__ = "14:09:45"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
@@ -60,24 +60,24 @@
     # General
     name=__title__,
     version=__version__,
     author=__author__,
     author_email=f'{__author__} <{__email__}>',
     maintainer=f'{__author__}',
     maintainer_email=f'{__author__} <{__email__}>',
-    url=__url__,
-    download_url=join(__url__, "section", "download.html"),
+    url="/".join([__url__, "index.html"]),
+    download_url="/".join([__url__, "Section", "Download.html"]),
     description=('Decorators: Singleton, Multiton, Observer, Observable, '
                  'generic Wrapper.'),
     long_description=description,
     long_description_content_type='text/x-rst',
     project_urls={
-        'Projekt': __url__,
-        'Release Notes': join(__url__, "section", "releasenotes.html"),
-        'Download': join(__url__, "section", "download.html")},
+        'Projekt': "/".join([__url__, "index.html"]),
+        'Release Notes': "/".join([__url__, "Section", "ReleaseNotes.html"]),
+        'Download': "/".join([__url__, "Section", "Download.html"])},
     keywords='decorator singleton multiton observer observable wrapper',
     # Technical
     license=__license__,
     platforms=['Operating System :: OS Independent'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

