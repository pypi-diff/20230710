# Comparing `tmp/airball-0.4.3.tar.gz` & `tmp/airball-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airball-0.4.3.tar", last modified: Sat Jul  1 04:49:16 2023, max compression
+gzip compressed data, was "airball-0.4.4.tar", last modified: Mon Jul 10 02:47:37 2023, max compression
```

## Comparing `airball-0.4.3.tar` & `airball-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.175901 airball-0.4.3/
--rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.4.3/LICENSE
--rw-r--r--   0 zyrxvo     (501) staff       (20)     2919 2023-07-01 04:49:16.175752 airball-0.4.3/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)     2368 2023-07-01 04:45:58.000000 airball-0.4.3/README.md
--rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.4.3/pyproject.toml
--rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-07-01 04:49:16.175961 airball-0.4.3/setup.cfg
--rw-r--r--   0 zyrxvo     (501) staff       (20)      922 2023-07-01 04:48:58.000000 airball-0.4.3/setup.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.172818 airball-0.4.3/src/
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.174527 airball-0.4.3/src/airball/
--rw-r--r--   0 zyrxvo     (501) staff       (20)      334 2023-07-01 04:49:03.000000 airball-0.4.3/src/airball/__init__.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     9107 2023-07-01 04:32:22.000000 airball-0.4.3/src/airball/analytic.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    14527 2023-06-30 08:16:39.000000 airball-0.4.3/src/airball/environments.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    11157 2023-06-29 08:34:54.000000 airball-0.4.3/src/airball/flybys.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     7787 2023-06-30 07:51:03.000000 airball-0.4.3/src/airball/imf.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.4.3/src/airball/particle.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    21713 2023-06-30 06:28:22.000000 airball-0.4.3/src/airball/stars.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     8774 2023-06-30 08:05:48.000000 airball-0.4.3/src/airball/tools.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)      181 2023-06-29 01:38:57.000000 airball-0.4.3/src/airball/units.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.175258 airball-0.4.3/src/airball.egg-info/
--rw-r--r--   0 zyrxvo     (501) staff       (20)     2919 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      419 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/SOURCES.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/dependency_links.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/requires.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/top_level.txt
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-10 02:47:37.653495 airball-0.4.4/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.4.4/LICENSE
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     2920 2023-07-10 02:47:37.653379 airball-0.4.4/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     2368 2023-07-01 04:45:58.000000 airball-0.4.4/README.md
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.4.4/pyproject.toml
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-07-10 02:47:37.653543 airball-0.4.4/setup.cfg
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      923 2023-07-10 02:40:16.000000 airball-0.4.4/setup.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-10 02:47:37.650944 airball-0.4.4/src/
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-10 02:47:37.652587 airball-0.4.4/src/airball/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      334 2023-07-10 02:40:25.000000 airball-0.4.4/src/airball/__init__.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     9107 2023-07-01 04:32:22.000000 airball-0.4.4/src/airball/analytic.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    14922 2023-07-10 02:44:33.000000 airball-0.4.4/src/airball/environments.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    11157 2023-06-29 08:34:54.000000 airball-0.4.4/src/airball/flybys.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     7787 2023-06-30 07:51:03.000000 airball-0.4.4/src/airball/imf.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.4.4/src/airball/particle.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    21700 2023-07-10 02:36:43.000000 airball-0.4.4/src/airball/stars.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     9037 2023-07-10 01:39:56.000000 airball-0.4.4/src/airball/tools.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      181 2023-06-29 01:38:57.000000 airball-0.4.4/src/airball/units.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-10 02:47:37.653216 airball-0.4.4/src/airball.egg-info/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     2920 2023-07-10 02:47:37.000000 airball-0.4.4/src/airball.egg-info/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      419 2023-07-10 02:47:37.000000 airball-0.4.4/src/airball.egg-info/SOURCES.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-07-10 02:47:37.000000 airball-0.4.4/src/airball.egg-info/dependency_links.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-07-10 02:47:37.000000 airball-0.4.4/src/airball.egg-info/requires.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-07-10 02:47:37.000000 airball-0.4.4/src/airball.egg-info/top_level.txt
```

### Comparing `airball-0.4.3/LICENSE` & `airball-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airball-0.4.3/PKG-INFO` & `airball-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.4.3
-Summary: A package for implementing flybys in hannorein/rebound
+Version: 0.4.4
+Summary: A package for running and managing flybys using REBOUND
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `airball-0.4.3/README.md` & `airball-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `airball-0.4.3/setup.py` & `airball-0.4.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="airball",
-    version="0.4.3",
+    version="0.4.4",
     author="Garett Brown",
     author_email="garett.brown@mail.utoronto.ca",
