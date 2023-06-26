# Comparing `tmp/atriumsports_sdk-1.2.0.tar.gz` & `tmp/atriumsports_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atriumsports_sdk-1.2.0.tar", last modified: Mon Jun 19 16:08:31 2023, max compression
+gzip compressed data, was "atriumsports_sdk-1.3.0.tar", last modified: Mon Jun 26 10:33:00 2023, max compression
```

## Comparing `atriumsports_sdk-1.2.0.tar` & `atriumsports_sdk-1.3.0.tar`

### file list

```diff
@@ -1,433 +1,436 @@
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:31.099343 atriumsports_sdk-1.2.0/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.2.0/LICENSE
--rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-06-19 16:08:31.099156 atriumsports_sdk-1.2.0/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.2.0/README.md
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:30.933895 atriumsports_sdk-1.2.0/atriumsports/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1096 2023-03-17 13:13:15.000000 atriumsports_sdk-1.2.0/atriumsports/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.2.0/atriumsports/atrium_response.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:30.935139 atriumsports_sdk-1.2.0/atriumsports/datacore/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6660 2023-04-24 10:52:41.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/datacore.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:30.938499 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/
--rw-r--r--   0 k.kieda    (502) staff       (20)    54239 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/__init__.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:30.977493 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/
--rw-r--r--   0 k.kieda    (502) staff       (20)     4630 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   121018 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/awards_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    40271 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/career_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18925 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/change_log_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    97107 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/competition_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127164 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/competitions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    78128 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/conduct_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   137833 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    66311 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/download_video_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    91278 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    21039 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127554 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70185 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entity_groups_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59444 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11205 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59323 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77945 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72387 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76686 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    89352 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   407884 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixtures_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   252466 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/images_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70633 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73398 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70024 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/leagues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73817 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70215 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/merge_records_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    66029 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/organizations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    36028 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/partner_apis_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23558 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   134432 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    91522 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   107461 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/rankings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   150045 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/roles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77289 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    49629 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71603 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    44646 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_leaders_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    50867 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71598 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_person_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    61140 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    97800 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    90287 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_series_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   177700 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   120275 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/seasons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    68423 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/sites_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   229910 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76768 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71710 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/standing_configurations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   137275 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/standings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71111 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/transfers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   100928 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/venues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73928 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76269 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72341 2023-06-19 16:07:58.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/video_streams_available_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28317 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api_client.py
--rw-r--r--   0 k.kieda    (502) staff       (20)      779 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    14866 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5022 2023-06-19 16:07:51.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/exceptions.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:31.096957 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/
--rw-r--r--   0 k.kieda    (502) staff       (20)    35377 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6094 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/award_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5926 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/award_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10475 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/awards_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2330 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/awards_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/awards_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3057 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/blank_model_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4448 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/change_log_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/change_log_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3532 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/change_log_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4405 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4302 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4401 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9341 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9112 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11710 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2316 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2376 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3567 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11966 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23827 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2938 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18995 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18856 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conference_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5174 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conference_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7587 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conferences_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2368 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conferences_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3555 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conferences_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3114 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/contact_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6109 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/division_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5676 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/division_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8546 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/divisions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/divisions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/divisions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18029 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2343 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5227 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5268 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4876 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11288 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4222 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3406 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11119 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13235 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_groups_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_groups_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4836 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15522 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4158 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3348 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15400 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1929 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/environmental_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2849 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/error_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2825 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/error_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6046 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12585 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9137 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2747 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4700 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5193 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2545 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2244 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2703 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5527 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_participant.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10059 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2425 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3605 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4486 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2660 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7624 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6090 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2546 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3138 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4767 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9886 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2416 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2309 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6942 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22216 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3960 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2650 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2393 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3225 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5970 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22088 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6724 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2386 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3884 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3201 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28618 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28554 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2359 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2292 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_round.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2305 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_series.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2274 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4979 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7681 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_person_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_person_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1897 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_identification.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2049 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2363 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2499 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9444 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2329 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1757 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1876 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/included_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3200 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2085 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1837 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3635 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5867 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2430 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3616 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2728 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6652 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/league_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6530 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/league_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8593 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leagues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leagues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leagues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5994 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organization_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5784 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organization_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7119 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organizations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3579 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organizations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5672 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5833 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2556 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_list_default_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13370 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5720 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13315 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15343 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6103 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/pool_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5679 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/pool_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5564 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4618 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4458 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2200 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/response_links.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3437 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/response_meta_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11638 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/role_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11517 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/role_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15525 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/roles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/roles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/roles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7057 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/round_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6627 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/round_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8848 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9018 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5624 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6248 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5241 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2526 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2442 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3772 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6931 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3893 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5731 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6195 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3783 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5105 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2522 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3750 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6836 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7006 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4072 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8501 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_pools_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_pools_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18148 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18363 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10457 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2378 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5981 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9996 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_rounds_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2370 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_rounds_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4466 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    16333 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5733 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stage_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5248 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stage_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7537 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stages_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stages_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5288 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3796 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5276 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11002 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2428 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3957 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22249 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_competition.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12210 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/series_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11915 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/series_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5211 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/site_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6538 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/site_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6354 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/site_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7786 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sites_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sites_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sites_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3245 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/social_media.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2237 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sorting.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12332 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12243 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    17425 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4994 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_building.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13200 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2482 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4849 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4563 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3688 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12098 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18313 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4442 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12099 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18136 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standings_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1778 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/success_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/success_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2624 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfer_component.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7246 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfer_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7087 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfer_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9588 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5219 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5326 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10631 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10463 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12568 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2328 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2248 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9562 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_file_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2163 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_download_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_download_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11486 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2361 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11747 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2441 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5343 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2433 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3473 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3312 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9468 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2449 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11463 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11577 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13664 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2447 2023-06-19 16:07:57.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3640 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12618 2023-06-19 16:07:56.000000 atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/rest.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:31.097460 atriumsports_sdk-1.2.0/atriumsports/datacore_stream/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.2.0/atriumsports/datacore_stream/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.2.0/atriumsports/datacore_stream/datacore_stream.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1942 2023-06-16 15:50:29.000000 atriumsports_sdk-1.2.0/atriumsports/endpoints.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-19 16:08:31.098856 atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/
--rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-06-19 16:08:30.000000 atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)    27051 2023-06-19 16:08:30.000000 atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)        1 2023-06-19 16:08:30.000000 atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)      108 2023-06-19 16:08:30.000000 atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/requires.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       13 2023-06-19 16:08:30.000000 atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/top_level.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.2.0/pyproject.toml
--rw-r--r--   0 k.kieda    (502) staff       (20)       38 2023-06-19 16:08:31.099390 atriumsports_sdk-1.2.0/setup.cfg
--rw-r--r--   0 k.kieda    (502) staff       (20)      947 2023-06-15 14:59:10.000000 atriumsports_sdk-1.2.0/setup.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:33:00.001567 atriumsports_sdk-1.3.0/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.0/LICENSE
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-06-26 10:33:00.001375 atriumsports_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.3.0/README.md
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:32:59.768841 atriumsports_sdk-1.3.0/atriumsports/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1096 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.0/atriumsports/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.0/atriumsports/atrium_response.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:32:59.769672 atriumsports_sdk-1.3.0/atriumsports/datacore/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6660 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/datacore.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:32:59.773127 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    54651 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/__init__.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:32:59.816857 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4630 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   121018 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/awards_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59847 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/career_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18925 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/change_log_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    97107 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/competition_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127164 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/competitions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    78128 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/conduct_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   137833 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    66311 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/download_video_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    91278 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    21039 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127554 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70185 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entity_groups_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59444 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11205 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59323 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77945 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72387 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76686 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    89352 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   407884 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixtures_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   252466 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/images_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70633 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73398 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70024 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/leagues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73817 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70215 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/merge_records_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    66029 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/organizations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    36028 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/partner_apis_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23558 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   134432 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    91522 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   107461 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/rankings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   150045 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/roles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77289 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    49629 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71603 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    44646 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_leaders_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    50867 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71598 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_person_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77803 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    97800 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    90287 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_series_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   177700 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   120275 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/seasons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    68423 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/sites_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   229910 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76768 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71710 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/standing_configurations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   137275 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/standings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71111 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/transfers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   100928 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/venues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73928 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76269 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72341 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/video_streams_available_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28317 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api_client.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)      779 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    14860 2023-06-26 10:32:24.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5022 2023-06-26 10:32:16.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/exceptions.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:32:59.999148 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    35789 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6094 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/award_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5926 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/award_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10475 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/awards_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2330 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/awards_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/awards_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3057 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/blank_model_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5041 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2530 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3762 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4448 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/change_log_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/change_log_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3532 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/change_log_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4405 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4302 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4401 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9341 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9112 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11710 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2316 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2376 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3567 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11966 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23827 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2938 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18995 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18856 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conference_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5174 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conference_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7587 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conferences_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2368 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conferences_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3555 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conferences_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3114 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/contact_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6109 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/division_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5676 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/division_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8546 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/divisions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/divisions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/divisions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18029 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2343 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5227 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5268 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4876 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11288 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4222 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3406 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11119 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13235 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_groups_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_groups_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4836 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15522 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4158 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3348 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15400 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1929 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/environmental_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2849 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/error_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2825 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/error_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6046 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12585 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9137 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2747 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4700 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5193 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2545 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2244 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2703 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5527 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_participant.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10059 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2425 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3605 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4486 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2660 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7624 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6090 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2546 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3138 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4767 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9886 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2416 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2309 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6942 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22216 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3960 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2650 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2393 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3225 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5970 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22088 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6724 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2386 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3884 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3201 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28618 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28554 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2359 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2292 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_round.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2305 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_series.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2274 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4979 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7681 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_person_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_person_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1897 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_identification.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2049 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2363 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2499 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9444 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2329 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1757 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1876 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/included_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3200 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2085 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1837 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3635 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5867 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2430 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3616 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2728 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6652 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/league_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6530 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/league_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8593 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leagues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leagues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leagues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5994 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organization_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5784 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organization_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7119 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organizations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3579 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organizations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5672 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5833 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2556 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_list_default_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13370 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5720 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13315 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15343 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6103 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/pool_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5679 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/pool_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5564 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4618 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4458 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2200 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/response_links.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3437 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/response_meta_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11638 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/role_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11517 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/role_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15525 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/roles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/roles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/roles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7057 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/round_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6627 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/round_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8848 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9018 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5624 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6248 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5241 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2526 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2442 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3772 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6931 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3893 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5731 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6195 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3783 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5105 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2522 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3750 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6836 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7006 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4072 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8501 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_pools_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_pools_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18148 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18363 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10457 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2378 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5981 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9996 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_rounds_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2370 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_rounds_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4466 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16333 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5733 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stage_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5248 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stage_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7537 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stages_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stages_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5288 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3796 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5276 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11002 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2428 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3957 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22249 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_competition.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12210 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/series_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11915 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/series_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5211 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/site_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6538 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/site_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6354 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/site_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7786 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sites_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sites_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sites_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3245 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/social_media.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2237 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sorting.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12332 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12243 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    17425 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4994 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_building.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13200 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2482 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4849 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4563 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3688 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12098 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18313 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4442 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12099 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18136 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standings_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1778 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/success_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/success_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2624 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfer_component.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7246 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfer_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7087 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfer_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9588 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5219 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5326 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10631 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10463 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12568 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2328 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2248 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9562 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_file_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2163 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_download_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_download_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11486 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2361 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11747 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2441 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5343 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2433 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3473 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3312 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9468 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2449 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11463 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11577 2023-06-26 10:32:26.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13664 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2447 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3640 2023-06-26 10:32:25.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12618 2023-06-26 10:32:24.000000 atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/rest.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:32:59.999674 atriumsports_sdk-1.3.0/atriumsports/datacore_stream/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.3.0/atriumsports/datacore_stream/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.3.0/atriumsports/datacore_stream/datacore_stream.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1942 2023-06-16 15:50:29.000000 atriumsports_sdk-1.3.0/atriumsports/endpoints.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-06-26 10:33:00.001095 atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-06-26 10:32:59.000000 atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)    27301 2023-06-26 10:32:59.000000 atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)        1 2023-06-26 10:32:59.000000 atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)      108 2023-06-26 10:32:59.000000 atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/requires.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       13 2023-06-26 10:32:59.000000 atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/top_level.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.3.0/pyproject.toml
+-rw-r--r--   0 k.kieda    (502) staff       (20)       38 2023-06-26 10:33:00.001621 atriumsports_sdk-1.3.0/setup.cfg
+-rw-r--r--   0 k.kieda    (502) staff       (20)      947 2023-06-26 10:31:58.000000 atriumsports_sdk-1.3.0/setup.py
```

### Comparing `atriumsports_sdk-1.2.0/LICENSE` & `atriumsports_sdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/PKG-INFO` & `atriumsports_sdk-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports_sdk
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.2.0/README.md` & `atriumsports_sdk-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/__init__.py` & `atriumsports_sdk-1.3.0/atriumsports/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/atrium_response.py` & `atriumsports_sdk-1.3.0/atriumsports/atrium_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/datacore.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/datacore.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/__init__.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
 This **access token** must then be sent in the `Authorization` header for each subsequent API call.  Access tokens have a finite life and will expire. When the token expires you will need to create a new token to make more API calls.  Creation of tokens is rate-limited, so you should use the existing token as long as possible.
 
 <!-- ReDoc-Inject: <security-definitions> -->
   # noqa: E501
 """
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 # import apis into sdk package
 from atriumsports.datacore.openapi.api.awards_api import AwardsApi
 from atriumsports.datacore.openapi.api.career_statistics_api import CareerStatisticsApi
 from atriumsports.datacore.openapi.api.change_log_api import ChangeLogApi
 from atriumsports.datacore.openapi.api.competition_statistics_api import CompetitionStatisticsApi
 from atriumsports.datacore.openapi.api.competitions_api import CompetitionsApi
@@ -315,14 +315,21 @@
 # import models into sdk package
 from atriumsports.datacore.openapi.models.award_post_body import AwardPostBody
 from atriumsports.datacore.openapi.models.award_put_body import AwardPutBody
 from atriumsports.datacore.openapi.models.awards_model import AwardsModel
 from atriumsports.datacore.openapi.models.awards_model_organization import AwardsModelOrganization
 from atriumsports.datacore.openapi.models.awards_response import AwardsResponse
 from atriumsports.datacore.openapi.models.blank_model_response import BlankModelResponse
+from atriumsports.datacore.openapi.models.career_person_season_statistics_model import CareerPersonSeasonStatisticsModel
+from atriumsports.datacore.openapi.models.career_person_season_statistics_model_organization import (
+    CareerPersonSeasonStatisticsModelOrganization,
+)
+from atriumsports.datacore.openapi.models.career_person_season_statistics_response import (
+    CareerPersonSeasonStatisticsResponse,
+)
 from atriumsports.datacore.openapi.models.career_person_statistics_model import CareerPersonStatisticsModel
 from atriumsports.datacore.openapi.models.career_person_statistics_model_organization import (
     CareerPersonStatisticsModelOrganization,
 )
 from atriumsports.datacore.openapi.models.career_person_statistics_response import CareerPersonStatisticsResponse
 from atriumsports.datacore.openapi.models.change_log_model import ChangeLogModel
 from atriumsports.datacore.openapi.models.change_log_model_organization import ChangeLogModelOrganization
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/__init__.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/awards_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/awards_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/career_statistics_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_leaders_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,39 +20,42 @@
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, ValidationError, conint, constr, validate_arguments
 from typing_extensions import Annotated
 
 from atriumsports.datacore.openapi.api_client import ApiClient
 from atriumsports.datacore.openapi.api_response import ApiResponse
 from atriumsports.datacore.openapi.exceptions import ApiTypeError, ApiValueError  # noqa: F401
-from atriumsports.datacore.openapi.models.career_person_statistics_response import CareerPersonStatisticsResponse
+from atriumsports.datacore.openapi.models.leader_summary_response import LeaderSummaryResponse
+from atriumsports.datacore.openapi.models.season_person_statistics_response import SeasonPersonStatisticsResponse
 
 logger = logging.getLogger("openapi")
 
 
-class CareerStatisticsApi(object):
+class SeasonLeadersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def caps_list(
+    def sl_list(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
+        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        statistic: Annotated[constr(strict=True, max_length=50), Field(..., description="The name of the statistic")],
         entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
@@ -98,28 +101,32 @@
         person_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the person")] = None,
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
-    ) -> CareerPersonStatisticsResponse:  # noqa: E501
-        """Person career statistics  # noqa: E501
+    ) -> SeasonPersonStatisticsResponse:  # noqa: E501
+        """Season statistical leaders  # noqa: E501
 
-        Return a list of person statistic totals for their career covering all competitions  # noqa: E501
+        Return a list of the leading persons for a statistic in a season.  This call is similar to the person fixture statistics call~ however this call applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.caps_list(organization_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
+        >>> thread = api.sl_list(organization_id, season_id, sport, statistic, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
+        :param season_id: The unique identifier of the season (required)
+        :type season_id: str
         :param sport: Sport name (required)
         :type sport: str
+        :param statistic: The name of the statistic (required)
+        :type statistic: str
         :param entity_id: The unique identifier of the entity
         :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
@@ -149,25 +156,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: CareerPersonStatisticsResponse
+        :rtype: SeasonPersonStatisticsResponse
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
             raise ValueError(
-                "Error! Please call the caps_list_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+                "Error! Please call the sl_list_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
             )
         try:
-            return self.caps_list_with_http_info(
+            return self.sl_list_with_http_info(
                 organization_id,
+                season_id,
                 sport,
+                statistic,
                 entity_id,
                 external,
                 fields,
                 fixture_type,
                 hide_null,
                 home_away,
                 include,
@@ -177,25 +186,27 @@
                 offset,
                 person_id,
                 starter,
                 win_loss,
                 **kwargs
             )  # noqa: E501
         except Exception as e:
-            logger.error("Exception when calling CareerStatisticsApi->caps_list: %s\n" % e)
+            logger.error("Exception when calling SeasonLeadersApi->sl_list: %s\n" % e)
             raise
 
     @validate_arguments
-    def caps_list_with_http_info(
+    def sl_list_with_http_info(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
+        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        statistic: Annotated[constr(strict=True, max_length=50), Field(..., description="The name of the statistic")],
         entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
@@ -242,27 +253,31 @@
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
     ) -> ApiResponse:  # noqa: E501
-        """Person career statistics  # noqa: E501
+        """Season statistical leaders  # noqa: E501
 
-        Return a list of person statistic totals for their career covering all competitions  # noqa: E501
+        Return a list of the leading persons for a statistic in a season.  This call is similar to the person fixture statistics call~ however this call applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.caps_list_with_http_info(organization_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
+        >>> thread = api.sl_list_with_http_info(organization_id, season_id, sport, statistic, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
+        :param season_id: The unique identifier of the season (required)
+        :type season_id: str
         :param sport: Sport name (required)
         :type sport: str
+        :param statistic: The name of the statistic (required)
+        :type statistic: str
         :param entity_id: The unique identifier of the entity
         :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
@@ -305,22 +320,24 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(CareerPersonStatisticsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(SeasonPersonStatisticsResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             "organization_id",
+            "season_id",
             "sport",
+            "statistic",
             "entity_id",
             "external",
             "fields",
             "fixture_type",
             "hide_null",
             "home_away",
             "include",
@@ -343,28 +360,34 @@
                 "_headers",
             ]
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method caps_list" % _key)
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method sl_list" % _key)
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["organization_id"]:
             _path_params["organizationId"] = _params["organization_id"]
 
+        if _params["season_id"]:
+            _path_params["seasonId"] = _params["season_id"]
+
         if _params["sport"]:
             _path_params["sport"] = _params["sport"]
 
+        if _params["statistic"]:
+            _path_params["statistic"] = _params["statistic"]
+
         # process the query parameters
         _query_params = []
         if _params.get("entity_id") is not None:  # noqa: E501
             _query_params.append(("entityId", _params["entity_id"]))
 
         if _params.get("external") is not None:  # noqa: E501
             _query_params.append(("external", _params["external"]))
@@ -415,19 +438,19 @@
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
         # authentication setting
         _auth_settings = ["OAuth2"]  # noqa: E501
 
         _response_types_map = {
-            "200": "CareerPersonStatisticsResponse",
+            "200": "SeasonPersonStatisticsResponse",
         }
 
         return self.api_client.call_api(
-            "/{sport}/o/{organizationId}/statistics/for/person/in/career",
+            "/{sport}/o/{organizationId}/statistics/leaders/for/{statistic}/in/seasons/{seasonId}",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -438,22 +461,23 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def caps_listperson(
+    def sl_list_summary(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
-        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
+        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
         fields: Annotated[
@@ -491,36 +515,43 @@
         ] = None,
         offset: Annotated[
             Optional[StrictInt],
             Field(
                 description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
+        person_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the person")] = None,
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
+        statistics: Annotated[
+            Optional[constr(strict=True, max_length=200)],
+            Field(description="The name of the statistic. Can specify multiple, delimited by comma."),
+        ] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
-    ) -> CareerPersonStatisticsResponse:  # noqa: E501
-        """Statistics for a person in their career  # noqa: E501
+    ) -> LeaderSummaryResponse:  # noqa: E501
+        """Season statistical leader summary  # noqa: E501
 
-        Return the statistics for a specific person in their career.  # noqa: E501
+        Return a summary of the leading persons for a number of statistics in a season.  This call allows you to specify multiple statistics at the same time.  It will return objects for each statistic.  In the 'statistics' object only the requested statistic will be returned, not all available statistics.  This call also applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.caps_listperson(organization_id, person_id, sport, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, starter, win_loss, async_req=True)
+        >>> thread = api.sl_list_summary(organization_id, season_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, statistics, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
-        :param person_id: The unique identifier of the person (required)
-        :type person_id: str
+        :param season_id: The unique identifier of the season (required)
+        :type season_id: str
         :param sport: Sport name (required)
         :type sport: str
+        :param entity_id: The unique identifier of the entity
+        :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
         :type fixture_type: str
         :param hide_null: Don't display data fields with null values or empty structures
@@ -533,66 +564,74 @@
         :type is_player: bool
         :param is_team_official: Is the person a entity official?
         :type is_team_official: bool
         :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
         :type limit: int
         :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
         :type offset: int
+        :param person_id: The unique identifier of the person
+        :type person_id: str
         :param starter: Is the person a starter in the fixture ?
         :type starter: bool
+        :param statistics: The name of the statistic. Can specify multiple, delimited by comma.
+        :type statistics: str
         :param win_loss: What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win
         :type win_loss: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: CareerPersonStatisticsResponse
+        :rtype: LeaderSummaryResponse
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
             raise ValueError(
-                "Error! Please call the caps_listperson_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+                "Error! Please call the sl_list_summary_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
             )
         try:
-            return self.caps_listperson_with_http_info(
+            return self.sl_list_summary_with_http_info(
                 organization_id,
-                person_id,
+                season_id,
                 sport,
+                entity_id,
                 external,
                 fields,
                 fixture_type,
                 hide_null,
                 home_away,
                 include,
                 is_player,
                 is_team_official,
                 limit,
                 offset,
+                person_id,
                 starter,
+                statistics,
                 win_loss,
                 **kwargs
             )  # noqa: E501
         except Exception as e:
-            logger.error("Exception when calling CareerStatisticsApi->caps_listperson: %s\n" % e)
+            logger.error("Exception when calling SeasonLeadersApi->sl_list_summary: %s\n" % e)
             raise
 
     @validate_arguments
-    def caps_listperson_with_http_info(
+    def sl_list_summary_with_http_info(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
-        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
+        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
         fields: Annotated[
@@ -630,36 +669,43 @@
         ] = None,
         offset: Annotated[
             Optional[StrictInt],
             Field(
                 description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
+        person_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the person")] = None,
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
+        statistics: Annotated[
+            Optional[constr(strict=True, max_length=200)],
+            Field(description="The name of the statistic. Can specify multiple, delimited by comma."),
+        ] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
     ) -> ApiResponse:  # noqa: E501
-        """Statistics for a person in their career  # noqa: E501
+        """Season statistical leader summary  # noqa: E501
 
-        Return the statistics for a specific person in their career.  # noqa: E501
+        Return a summary of the leading persons for a number of statistics in a season.  This call allows you to specify multiple statistics at the same time.  It will return objects for each statistic.  In the 'statistics' object only the requested statistic will be returned, not all available statistics.  This call also applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.caps_listperson_with_http_info(organization_id, person_id, sport, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, starter, win_loss, async_req=True)
+        >>> thread = api.sl_list_summary_with_http_info(organization_id, season_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, statistics, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
-        :param person_id: The unique identifier of the person (required)
-        :type person_id: str
+        :param season_id: The unique identifier of the season (required)
+        :type season_id: str
         :param sport: Sport name (required)
         :type sport: str
+        :param entity_id: The unique identifier of the entity
+        :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
         :type fixture_type: str
         :param hide_null: Don't display data fields with null values or empty structures
@@ -672,16 +718,20 @@
         :type is_player: bool
         :param is_team_official: Is the person a entity official?
         :type is_team_official: bool
         :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
         :type limit: int
         :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
         :type offset: int
+        :param person_id: The unique identifier of the person
+        :type person_id: str
         :param starter: Is the person a starter in the fixture ?
         :type starter: bool
+        :param statistics: The name of the statistic. Can specify multiple, delimited by comma.
+        :type statistics: str
         :param win_loss: What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win
         :type win_loss: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
@@ -698,34 +748,37 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(CareerPersonStatisticsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(LeaderSummaryResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             "organization_id",
-            "person_id",
+            "season_id",
             "sport",
+            "entity_id",
             "external",
             "fields",
             "fixture_type",
             "hide_null",
             "home_away",
             "include",
             "is_player",
             "is_team_official",
             "limit",
             "offset",
+            "person_id",
             "starter",
+            "statistics",
             "win_loss",
         ]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
@@ -735,33 +788,36 @@
                 "_headers",
             ]
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method caps_listperson" % _key)
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method sl_list_summary" % _key)
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["organization_id"]:
             _path_params["organizationId"] = _params["organization_id"]
 
-        if _params["person_id"]:
-            _path_params["personId"] = _params["person_id"]
+        if _params["season_id"]:
+            _path_params["seasonId"] = _params["season_id"]
 
         if _params["sport"]:
             _path_params["sport"] = _params["sport"]
 
         # process the query parameters
         _query_params = []
+        if _params.get("entity_id") is not None:  # noqa: E501
+            _query_params.append(("entityId", _params["entity_id"]))
+
         if _params.get("external") is not None:  # noqa: E501
             _query_params.append(("external", _params["external"]))
 
         if _params.get("fields") is not None:  # noqa: E501
             _query_params.append(("fields", _params["fields"]))
 
         if _params.get("fixture_type") is not None:  # noqa: E501
@@ -784,17 +840,23 @@
 
         if _params.get("limit") is not None:  # noqa: E501
             _query_params.append(("limit", _params["limit"]))
 
         if _params.get("offset") is not None:  # noqa: E501
             _query_params.append(("offset", _params["offset"]))
 
+        if _params.get("person_id") is not None:  # noqa: E501
+            _query_params.append(("personId", _params["person_id"]))
+
         if _params.get("starter") is not None:  # noqa: E501
             _query_params.append(("starter", _params["starter"]))
 
+        if _params.get("statistics") is not None:  # noqa: E501
+            _query_params.append(("statistics", _params["statistics"]))
+
         if _params.get("win_loss") is not None:  # noqa: E501
             _query_params.append(("winLoss", _params["win_loss"].value))
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
@@ -804,19 +866,19 @@
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
         # authentication setting
         _auth_settings = ["OAuth2"]  # noqa: E501
 
         _response_types_map = {
-            "200": "CareerPersonStatisticsResponse",
+            "200": "LeaderSummaryResponse",
         }
 
         return self.api_client.call_api(
-            "/{sport}/o/{organizationId}/statistics/for/person/in/career/persons/{personId}",
+            "/{sport}/o/{organizationId}/statistics/leaders/in/seasons/{seasonId}",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/change_log_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/change_log_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/competition_statistics_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/competition_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/competitions_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/competitions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/conduct_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/conduct_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/download_video_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/download_video_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entities_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/entity_groups_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/entity_groups_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_entities_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_persons_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixture_roster_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixture_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/fixtures_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/fixtures_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/images_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/images_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/leagues_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/leagues_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/merge_records_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/merge_records_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/organizations_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/partner_apis_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/partner_apis_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/persons_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/rankings_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/rankings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/roles_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_entities_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_leaders_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/career_statistics_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,42 +20,42 @@
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, ValidationError, conint, constr, validate_arguments
 from typing_extensions import Annotated
 
 from atriumsports.datacore.openapi.api_client import ApiClient
 from atriumsports.datacore.openapi.api_response import ApiResponse
 from atriumsports.datacore.openapi.exceptions import ApiTypeError, ApiValueError  # noqa: F401
-from atriumsports.datacore.openapi.models.leader_summary_response import LeaderSummaryResponse
-from atriumsports.datacore.openapi.models.season_person_statistics_response import SeasonPersonStatisticsResponse
+from atriumsports.datacore.openapi.models.career_person_season_statistics_response import (
+    CareerPersonSeasonStatisticsResponse,
+)
+from atriumsports.datacore.openapi.models.career_person_statistics_response import CareerPersonStatisticsResponse
 
 logger = logging.getLogger("openapi")
 
 
-class SeasonLeadersApi(object):
+class CareerStatisticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def sl_list(
+    def caps_list(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
-        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
-        statistic: Annotated[constr(strict=True, max_length=50), Field(..., description="The name of the statistic")],
         entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
@@ -101,32 +101,28 @@
         person_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the person")] = None,
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
-    ) -> SeasonPersonStatisticsResponse:  # noqa: E501
-        """Season statistical leaders  # noqa: E501
+    ) -> CareerPersonStatisticsResponse:  # noqa: E501
+        """Person career statistics  # noqa: E501
 
-        Return a list of the leading persons for a statistic in a season.  This call is similar to the person fixture statistics call~ however this call applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
+        Return a list of person statistic totals for their career covering all competitions  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sl_list(organization_id, season_id, sport, statistic, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
+        >>> thread = api.caps_list(organization_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
-        :param season_id: The unique identifier of the season (required)
-        :type season_id: str
         :param sport: Sport name (required)
         :type sport: str
-        :param statistic: The name of the statistic (required)
-        :type statistic: str
         :param entity_id: The unique identifier of the entity
         :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
@@ -156,27 +152,25 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: SeasonPersonStatisticsResponse
+        :rtype: CareerPersonStatisticsResponse
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
             raise ValueError(
-                "Error! Please call the sl_list_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+                "Error! Please call the caps_list_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
             )
         try:
-            return self.sl_list_with_http_info(
+            return self.caps_list_with_http_info(
                 organization_id,
-                season_id,
                 sport,
-                statistic,
                 entity_id,
                 external,
                 fields,
                 fixture_type,
                 hide_null,
                 home_away,
                 include,
@@ -186,27 +180,25 @@
                 offset,
                 person_id,
                 starter,
                 win_loss,
                 **kwargs
             )  # noqa: E501
         except Exception as e:
-            logger.error("Exception when calling SeasonLeadersApi->sl_list: %s\n" % e)
+            logger.error("Exception when calling CareerStatisticsApi->caps_list: %s\n" % e)
             raise
 
     @validate_arguments
-    def sl_list_with_http_info(
+    def caps_list_with_http_info(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
-        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
-        statistic: Annotated[constr(strict=True, max_length=50), Field(..., description="The name of the statistic")],
         entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
@@ -253,31 +245,27 @@
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
     ) -> ApiResponse:  # noqa: E501
-        """Season statistical leaders  # noqa: E501
+        """Person career statistics  # noqa: E501
 
-        Return a list of the leading persons for a statistic in a season.  This call is similar to the person fixture statistics call~ however this call applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
+        Return a list of person statistic totals for their career covering all competitions  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sl_list_with_http_info(organization_id, season_id, sport, statistic, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
+        >>> thread = api.caps_list_with_http_info(organization_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
-        :param season_id: The unique identifier of the season (required)
-        :type season_id: str
         :param sport: Sport name (required)
         :type sport: str
-        :param statistic: The name of the statistic (required)
-        :type statistic: str
         :param entity_id: The unique identifier of the entity
         :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
@@ -320,24 +308,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(SeasonPersonStatisticsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(CareerPersonStatisticsResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             "organization_id",
-            "season_id",
             "sport",
-            "statistic",
             "entity_id",
             "external",
             "fields",
             "fixture_type",
             "hide_null",
             "home_away",
             "include",
@@ -360,34 +346,28 @@
                 "_headers",
             ]
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method sl_list" % _key)
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method caps_list" % _key)
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["organization_id"]:
             _path_params["organizationId"] = _params["organization_id"]
 
-        if _params["season_id"]:
-            _path_params["seasonId"] = _params["season_id"]
-
         if _params["sport"]:
             _path_params["sport"] = _params["sport"]
 
-        if _params["statistic"]:
-            _path_params["statistic"] = _params["statistic"]
-
         # process the query parameters
         _query_params = []
         if _params.get("entity_id") is not None:  # noqa: E501
             _query_params.append(("entityId", _params["entity_id"]))
 
         if _params.get("external") is not None:  # noqa: E501
             _query_params.append(("external", _params["external"]))
@@ -438,19 +418,19 @@
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
         # authentication setting
         _auth_settings = ["OAuth2"]  # noqa: E501
 
         _response_types_map = {
-            "200": "SeasonPersonStatisticsResponse",
+            "200": "CareerPersonStatisticsResponse",
         }
 
         return self.api_client.call_api(
-            "/{sport}/o/{organizationId}/statistics/leaders/for/{statistic}/in/seasons/{seasonId}",
+            "/{sport}/o/{organizationId}/statistics/for/person/in/career",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -461,23 +441,22 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def sl_list_summary(
+    def caps_list_person_season(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
-        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
+        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
-        entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
         fields: Annotated[
@@ -515,43 +494,175 @@
         ] = None,
         offset: Annotated[
             Optional[StrictInt],
             Field(
                 description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
-        person_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the person")] = None,
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
-        statistics: Annotated[
-            Optional[constr(strict=True, max_length=200)],
-            Field(description="The name of the statistic. Can specify multiple, delimited by comma."),
+        win_loss: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
+        **kwargs
+    ) -> CareerPersonSeasonStatisticsResponse:  # noqa: E501
+        """Statistics for a person in their career by season and entity  # noqa: E501
+
+        Return the statistics for a specific person in their career by season and entity.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.caps_list_person_season(organization_id, person_id, sport, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, starter, win_loss, async_req=True)
+        >>> result = thread.get()
+
+        :param organization_id: The unique identifier of the organization (required)
+        :type organization_id: str
+        :param person_id: The unique identifier of the person (required)
+        :type person_id: str
+        :param sport: Sport name (required)
+        :type sport: str
+        :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
+        :type external: str
+        :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
+        :type fields: str
+        :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
+        :type fixture_type: str
+        :param hide_null: Don't display data fields with null values or empty structures
+        :type hide_null: bool
+        :param home_away: Where the result was >- `AWAY` Away >- `HOME` Home
+        :type home_away: str
+        :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
+        :type include: str
+        :param is_player: Is the person a player?
+        :type is_player: bool
+        :param is_team_official: Is the person a entity official?
+        :type is_team_official: bool
+        :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type limit: int
+        :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type offset: int
+        :param starter: Is the person a starter in the fixture ?
+        :type starter: bool
+        :param win_loss: What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win
+        :type win_loss: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: CareerPersonSeasonStatisticsResponse
+        """
+        kwargs["_return_http_data_only"] = True
+        if "_preload_content" in kwargs:
+            raise ValueError(
+                "Error! Please call the caps_list_person_season_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+            )
+        try:
+            return self.caps_list_person_season_with_http_info(
+                organization_id,
+                person_id,
+                sport,
+                external,
+                fields,
+                fixture_type,
+                hide_null,
+                home_away,
+                include,
+                is_player,
+                is_team_official,
+                limit,
+                offset,
+                starter,
+                win_loss,
+                **kwargs
+            )  # noqa: E501
+        except Exception as e:
+            logger.error("Exception when calling CareerStatisticsApi->caps_list_person_season: %s\n" % e)
+            raise
+
+    @validate_arguments
+    def caps_list_person_season_with_http_info(
+        self,
+        organization_id: Annotated[
+            constr(strict=True, max_length=5, min_length=5),
+            Field(..., description="The unique identifier of the organization"),
+        ],
+        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
+        sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        external: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
+            ),
+        ] = None,
+        fields: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information."
+            ),
+        ] = None,
+        fixture_type: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(
+                description="Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular "
+            ),
+        ] = None,
+        hide_null: Annotated[
+            Optional[StrictBool], Field(description="Don't display data fields with null values or empty structures")
+        ] = None,
+        home_away: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(description="Where the result was >- `AWAY` Away >- `HOME` Home "),
+        ] = None,
+        include: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information."
+            ),
+        ] = None,
+        is_player: Annotated[Optional[StrictBool], Field(description="Is the person a player?")] = None,
+        is_team_official: Annotated[Optional[StrictBool], Field(description="Is the person a entity official?")] = None,
+        limit: Annotated[
+            Optional[conint(strict=True, le=1000, ge=1)],
+            Field(
+                description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        offset: Annotated[
+            Optional[StrictInt],
+            Field(
+                description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
-    ) -> LeaderSummaryResponse:  # noqa: E501
-        """Season statistical leader summary  # noqa: E501
+    ) -> ApiResponse:  # noqa: E501
+        """Statistics for a person in their career by season and entity  # noqa: E501
 
-        Return a summary of the leading persons for a number of statistics in a season.  This call allows you to specify multiple statistics at the same time.  It will return objects for each statistic.  In the 'statistics' object only the requested statistic will be returned, not all available statistics.  This call also applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
+        Return the statistics for a specific person in their career by season and entity.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sl_list_summary(organization_id, season_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, statistics, win_loss, async_req=True)
+        >>> thread = api.caps_list_person_season_with_http_info(organization_id, person_id, sport, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, starter, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
-        :param season_id: The unique identifier of the season (required)
-        :type season_id: str
+        :param person_id: The unique identifier of the person (required)
+        :type person_id: str
         :param sport: Sport name (required)
         :type sport: str
-        :param entity_id: The unique identifier of the entity
-        :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
         :type fixture_type: str
         :param hide_null: Don't display data fields with null values or empty structures
@@ -564,74 +675,318 @@
         :type is_player: bool
         :param is_team_official: Is the person a entity official?
         :type is_team_official: bool
         :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
         :type limit: int
         :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
         :type offset: int
-        :param person_id: The unique identifier of the person
+        :param starter: Is the person a starter in the fixture ?
+        :type starter: bool
+        :param win_loss: What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win
+        :type win_loss: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(CareerPersonSeasonStatisticsResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            "organization_id",
+            "person_id",
+            "sport",
+            "external",
+            "fields",
+            "fixture_type",
+            "hide_null",
+            "home_away",
+            "include",
+            "is_player",
+            "is_team_official",
+            "limit",
+            "offset",
+            "starter",
+            "win_loss",
+        ]
+        _all_params.extend(
+            [
+                "async_req",
+                "_return_http_data_only",
+                "_preload_content",
+                "_request_timeout",
+                "_request_auth",
+                "_content_type",
+                "_headers",
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params["kwargs"].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'" " to method caps_list_person_season" % _key
+                )
+            _params[_key] = _val
+        del _params["kwargs"]
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params["organization_id"]:
+            _path_params["organizationId"] = _params["organization_id"]
+
+        if _params["person_id"]:
+            _path_params["personId"] = _params["person_id"]
+
+        if _params["sport"]:
+            _path_params["sport"] = _params["sport"]
+
+        # process the query parameters
+        _query_params = []
+        if _params.get("external") is not None:  # noqa: E501
+            _query_params.append(("external", _params["external"]))
+
+        if _params.get("fields") is not None:  # noqa: E501
+            _query_params.append(("fields", _params["fields"]))
+
+        if _params.get("fixture_type") is not None:  # noqa: E501
+            _query_params.append(("fixtureType", _params["fixture_type"].value))
+
+        if _params.get("hide_null") is not None:  # noqa: E501
+            _query_params.append(("hideNull", _params["hide_null"]))
+
+        if _params.get("home_away") is not None:  # noqa: E501
+            _query_params.append(("homeAway", _params["home_away"].value))
+
+        if _params.get("include") is not None:  # noqa: E501
+            _query_params.append(("include", _params["include"]))
+
+        if _params.get("is_player") is not None:  # noqa: E501
+            _query_params.append(("isPlayer", _params["is_player"]))
+
+        if _params.get("is_team_official") is not None:  # noqa: E501
+            _query_params.append(("isTeamOfficial", _params["is_team_official"]))
+
+        if _params.get("limit") is not None:  # noqa: E501
+            _query_params.append(("limit", _params["limit"]))
+
+        if _params.get("offset") is not None:  # noqa: E501
+            _query_params.append(("offset", _params["offset"]))
+
+        if _params.get("starter") is not None:  # noqa: E501
+            _query_params.append(("starter", _params["starter"]))
+
+        if _params.get("win_loss") is not None:  # noqa: E501
+            _query_params.append(("winLoss", _params["win_loss"].value))
+
+        # process the header parameters
+        _header_params = dict(_params.get("_headers", {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ["OAuth2"]  # noqa: E501
+
+        _response_types_map = {
+            "200": "CareerPersonSeasonStatisticsResponse",
+        }
+
+        return self.api_client.call_api(
+            "/{sport}/o/{organizationId}/statistics/for/person/in/career/seasons/persons/{personId}",
+            "GET",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get("async_req"),
+            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
+            _preload_content=_params.get("_preload_content", True),
+            _request_timeout=_params.get("_request_timeout"),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get("_request_auth"),
+        )
+
+    @validate_arguments
+    def caps_listperson(
+        self,
+        organization_id: Annotated[
+            constr(strict=True, max_length=5, min_length=5),
+            Field(..., description="The unique identifier of the organization"),
+        ],
+        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
+        sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        external: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
+            ),
+        ] = None,
+        fields: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information."
+            ),
+        ] = None,
+        fixture_type: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(
+                description="Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular "
+            ),
+        ] = None,
+        hide_null: Annotated[
+            Optional[StrictBool], Field(description="Don't display data fields with null values or empty structures")
+        ] = None,
+        home_away: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(description="Where the result was >- `AWAY` Away >- `HOME` Home "),
+        ] = None,
+        include: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information."
+            ),
+        ] = None,
+        is_player: Annotated[Optional[StrictBool], Field(description="Is the person a player?")] = None,
+        is_team_official: Annotated[Optional[StrictBool], Field(description="Is the person a entity official?")] = None,
+        limit: Annotated[
+            Optional[conint(strict=True, le=1000, ge=1)],
+            Field(
+                description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        offset: Annotated[
+            Optional[StrictInt],
+            Field(
+                description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
+        win_loss: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
+        ] = None,
+        **kwargs
+    ) -> CareerPersonStatisticsResponse:  # noqa: E501
+        """Statistics for a person in their career  # noqa: E501
+
+        Return the statistics for a specific person in their career.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.caps_listperson(organization_id, person_id, sport, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, starter, win_loss, async_req=True)
+        >>> result = thread.get()
+
+        :param organization_id: The unique identifier of the organization (required)
+        :type organization_id: str
+        :param person_id: The unique identifier of the person (required)
         :type person_id: str
