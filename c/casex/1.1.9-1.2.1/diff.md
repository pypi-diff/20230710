# Comparing `tmp/casex-1.1.9.tar.gz` & `tmp/casex-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\casex-1.1.9.tar", last modified: Mon May 23 13:56:47 2022, max compression
+gzip compressed data, was "dist\casex-1.2.1.tar", last modified: Mon Jul 10 13:26:58 2023, max compression
```

## Comparing `casex-1.1.9.tar` & `casex-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-05-23 13:56:47.000000 casex-1.1.9/
-drwxrwxrwx   0        0        0        0 2022-05-23 13:56:47.000000 casex-1.1.9/casex/
--rw-rw-rw-   0        0        0    18058 2020-12-05 15:03:30.000000 casex-1.1.9/casex/aircraft_specs.py
--rw-rw-rw-   0        0        0    11828 2022-05-22 21:24:51.000000 casex-1.1.9/casex/annex_f_parms.py
--rw-rw-rw-   0        0        0    14922 2022-05-22 21:21:27.000000 casex-1.1.9/casex/annex_f_tables.py
--rw-rw-rw-   0        0        0    11320 2020-12-18 07:43:14.000000 casex-1.1.9/casex/ballistic_descent_models.py
--rw-rw-rw-   0        0        0      225 2020-12-07 08:58:42.000000 casex-1.1.9/casex/constants.py
--rw-rw-rw-   0        0        0     2163 2020-11-23 15:00:03.000000 casex-1.1.9/casex/conversion.py
--rw-rw-rw-   0        0        0    19402 2022-05-22 20:21:52.000000 casex-1.1.9/casex/critical_area_models.py
--rw-rw-rw-   0        0        0     1122 2020-11-09 08:54:39.000000 casex-1.1.9/casex/enums.py
--rw-rw-rw-   0        0        0      367 2020-11-20 13:21:48.000000 casex-1.1.9/casex/exceptions.py
--rw-rw-rw-   0        0        0     9435 2020-12-18 07:43:14.000000 casex-1.1.9/casex/explosion_models.py
--rw-rw-rw-   0        0        0    28447 2022-05-22 20:24:28.000000 casex-1.1.9/casex/figures.py
--rw-rw-rw-   0        0        0      715 2021-08-10 07:40:48.000000 casex-1.1.9/casex/flyaway_models.py
--rw-rw-rw-   0        0        0     7941 2020-12-03 11:38:40.000000 casex-1.1.9/casex/friction_coefficient.py
--rw-rw-rw-   0        0        0     9778 2021-10-22 11:35:28.000000 casex-1.1.9/casex/ground_risk_buffer.py
--rw-rw-rw-   0        0        0     4617 2020-12-05 15:03:30.000000 casex-1.1.9/casex/misc.py
--rw-rw-rw-   0        0        0    40298 2021-02-05 12:05:45.000000 casex-1.1.9/casex/obstacles.py
--rw-rw-rw-   0        0        0     6993 2020-12-18 11:02:58.000000 casex-1.1.9/casex/obstacle_simulation.py
--rw-rw-rw-   0        0        0     1306 2021-02-23 22:47:23.000000 casex-1.1.9/casex/temporary_testing_figures.py
--rw-rw-rw-   0        0        0      472 2022-05-22 20:21:52.000000 casex-1.1.9/casex/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-23 13:56:47.000000 casex-1.1.9/casex.egg-info/
--rw-rw-rw-   0        0        0        1 2022-05-23 13:56:47.000000 casex-1.1.9/casex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-12-29 10:07:56.000000 casex-1.1.9/casex.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2786 2022-05-23 13:56:47.000000 casex-1.1.9/casex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       41 2022-05-23 13:56:47.000000 casex-1.1.9/casex.egg-info/requires.txt
--rw-rw-rw-   0        0        0      651 2022-05-23 13:56:47.000000 casex-1.1.9/casex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2022-05-23 13:56:47.000000 casex-1.1.9/casex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2020-10-20 09:11:26.000000 casex-1.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0     2786 2022-05-23 13:56:47.000000 casex-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2185 2021-02-23 11:19:58.000000 casex-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2022-05-23 13:56:47.000000 casex-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      933 2022-05-23 13:56:41.000000 casex-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:26:58.000000 casex-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:26:58.000000 casex-1.2.1/casex/
+-rw-rw-rw-   0        0        0    15514 2023-07-10 11:29:40.000000 casex-1.2.1/casex/aircraft_specs.py
+-rw-rw-rw-   0        0        0    12292 2023-07-10 11:29:16.000000 casex-1.2.1/casex/annex_f_parms.py
+-rw-rw-rw-   0        0        0    23506 2023-07-10 12:42:42.000000 casex-1.2.1/casex/annex_f_tables.py
+-rw-rw-rw-   0        0        0    11320 2023-07-10 12:24:08.000000 casex-1.2.1/casex/ballistic_descent_models.py
+-rw-rw-rw-   0        0        0      224 2023-07-10 09:35:41.000000 casex-1.2.1/casex/constants.py
+-rw-rw-rw-   0        0        0     2163 2020-11-23 15:00:03.000000 casex-1.2.1/casex/conversion.py
+-rw-rw-rw-   0        0        0    18061 2023-07-10 12:23:50.000000 casex-1.2.1/casex/critical_area_models.py
+-rw-rw-rw-   0        0        0      974 2023-07-07 10:55:23.000000 casex-1.2.1/casex/enums.py
+-rw-rw-rw-   0        0        0      494 2023-05-16 08:00:45.000000 casex-1.2.1/casex/exceptions.py
+-rw-rw-rw-   0        0        0     9435 2020-12-18 07:43:14.000000 casex-1.2.1/casex/explosion_models.py
+-rw-rw-rw-   0        0        0    27407 2023-07-10 13:12:13.000000 casex-1.2.1/casex/figures.py
+-rw-rw-rw-   0        0        0     7941 2020-12-03 11:38:40.000000 casex-1.2.1/casex/friction_coefficient.py
+-rw-rw-rw-   0        0        0     9778 2021-10-22 11:35:28.000000 casex-1.2.1/casex/ground_risk_buffer.py
+-rw-rw-rw-   0        0        0     4617 2020-12-05 15:03:30.000000 casex-1.2.1/casex/misc.py
+-rw-rw-rw-   0        0        0    40298 2021-02-05 12:05:45.000000 casex-1.2.1/casex/obstacles.py
+-rw-rw-rw-   0        0        0     6993 2020-12-18 11:02:58.000000 casex-1.2.1/casex/obstacle_simulation.py
+-rw-rw-rw-   0        0        0     1306 2021-02-23 22:47:23.000000 casex-1.2.1/casex/temporary_testing_figures.py
+-rw-rw-rw-   0        0        0      472 2023-07-07 10:54:37.000000 casex-1.2.1/casex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:26:58.000000 casex-1.2.1/casex.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:26:57.000000 casex-1.2.1/casex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-12-29 10:07:56.000000 casex-1.2.1/casex.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2789 2023-07-10 13:26:57.000000 casex-1.2.1/casex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-07-10 13:26:57.000000 casex-1.2.1/casex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      627 2023-07-10 13:26:57.000000 casex-1.2.1/casex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 13:26:57.000000 casex-1.2.1/casex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2020-10-20 09:11:26.000000 casex-1.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2789 2023-07-10 13:26:58.000000 casex-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2023-03-01 14:11:00.000000 casex-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:26:58.000000 casex-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-07-10 13:24:24.000000 casex-1.2.1/setup.py
```

### Comparing `casex-1.1.9/casex/aircraft_specs.py` & `casex-1.2.1/casex/aircraft_specs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,26 @@
 Class to hold parameters on the aircraft used in area computations.
 """
 import warnings
 import numpy as np
 
 from casex import enums, constants
 
-
 class AircraftSpecs:
     """    
     This class is designed to hold all the parameters on a specific aircraft for which a critical area is to be
     computed. Many of the these parameters are not used in computations of critical area, but are reserved for
     future use.
 
     Parameters
     ----------
     aircraft_type : :class:`enums.AircraftType`
         Type of aircraft.
     width : float
         [m] Width of aircraft (wingspan, characteristic dimension).
