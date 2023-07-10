# Comparing `tmp/aiovantage-0.6.0.tar.gz` & `tmp/aiovantage-0.7.0.tar.gz`

## Comparing `aiovantage-0.6.0.tar` & `aiovantage-0.7.0.tar`

### file list

```diff
@@ -1,157 +1,158 @@
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.pylintrc
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aiovantage-0.6.0/TODO
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.vscode/settings.json
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/dump_system.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/monitor_all.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/anemo_sensors/dump_anemo_sensors.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/anemo_sensors/monitor_anemo_sensors.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/light_sensors/dump_light_sensors.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/light_sensors/monitor_light_sensors.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/control_load.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/masters/dump_masters.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/masters/monitor_masters.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/stations/jingle_bells.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/tasks/run_task.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/temperature_sensors/dump_temperature_sensors.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/temperature_sensors/monitor_temperature_sensors.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/connection.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/discovery.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/errors.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/query.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/commands.py
--rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/light_sensor.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sounder.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/temperature.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/module.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/module_gen2.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/anemo_sensors.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/light_sensors.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/modules.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/temperature_sensors.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.6.0/LICENSE
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aiovantage-0.6.0/README.md
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 aiovantage-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 aiovantage-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.pylintrc
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 aiovantage-0.7.0/TODO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/dump_system.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/load_groups/monitor_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/masters/dump_masters.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/masters/monitor_masters.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/connection.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/discovery.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/module.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/module_gen2.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    13315 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/modules.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aiovantage-0.7.0/README.md
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 aiovantage-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 aiovantage-0.7.0/PKG-INFO
```

### Comparing `aiovantage-0.6.0/.pre-commit-config.yaml` & `aiovantage-0.7.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 repos:
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.276
+    rev: v0.0.277
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.4.1"
     hooks:
```

### Comparing `aiovantage-0.6.0/CONTRIBUTING.md` & `aiovantage-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/TODO` & `aiovantage-0.7.0/TODO`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # TODO
 
+- Add `Vantage.DmxDaliGateway` as a Station
+- Cleanup "ELAGG", etc subscriptions on shutdown to avoid memory leaks on the controller
 - Look into pointing xsdata to a module to parse objects
   - <https://xsdata.readthedocs.io/en/latest/models.html#type-wildcard>
 - Consider moving system objects to a top-level "models" module
 - Consider grouping like-objects into a single file, eg all stations into station.py
 - Consider grouped controllers like aiohue, eg. for sensors, loads, etc.
 - Consider renaming config_client/methods to config_client/interfaces and flattening
 - Consider renaming GMemController to VariablesController, MastersController to ControllersController
```

### Comparing `aiovantage-0.6.0/.github/ISSUE_TEMPLATE/bug.yml` & `aiovantage-0.7.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiovantage-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/dump_system.py` & `aiovantage-0.7.0/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/monitor_all.py` & `aiovantage-0.7.0/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/anemo_sensors/dump_anemo_sensors.py` & `aiovantage-0.7.0/examples/anemo_sensors/dump_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/anemo_sensors/monitor_anemo_sensors.py` & `aiovantage-0.7.0/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/areas/dump_areas.py` & `aiovantage-0.7.0/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.7.0/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/blinds/dump_blinds.py` & `aiovantage-0.7.0/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/blinds/monitor_blinds.py` & `aiovantage-0.7.0/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/buttons/dump_buttons.py` & `aiovantage-0.7.0/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/buttons/monitor_buttons.py` & `aiovantage-0.7.0/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/command_client/event_log.py` & `aiovantage-0.7.0/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/command_client/status_load.py` & `aiovantage-0.7.0/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/config_client/dump_objects.py` & `aiovantage-0.7.0/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/config_client/get_version.py` & `aiovantage-0.7.0/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.7.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.7.0/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/gmem/dump_gmem.py` & `aiovantage-0.7.0/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/gmem/monitor_gmem.py` & `aiovantage-0.7.0/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/gmem/set_gmem.py` & `aiovantage-0.7.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/light_sensors/dump_light_sensors.py` & `aiovantage-0.7.0/examples/light_sensors/dump_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/light_sensors/monitor_light_sensors.py` & `aiovantage-0.7.0/examples/light_sensors/monitor_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/load_groups/dump_load_groups.py` & `aiovantage-0.7.0/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/loads/control_load.py` & `aiovantage-0.7.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/loads/dump_loads.py` & `aiovantage-0.7.0/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/loads/monitor_loads.py` & `aiovantage-0.7.0/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/loads/poll_on_loads.py` & `aiovantage-0.7.0/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/loads/toggle_load.py` & `aiovantage-0.7.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/masters/dump_masters.py` & `aiovantage-0.7.0/examples/masters/dump_masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/masters/monitor_masters.py` & `aiovantage-0.7.0/examples/masters/monitor_masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.7.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.7.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.7.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.7.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/stations/dump_stations.py` & `aiovantage-0.7.0/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/stations/jingle_bells.py` & `aiovantage-0.7.0/examples/stations/jingle_bells.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/tasks/dump_tasks.py` & `aiovantage-0.7.0/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/tasks/run_task.py` & `aiovantage-0.7.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/temperature_sensors/dump_temperature_sensors.py` & `aiovantage-0.7.0/examples/temperature_sensors/dump_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/examples/temperature_sensors/monitor_temperature_sensors.py` & `aiovantage-0.7.0/examples/temperature_sensors/monitor_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/connection.py` & `aiovantage-0.7.0/src/aiovantage/connection.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -124,13 +124,13 @@
         # Make sure we're connected
         if self._reader is None or self.closed:
             raise ClientConnectionError("Client not connected.")
 
         # Read the response, with optional timeout
         try:
             data = await asyncio.wait_for(self._reader.readuntil(separator), timeout)