+        :param sport: Sport name (required)
+        :type sport: str
+        :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
+        :type external: str
+        :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
+        :type fields: str
+        :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
+        :type fixture_type: str
+        :param hide_null: Don't display data fields with null values or empty structures
+        :type hide_null: bool
+        :param home_away: Where the result was >- `AWAY` Away >- `HOME` Home
+        :type home_away: str
+        :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
+        :type include: str
+        :param is_player: Is the person a player?
+        :type is_player: bool
+        :param is_team_official: Is the person a entity official?
+        :type is_team_official: bool
+        :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type limit: int
+        :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type offset: int
         :param starter: Is the person a starter in the fixture ?
         :type starter: bool
-        :param statistics: The name of the statistic. Can specify multiple, delimited by comma.
-        :type statistics: str
         :param win_loss: What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win
         :type win_loss: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: LeaderSummaryResponse
+        :rtype: CareerPersonStatisticsResponse
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
             raise ValueError(
-                "Error! Please call the sl_list_summary_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+                "Error! Please call the caps_listperson_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
             )
         try:
-            return self.sl_list_summary_with_http_info(
+            return self.caps_listperson_with_http_info(
                 organization_id,
-                season_id,
+                person_id,
                 sport,
-                entity_id,
                 external,
                 fields,
                 fixture_type,
                 hide_null,
                 home_away,
                 include,
                 is_player,
                 is_team_official,
                 limit,
                 offset,
-                person_id,
                 starter,
-                statistics,
                 win_loss,
                 **kwargs
             )  # noqa: E501
         except Exception as e:
-            logger.error("Exception when calling SeasonLeadersApi->sl_list_summary: %s\n" % e)
+            logger.error("Exception when calling CareerStatisticsApi->caps_listperson: %s\n" % e)
             raise
 
     @validate_arguments
-    def sl_list_summary_with_http_info(
+    def caps_listperson_with_http_info(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
-        season_id: Annotated[StrictStr, Field(..., description="The unique identifier of the season")],
+        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
         sport: Annotated[StrictStr, Field(..., description="Sport name")],
-        entity_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the entity")] = None,
         external: Annotated[
             Optional[StrictStr],
             Field(
                 description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
             ),
         ] = None,
         fields: Annotated[
@@ -669,43 +1024,36 @@
         ] = None,
         offset: Annotated[
             Optional[StrictInt],
             Field(
                 description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
-        person_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the person")] = None,
         starter: Annotated[Optional[StrictBool], Field(description="Is the person a starter in the fixture ?")] = None,
-        statistics: Annotated[
-            Optional[constr(strict=True, max_length=200)],
-            Field(description="The name of the statistic. Can specify multiple, delimited by comma."),
-        ] = None,
         win_loss: Annotated[
             Optional[constr(strict=True, max_length=50)],
             Field(description="What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win "),
         ] = None,
         **kwargs
     ) -> ApiResponse:  # noqa: E501
-        """Season statistical leader summary  # noqa: E501
+        """Statistics for a person in their career  # noqa: E501
 
-        Return a summary of the leading persons for a number of statistics in a season.  This call allows you to specify multiple statistics at the same time.  It will return objects for each statistic.  In the 'statistics' object only the requested statistic will be returned, not all available statistics.  This call also applies the qualification criteria (defined in the leaders qualification api calls) to each person.  # noqa: E501
+        Return the statistics for a specific person in their career.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sl_list_summary_with_http_info(organization_id, season_id, sport, entity_id, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, person_id, starter, statistics, win_loss, async_req=True)
+        >>> thread = api.caps_listperson_with_http_info(organization_id, person_id, sport, external, fields, fixture_type, hide_null, home_away, include, is_player, is_team_official, limit, offset, starter, win_loss, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
-        :param season_id: The unique identifier of the season (required)
-        :type season_id: str
+        :param person_id: The unique identifier of the person (required)
+        :type person_id: str
         :param sport: Sport name (required)
         :type sport: str
-        :param entity_id: The unique identifier of the entity
-        :type entity_id: str
         :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
         :type external: str
         :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
         :type fields: str
         :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
         :type fixture_type: str
         :param hide_null: Don't display data fields with null values or empty structures
@@ -718,20 +1066,16 @@
         :type is_player: bool
         :param is_team_official: Is the person a entity official?
         :type is_team_official: bool
         :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
         :type limit: int
         :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
         :type offset: int
-        :param person_id: The unique identifier of the person
-        :type person_id: str
         :param starter: Is the person a starter in the fixture ?
         :type starter: bool
-        :param statistics: The name of the statistic. Can specify multiple, delimited by comma.
-        :type statistics: str
         :param win_loss: What the result was >- `DRAW` Draw >- `LOSS` Loss >- `WIN` Win
         :type win_loss: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
@@ -748,37 +1092,34 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(LeaderSummaryResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(CareerPersonStatisticsResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             "organization_id",
-            "season_id",
+            "person_id",
             "sport",
-            "entity_id",
             "external",
             "fields",
             "fixture_type",
             "hide_null",
             "home_away",
             "include",
             "is_player",
             "is_team_official",
             "limit",
             "offset",
-            "person_id",
             "starter",
-            "statistics",
             "win_loss",
         ]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
@@ -788,36 +1129,33 @@
                 "_headers",
             ]
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method sl_list_summary" % _key)
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method caps_listperson" % _key)
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["organization_id"]:
             _path_params["organizationId"] = _params["organization_id"]
 
-        if _params["season_id"]:
-            _path_params["seasonId"] = _params["season_id"]
+        if _params["person_id"]:
+            _path_params["personId"] = _params["person_id"]
 
         if _params["sport"]:
             _path_params["sport"] = _params["sport"]
 
         # process the query parameters
         _query_params = []
-        if _params.get("entity_id") is not None:  # noqa: E501
-            _query_params.append(("entityId", _params["entity_id"]))
-
         if _params.get("external") is not None:  # noqa: E501
             _query_params.append(("external", _params["external"]))
 
         if _params.get("fields") is not None:  # noqa: E501
             _query_params.append(("fields", _params["fields"]))
 
         if _params.get("fixture_type") is not None:  # noqa: E501
@@ -840,23 +1178,17 @@
 
         if _params.get("limit") is not None:  # noqa: E501
             _query_params.append(("limit", _params["limit"]))
 
         if _params.get("offset") is not None:  # noqa: E501
             _query_params.append(("offset", _params["offset"]))
 
-        if _params.get("person_id") is not None:  # noqa: E501
-            _query_params.append(("personId", _params["person_id"]))
-
         if _params.get("starter") is not None:  # noqa: E501
             _query_params.append(("starter", _params["starter"]))
 
-        if _params.get("statistics") is not None:  # noqa: E501
-            _query_params.append(("statistics", _params["statistics"]))
-
         if _params.get("win_loss") is not None:  # noqa: E501
             _query_params.append(("winLoss", _params["win_loss"].value))
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
@@ -866,19 +1198,19 @@
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
         # authentication setting
         _auth_settings = ["OAuth2"]  # noqa: E501
 
         _response_types_map = {
-            "200": "LeaderSummaryResponse",
+            "200": "CareerPersonStatisticsResponse",
         }
 
         return self.api_client.call_api(
-            "/{sport}/o/{organizationId}/statistics/leaders/in/seasons/{seasonId}",
+            "/{sport}/o/{organizationId}/statistics/for/person/in/career/persons/{personId}",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_person_placings_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_person_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_persons_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_persons_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,366 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
+    def season_person_list(
+        self,
+        organization_id: Annotated[
+            constr(strict=True, max_length=5, min_length=5),
+            Field(..., description="The unique identifier of the organization"),
+        ],
+        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
+        sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        added: Annotated[
+            Optional[datetime], Field(description="Record was added after this date/time. In UTC.")
+        ] = None,
+        external: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
+            ),
+        ] = None,
+        fields: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information."
+            ),
+        ] = None,
+        hide_null: Annotated[
+            Optional[StrictBool], Field(description="Don't display data fields with null values or empty structures")
+        ] = None,
+        include: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information."
+            ),
+        ] = None,
+        limit: Annotated[
+            Optional[conint(strict=True, le=1000, ge=1)],
+            Field(
+                description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        offset: Annotated[
+            Optional[StrictInt],
+            Field(
+                description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        season_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the season")] = None,
+        updated: Annotated[
+            Optional[datetime], Field(description="Record was modified after this date/time. In UTC.")
+        ] = None,
+        **kwargs
+    ) -> SeasonPersonsListResponse:  # noqa: E501
+        """Get a list of seasons for person  # noqa: E501
+
+        Return a list of seasons that person participated in  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.season_person_list(organization_id, person_id, sport, added, external, fields, hide_null, include, limit, offset, season_id, updated, async_req=True)
+        >>> result = thread.get()
+
+        :param organization_id: The unique identifier of the organization (required)
+        :type organization_id: str
+        :param person_id: The unique identifier of the person (required)
+        :type person_id: str
+        :param sport: Sport name (required)
+        :type sport: str
+        :param added: Record was added after this date/time. In UTC.
+        :type added: datetime
+        :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
+        :type external: str
+        :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
+        :type fields: str
+        :param hide_null: Don't display data fields with null values or empty structures
+        :type hide_null: bool
+        :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
+        :type include: str
+        :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type limit: int
+        :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type offset: int
+        :param season_id: The unique identifier of the season
+        :type season_id: str
+        :param updated: Record was modified after this date/time. In UTC.
+        :type updated: datetime
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: SeasonPersonsListResponse
+        """
+        kwargs["_return_http_data_only"] = True
+        if "_preload_content" in kwargs:
+            raise ValueError(
+                "Error! Please call the season_person_list_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+            )
+        try:
+            return self.season_person_list_with_http_info(
+                organization_id,
+                person_id,
+                sport,
+                added,
+                external,
+                fields,
+                hide_null,
+                include,
+                limit,
+                offset,
+                season_id,
+                updated,
+                **kwargs
+            )  # noqa: E501
+        except Exception as e:
+            logger.error("Exception when calling SeasonPersonsApi->season_person_list: %s\n" % e)
+            raise
+
+    @validate_arguments
+    def season_person_list_with_http_info(
+        self,
+        organization_id: Annotated[
+            constr(strict=True, max_length=5, min_length=5),
+            Field(..., description="The unique identifier of the organization"),
+        ],
+        person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
+        sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        added: Annotated[
+            Optional[datetime], Field(description="Record was added after this date/time. In UTC.")
+        ] = None,
+        external: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
+            ),
+        ] = None,
+        fields: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information."
+            ),
+        ] = None,
+        hide_null: Annotated[
+            Optional[StrictBool], Field(description="Don't display data fields with null values or empty structures")
+        ] = None,
+        include: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information."
+            ),
+        ] = None,
+        limit: Annotated[
+            Optional[conint(strict=True, le=1000, ge=1)],
+            Field(
+                description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        offset: Annotated[
+            Optional[StrictInt],
+            Field(
+                description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        season_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the season")] = None,
+        updated: Annotated[
+            Optional[datetime], Field(description="Record was modified after this date/time. In UTC.")
+        ] = None,
+        **kwargs
+    ) -> ApiResponse:  # noqa: E501
+        """Get a list of seasons for person  # noqa: E501
+
+        Return a list of seasons that person participated in  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.season_person_list_with_http_info(organization_id, person_id, sport, added, external, fields, hide_null, include, limit, offset, season_id, updated, async_req=True)
+        >>> result = thread.get()
+
+        :param organization_id: The unique identifier of the organization (required)
+        :type organization_id: str
+        :param person_id: The unique identifier of the person (required)
+        :type person_id: str
+        :param sport: Sport name (required)
+        :type sport: str
+        :param added: Record was added after this date/time. In UTC.
+        :type added: datetime
+        :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
+        :type external: str
+        :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
+        :type fields: str
+        :param hide_null: Don't display data fields with null values or empty structures
+        :type hide_null: bool
+        :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
+        :type include: str
+        :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type limit: int
+        :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type offset: int
+        :param season_id: The unique identifier of the season
+        :type season_id: str
+        :param updated: Record was modified after this date/time. In UTC.
+        :type updated: datetime
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(SeasonPersonsListResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            "organization_id",
+            "person_id",
+            "sport",
+            "added",
+            "external",
+            "fields",
+            "hide_null",
+            "include",
+            "limit",
+            "offset",
+            "season_id",
+            "updated",
+        ]
+        _all_params.extend(
+            [
+                "async_req",
+                "_return_http_data_only",
+                "_preload_content",
+                "_request_timeout",
+                "_request_auth",
+                "_content_type",
+                "_headers",
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params["kwargs"].items():
+            if _key not in _all_params:
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method season_person_list" % _key)
+            _params[_key] = _val
+        del _params["kwargs"]
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params["organization_id"]:
+            _path_params["organizationId"] = _params["organization_id"]
+
+        if _params["person_id"]:
+            _path_params["personId"] = _params["person_id"]
+
+        if _params["sport"]:
+            _path_params["sport"] = _params["sport"]
+
+        # process the query parameters
+        _query_params = []
+        if _params.get("added") is not None:  # noqa: E501
+            if isinstance(_params["added"], datetime):
+                _query_params.append(
+                    ("added", _params["added"].strftime(self.api_client.configuration.datetime_format))
+                )
+            else:
+                _query_params.append(("added", _params["added"]))
+
+        if _params.get("external") is not None:  # noqa: E501
+            _query_params.append(("external", _params["external"]))
+
+        if _params.get("fields") is not None:  # noqa: E501
+            _query_params.append(("fields", _params["fields"]))
+
+        if _params.get("hide_null") is not None:  # noqa: E501
+            _query_params.append(("hideNull", _params["hide_null"]))
+
+        if _params.get("include") is not None:  # noqa: E501
+            _query_params.append(("include", _params["include"]))
+
+        if _params.get("limit") is not None:  # noqa: E501
+            _query_params.append(("limit", _params["limit"]))
+
+        if _params.get("offset") is not None:  # noqa: E501
+            _query_params.append(("offset", _params["offset"]))
+
+        if _params.get("season_id") is not None:  # noqa: E501
+            _query_params.append(("seasonId", _params["season_id"]))
+
+        if _params.get("updated") is not None:  # noqa: E501
+            if isinstance(_params["updated"], datetime):
+                _query_params.append(
+                    ("updated", _params["updated"].strftime(self.api_client.configuration.datetime_format))
+                )
+            else:
+                _query_params.append(("updated", _params["updated"]))
+
+        # process the header parameters
+        _header_params = dict(_params.get("_headers", {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ["OAuth2"]  # noqa: E501
+
+        _response_types_map = {
+            "200": "SeasonPersonsListResponse",
+        }
+
+        return self.api_client.call_api(
+            "/{sport}/o/{organizationId}/seasons/persons/{personId}",
+            "GET",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get("async_req"),
+            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
+            _preload_content=_params.get("_preload_content", True),
+            _request_timeout=_params.get("_request_timeout"),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get("_request_auth"),
+        )
+
+    @validate_arguments
     def season_persons_delete(
         self,
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
         person_id: Annotated[StrictStr, Field(..., description="The unique identifier of the person")],
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_roster_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_series_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_series_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/season_statistics_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/season_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/seasons_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/seasons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/sites_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/sites_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/standing_configurations_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/standing_configurations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/standings_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/standings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/transfers_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/transfers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/venues_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/venues_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api/video_streams_available_api.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api/video_streams_available_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api_client.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "AtriumSportsSDK/1.2.0"
+        self.user_agent = "AtriumSportsSDK/1.3.0"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/api_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/api_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/configuration.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         server_index=None,
         server_variables=None,
         server_operation_index=None,
         server_operation_variables=None,
         ssl_ca_cert=None,
     ):
         """Constructor"""
-        self._base_path = "https://api.dc.prod.cloud.atriumsports.com/v1" if host is None else host
+        self._base_path = "https://api.dc.connect.sportradar.com/v1" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -388,29 +388,29 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: v1\n"
-            "SDK Package Version: 1.2.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 1.3.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                "url": "https://api.dc.prod.cloud.atriumsports.com/v1",
+                "url": "https://api.dc.connect.sportradar.com/v1",
                 "description": "Production server",
             },
             {
-                "url": "https://api.dc.nonprod.cloud.atriumsports.com/v1",
+                "url": "https://api.dc.stg.connect-nonprod.sportradar.dev/v1",
                 "description": "NonProduction/Staging server",
             },
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/exceptions.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/__init__.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 # import models into model package
 from atriumsports.datacore.openapi.models.award_post_body import AwardPostBody
 from atriumsports.datacore.openapi.models.award_put_body import AwardPutBody
 from atriumsports.datacore.openapi.models.awards_model import AwardsModel
 from atriumsports.datacore.openapi.models.awards_model_organization import AwardsModelOrganization
 from atriumsports.datacore.openapi.models.awards_response import AwardsResponse
 from atriumsports.datacore.openapi.models.blank_model_response import BlankModelResponse
+from atriumsports.datacore.openapi.models.career_person_season_statistics_model import CareerPersonSeasonStatisticsModel
+from atriumsports.datacore.openapi.models.career_person_season_statistics_model_organization import (
+    CareerPersonSeasonStatisticsModelOrganization,
+)
+from atriumsports.datacore.openapi.models.career_person_season_statistics_response import (
+    CareerPersonSeasonStatisticsResponse,
+)
 from atriumsports.datacore.openapi.models.career_person_statistics_model import CareerPersonStatisticsModel
 from atriumsports.datacore.openapi.models.career_person_statistics_model_organization import (
     CareerPersonStatisticsModelOrganization,
 )
 from atriumsports.datacore.openapi.models.career_person_statistics_response import CareerPersonStatisticsResponse
 from atriumsports.datacore.openapi.models.change_log_model import ChangeLogModel
 from atriumsports.datacore.openapi.models.change_log_model_organization import ChangeLogModelOrganization
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/award_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/award_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/award_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/award_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/awards_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/awards_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/awards_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/awards_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/awards_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/awards_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/blank_model_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/blank_model_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/change_log_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/change_log_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/change_log_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/change_log_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/change_log_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/change_log_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_historical_name.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competition_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competition_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_model_league.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conduct_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conduct_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conference_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conference_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conference_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conference_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conferences_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conferences_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conferences_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conferences_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/conferences_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/conferences_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/contact_details.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/contact_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/division_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/division_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/division_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/division_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/divisions_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/divisions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/divisions_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/divisions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/divisions_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/divisions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entities_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_additional_details.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_address.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_address.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_group_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_group_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_groups_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_groups_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_groups_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_groups_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_historical_name.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/entity_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/entity_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/environmental_details.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/environmental_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/error_list_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/error_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/error_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/error_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_competitor.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entities_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_participant.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_participant.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_persons_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_roster_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_round.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_round.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_series.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_series.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/fixtures_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/fixtures_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_entity_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_entity_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_entity_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_person_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_person_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/game_log_person_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/game_log_person_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_identification.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_identification.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/images_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/images_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/included_data.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/included_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_criteria_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_criteria_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_summary_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leader_summary_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leader_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/league_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/league_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/league_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/league_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leagues_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leagues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leagues_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leagues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/leagues_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/leagues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organization_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organization_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organization_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organization_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organizations_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organizations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/organizations_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/organizations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_additional_details.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_historical_name.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_list_default_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_list_default_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/person_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/person_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/persons_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/persons_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/persons_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/pool_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/pool_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/pool_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/pool_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/ranking_rows_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/ranking_rows_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/response_links.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/response_links.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/response_meta_data.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/response_meta_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/role_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/role_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/role_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/role_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/roles_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/roles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/roles_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/roles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/roles_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/roles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/round_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/round_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/round_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/round_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_list_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_list_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entities_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_placings_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_placings_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_list_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_list_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_persons_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_pools_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_pools_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_pools_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_pools_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_roster_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_rounds_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_rounds_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_rounds_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_rounds_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_competitor.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_series_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_series_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stage_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stage_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stage_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stage_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stages_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stages_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_stages_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_stages_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_address.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/season_venues_list_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/season_venues_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_competition.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_competition.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/seasons_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/seasons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/series_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/series_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/series_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/series_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/site_address.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/site_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/site_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/site_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/site_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/site_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sites_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sites_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sites_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sites_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sites_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sites_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/social_media.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/social_media.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/sorting.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/sorting.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_building.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_building.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configuration.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_configurations_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_configurations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standing_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standing_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standings_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standings_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standings_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/standings_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/standings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/success_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/success_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/success_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/success_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfer_component.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfer_component.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfer_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfer_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfer_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfer_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfers_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfers_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfers_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/transfers_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/transfers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_address.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_historical_name.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venue_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venue_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_model_site.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/venues_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/venues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_file_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_file_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_download_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_download_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_download_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_download_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_files_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_files_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_local_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_local_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore/openapi/rest.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore/openapi/rest.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/datacore_stream/datacore_stream.py` & `atriumsports_sdk-1.3.0/atriumsports/datacore_stream/datacore_stream.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports/endpoints.py` & `atriumsports_sdk-1.3.0/atriumsports/endpoints.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/PKG-INFO` & `atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports-sdk
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.2.0/atriumsports_sdk.egg-info/SOURCES.txt` & `atriumsports_sdk-1.3.0/atriumsports_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 atriumsports/datacore/openapi/models/__init__.py
 atriumsports/datacore/openapi/models/award_post_body.py
 atriumsports/datacore/openapi/models/award_put_body.py
 atriumsports/datacore/openapi/models/awards_model.py
 atriumsports/datacore/openapi/models/awards_model_organization.py
 atriumsports/datacore/openapi/models/awards_response.py
 atriumsports/datacore/openapi/models/blank_model_response.py
+atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
+atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
+atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
 atriumsports/datacore/openapi/models/career_person_statistics_model.py
 atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
 atriumsports/datacore/openapi/models/career_person_statistics_response.py
 atriumsports/datacore/openapi/models/change_log_model.py
 atriumsports/datacore/openapi/models/change_log_model_organization.py
 atriumsports/datacore/openapi/models/change_log_response.py
 atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
```

### Comparing `atriumsports_sdk-1.2.0/setup.py` & `atriumsports_sdk-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     setuptools.setup(
         name="atriumsports_sdk",
-        version="1.2.0",
+        version="1.3.0",
         author="Atrium Sports",
         author_email="python_dev@atriumsports.com",
         description="Python module for integration to Atrium Sports APIs",
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=setuptools.find_packages(),
         classifiers=[
```

