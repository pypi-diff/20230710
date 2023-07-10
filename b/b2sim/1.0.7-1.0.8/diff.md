# Comparing `tmp/b2sim-1.0.7.tar.gz` & `tmp/b2sim-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.0.7.tar", last modified: Tue Jul  4 07:53:29 2023, max compression
+gzip compressed data, was "b2sim-1.0.8.tar", last modified: Mon Jul 10 20:01:11 2023, max compression
```

## Comparing `b2sim-1.0.7.tar` & `b2sim-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:21.390490 b2sim-1.0.7/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.7/LICENSE
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.0.7/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-04 23:22:21.384513 b2sim-1.0.7/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    12046 2023-07-02 13:19:26.000000 b2sim-1.0.7/README.md
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:20.872831 b2sim-1.0.7/b2sim/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.0.7/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10431 2023-07-04 00:29:36.000000 b2sim-1.0.7/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8687 2023-07-04 00:16:01.000000 b2sim-1.0.7/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   102968 2023-07-04 23:16:26.000000 b2sim-1.0.7/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     3818 2023-07-04 23:08:48.000000 b2sim-1.0.7/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:21.329912 b2sim-1.0.7/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.7/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      412 2023-06-19 10:21:44.000000 b2sim-1.0.7/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:21.221090 b2sim-1.0.7/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-04 23:22:20.000000 b2sim-1.0.7/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-04 23:22:21.393490 b2sim-1.0.7/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-04 00:04:31.000000 b2sim-1.0.7/setup.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.359218 b2sim-1.0.8/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.8/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.8/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-10 20:01:11.358216 b2sim-1.0.8/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    13115 2023-07-04 23:24:21.000000 b2sim-1.0.8/README.md
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.297161 b2sim-1.0.8/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.8/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10431 2023-07-04 00:29:36.000000 b2sim-1.0.8/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8687 2023-07-04 00:16:01.000000 b2sim-1.0.8/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)   102973 2023-07-05 03:18:50.000000 b2sim-1.0.8/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3818 2023-07-04 23:08:48.000000 b2sim-1.0.8/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.356216 b2sim-1.0.8/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.8/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      413 2023-07-06 22:49:54.000000 b2sim-1.0.8/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-10 20:01:11.310173 b2sim-1.0.8/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-10 20:01:10.000000 b2sim-1.0.8/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-10 20:01:11.359218 b2sim-1.0.8/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-05 03:07:31.000000 b2sim-1.0.8/setup.py
```

### Comparing `b2sim-1.0.7/LICENSE` & `b2sim-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.7/README.md` & `b2sim-1.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Welcome!
 
 Hi there! I'm redlaserbm, the main developer of the BTDB2 Eco simulator. To get started with using the code, please read through this README file! 
 
 - To learn how to operate the code, see the examples folder.
 - Want to request features for the code? Want to help out with the code? Found a bug? Don't hesitate to contact me! The most immediate way to get my attention with regards to this code is to join the b2 Popology discord server and ping me there: https://discord.gg/axHnkcVe6E
+- Potential collaborators interested with helping out with the code should view the "Feature Requests" section below for more info on tasks that need to be completed.
 
 # Operating the Code
 
 To run the code, do the following: 
 1. Install python on your computer. 
 2. In the terminal, do `pip install b2sim`.
 3. Using an IDE like Visual Studio Code, open a new .ipynb file and type `import b2sim as b2` in the first line and hit enter.
@@ -17,14 +18,17 @@
 
 1. **Simultaneous simulation of eco, farms, and alt-eco:** When given an eco send to use and some arrangement of farms and alt-eco, the simulator accurately tracks the progression of the player's cash and eco over time. The results of the simulator are nearly true to the game.
 2. **Easy operation:** Simply input your initial cash and eco, the round to start on, and the purchases you intend to make and the eco flowchart you intend to follow over the course of the match. The code runs in one click and delivers results in seconds.
 3. **Complete Farm support:** The simulator supports IMF Loans and Monkeyopolis. Also, the simulator supports compound purchases, such as selling into Monkey Wall Street.
 4. **Advanced Optimization Potential:** The code can be used in conjuction with optimization or nonlinear root-finding methods to determine the absolute best times to makes your moves during the game. 
 
 # Update Log
+- (July 2, 2023 - v1.0.6)
+   - Fixed an issue which effectively caused the attack queue size to be 5 instead of 6.
+   - New action `sellAllFarms` for rapidly selling all farms.
 - (July 2, 2023 - v1.0.5)
    - Improved support for eco numbers. It is no longer mandatory when specifying eco sends in the eco queue to specify a time for the player to start triggering that send. Note that if you place a send in the queue without a time specified, the previous send must have some sort of break condition (like `max_eco_amount` or `max_send_amount`) specified which compels the simulator to switch sends, otherwise the next send in the queue will never be triggered.
 - (July 1, 2023 - v1.0.4)
    - Fixed an issue which caused the attack queue (which concerns the queue of bloons sent to your opponent) to sometimes fail to remove sends from the queue that already finished sending, resulting in the simulator computing incorrect eco amounts during simulation.
    - You can now change the text size of the legend in the `viewCashEcoHistory` by using the `text_size` argument.
 - (July 1, 2023 - v1.0.3)
    - Added back support for *eco impact*. Whenever a farm is used in a simulation, the simulator computes the equivalent amount of eco that would've made the exact same money as the farm during its lifetime in the simulation. Thus, a farm that is on screen for 6 seconds and generates 100 dollars would have an eco impact of 100.