-        except (OSError, asyncio.IncompleteReadError) as err:
-            raise ClientConnectionError from err
         except asyncio.TimeoutError as err:
             raise ClientTimeoutError from err
+        except (OSError, asyncio.IncompleteReadError) as err:
+            raise ClientConnectionError from err
 
         return data.decode()
```

### Comparing `aiovantage-0.6.0/src/aiovantage/discovery.py` & `aiovantage-0.7.0/src/aiovantage/discovery.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/errors.py` & `aiovantage-0.7.0/src/aiovantage/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/query.py` & `aiovantage-0.7.0/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/README.md` & `aiovantage-0.7.0/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/__init__.py` & `aiovantage-0.7.0/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/commands.py` & `aiovantage-0.7.0/src/aiovantage/command_client/commands.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/events.py` & `aiovantage-0.7.0/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/utils.py` & `aiovantage-0.7.0/src/aiovantage/command_client/utils.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/anemo_sensor.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/anemo_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/light_sensor.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/light_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sounder.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sounder.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/temperature.py` & `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/README.md` & `aiovantage-0.7.0/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.7.0/src/aiovantage/config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/helpers.py` & `aiovantage-0.7.0/src/aiovantage/config_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.7.0/src/aiovantage/config_client/xml_dataclass.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/methods/types.py` & `aiovantage-0.7.0/src/aiovantage/config_client/methods/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.7.0/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/methods/login/login.py` & `aiovantage-0.7.0/src/aiovantage/config_client/methods/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/load_group.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/load_group.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/master.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/master.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/config_client/objects/system_object.py` & `aiovantage-0.7.0/src/aiovantage/config_client/objects/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/anemo_sensors.py` & `aiovantage-0.7.0/src/aiovantage/controllers/anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/base.py` & `aiovantage-0.7.0/src/aiovantage/controllers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Sequence,
+    Set,
     Tuple,
     TypeVar,
     Union,
 )
 
 from aiovantage.command_client import CommandClient, Event, EventStream, EventType
 from aiovantage.command_client.utils import tokenize_response
@@ -50,19 +51,24 @@
     status_types: Optional[Tuple[str, ...]] = None
     """Which Vantage 'STATUS' types this controller handles, if any."""
 
     enhanced_log_status_methods: Optional[Union[Tuple[str, ...], Literal["*"]]] = None
     """Which status methods this controller handles from the Enhanced Log."""
 
     def __init__(self, vantage: "Vantage") -> None:
-        """Initialize instance."""
+        """Initialize a controller.
+
+        Args:
+            vantage: The Vantage instance.
+            init_callback: A callback to call when the controller is initialized.
+        """
         self._vantage = vantage
         self._items: Dict[int, T] = {}
         self._logger = logging.getLogger(__package__)