-    length : float
-        [m] Length of aircraft.
     mass : float
         [kg] Mass of the aircraft.
     fuel_type : :class:'enums.FuelType, optional
         Fuel type, such as fossil fuels or batteries (the default is `FuelType.GASOLINE`).
     fuel_quantity : float, optional
         [L] The quantity of fuel in liters. For batteries the quantity is also given in L,
         i.e. the volume of the battery (the default is 0, which means that no deflagration is assumed upon crash).
@@ -32,16 +29,14 @@
     Attributes
     ----------
     width : float
         [m] The width of the aircraft is the horizontal size of the aircraft orthogonal to the direction of travel.
         This value is used to determine the width of the glide and slide areas. Therefore, this value is the wingspan
         for fixed wing aircraft, the rotor diameter for rotorcraft, and the rotortip to rotortip distance for
         multirotor aircraft.
-    length : float
-        [m] Length of the aircraft. The concept is the same as width. The length is only used in the RCC model.
     mass : float
         [kg] Mass of the aircraft in kg. This is the total mass at the time of crash, including fuel.
     aircraft_type : :class:`enums.AircraftType`
         The type of aircraft.
     fuel_type : :class:`enums.FuelType`
         Fuel type, such as fossil fuels or batteries (the default is `FuelType.GASOLINE`).
     fuel_quantity : float
@@ -71,39 +66,38 @@
         [s] Deployment time for the parachute, measured from the time deployment is signalled to full deployment.
     parachute_area : float
         [m^2] Area of the parachute generating drag during descent and full deployment.
     parachute_drag_coef : float
         [-] Drag coefficient.
     """
 
-    def __init__(self, aircraft_type, width, length, mass, fuel_type=enums.FuelType.GASOLINE, fuel_quantity=0):
+    def __init__(self, aircraft_type, width, mass, fuel_type=enums.FuelType.GASOLINE, fuel_quantity=0):
         self.ballistic_frontal_area = None
         self.ballistic_drag_coefficient = None
         self.glide_drag_coefficient = None
         self.max_flight_time = None
         self.cruise_speed = None
         self.glide_speed = None
         self.glide_ratio = None
         self.parachute_deployment_time = None
         self.parachute_area = None
         self.parachute_drag_coef = None
 
         self.reset_values()
 
         self.width = width
-        self.length = length
         self.mass = mass
 
         # Default values.
         self.friction_coefficient = 0.6
         self.coefficient_of_restitution = 0.7
         self.fuel_type = fuel_type
         self.fuel_quantity = fuel_quantity
 
-        self.width_length_mass_check()
+        self.width_mass_check()
 
         if not isinstance(aircraft_type, enums.AircraftType):
             warnings.warn("Aircraft type not recognized. Type set to fixed wing.")
             self.aircraft_type = enums.AircraftType.FIXED_WING
         else:
             self.aircraft_type = aircraft_type
 
@@ -138,50 +132,35 @@
             [m] Width of the aircraft
             
         Returns
         -------
         None
         """
         self.width = width
-        self.width_length_mass_check()
-
-    def set_length(self, length):
-        """Set the aircraft length.
-        
-        Parameters
-        ----------
-        length : float
-            [m] Length of the aircraft.
-
-        Returns
-        -------
-        None
-        """
-        self.length = length
-        self.width_length_mass_check()
+        self.width_mass_check()
 
     def set_mass(self, mass):
         """Set the aircraft mass.
                 
         Parameters
         ----------
         mass : float
             [kg] Mass of aircraft.
 
         Returns
         -------
         None
         """
         self.mass = mass
-        self.width_length_mass_check()
+        self.width_mass_check()
 
-    def width_length_mass_check(self):
-        """Out of range check on width, length, and mass.
+    def width_mass_check(self):
+        """Out of range check on width and mass.
         
-        Performs an out of range check of width, length, and mass. Warnings are issued for parameters out of range.
+        Performs an out of range check of width and mass. Warnings are issued for parameters out of range.
         
         Parameters
         ----------
 
         Returns
         -------
         None
@@ -190,19 +169,14 @@
             warnings.warn("Non-positive mass does not make sense. Subsequent results are invalid.")
         elif np.any(self.mass < 1):
             warnings.warn("This package is not designed for a mass below 1 kg. Subsequent results cannot be trusted.")
         if np.any(self.width <= 0):
             warnings.warn("Non-positive width does not make sense. Subsequent results are invalid.")
         elif np.any(self.width < 0.1):
             warnings.warn("This package is not designed for a width below 0.1 m. Subsequent results cannot be trusted.")
-        if np.any(self.length <= 0):
-            warnings.warn("Non-positive length does not make sense. Subsequent results are invalid.")
-        elif np.any(self.length < 0.1):
-            warnings.warn(
-                "This package is not designed for a length below 0.1 m. Subsequent results cannot be trusted.")
 
     def set_fuel_type(self, fuel_type):
         """Set the type of fuel.
         
         Sets the type of fuel onboard the aircraft. For a list of options, see :class:`enums.FuelType`.
         
         Parameters
@@ -258,24 +232,24 @@
 
     def set_coefficient_of_restitution(self, coefficient_of_restitution):
         """Set coefficient of restitution.
         
         Parameters
         ----------
         coefficient_of_restitution : float
-            [-] Coefficient of restitution for the ground impact (the default is 0.7).
+            [-] Coefficient of restitution for the ground impact.
  
         Returns
         -------
         None
         """
         if np.any(coefficient_of_restitution <= 0):
             warnings.warn(
                 "Non-positive coefficient of restitution does not make sense. Subsequent results are invalid.")
-        if np.any(coefficient_of_restitution > 1.5):
+        if np.any(coefficient_of_restitution > 1.0):
             warnings.warn("Coefficient of restitution seems very large. Subsequent results may be invalid.")
 
         self.coefficient_of_restitution = coefficient_of_restitution
 
     def set_ballistic_frontal_area(self, ballistic_frontal_area):
         """Set frontal area for computation of terminal velocity in ballistic descent.
         
@@ -421,62 +395,26 @@
         -------
         terminal_velocity : float
             [m/s] The terminal velocity for the aircraft.
         """
         return np.sqrt(2 * self.mass * constants.GRAVITY / constants.AIR_DENSITY / self.ballistic_frontal_area /
                        self.ballistic_drag_coefficient)
 
-    def COR_from_impact_angle(self, impact_angle, angles=None, CoRs=None):
-        """Compute a coefficient of restitution for a given impact angle.
-        
-        This method assumes an affine relation between impact angle and CoR. Therefore, two angles and two CoR values
-        are used to determine this relation. The default is as described in Annex F that the CoR is 0.9 at a 9 degree
-        impact and 0.6 at a 90 degree (vertical) impact. This values are used as defaults, but others can be specified.
-        
-        Parameters
-        ----------        
-        impact_angle : float
-            [deg] The impact angle between 0 and 90.
-        angles : float array, optional
-            [deg] Array with two different angle of impact values (the default is [9, 90]).
-        CoRs : float array, optional
-            [-] Array with two COR values corresponding to the two angles (the default is [0.9, 0.6]).
-
-        Returns
-        -------
-        coefficient of restitution : float
-            [-] The coefficient of restitution for the given impact angle.
-        """
-        if angles is None:
-            angles = [9, 90]
-        if CoRs is None:
-            CoRs = [0.9, 0.6]
-
-        if np.any(impact_angle < 0):
-            warnings.warn("Impact angle must be positive. Output is not valid.")
-        if np.any(impact_angle > 90):
-            warnings.warn("Impact angle must be less than 90 degrees. Output is not valid.")
-
-        param = np.polyfit(angles, CoRs, 1)
-
-        return param[0] * impact_angle + param[1]
-
     def reset_values(self):
         """Reset all aircraft parameters.
 
         Parameters
         ----------
  
         Returns
         -------
         None
         """
         self.aircraft_type = None
         self.width = None
-        self.length = None
         self.mass = None
         self.cruise_speed = None
         self.max_flight_time = None
         self.fuel_type = None
         self.fuel_quantity = None
         self.glide_speed = None
         self.glide_ratio = None
```

### Comparing `casex-1.1.9/casex/annex_f_parms.py` & `casex-1.2.1/casex/annex_f_parms.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,70 +12,75 @@
 
 class AnnexFParms:
     """This class contains the following parameters for the 5 size classes in the iGRC table:
 
     Parameters
     ----------
     impact_angle : float
