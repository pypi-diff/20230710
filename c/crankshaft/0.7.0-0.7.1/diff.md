# Comparing `tmp/crankshaft-0.7.0.tar.gz` & `tmp/crankshaft-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crankshaft-0.7.0.tar", max compression
+gzip compressed data, was "crankshaft-0.7.1.tar", max compression
```

## Comparing `crankshaft-0.7.0.tar` & `crankshaft-0.7.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1067 2023-07-09 19:11:22.151048 crankshaft-0.7.0/LICENSE
--rw-r--r--   0        0        0     1564 2023-07-09 19:11:22.151048 crankshaft-0.7.0/README.md
--rw-r--r--   0        0        0      326 2023-07-09 19:12:04.699584 crankshaft-0.7.0/crankshaft/__init__.py
--rw-r--r--   0        0        0      133 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/api.bolt
--rw-r--r--   0        0        0      216 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/config.bolt
--rw-r--r--   0        0        0      513 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/defer.bolt
--rw-r--r--   0        0        0     3872 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/event_handler.bolt
--rw-r--r--   0        0        0     1605 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_entity_attack_player.bolt
--rw-r--r--   0        0        0      207 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_load.bolt
--rw-r--r--   0        0        0      344 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_player_airborne.bolt
--rw-r--r--   0        0        0      644 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_player_airborne_end.bolt
--rw-r--r--   0        0        0      646 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_player_airborne_start.bolt
--rw-r--r--   0        0        0     1605 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_player_attack_entity.bolt
--rw-r--r--   0        0        0      328 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_player_burn.bolt
--rw-r--r--   0        0        0      629 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events/on_player_burn_end.bolt
--rw-r--r--   0        0        0      632 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_burn_start.bolt
--rw-r--r--   0        0        0      558 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_charge_bow.bolt
--rw-r--r--   0        0        0      973 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_charge_bow_end.bolt
--rw-r--r--   0        0        0      665 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_charge_bow_start.bolt
--rw-r--r--   0        0        0      332 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_glide.bolt
--rw-r--r--   0        0        0      632 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_glide_end.bolt
--rw-r--r--   0        0        0      636 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_glide_start.bolt
--rw-r--r--   0        0        0      677 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_inventory_change.bolt
--rw-r--r--   0        0        0      501 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_join.bolt
--rw-r--r--   0        0        0      495 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_jump.bolt
--rw-r--r--   0        0        0      608 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_land.bolt
--rw-r--r--   0        0        0      471 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_load.bolt
--rw-r--r--   0        0        0      734 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_shoot_bow.bolt
--rw-r--r--   0        0        0      335 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_sneak.bolt
--rw-r--r--   0        0        0      635 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_sneak_end.bolt
--rw-r--r--   0        0        0      638 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_sneak_start.bolt
--rw-r--r--   0        0        0      341 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_sprint.bolt
--rw-r--r--   0        0        0      642 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_sprint_end.bolt
--rw-r--r--   0        0        0      644 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_sprint_start.bolt
--rw-r--r--   0        0        0      332 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_swim.bolt
--rw-r--r--   0        0        0      632 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_swim_end.bolt
--rw-r--r--   0        0        0      635 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_swim_start.bolt
--rw-r--r--   0        0        0      263 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_tick.bolt
--rw-r--r--   0        0        0      558 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_use_coas.bolt
--rw-r--r--   0        0        0      573 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_player_use_wfoas.bolt
--rw-r--r--   0        0        0      207 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/events/on_tick.bolt
--rw-r--r--   0        0        0     2118 2023-07-09 19:11:22.151048 crankshaft-0.7.0/crankshaft/modules/events.bolt
--rw-r--r--   0        0        0     3398 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flag.bolt
--rw-r--r--   0        0        0      377 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_airborne.bolt
--rw-r--r--   0        0        0      402 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_baby.bolt
--rw-r--r--   0        0        0      411 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_burning.bolt
--rw-r--r--   0        0        0     1258 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_charging_bow.bolt
--rw-r--r--   0        0        0      377 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_gliding.bolt
--rw-r--r--   0        0        0      379 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_in_ground.bolt
--rw-r--r--   0        0        0      379 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_on_ground.bolt
--rw-r--r--   0        0        0      158 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_player.bolt
--rw-r--r--   0        0        0      414 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_sneaking.bolt
--rw-r--r--   0        0        0      417 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_sprinting.bolt
--rw-r--r--   0        0        0      414 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags/is_swimming.bolt
--rw-r--r--   0        0        0      535 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/flags.bolt
--rw-r--r--   0        0        0      443 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/lib/entity_hit_matching/api.bolt
--rw-r--r--   0        0        0      124 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/lib/entity_hit_matching/credits.txt
--rw-r--r--   0        0        0    58171 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/lib/entity_hit_matching/main.bolt
--rw-r--r--   0        0        0      207 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/modules/utils.bolt
--rw-r--r--   0        0        0        0 2023-07-09 19:11:22.155048 crankshaft-0.7.0/crankshaft/py.typed
--rw-r--r--   0        0        0     1329 2023-07-09 19:12:04.719584 crankshaft-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 crankshaft-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-10 19:23:26.122010 crankshaft-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1564 2023-07-10 19:23:26.122010 crankshaft-0.7.1/README.md
+-rw-r--r--   0        0        0      326 2023-07-10 19:24:07.921135 crankshaft-0.7.1/crankshaft/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/api.bolt
+-rw-r--r--   0        0        0      216 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/config.bolt
+-rw-r--r--   0        0        0      513 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/defer.bolt
+-rw-r--r--   0        0        0     3872 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/event_handler.bolt
+-rw-r--r--   0        0        0     1605 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_entity_attack_player.bolt
+-rw-r--r--   0        0        0      207 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_load.bolt
+-rw-r--r--   0        0        0      344 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_airborne.bolt
+-rw-r--r--   0        0        0      644 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_airborne_end.bolt
+-rw-r--r--   0        0        0      646 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_airborne_start.bolt
+-rw-r--r--   0        0        0     1605 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_attack_entity.bolt
+-rw-r--r--   0        0        0      328 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_burn.bolt
+-rw-r--r--   0        0        0      629 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_burn_end.bolt
+-rw-r--r--   0        0        0      632 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_burn_start.bolt
+-rw-r--r--   0        0        0      589 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_charge_bow.bolt
+-rw-r--r--   0        0        0      975 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_charge_bow_end.bolt
+-rw-r--r--   0        0        0      665 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_charge_bow_start.bolt
+-rw-r--r--   0        0        0      332 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_glide.bolt
+-rw-r--r--   0        0        0      632 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_glide_end.bolt
+-rw-r--r--   0        0        0      636 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_glide_start.bolt
+-rw-r--r--   0        0        0      677 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_inventory_change.bolt
+-rw-r--r--   0        0        0      501 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_join.bolt
+-rw-r--r--   0        0        0      495 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_jump.bolt
+-rw-r--r--   0        0        0      608 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_land.bolt
+-rw-r--r--   0        0        0      471 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_load.bolt
+-rw-r--r--   0        0        0      736 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_shoot_bow.bolt
+-rw-r--r--   0        0        0      335 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_sneak.bolt
+-rw-r--r--   0        0        0      635 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_sneak_end.bolt
+-rw-r--r--   0        0        0      638 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_sneak_start.bolt
+-rw-r--r--   0        0        0      341 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_sprint.bolt
+-rw-r--r--   0        0        0      642 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_sprint_end.bolt
+-rw-r--r--   0        0        0      644 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_sprint_start.bolt
+-rw-r--r--   0        0        0      332 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_swim.bolt
+-rw-r--r--   0        0        0      632 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_swim_end.bolt
+-rw-r--r--   0        0        0      635 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_swim_start.bolt
+-rw-r--r--   0        0        0      263 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_tick.bolt
+-rw-r--r--   0        0        0      558 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_use_coas.bolt
+-rw-r--r--   0        0        0      573 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_player_use_wfoas.bolt
+-rw-r--r--   0        0        0      207 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events/on_tick.bolt
+-rw-r--r--   0        0        0     2118 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/events.bolt
+-rw-r--r--   0        0        0     3398 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flag.bolt
+-rw-r--r--   0        0        0      377 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_airborne.bolt
+-rw-r--r--   0        0        0      402 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_baby.bolt
+-rw-r--r--   0        0        0      411 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_burning.bolt
+-rw-r--r--   0        0        0     1258 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_charging_bow.bolt
+-rw-r--r--   0        0        0      377 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_gliding.bolt
+-rw-r--r--   0        0        0      379 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_in_ground.bolt
+-rw-r--r--   0        0        0      379 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_on_ground.bolt
+-rw-r--r--   0        0        0      158 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_player.bolt
+-rw-r--r--   0        0        0      414 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_sneaking.bolt
+-rw-r--r--   0        0        0      417 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_sprinting.bolt
+-rw-r--r--   0        0        0      414 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags/is_swimming.bolt
+-rw-r--r--   0        0        0      535 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/flags.bolt
+-rw-r--r--   0        0        0      443 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/lib/entity_hit_matching/api.bolt
+-rw-r--r--   0        0        0      124 2023-07-10 19:23:26.122010 crankshaft-0.7.1/crankshaft/modules/lib/entity_hit_matching/credits.txt
+-rw-r--r--   0        0        0    58171 2023-07-10 19:23:26.126008 crankshaft-0.7.1/crankshaft/modules/lib/entity_hit_matching/main.bolt
+-rw-r--r--   0        0        0      207 2023-07-10 19:23:26.126008 crankshaft-0.7.1/crankshaft/modules/utils.bolt
+-rw-r--r--   0        0        0        0 2023-07-10 19:23:26.126008 crankshaft-0.7.1/crankshaft/py.typed
+-rw-r--r--   0        0        0     1329 2023-07-10 19:24:07.941135 crankshaft-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 crankshaft-0.7.1/PKG-INFO
```

### Comparing `crankshaft-0.7.0/LICENSE` & `crankshaft-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/README.md` & `crankshaft-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/defer.bolt` & `crankshaft-0.7.1/crankshaft/modules/defer.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/event_handler.bolt` & `crankshaft-0.7.1/crankshaft/modules/event_handler.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_entity_attack_player.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_entity_attack_player.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_airborne_end.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_airborne_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_airborne_start.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_airborne_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_attack_entity.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_attack_entity.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_burn_end.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_burn_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_burn_start.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_burn_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_charge_bow.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_charge_bow.bolt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from wicked_expressions:api import Scoreboard
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../flags/is_charging_bow import is_charging_bow
+from ../config import Config
 
 
 def handler(event):