-        self._subscribed_to_event_stream = False
+        self._subscribed_to_state_changes = False
         self._subscriptions: List[EventSubscription[T]] = []
         self._id_subscriptions: Dict[int, List[EventSubscription[T]]] = {}
         self._initialized = False
 
         QuerySet.__init__(self, self._items, self._lazy_initialize)
 
         self.__post_init__()
@@ -90,18 +96,28 @@
 
     @property
     def event_stream(self) -> EventStream:
         """Return the event stream instance."""
         return self._vantage.event_stream
 
     @property
+    def initialized(self) -> bool:
+        """Return True if this controller has been initialized."""
+        return self._initialized
+
+    @property
     def stateful(self) -> bool:
         """Return True if this controller manages stateful objects."""
         return bool(self.status_types or self.enhanced_log_status_methods)
 
+    @property
+    def known_ids(self) -> Set[int]:
+        """Return a set of all known object IDs."""
+        return set(self._items.keys())
+
     async def fetch_object_state(self, _vid: int) -> State:
         """Fetch the full state of an object, should be overridden by subclasses."""
         return None
 
     def parse_object_update(
         self, _vid: int, _status: str, _args: Sequence[str]
     ) -> State:
@@ -133,49 +149,76 @@
                     for field in fields(prev_obj)
                     if getattr(prev_obj, field.name) != getattr(obj, field.name)
                     and field.name != "mtime"
                 ]
 
                 # If any attributes changed, update the object and notify subscribers
                 if attrs_changed:
-                    self._items[obj.id] = obj
+                    for attr in attrs_changed:
+                        try:
+                            setattr(prev_obj, attr, getattr(obj, attr))
+                        except AttributeError:
+                            self._logger.warning("Object has no attribute '%s'", attr)
+
                     self.emit(
                         VantageEvent.OBJECT_UPDATED,
                         obj,
                         {"attrs_changed": attrs_changed},
                     )
 
             # Keep track of which objects we've seen
             cur_ids.add(obj.id)
 
         # Handle objects that were removed
         for vid in prev_ids - cur_ids:
             obj = self._items.pop(vid)
             self.emit(VantageEvent.OBJECT_DELETED, obj)
 
-        # Subscribe to the event stream if this is the first subscription
-        if self.stateful and fetch_state and not self._subscribed_to_event_stream:
-            await self._subscribe_to_event_stream()
+        # Subscribe to state changes for objects managed by this controller
+        if fetch_state:
+            await self.subscribe_to_state_changes()
 
-        self._initialized = True
-        self._logger.info("%s initialized", self.__class__.__name__)
+        # Mark the controller as initialized
+        if not self._initialized:
+            self._initialized = True
+            self._logger.info("%s initialized", self.__class__.__name__)
+        else:
+            self._logger.info("%s reinitialized", self.__class__.__name__)
 
-    async def fetch_full_state(self, subscribe: bool = True) -> None:
+    async def fetch_full_state(self) -> None:
         """Fetch the full state of all objects managed by this controller."""
         if not self.stateful:
             return
 
         for obj in self._items.values():
             self._update_state(obj.id, await self.fetch_object_state(obj.id))
 
-        if subscribe and not self._subscribed_to_event_stream:
-            await self._subscribe_to_event_stream()
-
         self._logger.info("%s fetched state", self.__class__.__name__)
 