-        [deg] The impact angle of the descending aircraft, measured relative to the ground.
+        [deg] The impact angle of the descending aircraft, relative to horizontal.
 
     Attributes
     ----------
-    wingspan : float
-        Characteristic dimension of the aircraft. See Annex F :cite:`a-JARUS_AnnexF`
-        for more detailed explanation on what that is.
-    critical_area_target : float
-        [m^2] Size of the largest critical area for each size class.
-    cruise_speed : float
-        [m/s]Maximum cruise speed for each size class.
-    mass : float
-        [kg] Assumed biggest mass for each size class.
-    KE_critical : float
-        [J] Non-lethal energy during slide.
-    friction_coefficient = 0.5 : float
-        [-] The friction coefficient is assumed constant at 0.5 throughout Annex F :cite:`a-JARUS_AnnexF`.
-    glide_reduce = 0.7 : float
-        [-] Reduction in glide speed relative to cruise speed.
-    glide_speed : float
-        [m/s] The glide speed resulting from multiplying the cruise speed by glide_reduce.
     aircraft : :class:`AircraftSpecs`
         The class containing information about the aircraft.
-    scenario_angles = [9, 35, 80] : float array
-        [deg] The three impact angles for the three descent scenarios. The 80 degrees is not actually used but
-        recomputed for each ballistic descent.
-    terminal_velocity : float
-        [m/s] Terminal velocity for aircraft.
-    ballistic_frontal_area : float
-        [m^2] Assumed frontal area used in ballistic computations.
-    ballistic_drag_coefficient = 0.7 : float
-        [-] Drag coefficient used for ballistic descent.
+    aircraft_type : :class:`enums.AircraftType`
+        The type of aircraft. This parameters is not currently used.
+    critical_area_target : float
+        [m^2] Size of the largest critical area for each size class.
     ballistic_descent_altitude : float
         [m] Assumed altitude for beginning of ballistic descent.
-    ballistic_impact_velocity :float
-        [m/s] Assumed horizontal velocity for beginning of ballistic descent.
-    ballistic_impact_angle : float
-        [deg] Computed impact angle with 0 being horizontal.
+    ballistic_descent_time : float
+        [s] Computed descent time for ballistic descent.
     ballistic_distance : float
         [m] Computed horizontal distance traveled during ballistic descent.
+    ballistic_drag_coefficient = 0.8 : float
+        [-] Drag coefficient used for ballistic descent.
+    ballistic_frontal_area : float
+        [m^2] Assumed frontal area used in ballistic computations.
+    ballistic_impact_angle : float
+        [deg] Computed impact angle with 0 being horizontal.
     ballistic_impact_KE : float
         [J] Computed kinetic energy of aircraft just prior to impact.
-    ballistic_descent_time : float
-        [s] Computed descent time for ballistic descent.
+    ballistic_impact_velocity : float
+        [m/s] Assumed horizontal velocity for beginning of ballistic descent.
+    cruise_speed : float
+        [m/s]Maximum cruise speed for each size class.
+    friction_coefficient = 0.65 : float
+        [-] The friction coefficient is assumed constant at 0.65 throughout Annex F :cite:`a-JARUS_AnnexF`.
+    glide_reduce = 0.65 : float
+        [-] Reduction in glide speed relative to cruise speed.
+    glide_speed : float
+        [m/s] The glide speed resulting from multiplying the cruise speed by glide_reduce.
     impact_angle : float
         [deg] The impact angle of the aircraft when crashing, measure relative to horizontal.
-    aircraft_type : :class:`enums.AircraftType`
-        The type of aircraft. This parameters is not currently used.
-    horizontal_COR : float
-        [-] The coefficient of restitution for a near horizontal impact.
-    vertical_COR : float
-        [-] The coefficient of restitution for a vertical impact. The actual COR is determined
-        as a first order interpolation between `horizontal_COR` for 0 degrees and `vertical_COR`
-        for 90 degrees.
+    KE_critical : float
+        [J] Non-lethal energy during slide.
+    mass : float
+        [kg] Assumed biggest mass for each size class.
+    population_bands = [0.25 25 250 2500 25000 250000] : float array
+        [ppl/km2] The population density bands used for the iGRC.
+    scenario_angles = [10, 35, 62] : float array
+        [deg] The three impact angles for the three descent scenarios. The 62 degrees is not actually used but
+        recomputed for each ballistic descent.
+    terminal_velocity : float
+        [m/s] Terminal velocity for aircraft.
+    wingspan : float
+        Characteristic dimension of the aircraft. See Annex F :cite:`a-JARUS_AnnexF`
+        for more detailed explanation on what that is.
     """
 
+    person_radius = 0.3
+    person_height= 1.8
+    lethal_kinetic_energy = 290
+    obstacle_reduction_factor = 0.6
+    scenario_angles = np.array([10, 35, 62])
+    glide_reduce = 0.65
+    friction_coefficient = 0.65
+    ballistic_drag_coefficient = 0.8
+
     # This dataclass make the programming and plotting more smooth in allowing for looping for virtually all values.
     @dataclass
     class CAParameters:
         wingspan: float
         critical_area_target: float
         cruise_speed: float
         iGRC_impact_angle : float
@@ -88,65 +93,56 @@
         ballistic_impact_angle: float = 0
         ballistic_distance: float = 0
         ballistic_impact_KE: float = 0
         ballistic_descent_time: float = 0
         glide_speed: float = 0
         aircraft: AircraftSpecs = None
 
-    def __init__(self, impact_angle):
-        self.glide_reduce = 0.7
-        self.friction_coefficient = 0.5
-        self.ballistic_drag_coefficient = 0.7
-        self.scenario_angles = np.array([9, 35, 80])
-
-        self.impact_angle = impact_angle
+    def __init__(self):
+        self.population_bands = [0.25, 25, 250, 2500, 25000, 250000]
 
         # Set aircraft type, the type has no effect in this example, but must be given a value.
         self.aircraft_type = enums.AircraftType.GENERIC
 
         # Setup the parameters used in the plotting.
         self.CA_parms = []
-        #                                      Width   CA       Speed    iGRC angle  Drag area   Mass     lethal KE   Altitude
-        self.CA_parms.append(self.CAParameters(1,      6.5,     25,      35,         0.1,        3,       290/0.5,    50))
-        self.CA_parms.append(self.CAParameters(3,      200,     35,      35,         0.5,        50,      290,        100))
-        self.CA_parms.append(self.CAParameters(8,      2000,    75,      35,         2.0,        400,     290,        200))
-        self.CA_parms.append(self.CAParameters(20,     20000,   150,     35,         8.0,        5000,    290,        500))
-        self.CA_parms.append(self.CAParameters(40,     66000,   200,     35,         14,         10000,   290,        1000))
-    
-        # Upper and low value for coefficient of restitution (over 9 to 90 degree impact angles).
-        self.horizontal_COR = 0.9
-        self.vertical_COR = 0.6
+        #                                      Width   CA       Speed    iGRC angle                  Drag area      Mass        lethal KE                     Altitude
+        self.CA_parms.append(self.CAParameters(1,      8,        25,      self.scenario_angles[1],         0.1,        3,       self.lethal_kinetic_energy/0.5,    75))
+        self.CA_parms.append(self.CAParameters(3,      80,       35,      self.scenario_angles[1],         0.5,        50,      self.lethal_kinetic_energy,        100))
+        self.CA_parms.append(self.CAParameters(8,      800,      75,      self.scenario_angles[1],         2.0,        400,     self.lethal_kinetic_energy,        200))
+        self.CA_parms.append(self.CAParameters(20,     8000,     150,     self.scenario_angles[1],         8.0,        5000,    self.lethal_kinetic_energy,        500))
+        self.CA_parms.append(self.CAParameters(40,     43000,    200,     self.scenario_angles[1],         14,         10000,   self.lethal_kinetic_energy,        1000))
 
-        self.recompute_parameters()
+        self.recompute_parameters(self.scenario_angles[1])
 
-    def recompute_parameters(self):
+    def recompute_parameters(self, impact_angle):
         BDM = BallisticDescent2ndOrderDragApproximation()
 
         # Compute the parameters for each of the 5 size classes.
         for k in range(5):
             # Compute glide speed based on cruise speed
             self.CA_parms[k].glide_speed = self.glide_reduce * self.CA_parms[k].cruise_speed
 
             # Define the aircraft.
-            self.CA_parms[k].aircraft = AircraftSpecs(self.aircraft_type, self.CA_parms[k].wingspan, 1,
-                                                      self.CA_parms[k].mass)
+            self.CA_parms[k].aircraft = AircraftSpecs(self.aircraft_type, self.CA_parms[k].wingspan, self.CA_parms[k].mass)
 
             # Set parameters into aircraft.
             self.CA_parms[k].aircraft.set_ballistic_frontal_area(self.CA_parms[k].ballistic_frontal_area)
             self.CA_parms[k].aircraft.set_ballistic_drag_coefficient(self.ballistic_drag_coefficient)
             self.CA_parms[k].aircraft.set_friction_coefficient(self.friction_coefficient)
 
             if k == 0:
-                # The 1 m column uses 0.9 as CoR in all cases.
-                self.CA_parms[k].aircraft.set_coefficient_of_restitution(0.9)
+                # The 1 m column uses 0.8 as CoR in all cases.
+                if isinstance(impact_angle, np.ndarray):
+                    self.CA_parms[k].aircraft.set_coefficient_of_restitution(self.CoR_from_impact_angle(np.full(len(impact_angle), 10)))
+                else:
+                    self.CA_parms[k].aircraft.set_coefficient_of_restitution(self.CoR_from_impact_angle(10))
             else:
                 # The other columns uses a CoR depending on angle.
-                self.CA_parms[k].aircraft.set_coefficient_of_restitution(
-                    self.CA_parms[k].aircraft.COR_from_impact_angle(self.impact_angle, [self.scenario_angles[0], 90],
-                                                                    [self.horizontal_COR, self.vertical_COR]))
+                self.CA_parms[k].aircraft.set_coefficient_of_restitution(self.CoR_from_impact_angle(impact_angle))
 
             # Compute terminal velocity.
             self.CA_parms[k].terminal_velocity = self.CA_parms[k].aircraft.terminal_velocity()
 
             # Compute ballistic descent values.
             BDM.set_aircraft(self.CA_parms[k].aircraft)
             p = BDM.compute_ballistic_distance(self.CA_parms[k].ballistic_descent_altitude,
@@ -154,15 +150,15 @@
             self.CA_parms[k].ballistic_impact_velocity = p[1]
             self.CA_parms[k].ballistic_impact_angle = p[2] * 180 / np.pi
             self.CA_parms[k].ballistic_distance = p[0]
             self.CA_parms[k].ballistic_descent_time = p[3]
             self.CA_parms[k].ballistic_impact_KE = 0.5 * self.CA_parms[k].mass * np.power(p[1], 2)        
 
     @staticmethod
-    def iGRC(pop_dens, CA, TLOS=1E-6, width = 0, use_obstacle_reduction = False, use_integer_reduction = False):
+    def iGRC(pop_dens, CA, TLOS=1E-6, width = 0, use_conservative_compensation = False):
         """Compute the finale integer iGRC as described in Annex F :cite:`a-JARUS_AnnexF`.
         
         This method computes the integer and the raw iGRC values for a given population density and
         size of critical area. The TLOS, target level of safety, can also be set, but the default value
         is :math:`10^{-6}` as described in Annex F :cite:`a-JARUS_AnnexF`.
         
         .. note:: This method converts the population density to ppl/m^2 as needed for the equation.