-    charge_time = Scoreboard(f"Config.SCOREBOARD_ROOT.event.{event.id}")['@s']
+    charge_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}")['@s']
 
     if is_charging_bow:
         charge_time += 1
         event.trigger(charge_time)
     else:
         charge_time = 0
```

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_charge_bow_end.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_charge_bow_end.bolt`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ../event_handler import BuiltinEvent, Entrypoint
 from ../config import Config
 from ../flags/is_charging_bow import is_charging_bow
 from ./on_player_tick import on_player_tick
 
 
 def handler(event):
-    charge_time = Scoreboard(f"Config.SCOREBOARD_ROOT.event.{event.id}")['@s']
+    charge_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}")['@s']
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if not is_charging_bow:
         execute function event.path('nested_0'):
             if entity @s[tag=event_fired_tag] function event.path('nested_1'):
                 untag(event_fired_tag)
                 event.trigger(charge_time)
```

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_charge_bow_start.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_charge_bow_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_glide_end.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_glide_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_glide_start.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_glide_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_inventory_change.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_inventory_change.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_land.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_land.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_shoot_bow.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_shoot_bow.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ../flags/is_charging_bow import is_charging_bow
 from ../config import Config
 from ./on_player_tick import on_player_tick
 
 
 
 def handler(event):
-    charge_time = Scoreboard(f"Config.SCOREBOARD_ROOT.event.{event.id}")['@s']
+    charge_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}")['@s']
     shoot_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}", 'used:bow')['@s']
 
     if is_charging_bow:
         charge_time += 1
     else:
         charge_time = 0
```

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_sneak_end.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_sneak_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_sneak_start.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_sneak_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_sprint_end.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_sprint_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_sprint_start.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_sprint_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_swim_end.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_swim_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_swim_start.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_swim_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_use_coas.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_use_coas.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events/on_player_use_wfoas.bolt` & `crankshaft-0.7.1/crankshaft/modules/events/on_player_use_wfoas.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/events.bolt` & `crankshaft-0.7.1/crankshaft/modules/events.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/flag.bolt` & `crankshaft-0.7.1/crankshaft/modules/flag.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/flags/is_charging_bow.bolt` & `crankshaft-0.7.1/crankshaft/modules/flags/is_charging_bow.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/flags.bolt` & `crankshaft-0.7.1/crankshaft/modules/flags.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/crankshaft/modules/lib/entity_hit_matching/main.bolt` & `crankshaft-0.7.1/crankshaft/modules/lib/entity_hit_matching/main.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.0/pyproject.toml` & `crankshaft-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crankshaft"
-version = "0.7.0"
+version = "0.7.1"
 description = "Bolt datapack flow control library."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/crankshaft"
 readme = "README.md"
```

### Comparing `crankshaft-0.7.0/PKG-INFO` & `crankshaft-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crankshaft
-Version: 0.7.0
+Version: 0.7.1
 Summary: Bolt datapack flow control library.
 Home-page: https://github.com/reapermc/crankshaft
 License: MIT
 Keywords: beet,mecha,bolt,python,minecraft,datapack,minecraft-commands,mcfunction,crankshaft,library,reapermc,flow-control,event,event-handler
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

