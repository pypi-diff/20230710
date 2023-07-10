# Comparing `tmp/atriumsports_sdk-1.3.1.tar.gz` & `tmp/atriumsports_sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atriumsports_sdk-1.3.1.tar", last modified: Mon Jul 10 10:39:20 2023, max compression
+gzip compressed data, was "atriumsports_sdk-1.3.2.tar", last modified: Mon Jul 10 10:51:03 2023, max compression
```

## Comparing `atriumsports_sdk-1.3.1.tar` & `atriumsports_sdk-1.3.2.tar`

### file list

```diff
@@ -1,436 +1,436 @@
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:20.342236 atriumsports_sdk-1.3.1/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.1/LICENSE
--rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-10 10:39:20.341972 atriumsports_sdk-1.3.1/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.3.1/README.md
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:19.855568 atriumsports_sdk-1.3.1/atriumsports/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1096 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.1/atriumsports/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.1/atriumsports/atrium_response.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:19.856989 atriumsports_sdk-1.3.1/atriumsports/datacore/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6660 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/datacore.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:19.871280 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/
--rw-r--r--   0 k.kieda    (502) staff       (20)    54651 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/__init__.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:19.954332 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/
--rw-r--r--   0 k.kieda    (502) staff       (20)     4630 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   121018 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/awards_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59847 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/career_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18925 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/change_log_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    97107 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/competition_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127164 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/competitions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    78128 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/conduct_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   137833 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/conferences_divisions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    66311 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/download_video_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    91278 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    21039 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127554 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70185 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entity_groups_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59444 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11205 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59323 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77945 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72387 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_profiles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76686 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_progressions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    89352 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   407884 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixtures_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   252466 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/images_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70633 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73398 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70024 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/leagues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73817 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70215 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/merge_records_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    66029 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/organizations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    36028 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/partner_apis_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23558 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/person_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   134432 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    91522 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   107461 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/rankings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   150045 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/roles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77289 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    49629 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71603 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_entity_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    44646 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_leaders_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    50867 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71598 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_person_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77803 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    97800 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    90287 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_series_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   177700 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   120275 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/seasons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    68423 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/sites_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   229910 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76768 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/standing_adjustments_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71710 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/standing_configurations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   137275 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/standings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71111 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/transfers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   100928 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/venues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73928 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76269 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72341 2023-07-10 10:36:56.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/video_streams_available_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28316 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api_client.py
--rw-r--r--   0 k.kieda    (502) staff       (20)      779 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    14860 2023-07-10 10:36:54.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5022 2023-07-10 10:36:21.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/exceptions.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:20.338272 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/
--rw-r--r--   0 k.kieda    (502) staff       (20)    35789 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6094 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/award_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5926 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/award_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10475 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/awards_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2330 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/awards_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/awards_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3057 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/blank_model_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5041 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2530 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3762 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4448 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/change_log_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/change_log_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3532 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/change_log_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4405 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4302 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4401 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9341 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9112 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11710 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2316 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2376 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3567 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11966 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23827 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2938 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_penalty_result.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18995 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18856 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conference_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5174 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conference_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7587 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conferences_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2368 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conferences_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3555 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conferences_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3114 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/contact_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6109 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/division_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5676 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/division_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8546 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/divisions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/divisions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/divisions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18029 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_model_entity_group.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2343 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5227 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5268 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4876 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11288 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4222 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3406 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11119 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13235 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_groups_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_groups_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4836 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15522 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4158 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3348 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15400 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1929 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/environmental_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2849 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/error_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2825 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/error_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6046 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12585 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9137 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2747 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4700 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5193 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2545 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2244 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2703 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5527 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_participant.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10059 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2425 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3605 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4486 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2660 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7624 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6090 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2546 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3138 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4767 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9886 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2416 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2309 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6942 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22216 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3960 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2650 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2393 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3225 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5970 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22088 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6724 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2386 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3884 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3201 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28618 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28554 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2359 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2292 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_round.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2305 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_series.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2274 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_venue.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4979 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7681 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_person_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_person_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1897 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_identification.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2049 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2363 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_resolution.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2499 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9444 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2329 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1757 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1876 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/included_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3200 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2085 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1837 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3635 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5867 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2430 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3616 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2728 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6652 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/league_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6530 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/league_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8593 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leagues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leagues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leagues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5994 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organization_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5784 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organization_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7119 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organizations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3579 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organizations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5672 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5833 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2556 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_list_default_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13370 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5720 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13315 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15343 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6103 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/pool_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5679 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/pool_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5564 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4618 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4458 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2200 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/response_links.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3437 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/response_meta_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11638 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/role_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11517 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/role_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15525 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/roles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/roles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/roles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7057 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/round_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6627 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/round_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8848 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9018 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5624 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6248 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5241 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2526 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2442 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3772 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6931 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3893 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5731 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6195 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3783 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5105 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2522 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3750 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6836 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7006 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4072 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8501 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_pools_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_pools_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_pools_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18148 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18363 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10457 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2378 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5981 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9996 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_rounds_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2370 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_rounds_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4466 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    16333 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5733 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stage_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5248 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stage_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7537 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stages_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stages_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stages_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5288 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3796 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5276 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11002 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2428 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3957 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonroster_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22249 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_competition.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12210 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/series_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11915 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/series_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5211 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/site_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6538 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/site_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6354 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/site_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7786 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sites_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sites_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sites_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3245 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/social_media.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2237 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sorting.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12332 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12243 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    17425 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustments_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustments_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4994 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_building.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13200 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2482 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4849 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4563 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3688 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12098 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18313 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4442 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12099 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18136 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standings_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1778 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/success_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/success_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2624 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfer_component.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7246 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfer_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7087 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfer_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9588 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5219 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5326 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10631 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10463 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12568 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2328 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2248 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9562 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_file_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2163 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_download_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_download_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11486 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2361 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11747 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2441 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5343 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2433 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3473 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3312 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9468 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2449 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11463 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscription_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11577 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscription_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13664 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscriptions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2447 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3640 2023-07-10 10:36:55.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscriptions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12617 2023-07-10 10:36:54.000000 atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/rest.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:20.339182 atriumsports_sdk-1.3.1/atriumsports/datacore_stream/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.3.1/atriumsports/datacore_stream/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.3.1/atriumsports/datacore_stream/datacore_stream.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1942 2023-07-03 16:04:32.000000 atriumsports_sdk-1.3.1/atriumsports/endpoints.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:39:20.341575 atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/
--rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-10 10:39:19.000000 atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)    27301 2023-07-10 10:39:19.000000 atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)        1 2023-07-10 10:39:19.000000 atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)      108 2023-07-10 10:39:19.000000 atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/requires.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       13 2023-07-10 10:39:19.000000 atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/top_level.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.3.1/pyproject.toml
--rw-r--r--   0 k.kieda    (502) staff       (20)       38 2023-07-10 10:39:20.342286 atriumsports_sdk-1.3.1/setup.cfg
--rw-r--r--   0 k.kieda    (502) staff       (20)      947 2023-07-10 10:34:32.000000 atriumsports_sdk-1.3.1/setup.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.930160 atriumsports_sdk-1.3.2/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.2/LICENSE
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-10 10:51:03.929678 atriumsports_sdk-1.3.2/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.3.2/README.md
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.626665 atriumsports_sdk-1.3.2/atriumsports/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1096 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.2/atriumsports/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.2/atriumsports/atrium_response.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.628432 atriumsports_sdk-1.3.2/atriumsports/datacore/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6660 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/datacore.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.633136 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    54651 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/__init__.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.682530 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4630 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   121018 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/awards_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59847 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/career_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18925 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/change_log_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    97107 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competition_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127164 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competitions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    78128 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conduct_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   137833 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conferences_divisions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    66311 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/download_video_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    91278 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    21039 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127554 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70185 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_groups_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59444 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11205 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59323 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77945 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72387 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_profiles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76686 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_progressions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    89352 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   407884 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixtures_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   252466 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/images_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70633 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73398 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70024 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leagues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73817 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70215 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/merge_records_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    66029 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/organizations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    36028 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/partner_apis_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23558 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   134432 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    91522 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   107461 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/rankings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   150045 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/roles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77289 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    49629 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71603 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    44646 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_leaders_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    50867 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71598 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77803 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    97800 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    90287 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_series_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   177700 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   120275 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/seasons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    68423 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/sites_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   229910 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76768 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_adjustments_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71710 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_configurations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   137275 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71111 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/transfers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   100928 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/venues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73928 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76269 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72341 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_streams_available_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28316 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_client.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)      779 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    14860 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5022 2023-07-10 10:50:15.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/exceptions.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.926386 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    35789 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6094 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5926 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10475 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2330 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3057 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/blank_model_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5041 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2530 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3762 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4448 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3532 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4405 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4302 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4401 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9341 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9112 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11710 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2316 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2376 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3567 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11966 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23827 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2938 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_penalty_result.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18995 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18856 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5174 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7587 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2368 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3555 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3114 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/contact_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6109 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5676 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8546 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18029 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_entity_group.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2343 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5227 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5268 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4876 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11288 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4222 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3406 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11119 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13235 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4836 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15522 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4158 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3348 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15400 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1929 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/environmental_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2849 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2825 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6046 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12585 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9137 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2747 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4700 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5193 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2545 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2244 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2703 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5527 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_participant.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10059 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2425 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3605 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4486 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2660 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7624 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6090 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2546 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3138 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4767 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9886 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2416 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2309 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6942 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22216 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3960 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2650 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2393 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3225 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5970 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22088 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6724 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2386 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3884 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3201 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28618 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28554 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2359 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2292 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_round.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2305 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_series.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2274 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_venue.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4979 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7681 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1897 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2049 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2363 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2499 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9444 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2329 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1757 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1876 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/included_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3200 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2085 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1837 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3635 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5867 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2430 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3616 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2728 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6652 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6530 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8593 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5994 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5784 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7119 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3579 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5672 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5833 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2556 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_list_default_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13370 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5720 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13315 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15343 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6103 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5679 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5564 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4618 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4458 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2200 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_links.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3437 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_meta_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11638 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11517 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15525 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7057 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6627 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8848 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9018 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5624 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6248 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5241 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2526 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2442 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3772 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6931 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3893 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5731 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6195 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3783 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5105 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2522 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3750 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6836 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7006 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4072 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8501 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18148 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18363 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10457 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2378 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5981 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9996 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2370 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4466 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16333 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5733 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5248 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7537 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5288 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3796 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5276 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11002 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2428 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3957 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonroster_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22249 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_competition.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12210 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11915 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5211 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6538 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7786 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3245 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/social_media.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2237 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sorting.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12332 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12243 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    17425 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4994 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_building.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13200 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2482 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4849 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4563 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3688 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12098 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18313 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4442 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12099 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18136 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1778 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2624 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_component.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7246 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7087 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9588 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5219 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5326 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10631 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10463 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2328 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2248 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9562 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_file_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2163 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11486 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2361 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11747 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2441 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5343 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2433 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3473 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3312 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9468 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2449 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11463 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11577 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13664 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2447 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3640 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12617 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/rest.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.927172 atriumsports_sdk-1.3.2/atriumsports/datacore_stream/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.3.2/atriumsports/datacore_stream/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.3.2/atriumsports/datacore_stream/datacore_stream.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1942 2023-07-03 16:04:32.000000 atriumsports_sdk-1.3.2/atriumsports/endpoints.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.929208 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)    27301 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)        1 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)      115 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/requires.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       13 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/top_level.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.3.2/pyproject.toml
+-rw-r--r--   0 k.kieda    (502) staff       (20)       38 2023-07-10 10:51:03.930240 atriumsports_sdk-1.3.2/setup.cfg
+-rw-r--r--   0 k.kieda    (502) staff       (20)      954 2023-07-10 10:49:42.000000 atriumsports_sdk-1.3.2/setup.py
```

### Comparing `atriumsports_sdk-1.3.1/LICENSE` & `atriumsports_sdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/PKG-INFO` & `atriumsports_sdk-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports_sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.3.1/README.md` & `atriumsports_sdk-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/__init__.py` & `atriumsports_sdk-1.3.2/atriumsports/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/atrium_response.py` & `atriumsports_sdk-1.3.2/atriumsports/atrium_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/datacore.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/datacore.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/__init__.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
 This **access token** must then be sent in the `Authorization` header for each subsequent API call.  Access tokens have a finite life and will expire. When the token expires you will need to create a new token to make more API calls.  Creation of tokens is rate-limited, so you should use the existing token as long as possible.
 
 <!-- ReDoc-Inject: <security-definitions> -->
   # noqa: E501
 """
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 
 # import apis into sdk package
 from atriumsports.datacore.openapi.api.awards_api import AwardsApi
 from atriumsports.datacore.openapi.api.career_statistics_api import CareerStatisticsApi
 from atriumsports.datacore.openapi.api.change_log_api import ChangeLogApi
 from atriumsports.datacore.openapi.api.competition_statistics_api import CompetitionStatisticsApi
 from atriumsports.datacore.openapi.api.competitions_api import CompetitionsApi
```

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/__init__.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/awards_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/awards_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/career_statistics_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/career_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/change_log_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/change_log_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/competition_statistics_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competition_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/competitions_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competitions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/conduct_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conduct_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/conferences_divisions_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conferences_divisions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/download_video_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/download_video_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entities_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entity_fixture_history_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/entity_groups_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_groups_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_entities_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_live_summary_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_live_summary_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_persons_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_profiles_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_profiles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_progressions_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_progressions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixture_roster_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/fixtures_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixtures_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/images_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/images_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/leader_qualifiers_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_qualifiers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/leagues_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leagues_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/local_video_endpoints_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/local_video_endpoints_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/merge_records_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/merge_records_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/organizations_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/partner_apis_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/partner_apis_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/person_fixture_history_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/persons_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/rankings_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/rankings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/roles_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_entities_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_entity_placings_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_leaders_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_leaders_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_person_placings_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_persons_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_roster_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_series_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_series_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/season_statistics_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/seasons_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/seasons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/sites_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/sites_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/standing_adjustments_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_adjustments_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/standing_configurations_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_configurations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/standings_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/transfers_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/transfers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/venues_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/venues_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/video_stream_inputs_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_inputs_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api/video_streams_available_api.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_streams_available_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api_client.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "AtriumSportsSDK/1.3.1"
+        self.user_agent = "AtriumSportsSDK/1.3.2"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/api_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/configuration.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: v1\n"
-            "SDK Package Version: 1.3.1".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 1.3.2".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/exceptions.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/__init__.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/award_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/award_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/awards_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/awards_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/awards_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/blank_model_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/blank_model_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/career_person_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/change_log_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/change_log_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/change_log_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_historical_name.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_person_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_person_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competition_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_model_league.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/competitions_season_status_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_penalty_result.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_penalty_result.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conduct_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conference_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conference_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conferences_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conferences_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/conferences_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/contact_details.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/contact_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/division_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/division_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/divisions_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/divisions_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/divisions_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_model_entity_group.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_entity_group.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entities_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_additional_details.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_address.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_address.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_historical_name.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_group_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_groups_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_groups_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_groups_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_historical_name.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_post_body_colors.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/entity_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/environmental_details.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/environmental_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/error_list_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/error_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_competitor.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_division.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_division.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entities_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_live_summary_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_live_summary_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_participant.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_participant.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_pbp_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_model_person.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_person.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_persons_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_profiles_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progression_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progression_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_progressions_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_roster_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_round.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_round.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_series.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_series.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_model_venue.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_venue.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/fixtures_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_entity_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_entity_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_person_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_person_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/game_log_person_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_identification.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_resolution.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/images_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/included_data.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/included_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_criteria_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_qualifiers_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_summary_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leader_summary_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/league_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/league_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leagues_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leagues_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/leagues_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organization_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organization_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organizations_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/organizations_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_additional_details.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_historical_name.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_list_default_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_list_default_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/person_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/persons_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/persons_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/persons_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/pool_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/pool_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/ranking_rows_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/response_links.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_links.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/response_meta_data.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_meta_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/role_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/role_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/roles_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/roles_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/roles_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/round_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/round_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_list_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_list_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entities_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_placings_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_placings_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_entity_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_placings_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_placings_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_list_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_list_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_persons_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_pools_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_pools_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_pools_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_roster_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_rounds_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_rounds_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_rounds_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_competitor.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_series_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stage_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stage_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stages_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stages_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_stages_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_address.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_model_site.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/season_venues_list_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasonroster_configuration.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonroster_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_competition.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_competition.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/seasons_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/series_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/series_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/site_address.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/site_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/site_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sites_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sites_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sites_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/social_media.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/social_media.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/sorting.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sorting.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustments_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_adjustments_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_building.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_building.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configuration.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_configurations_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_post_body_points_value.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_points_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standing_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standings_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standings_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/standings_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/success_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/success_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfer_component.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_component.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfer_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfer_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfers_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfers_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/transfers_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_address.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_historical_name.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venue_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_model_site.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/venues_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_file_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_file_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_download_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_download_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_files_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_inputs_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_inputs_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_local_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_outputs_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_stream_outputs_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscription_post_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscription_put_body.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscriptions_model.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/models/video_subscriptions_response.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore/openapi/rest.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/rest.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/datacore_stream/datacore_stream.py` & `atriumsports_sdk-1.3.2/atriumsports/datacore_stream/datacore_stream.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports/endpoints.py` & `atriumsports_sdk-1.3.2/atriumsports/endpoints.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/PKG-INFO` & `atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.3.1/atriumsports_sdk.egg-info/SOURCES.txt` & `atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.1/setup.py` & `atriumsports_sdk-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     setuptools.setup(
         name="atriumsports_sdk",
-        version="1.3.1",
+        version="1.3.2",
         author="Atrium Sports",
         author_email="python_dev@atriumsports.com",
         description="Python module for integration to Atrium Sports APIs",
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=setuptools.find_packages(),
         classifiers=[
@@ -19,11 +19,11 @@
         python_requires=">=3.7",
         install_requires=[
             "requests",
             "paho-mqtt",
             "python-dateutil>=2.5.3",
             "setuptools>=21.0.0",
             "urllib3>=1.25.3",
-            "pydantic>=1.10.2",
+            "pydantic>=1.10.2,<2.0.0",
             "aenum>=3.1.11",
         ],
     )
```