@@ -174,76 +170,88 @@
         pop_dens : float
             [ppl/km^2] Population density
         CA : float
             [m^2] Size of the critical area.
         TLOS : float, optional
             [fatalities per flight hour] Target level of safety (the default is 1e-6).
             This value is described in more detail in Annex F :cite:`a-JARUS_AnnexF`.
-        use_obstacle_reduction : bool, optional
-            If True, the obstacle reduction (see obstacle_reduction_factor()) is applied to the iGRC value. This requires width to be set.
-            Default value is False.
         width : float, optional
             Width of the aircraft. This is needed if use_obstacle_reduction is set to True. Otherwise, it is ignored.
             Default value is 0.
-        use_integer_reduction: bool, optional
+        use_conservative_compensation: bool, optional
             if True, the 0.3 reduction in iGRC value is applied.
             
         Returns
         -------
         iGRC : integer
             The intrinsic ground risk class (as an integer). This is the raw value rounded up to nearest integer.
         raw iGRC : float
             The raw iGRC before rounding up.
         """
-        if use_obstacle_reduction:
-            if width == 0:
-                warnings.warn("width is not set. Using value of 1 m.")
-                width = 1
-            pop_dens = pop_dens * AnnexFParms.obstacle_reduction_factor(pop_dens, width)
-        
         # Note that the 1E-6 here is the conversion from km^2 to m^2.
         raw_iGRC_value = 1 - math.log10(TLOS / (pop_dens * 1E-6 * CA))
         
-        if use_integer_reduction:
+        if use_conservative_compensation:
             raw_iGRC_value = raw_iGRC_value - 0.3
             
         # The raw iGRC value may be rounded to one decimal.
         raw_iGRC_value = round(raw_iGRC_value * 10) / 10
 
         return math.ceil(raw_iGRC_value), raw_iGRC_value
 
     @staticmethod
-    def obstacle_reduction_factor(pop_dens, width):
+    def applied_obstacle_reduction_factor(width):
         """Compute the obstacle reduction factor used in the iGRC in Annex F :cite:`a-JARUS_AnnexF`.
         
-        The obstacle reduction factor as shown in the table below:
-
-        +---------------------------------+--------------------+---------------------+
-        |                                 | 1 m < width <= 3 m | 3 m < width <= 20 m |
-        +---------------------------------+--------------------+---------------------+
-        | 1,500 <= pop density < 100,000  |    120/200         |     700/2000        |
-        +---------------------------------+--------------------+---------------------+
-
-        and 1 if either pop density or width is outside ranges in the table.
-        
         Parameters
         ----------
         pop_dens : float
             [ppl/km^2] Population density
-        width : float
-            [m] Width of aircraft.
             
         Returns
         -------
         obstacle_reduction_factor : float
             The reduction factor for use in iGRC.
         """
 
-        obstacle_reduction_factor = 1
+        if isinstance(width, np.ndarray):
+            resulting_factor = np.where(np.logical_and(width > 1, width < 40), AnnexFParms.obstacle_reduction_factor, 1)
+        else:
+            resulting_factor = AnnexFParms.obstacle_reduction_factor if 1 < width < 40 else 1
+           
+        return resulting_factor
 
-        if 1500 <= pop_dens < 100000:
-            if 1 < width <= 3:
-                obstacle_reduction_factor = 120 / 200
-            elif 3 < width <= 20:
-                obstacle_reduction_factor = 700 / 2000
-            
-        return obstacle_reduction_factor
+    @staticmethod
+    def CoR_from_impact_angle(impact_angle, angles = None, CoRs = None):
+        """Compute a coefficient of restitution for a given impact angle.
+        
+        This method assumes an affine relation between impact angle and CoR. Therefore, two angles and two CoR values
+        are used to determine this relation. The default is as described in Annex F that the CoR is 0.8 at a 10 degree
+        impact and 0.6 at a 90 degree (vertical) impact. This values are used as defaults, but others can be specified.
+        
+        Parameters
+        ----------        
+        impact_angle : float
+            [deg] The impact angle between 0 and 90.
+        angles : float array, optional
+            [deg] Array with two different angle of impact values (the default is [10, 90]).
+        CoRs : float array, optional
+            [-] Array with two COR values corresponding to the two angles (the default is [0.8, 0.6]).
+
+        Returns
+        -------
+        coefficient of restitution : float
+            [-] The coefficient of restitution for the given impact angle.
+        """
+        if angles is None:
+            angles = [10, 90]
+        if CoRs is None:
+            CoRs = [0.8, 0.6]
+
+        if np.any(impact_angle < 0):
+            warnings.warn("Impact angle must be positive. Output is not valid.")
+        if np.any(impact_angle > 90):
+            warnings.warn("Impact angle must be less than 90 degrees. Output is not valid.")
+
+        param = np.polyfit(angles, CoRs, 1)
+
+        return param[0] * impact_angle + param[1]
```

### Comparing `casex-1.1.9/casex/ballistic_descent_models.py` & `casex-1.2.1/casex/ballistic_descent_models.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/conversion.py` & `casex-1.2.1/casex/conversion.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/critical_area_models.py` & `casex-1.2.1/casex/critical_area_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 """
 import math
 import warnings
 from collections.abc import Iterable
 
 import numpy as np
 