@@ -70,22 +74,29 @@
    - Graphs from `GameState.viewCashEcoHistory()` are now more informative.
    - `GameState.viewCashEcoHistory(dim=(w,h))` lets you set the width and height of the graphs.
    - Fixed a bug which would cause the code to get stuck in an infinite loop if `GameState.fastForward()` if the argument interval was set to a small number.
    - `GameState.fastForward()` now by default uses `interval = 0.1`. This will lead to sharper graphs and surprisngly does not appear to slow down the code much.
 - (May 11, 2023 - v0.9.1) 
    - Added druid farm support. Currently untested!
 
-# Feature To-Do List
+# Feature Requests
 
-- (High priority) Expanded revenue tracking:
+- (High Priority) More actions in `actions.py` to expand functionality and improve ease of use, including:
+   - Selling all Supply Drops, Selling all Druid Farms, Selling all Boat Farms
+   - Selling into a farm upgrade
+   - Withdrawing from all banks at once
+   - Buying, selling, and using overclock (on farms)
+- (High Priority) Expanded revenue tracking:
    - It would also be nice if the sim could track stats related to alt eco. Such stats could include revenue, expenses, long-run eco, and the aggregate revenue and expenses of each alt eco over the course of the simulation.
-   - For farms in particular, I wish to implement a stat called "equivalent eco impact" which shows the amount of eco that would've earned exactly the same amount that the farm did during its lifespan within simulation time. 
-- (High Priority) Improved Jeri functionality
-   - The improved Jericho functionality would ideally include support for Highwayman steals, as well as support for being stolen from.
-   - Although cumbersome with diminishing returns to accompany it, the computation of hero XP and hero levels would help to simplify the experience of using Jericho in the sim.
+   - In order for players to understand the `eco impact` statistic, display the farm's start and end of availability during the simulation.
+- (High Priority) Change the formatting for storing farms and boat farms:
+   - In a previous update, the behavior of farm selling was changed so that, from the perspective of the simulator, the farm is not sold, but rather "disabled". The `GameState` class continues to store the farms but does not compute their payments or award them.
+   - This new behavior circumvents an issue in early builds that used a list structure to store farms where a selling one farm could cause other farms' identifying index to shift, essentially making it impossible to implement support for compound transactions.
+   - Because of this, farms can now be stored in a simple list structure.
+   - Naturally, when revenue/expense tracking support is also implemented for boat farms, we will in the same way want to change the data structure for storing them to a list.
 - (Medium priority) Village support:
    - Village support would help answer the question of how useful Monkey City/Monkey Town actually are.
 - (Medium priority) Restructure the code:
    - There may be a way to rewrite 'processBuyQueue' so that it uses less lines of code and is easier to understand. (will explain idea here later)
 - (Low priority) Robust logging when comparing different strategies
    - The idea here is this: If I have two or more game states that share the same round class and are simulated over the same time span, they are directly comparable. While a method already exists to compare multiple game states with this principle, because it does not share code with the `Game State` class method `viewCashAndEcoHistory`, it is currently inflexible with regards to updates and lacks some of the pizazz the class method has right now.
 - (Low Priority) Optimization of the buy queue to prevent redundant computations
```

### Comparing `b2sim-1.0.7/b2sim/actions.py` & `b2sim-1.0.8/b2sim/actions.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.7/b2sim/info.py` & `b2sim-1.0.8/b2sim/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.7/b2sim/main.py` & `b2sim-1.0.8/b2sim/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,29 +114,30 @@
                         self.T5_exists[i] = True
                     elif self.farms[self.key].upgrades[i] == 5 and self.T5_exists[i] == True:
                         self.farms[self.key].upgrades[i] = 4
                 
                 self.key += 1
 
         #Next, boat farms!
-        self.boat_farms = initial_state.get('Boat Farms')
+        boat_info = initial_state.get('Boat Farms')
         self.Tempire_exists = False
+        self.boat_farms = {}
         self.boat_key = 0
-        if self.boat_farms is not None:
-            for key in self.boat_farms.keys():
-                if key >= self.key:
-                    self.key = key+1
-
-                boat_farm = self.boat_farms[key]
+        if boat_info is not None:
+            for boat_entry in boat_info:
                 #If the boat farm is a Tempire, mark it as such appropriately.
                 #Do not allow the user to initialize with multiple Tempires!
-                if boat_farm['Upgrade'] == 5 and self.Tempire_exists[i] == False:
+                if boat_entry['Upgrade'] == 5 and self.Tempire_exists[i] == False:
                     self.Tempire_exists = True
-                elif boat_farm['Upgrade'] == 5 and self.Tempire_exists[i] == True:
-                    boat_farm['Upgrade'] = 4
+                elif boat_entry['Upgrade'] == 5 and self.Tempire_exists[i] == True:
+                    boat_entry['Upgrade'] = 4
+                self.boat_farms[self.boat_key] = boat_entry
+
+                self.boat_key += 1
+                
 
         #Next, druid farms!
         self.druid_farms = initial_state.get('Druid Farms')
         if self.druid_farms is not None:
             self.sotf = self.druid_farms['Spirit of the Forest Index']
             self.druid_key = len(self.druid_farms) - 2
         else:
```

### Comparing `b2sim-1.0.7/b2sim/rounds.py` & `b2sim-1.0.8/b2sim/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.7/b2sim/templates/eco_send_info.csv` & `b2sim-1.0.8/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