-    description="A package for implementing flybys in hannorein/rebound",
+    description="A package for running and managing flybys using REBOUND",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zyrxvo/airball/",
     project_urls={
         "Bug Tracker": "https://github.com/zyrxvo/airball/issues",
     },
     classifiers=[
```

### Comparing `airball-0.4.3/src/airball/analytic.py` & `airball-0.4.4/src/airball/analytic.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.3/src/airball/environments.py` & `airball-0.4.4/src/airball/environments.py`

 * *Files 11% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     '''
       The number density of the environment.
       Default units: pc^{-3}.
     '''
     if isQuantity(value):
       if value.unit.is_equivalent(units.stars/units.m**3): self._density = value.to(self.units.units['density'])
       elif value.unit.is_equivalent(1/units.m**3): self._density = (value * self.units.units['object']).to(self.units.units['density'])
-      else: AssertionError('The given density units are not compatible.')
+      else: raise AssertionError('The given density units are not compatible.')
     else: self._density = value * self.units.units['density']
 
   @property
   def velocity_dispersion(self):
     '''
       Return the velocity dispersion of the environment.
       Default units: km/s.
@@ -263,17 +263,16 @@
   short_name = 'Local'
   def local_mass_function(x):
     '''
       This defined using Chabrier (2003) for single stars when m < 1 and a power-law model from Bovy (2017) for stars m ≥ 1 to account for depleted stars due to stellar evolution.
     '''
     return chabrier_2003_single(1, 0.0567) * (x)**-4.7 if x > 1 else chabrier_2003_single(x, 0.0567)
 
-  def __init__(self, stellar_density = 0.14 * units.stars/units.pc**3, velocity_dispersion = 20.8 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 8 * units.solMass, maximum_impact_parameter=None, UNIT_SYSTEM=[], mass_function=local_mass_function):
+  def __init__(self, stellar_density = 0.14 * units.stars/units.pc**3, velocity_dispersion = 20.8 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 8 * units.solMass, maximum_impact_parameter=10000 * units.au, UNIT_SYSTEM=[], mass_function=local_mass_function):
     super().__init__(stellar_density=stellar_density, velocity_dispersion=velocity_dispersion, lower_mass_limit=lower_mass_limit, upper_mass_limit=upper_mass_limit, mass_function=mass_function, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Local Neighborhood')
-    self.maximum_impact_parameter = 10000 * units.au if maximum_impact_parameter is None else maximum_impact_parameter
 
 class OpenCluster(StellarEnvironment):
   '''
     This is a AIRBALL StellarEnvironment subclass for a generic Open Cluster.
     It encapsulates the relevant data for a static stellar environment representing a generic open cluster.
 
     The stellar density is 100 pc^-3 informed by Adams (2010).
@@ -283,32 +282,28 @@
     # Example
     my_open = airball.OpenCluster()
     my_10stars = my_open.random_star(size=10)
     # returns a Stars object with the masses, impact parameters, velocities, and orientation of the 10 Star objects in a heliocentric model.
   '''
   short_name = 'Open'
   
-  def __init__(self, maximum_impact_parameter=None, UNIT_SYSTEM=[]):
-    super().__init__(stellar_density = 100 * units.stars * units.pc**-3, velocity_dispersion = 1 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 100 * units.solMass, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Open Cluster')
-    self._maximum_impact_parameter = 1000 * units.au
+  def __init__(self, stellar_density = 100 * units.stars * units.pc**-3, velocity_dispersion = 1 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 100 * units.solMass, maximum_impact_parameter=1000 * units.au, UNIT_SYSTEM=[]):
+    super().__init__(stellar_density=stellar_density, velocity_dispersion=velocity_dispersion, lower_mass_limit=lower_mass_limit, upper_mass_limit=upper_mass_limit, mass_function=None, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Open Cluster')
 
 class GlobularCluster(StellarEnvironment):
   short_name = 'Globular'
   
-  def __init__(self, maximum_impact_parameter=None, UNIT_SYSTEM=[]):
-    super().__init__(stellar_density = 1000 * units.stars * units.pc**-3, velocity_dispersion = 10 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 1 * units.solMass, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Globular Cluster')
-    self._maximum_impact_parameter = 5000 * units.au
+  def __init__(self, stellar_density = 1000 * units.stars * units.pc**-3, velocity_dispersion = 10 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 1 * units.solMass, maximum_impact_parameter=5000 * units.au, UNIT_SYSTEM=[]):
+    super().__init__(stellar_density=stellar_density, velocity_dispersion=velocity_dispersion, lower_mass_limit=lower_mass_limit, upper_mass_limit=upper_mass_limit, mass_function=None, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Globular Cluster')
 
 class GalacticBulge(StellarEnvironment):
   short_name = 'Bulge'
   
-  def __init__(self, maximum_impact_parameter=None, UNIT_SYSTEM=[]):
-    super().__init__(stellar_density = 50 * units.stars * units.pc**-3, velocity_dispersion = 120 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 10 * units.solMass, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Milky Way Bulge')
-    self._maximum_impact_parameter = 50000 * units.au
+  def __init__(self, stellar_density = 50 * units.stars * units.pc**-3, velocity_dispersion = 120 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 10 * units.solMass, maximum_impact_parameter=50000 * units.au, UNIT_SYSTEM=[]):
+    super().__init__(stellar_density=stellar_density, velocity_dispersion=velocity_dispersion, lower_mass_limit=lower_mass_limit, upper_mass_limit=upper_mass_limit, mass_function=None, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Milky Way Bulge')
 
 class GalacticCore(StellarEnvironment):
   short_name = 'Core'
   
-  def __init__(self, maximum_impact_parameter=None, UNIT_SYSTEM=[]):
-    super().__init__(stellar_density = 10000 * units.stars * units.pc**-3, velocity_dispersion = 170 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 10 * units.solMass, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Milky Way Core')
-    self._maximum_impact_parameter = 50000 * units.au
+  def __init__(self, stellar_density = 10000 * units.stars * units.pc**-3, velocity_dispersion = 170 * units.km/units.s, lower_mass_limit=0.08 * units.solMass, upper_mass_limit = 10 * units.solMass, maximum_impact_parameter=50000 * units.au, UNIT_SYSTEM=[units.yr]):
+    super().__init__(stellar_density=stellar_density, velocity_dispersion=velocity_dispersion, lower_mass_limit=lower_mass_limit, upper_mass_limit=upper_mass_limit, mass_function=None, maximum_impact_parameter=maximum_impact_parameter, UNIT_SYSTEM=UNIT_SYSTEM, name = 'Milky Way Core')
```

### Comparing `airball-0.4.3/src/airball/flybys.py` & `airball-0.4.4/src/airball/flybys.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.3/src/airball/imf.py` & `airball-0.4.4/src/airball/imf.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.3/src/airball/particle.py` & `airball-0.4.4/src/airball/particle.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.3/src/airball/stars.py` & `airball-0.4.4/src/airball/stars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import numpy as _numpy
 from scipy.stats import uniform as _uniform
 from .tools import *
 
-try:
-    # Required for Python>=3.9
-    from collections.abc import MutableMapping
-except:
-    from collections import MutableMapping
-
+try: from collections.abc import MutableMapping # Required for Python>=3.9
+except: from collections import MutableMapping
 
 class Star:
   '''
     This is the AIRBALL Star class.
     It encapsulates the relevant parameters for a given star.
     Only the mass is an quantity intrinsic to the object.
     The impact parameter, velocity, inclination, argument of periastron, and longitude of the ascending node quantities are defined with respect to the host star and plane passing through the star.
```

### Comparing `airball-0.4.3/src/airball/tools.py` & `airball-0.4.4/src/airball/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,21 @@
       self._units['angle'] = angleUnit[0] if angleUnit != [] else self._units['angle']
 
       objectUnit = [this for this in UNIT_SYSTEM if this.is_equivalent(units.stars)]
       self._units['object'] = objectUnit[0] if objectUnit != [] else units.stars
 
       densityUnit = [this for this in UNIT_SYSTEM if this.is_equivalent(units.stars/units.m**3)]
       densityUnit2 = [this for this in UNIT_SYSTEM if this.is_equivalent(1/units.m**3)]
-      if densityUnit == [] and densityUnit2 != []: densityUnit = [self._object_unit * densityUnit2[0]]
-      elif densityUnit == [] and objectUnit != [] and lengthUnit != []: densityUnit = [self._units['object']/self._units['length']**3]
+      if densityUnit == [] and densityUnit2 != []: 
+        densityUnit = [self._units['object'] * densityUnit2[0]]
+      elif densityUnit == [] and objectUnit != [] and lengthUnit != []: 
+        densityUnit = [self._units['object']/self._units['length']**3]
+      elif densityUnit == [] and densityUnit2 == [] and objectUnit != []:
+         densityLength = [this for this in self._units['density'].bases if this.is_equivalent(units.m)][0]
+         densityUnit = [self._units['object']/densityLength**3]
       self._units['density'] = densityUnit[0] if densityUnit != [] else self._units['density']
     
     self._UNIT_SYSTEM = list(self._units.values())
 
 
 
 ############################################################
@@ -172,15 +177,15 @@
         R : interaction radius (default units: AU)
         M : mass of a typical flyby star (default units: solMass)
     '''
     n = verify_unit(n, unit_set.units['density'])
     v = verify_unit(v, unit_set.units['velocity'])
     R = verify_unit(R, unit_set.units['length'])
     M = verify_unit(M, unit_set.units['mass'])
-    
+
     return n * v * cross_section(M, R, v, unit_set)
 
 def verify_unit(value, unit):
     return value.to(unit) if isQuantity(value) else value * unit
 
 def isList(l):
     '''Determines if an object is a list or numpy array. Used for flyby parallelization.'''
```

### Comparing `airball-0.4.3/src/airball.egg-info/PKG-INFO` & `airball-0.4.4/src/airball.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.4.3
-Summary: A package for implementing flybys in hannorein/rebound
+Version: 0.4.4
+Summary: A package for running and managing flybys using REBOUND
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