-from casex import enums, aircraft_specs, explosion_models, Conversion, constants, exceptions
-
+from casex import AnnexFParms, enums, aircraft_specs, explosion_models, Conversion, constants, exceptions
 
 class CriticalAreaModels:
     """
-    This class is used for computing the critical area for a crash when the basic parameters for the
-    aircraft is known. It support five different models, including the JARUS model, as described in
+    This class is used for computing the critical area using the JARUS model for a crash when the basic parameters for the
+    aircraft is known. The math behind the model is described in
     Appendix B in Annex F :cite:`c-JARUS_AnnexF`.
     
     The main method in this class is `critical_area`, which computes the size of the critical area given
     a number of input arguments relating to the aircraft.
     
     There are two attributes in this class for describing
     a standard person, namely `buffer` and `height`.
@@ -33,225 +32,197 @@
     ----------
     buffer : float, optional
         [m] Radius of a standard person as seen from above (the default is 0.3 m).
     height : float, optional
         [m] The altitude above the ground at which the aircraft can first impact a person (the default is 1.8 m).
     """
 
-    def __init__(self, buffer=0.3, height=1.8):
+    def __init__(self, buffer = AnnexFParms.person_radius, height = AnnexFParms.person_height):
         self.buffer = buffer
         self.height = height
 
-    def critical_area(self, critical_area_model, aircraft, impact_speed, impact_angle, critical_areas_overlap, var1=-1):
+    def critical_area(self, aircraft, impact_speed, impact_angle, critical_areas_overlap = 0, lethal_kinetic_energy = -1, use_obstacle_reduction = True):
         """Computes the lethal area as modeled by different models.
         
-        The models are described in more detail in Annex F :cite:`c-JARUS_AnnexF`. References for each model is given
-        in the code.
-        
         This function supports one of the following input parameters to be a vector, which will give a vector of the
         same size as output:
             
         * `impact_speed`
         * `impact_angle`
         * `critical_area_overlap`
         * `aircraft.width`
-        * `aircraft.length`
         * `aircraft.fuel_quantity`
         
         This vector is given as ``numpy.array``, and only one of the parameters can be a vector for each call.
         The return values are then also ``numpy.array`` IF the input parameter that is a ``numpy.array`` is used in the
         computation.
 
         Parameters
         ----------       
-        critical_area_model : :class:`enums.CriticalAreaModel`
-            Choice of model (RCC :cite:`c-RangeCommandersCouncil1999`, RTI :cite:`c-Montgomery1995`, FAA :cite:`c-FAA2011`,
-            NAWCAD :cite:`c-Ball2012`, JARUS :cite:`c-JARUS_AnnexF`). See Annex F for details :cite:`c-JARUS_AnnexF`.
         aircraft : :class:`casex.AircraftSpecs`
             Class with information about the aircraft.
         impact_speed : float
             [m/s] Impact speed of aircraft (this is speed along the velocity vector).
         impact_angle : float
-            [deg] Impact angle relative to ground (90 is vertical, straight down).
-        critical_areas_overlap : float
-            [0 to 1] Fraction of overlap between lethal area from glide/slide and from explosion/deflagration.
-        var1 : float, optional
-            An additional variable that is used in FAA, NAWCAD, and JARUS models.
-            For the FAA model, `var1` = :math:`F_A`, the ratio of secondary debris field to primary debris field. If not
-            specified, :math:`F_A` = 4.36 will be used. See :cite:`c-FAA2011` page 98.
-
-            For the NAWCAD model, `var1` is the lethal kinetic energy threshold in J. If not specified (or set to -1)
-            the value 73.2 J is used.
-
-            For the JARUS model, `var1` is the lethal kinetic energy threshold in J. If not specified (or set to -1),
-            the following is done (see Annex F Appendix A :cite:`c-JARUS_AnnexF` for details): `var1` is set to 290 J,
-            except when the width of the aircraft is <= 1 m, in which case `var1` is set to :math:`2 \cdot 290` J.
+            [deg] Impact angle relative to ground (90 is vertical, straight down). Note that when using the JARUS model
+            and the width of the aircraft is <= 1 m, the impact angle used is minimum 35 degrees, regardless of input.
+            See Appendix A.5 in Annex F :cite:`c-JARUS_AnnexF` for details.
+        critical_areas_overlap : float, optional
+            [0 to 1] Fraction of overlap between lethal area from glide/slide and from explosion/deflagration. Default is 0.
+        lethal_kinetic_energy : float, optional
+            The lethal kinetic energy threshold in J. If not specified (or set to -1),
+            the standard approach as described in Annex F Appendix A :cite:`c-JARUS_AnnexF` is used.
+            If set to a positive value, this value is used independently of all other parameters. If set to a negative value other than -1,
+            this value is used following the Annex F standard approach, but with absolute of the given value.
+        use_obstacle_reduction : bool, optional
+            If set to true, the Annex F obstacle reduction is applied as described in the Annex.
+            If set to false, no obstacle reduction is applied.
+            Default is true.
         
         Returns
         -------       
         critical area : float
             [:math:`\mathrm{m}^2`] Size of the critical area for the selected model.
         estimated glide area : float
             [:math:`\mathrm{m}^2`] The glide and slide areas are estimated as the relation between the glide and slide
             distances multiplied by the glide+slide area.
         estimated slide area : float
             [:math:`\mathrm{m}^2`] The estimated slide area.
         critical area inert : float
             [:math:`\mathrm{m}^2`] The inert part of the critical area.
         deflagration area : float
-            [:math:`\mathrm{m}^2`] The deflagration area as given by the deflagration model.
+            [:math:`\mathrm{m}^2`] The deflagration area as given by the deflagration model. Always 0 for non-JARUS models.
+        glide distance : float
+            [:math:`\mathrm{m}`] The glide distance.
+        slide distance non lethal: float
+            [:math:`\mathrm{m}`] The slide distance until non-lethal. Always 0 for non-JARUS models.
+        velocity min kill : float
+            [:math:`\mathrm{m/s}`] The speed at which the slide is no longer lethal. Always 0 for non-JARUS and NAWCAD models.
+        t safe : float
+            [:math:`\mathrm{s}`] The time between impact and when slide speed is non-lethal. Always 0 for non-JARUS and NAWCAD models.
 
         Raises
         ------
         InvalidAircraftError
             If the aircraft is not of type AircraftSpecs.
+        OnlyOneVetorInputError
+            There is more than one vector input, which is not supported.
         """
-        # Check on input argument validity
-        if not isinstance(critical_area_model, enums.CriticalAreaModel):
-            warnings.warn("Critical area model not recognized. Type set to RCC.")
-            critical_area_model = enums.CriticalAreaModel.RCC
-
         if not isinstance(aircraft, aircraft_specs.AircraftSpecs):
             raise exceptions.InvalidAircraftError("Aircraft not recognized. Must be of type AircraftSpecs.")
 
         # Instantiate necessary classes.
         exp = explosion_models.ExplosionModels()
 
+        # True if we should use the Annex F approach to applying KE to the crash. False otherwise.
+        KE_AnnexF_approach = lethal_kinetic_energy < 0
+        
+        # Set the correct lethal kinetic energy
+        if lethal_kinetic_energy == -1:
+            lethal_kinetic_energy = AnnexFParms.lethal_kinetic_energy
+        else:
+            lethal_kinetic_energy = abs(lethal_kinetic_energy)
+            
+        # Implement the Annex F approach
+        if KE_AnnexF_approach:
+            # Set value for a scalar width.
+            if not isinstance(aircraft.width, np.ndarray):
+                if aircraft.width <= 1:
+                    lethal_kinetic_energy = lethal_kinetic_energy * 2
+            # Set value for array width.
+            else:
+                #lethal_kinetic_energy = np.full(len(aircraft.width), lethal_kinetic_energy)
+                lethal_kinetic_energy = np.where(aircraft.width <= 1, 2 * lethal_kinetic_energy, lethal_kinetic_energy)
+
         # Compute additional parameters.
         horizontal_impact_speed = self.horizontal_speed_from_angle(impact_angle, impact_speed)
         glide_distance = self.glide_distance(impact_angle)