+    async def subscribe_to_state_changes(self) -> None:
+        """Subscribe to state changes for objects managed by this controller."""
+        if self._subscribed_to_state_changes or not self.stateful:
+            return
+
+        # Ensure that the event stream is running
+        await self.event_stream.start()
+
+        # Subscribe to "STATUS {type}" updates, if this controller cares about them
+        if self.status_types:
+            self.event_stream.subscribe_status(self._handle_event, self.status_types)
+
+        # Subscribe to object status events from the "Enhanced Log"
+        if self.enhanced_log_status_methods:
+            self.event_stream.subscribe_enhanced_log(
+                self._handle_event, ("STATUS", "STATUSEX")
+            )
+
+        self._subscribed_to_state_changes = True
+        self._logger.info("%s subscribed to state changes", self.__class__.__name__)
+
     def subscribe(
         self,
         callback: EventCallback[T],
         id_filter: Union[int, Tuple[int], None] = None,
         event_filter: Union[VantageEvent, Tuple[VantageEvent, ...], None] = None,
     ) -> Callable[[], None]:
         """Subscribe to status changes for objects managed by this controller.
@@ -277,38 +320,17 @@
         if len(attrs_changed) > 0:
             self.emit(
                 VantageEvent.OBJECT_UPDATED,
                 obj,
                 {"attrs_changed": attrs_changed},
             )
 
-    async def _subscribe_to_event_stream(self) -> None:
-        # Ensure that the event stream is running
-        await self.event_stream.start()
-
-        # Re-fetch the full state of all objects after reconnecting
-        self.event_stream.subscribe(self._handle_event, EventType.RECONNECTED)
-
-        # Subscribe to "STATUS {type}" updates, if this controller cares about them
-        if self.status_types:
-            self.event_stream.subscribe_status(self._handle_event, self.status_types)
-
-        # Subscribe to object status events from the "Enhanced Log"
-        if self.enhanced_log_status_methods:
-            self.event_stream.subscribe_enhanced_log(
-                self._handle_event, ("STATUS", "STATUSEX")
-            )
-
-        self._subscribed_to_event_stream = True
-        self._logger.info("%s subscribed to event stream", self.__class__.__name__)
-
     async def _handle_event(self, event: Event) -> None:
         # Handle events from the event stream
         # pylint: disable=assignment-from-none
-
         if event["type"] == EventType.STATUS:
             # Ignore events for objects that this controller doesn't manage
             if event["id"] not in self._items:
                 return
 
             # Pass the event to the controller
             state = self.parse_object_update(
@@ -335,14 +357,11 @@
             if vid not in self._items:
                 return
 
             # Pass the event to the controller
             state = self.parse_object_update(vid, method, args)
             self._update_state(vid, state)
 
-        elif event["type"] == EventType.RECONNECTED:
-            # Fetch the full state of all objects after reconnecting
-            await self.fetch_full_state()
-
     async def _lazy_initialize(self) -> None:
+        # Initialize the controller if it isn't already initialized
         if not self._initialized:
             await self.initialize()
```

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.7.0/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.7.0/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.7.0/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.7.0/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/gmem.py` & `aiovantage-0.7.0/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/light_sensors.py` & `aiovantage-0.7.0/src/aiovantage/controllers/light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.7.0/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.7.0/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/masters.py` & `aiovantage-0.7.0/src/aiovantage/controllers/masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.7.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.7.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/stations.py` & `aiovantage-0.7.0/src/aiovantage/controllers/stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/tasks.py` & `aiovantage-0.7.0/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/src/aiovantage/controllers/temperature_sensors.py` & `aiovantage-0.7.0/src/aiovantage/controllers/temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/LICENSE` & `aiovantage-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/README.md` & `aiovantage-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.6.0/pyproject.toml` & `aiovantage-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Issues = "https://github.com/loopj/aiovantage/issues"
 Source = "https://github.com/loopj/aiovantage"
 
 [project.optional-dependencies]
 dev = [
     "black==23.3.0",
     "mypy==1.4.1",
-    "ruff==0.0.275",
+    "ruff==0.0.277",
     "pre-commit==3.3.3",
 ]
 
 [tool.hatch.version]
 path = "src/aiovantage/__about__.py"
 
 [[tool.hatch.envs.all.matrix]]
```

### Comparing `aiovantage-0.6.0/PKG-INFO` & `aiovantage-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.6.0
+Version: 0.7.0
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -16,15 +16,15 @@
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions<5.0,>=4.6.3
 Requires-Dist: xsdata==23.6
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: mypy==1.4.1; extra == 'dev'
 Requires-Dist: pre-commit==3.3.3; extra == 'dev'
-Requires-Dist: ruff==0.0.275; extra == 'dev'
+Requires-Dist: ruff==0.0.277; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # aiovantage
 
 aiovantage is a Python library for interacting with and controlling Vantage InFusion home automation controllers.
 
 Uses a *controller* pattern inspired heavily by the [aiohue](https://github.com/home-assistant-libs/aiohue) library.
```