+        
+        # Default to zero.
+        slide_distance_non_lethal = 0
+        velocity_min_kill = 0
+        t_safe = 0
 
-        # Compute the inert LA.
-        if critical_area_model == enums.CriticalAreaModel.RCC:
-            # Slide distance based on friction.
-            slide_distance_friction = self.slide_distance_friction(horizontal_impact_speed,
-                                                                   aircraft.friction_coefficient)
-            # [RCC, p. D-4]
-            glide_area = np.multiply(aircraft.length + glide_distance + 2 * self.buffer,
-                                     aircraft.width + 2 * self.buffer)
-            slide_area = np.multiply(slide_distance_friction, aircraft.width + 2 * self.buffer)
-
-        elif critical_area_model == enums.CriticalAreaModel.RTI:
-            # Slide distance based on friction.
-            slide_distance_friction = self.slide_distance_friction(
-                aircraft.coefficient_of_restitution * horizontal_impact_speed, aircraft.friction_coefficient)
-
-            # [1, p. 6]
-            glide_area = 2 * (self.buffer + aircraft.width / 2) * glide_distance + math.pi * np.power(
-                self.buffer + aircraft.width / 2, 2)
-            slide_area = slide_distance_friction * (2 * self.buffer + aircraft.width)
-
-        elif critical_area_model == enums.CriticalAreaModel.FAA:
-            # [FAA, p. 99]
-            r_D = self.buffer + aircraft.width / 2
-
-            # F_A comes from table 6-5 in [FAA, p. 98]. Here using the median for 20/80 distribution between hard and
-            # soft surfaces.
-            if var1 == -1:
-                F_A = 4.36
-            else:
-                F_A = var1
-
-            r_Ac = self.buffer + aircraft.width / 2 * np.sqrt(F_A)
-            hs = self.height * np.sin(np.deg2rad(90 - impact_angle))
-            y2m = np.power(2 * r_Ac * hs, 2) - np.power(np.power(r_Ac, 2) + np.power(hs, 2) - np.power(r_D, 2), 2)
-
-            # If y2m becomes negative, it means that A_C_mark should become zero, because the secondary
-            # debris area is larger than the total glide area. This is accomplished by simply setting y2 = 0.
-            y2m = np.maximum(0, y2m)
-            y2 = np.sqrt(y2m) / (2 * hs)
-
-            A_C_mark = 2 * y2 * hs
-            A_C_mark = A_C_mark + (
-                    y2 * np.sqrt(np.power(r_D, 2) - np.power(y2, 2)) + np.power(r_D, 2) * np.arcsin(y2 / r_D))
-            A_C_mark = A_C_mark - (
-                    y2 * np.sqrt(np.power(r_Ac, 2) - np.power(y2, 2)) + np.power(r_Ac, 2) * np.arcsin(y2 / r_Ac))
-
-            # Note that this is not identical to (12), since (12) assumes 0 degrees is vertical and not horizontal.
-            LA_inert = math.pi * np.power(self.buffer + aircraft.width / 2 * np.sqrt(F_A), 2) + A_C_mark
-
-            glide_area = math.pi * np.power(self.buffer + aircraft.width / 2, 2)
-            slide_area = LA_inert - glide_area
-
-        elif critical_area_model == enums.CriticalAreaModel.NAWCAD:
-            # All from NAWCAD model
-            if var1 == -1:
-                KE_lethal = Conversion.ftlb_to_J(54)
-            else:
-                KE_lethal = var1
-
-            # P. 18 (the following equation is just KE to mass and velocity, not taken from NAWCAD)
-            velocity_min_kill = np.sqrt(2 * KE_lethal / aircraft.mass)
-
-            # Intermediate variable
-            acceleration = aircraft.friction_coefficient * constants.GRAVITY
-
-            # P. 17
-            # This is (15), but it seems to be wrong; normally at = v, not 2at = v
-            # t_safe = (horizontal_impact_speed - velocity_min_kill) / 2 / aircraft.friction_coefficient / constants.GRAVITATIONAL
-            # This seems to be the correct formula
-            t_safe = (horizontal_impact_speed - velocity_min_kill) / acceleration
-
-            # If t_safe is negative, it can safely be set to zero to be ignored in the following computations.
-            t_safe = np.maximum(0, t_safe)
-
-            # P. 17
-            skid_distance_lethal = (horizontal_impact_speed * t_safe) - (0.5 * acceleration * t_safe * t_safe)
-
-            # P. 25
-            glide_area = glide_distance * (2 * self.buffer + aircraft.width)
-            slide_area = skid_distance_lethal * (2 * self.buffer + aircraft.width)
-
-        elif critical_area_model == enums.CriticalAreaModel.JARUS:
-            if var1 == -1:
-                # Set default value for a scalar width.
-                if not isinstance(aircraft.width, np.ndarray):
-                    if aircraft.width <= 1:
-                        KE_lethal = 290 * 2
-                    else:
-                        KE_lethal = 290
-                # Set default value for array width.
+        default_impact_angle = AnnexFParms.scenario_angles[1]
+        
+        # Get the obstacle reduction factor as described in Annex F.
+        obstacle_reduction_factor = AnnexFParms.applied_obstacle_reduction_factor(aircraft.width)
+        
+        # Special concession on impact angle for below 1 m.
+        if isinstance(aircraft.width, np.ndarray):
+            if isinstance(impact_angle, np.ndarray):
+                raise Exception("impact_angle and aircraft.width cannot both be vectors.")
+            impact_angle = np.where(aircraft.width <= 1, max(default_impact_angle, impact_angle), impact_angle)
+        else:
+            if aircraft.width <= 1:
+                if not isinstance(impact_angle, np.ndarray):
+                    impact_angle = max(default_impact_angle, impact_angle)
                 else:
-                    KE_lethal = np.full(len(aircraft.width), 290)
-                    KE_lethal = np.where(aircraft.width <= 1, 2 * KE_lethal, KE_lethal)
-            else:
-                KE_lethal = var1
+                    impact_angle = np.where(impact_angle < default_impact_angle, default_impact_angle, impact_angle)                 
 
-            velocity_min_kill = np.sqrt(2 * KE_lethal / aircraft.mass)
-            acceleration = aircraft.friction_coefficient * constants.GRAVITY
-
-            t_safe = (aircraft.coefficient_of_restitution * horizontal_impact_speed - velocity_min_kill) / acceleration
-            t_safe = np.maximum(0, t_safe)
+        velocity_min_kill = np.sqrt(2 * lethal_kinetic_energy / aircraft.mass)
+        acceleration = aircraft.friction_coefficient * constants.GRAVITY
+        
+        t_safe = (aircraft.coefficient_of_restitution * horizontal_impact_speed - velocity_min_kill) / acceleration
+        t_safe = np.maximum(0, t_safe)
 
-            slide_distance_lethal = (aircraft.coefficient_of_restitution * horizontal_impact_speed * t_safe) - (
-                    0.5 * acceleration * t_safe * t_safe)
+        slide_distance_non_lethal = (aircraft.coefficient_of_restitution * horizontal_impact_speed * t_safe) - (
+                0.5 * acceleration * t_safe * t_safe)
 
-            circular_end = math.pi * np.power(self.buffer + aircraft.width / 2, 2)
-            glide_area = 2 * (self.buffer + aircraft.width / 2) * glide_distance + circular_end
-            slide_area = slide_distance_lethal * (2 * self.buffer + aircraft.width) + circular_end
+        # Compute a half disc to attach to one end of glide and slide.
+        circular_end = math.pi * np.power(self.buffer + aircraft.width / 2, 2) / 2
+        
+        glide_area = 2 * (self.buffer + aircraft.width / 2) * glide_distance + circular_end
+        slide_area = slide_distance_non_lethal * (2 * self.buffer + aircraft.width) + circular_end
 
-            # Concession for aircraft below 1 m.
+        # Concession for aircraft below 1 m.
+        if not isinstance(aircraft.width, np.ndarray):
             if aircraft.width <= 1:
-                slide_distance_lethal = 0
-                slide_area = 0
+                if not isinstance(slide_distance_non_lethal, np.ndarray):
+                    slide_distance_non_lethal = 0
+                else:
+                    slide_distance_non_lethal = np.full(len(slide_distance_non_lethal), 0)
+                if not isinstance(slide_area, np.ndarray):
+                    slide_area = 0
+                else:
+                    slide_area = np.full(len(slide_area), 0)
+        else:
+            slide_distance_non_lethal[aircraft.width <= 1] = 0
+            slide_area[aircraft.width <= 1] = 0
+
+        # Obstacle reduction is applied to the right variables
+        if use_obstacle_reduction:
+            glide_area = glide_area * obstacle_reduction_factor
+            slide_area = slide_area * obstacle_reduction_factor
+            glide_distance = glide_distance * obstacle_reduction_factor
 
         # Add glide and slide from model.
-        LA_inert = glide_area + slide_area
+        CA_inert = glide_area + slide_area
 
         # Compute deflagration area based on both fireball and thermal lethal area.
         TNT = exp.TNT_equivalent_mass(aircraft.fuel_type, aircraft.fuel_quantity)
         FB = exp.fireball_area(TNT)
         p_lethal = 0.1
         TLA = exp.lethal_area_thermal(TNT, p_lethal)
-        LA_deflagration = np.maximum(FB, TLA)
+        CA_deflagration = np.maximum(FB, TLA)
 
         # Compute the overlapping area between inert and deflagration.
-        overlapping_area = np.minimum(LA_inert, LA_deflagration) * np.maximum(0, np.minimum(critical_areas_overlap, 1))
-
-        return LA_inert + LA_deflagration - overlapping_area, glide_area, slide_area, LA_inert, LA_deflagration
+        if np.any(critical_areas_overlap) < 0 or np.any(critical_areas_overlap) > 1:
+            warnings.warn("Critical area overlap must be between 0 and 1. Subsequent computations are not valid.")
+        overlapping_area = np.minimum(CA_inert, CA_deflagration) * critical_areas_overlap
+
+        return CA_inert + CA_deflagration - overlapping_area, \
+                glide_area, \
+                slide_area, \
+                CA_inert, \
+                CA_deflagration, \
+                glide_distance, \
+                slide_distance_non_lethal, \
+                velocity_min_kill, \
+                t_safe
 
     @staticmethod
     def slide_distance_friction(velocity, friction_coefficient):
         """Computes slide distance based on initial velocity and friction.
         
         Sliding distance computed based on the assumption
```

### Comparing `casex-1.1.9/casex/explosion_models.py` & `casex-1.2.1/casex/explosion_models.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/figures.py` & `casex-1.2.1/casex/figures.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,41 +136,37 @@
         save_fig : bool, optional
             If True save the figure to a PNG (default is False).
             
         Returns
         -------
         None
         """
-        # Data on person size.
-        person_width = 0.3
-        person_height = 1.8
-
         # Instantiate necessary class.
-        CA = CriticalAreaModels(person_width, person_height)
+        CA = CriticalAreaModels()
 
         # Sampling density.
         angle_samples = 100
         speed_samples = 100
 
         # Plotting range for the impact angle.
         impact_angle = np.linspace(1, 80, angle_samples)
 
-        # Plotting range for the speed for each of the four scenarios.
+        # Plotting range for the speed for each of the five graphs.
         speed_plot_range = np.array([50, 70, 120, 250, 300])
 
         # Get the four scenario.
-        AFP = AnnexFParms(impact_angle)
+        AFP = AnnexFParms()
 
         # Contour levels for each plot.
         # Note that the CA target is not included, since it is already listed above (and is plotted in different color).
         contour_levels = []
         contour_levels.append(np.array([5, 10, 30, 50, 100]))
-        contour_levels.append(np.array([100, 300, 400, 600]))
-        contour_levels.append(np.array([500, 1000, 3000, 5000]))
-        contour_levels.append(np.array([5000, 10000, 30000, 50000]))
+        contour_levels.append(np.array([30, 50, 100, 200, 300]))
+        contour_levels.append(np.array([300, 500, 1000, 2000]))
+        contour_levels.append(np.array([1000, 4000, 10000, 20000]))
         contour_levels.append(np.array([5000, 10000, 30000, 50000]))
 
         # Set to true to plot the COR.
         if show_contours:
             fig, axcor = plt.subplots(1, 1, figsize=(12, 6))
 
             axcor.plot(impact_angle, AFP.CA_parms[0].aircraft.coefficient_of_restitution)
@@ -183,42 +179,39 @@
         if show_matrix:
             main_color = 'yellow'
             side_color = 'white'
         else:
             main_color = 'black'
             side_color = 'grey'
 
-        print("Ballistic descent computations")
-        print("------------------------------")
-        print("Class   Init horiz     From     Terminal   Impact   Impact   Distance   Descent      KE")
-        print("          speed      altitude   velocity   speed    angle    traveled    time      impact")
+        overlap = 0
 
         c = 0
         for j in range(2):
             for k in range(3):
 
+                # There is not sixth graph.
                 if c > 4:
                     break
 
                 # Speed range for the plot.
                 impact_speed = np.linspace(0, speed_plot_range[c], speed_samples)
 
                 # Initialize CA matrix.
                 CA_matrix = np.zeros((speed_samples, angle_samples))
 
+                #obstacle_reduction_factor = AFP.obstacle_reduction_factor if AFP.CA_parms[c].aircraft.width < 40 else 1
+
                 # Compute the CA matrix.
                 for i in range(speed_samples):
                     impact_speed_i = impact_speed[i]
 
-                    overlap = 0
-
-                    CA_matrix[i, :] = CA.critical_area(enums.CriticalAreaModel.JARUS, AFP.CA_parms[c].aircraft,
-                                                       impact_speed_i, impact_angle, overlap,
-                                                       AFP.CA_parms[c].KE_critical)[0]
-
+                    CA_matrix[i, :] = CA.critical_area(AFP.CA_parms[c].aircraft, impact_speed_i, impact_angle,
+                                                       overlap)[0]
+                    
                 # Show the CA matrix.
                 if show_matrix:
                     im = ax[j, k].imshow(np.log(CA_matrix),
                                          extent=[impact_angle[0], impact_angle[-1], impact_speed[0], impact_speed[-1]],
                                          aspect='auto', origin='lower')
 
                     # This is code for getting a colorbar. Not so useful in the combined plot, but can be used if
@@ -251,22 +244,15 @@
 
                 ax[j, k].set_ylabel('Impact speed  [m/s]')
                 ax[j, k].set_title('Critical area [m$^2$] for {:d} m'.format(AFP.CA_parms[c].wingspan))
 
                 ax[j, k].set_xlim(0, 80)
                 ax[j, k].grid()
 
-                ax[j, k].legend(['9 deg scenario', '35 deg scenario', 'Ballistic scenario'])
-
-                print("{:2d} m      {:3d} m/s     {:4d} m    {:3.0f} m/s   {:3.0f} m/s   {:1.0f} deg    {:4.0f} m     "
-                      "{:4.1f} s   {:6.0f} kJ".format(
-                    AFP.CA_parms[c].wingspan, AFP.CA_parms[c].cruise_speed, AFP.CA_parms[c].ballistic_descent_altitude,
-                    AFP.CA_parms[c].terminal_velocity, AFP.CA_parms[c].ballistic_impact_velocity,
-                    AFP.CA_parms[c].ballistic_impact_angle, AFP.CA_parms[c].ballistic_distance,
-                    AFP.CA_parms[c].ballistic_descent_time, AFP.CA_parms[c].ballistic_impact_KE / 1000))
+                ax[j, k].legend(['10 deg scenario', '35 deg scenario', 'Ballistic scenario'])
 
                 c = c + 1
 
         # The loop above was interrupted, and c was left one too large.
         c = c - 1
 
         # Show x axis label only for the two lower plots.
@@ -343,29 +329,29 @@
         None
         """
         # TODO: Update this when Annex F is finished.
 
         show_old_quantization = show_old_quantization and show_reduced_CA_axis
 
         # Instantiate the Annex F class. The impact angle is not relevant for this example, so the value is random.
-        impact_angle = 35
-        AFP = AnnexFParms(impact_angle)
+        #impact_angle = 35
+        AFP = AnnexFParms()
 
         # Let CA span from 1 to 66k (we need to add a bit to the upper limit, so the numerics of the log10 does not
-        # exclude he value from the axis).
+        # exclude the value from the axis).
         CA = np.logspace(math.log10(1), math.log10(66e3 + 100), 500)
         # Let pop_density span from 0.01 to 500k.
         pop_density = np.logspace(math.log10(0.01), math.log10(5e5 + 3000), 500)
 
         M = np.zeros((len(CA), len(pop_density)))
 
         for pop_density_i in range(len(pop_density)):
             for CA_i in range(len(CA)):
-                ORF = AFP.obstacle_reduction_factor(pop_density[pop_density_i], CA[CA_i]) if show_with_obstacles else 1
-                M[pop_density_i][CA_i] = AFP.iGRC(pop_density[pop_density_i], CA[CA_i] * ORF)[0] - 0.3
+                ORF = AnnexFParms.obstacle_reduction_factor if CA[CA_i] > 8 and CA[CA_i] < 43000 and show_with_obstacles else 1
+                M[pop_density_i][CA_i] = AFP.iGRC(pop_density[pop_density_i], CA[CA_i] * ORF, use_conservative_compensation = True)[0]
 
         fig = plt.figure(figsize=(16, 9))
         ax = plt.axes()
 
         # Show the matrix as an image.
         im = ax.imshow(M, extent=[math.log10(CA[0]), math.log10(CA[-1]), math.log10(pop_density[0]),
                                   math.log10(pop_density[-1])], aspect='auto', origin='lower')
@@ -373,16 +359,15 @@
         # Change this to true to get a color bar.
         if show_colorbar:
             divider = make_axes_locatable(ax)
             cax = divider.append_axes('right', size='5%', pad=0.05)
             fig.colorbar(im, cax=cax, orientation='vertical')
 
         # CA axis tick values in log10.
-        #CA_ticks = np.array([math.log10(CA[0]), 0.813, 2.3, 3.3, 4.3, 4.82])
-        CA_ticks = np.log10(np.array([CA[0], 6.5, 200, 2000, 20000, 66000]))
+        CA_ticks = np.log10(np.array([CA[0], 8, 80, 800, 8000, 43000]))
         CA_ticks_additional = np.log10(np.array([20, 50, 100, 500, 1000, 5E3, 10E3, 4E4, 10E4])) if show_additional_grid else []
 
         xtick_actual_values = np.sort(np.concatenate([CA_ticks, CA_ticks_additional]))
 
         # Add x tick labels.
         xtick_wingspan = ['1', 'n/a', '0.5', '1.2', '3', '1.6', '3.9', '8', '4.5', '9.5', '20', '22', '36']
         xtick_velocity = ['25', 'n/a', '35', '35', '35', '75', '75', '75', '150', '150', '150', '200', '200']
```

### Comparing `casex-1.1.9/casex/friction_coefficient.py` & `casex-1.2.1/casex/friction_coefficient.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/ground_risk_buffer.py` & `casex-1.2.1/casex/ground_risk_buffer.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/misc.py` & `casex-1.2.1/casex/misc.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/obstacles.py` & `casex-1.2.1/casex/obstacles.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/obstacle_simulation.py` & `casex-1.2.1/casex/obstacle_simulation.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex/temporary_testing_figures.py` & `casex-1.2.1/casex/temporary_testing_figures.py`

 * *Files identical despite different names*

### Comparing `casex-1.1.9/casex.egg-info/PKG-INFO` & `casex-1.2.1/casex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: casex
-Version: 1.1.9
+Version: 1.2.1
 Summary: Casualty expectation toolbox
 Home-page: UNKNOWN
 Author: Anders la Cour-Harbo et al
 Author-email: anders@lacourfamily.dk
 License: CC-BY-4.0
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
@@ -48,24 +48,19 @@
 for any purpose, even commercially. The licensor cannot revoke these freedoms as long as you follow the license terms.
 You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.
 
 Do note that according to this license you must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
 
 We recommend the following reference to CasEx:
 
-    CasEx: Casual Expectation Toolbox in Python. JARUS WG-6 SORA Annex F Quantitative Methods subgroup, 2021. Available at https://casex.readthedocs.io.
+    CasEx: Casual Expectation Toolbox in Python. JARUS WG-6 SORA Annex F Quantitative Methods subgroup, 2023. Available at https://casex.readthedocs.io.
 
 And as BibTeX:
 
 
-    @misc{JARUSWG6QuantitativeMethodssubgroup2021,
+    @misc{JARUSWG6QuantitativeMethodssubgroup2023,
     author = {{JARUS WG-6 SORA Annex F Quantitative Methods subgroup}},
     title = {{CasEx: Casual Expectation Toolbox in Python}},
     url = {casex.readthedocs.io},
-    year = {2021}
+    year = {2023}
     }
 
-
-
-
-
-
```

### Comparing `casex-1.1.9/casex.egg-info/SOURCES.txt` & `casex-1.2.1/casex.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 casex/constants.py
 casex/conversion.py
 casex/critical_area_models.py
 casex/enums.py
 casex/exceptions.py
 casex/explosion_models.py
 casex/figures.py
-casex/flyaway_models.py
 casex/friction_coefficient.py
 casex/ground_risk_buffer.py
 casex/misc.py
 casex/obstacle_simulation.py
 casex/obstacles.py
 casex/temporary_testing_figures.py
 casex.egg-info/PKG-INFO
```

### Comparing `casex-1.1.9/PKG-INFO` & `casex-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: casex
-Version: 1.1.9
+Version: 1.2.1
 Summary: Casualty expectation toolbox
 Home-page: UNKNOWN
 Author: Anders la Cour-Harbo et al
 Author-email: anders@lacourfamily.dk
 License: CC-BY-4.0
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
@@ -48,24 +48,19 @@
 for any purpose, even commercially. The licensor cannot revoke these freedoms as long as you follow the license terms.
 You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.
 
 Do note that according to this license you must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
 
 We recommend the following reference to CasEx:
 
-    CasEx: Casual Expectation Toolbox in Python. JARUS WG-6 SORA Annex F Quantitative Methods subgroup, 2021. Available at https://casex.readthedocs.io.
+    CasEx: Casual Expectation Toolbox in Python. JARUS WG-6 SORA Annex F Quantitative Methods subgroup, 2023. Available at https://casex.readthedocs.io.
 
 And as BibTeX:
 
 
-    @misc{JARUSWG6QuantitativeMethodssubgroup2021,
+    @misc{JARUSWG6QuantitativeMethodssubgroup2023,
     author = {{JARUS WG-6 SORA Annex F Quantitative Methods subgroup}},
     title = {{CasEx: Casual Expectation Toolbox in Python}},
     url = {casex.readthedocs.io},
-    year = {2021}
+    year = {2023}
     }
 
-
-
-
-
-
```

### Comparing `casex-1.1.9/README.md` & `casex-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,18 @@
 for any purpose, even commercially. The licensor cannot revoke these freedoms as long as you follow the license terms.
 You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.
 
 Do note that according to this license you must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
 
 We recommend the following reference to CasEx:
 
-    CasEx: Casual Expectation Toolbox in Python. JARUS WG-6 SORA Annex F Quantitative Methods subgroup, 2021. Available at https://casex.readthedocs.io.
+    CasEx: Casual Expectation Toolbox in Python. JARUS WG-6 SORA Annex F Quantitative Methods subgroup, 2023. Available at https://casex.readthedocs.io.
 
 And as BibTeX:
 
 
-    @misc{JARUSWG6QuantitativeMethodssubgroup2021,
+    @misc{JARUSWG6QuantitativeMethodssubgroup2023,
     author = {{JARUS WG-6 SORA Annex F Quantitative Methods subgroup}},
     title = {{CasEx: Casual Expectation Toolbox in Python}},
     url = {casex.readthedocs.io},
-    year = {2021}
-    }
-
-
-
-
+    year = {2023}
+    }
```

### Comparing `casex-1.1.9/setup.py` & `casex-1.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='casex',
-    version='1.1.9',
+    version='1.2.1',
     description='Casualty expectation toolbox',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'License :: Other/Proprietary License',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
         'Topic :: Scientific/Engineering',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
     ],
     author='Anders la Cour-Harbo et al',
     author_email='anders@lacourfamily.dk',
     license='CC-BY-4.0',
```

