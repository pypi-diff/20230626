# Comparing `tmp/dcicsnovault-8.2.0.1b40.tar.gz` & `tmp/dcicsnovault-8.2.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.2.0.1b40.tar", max compression
+gzip compressed data, was "dcicsnovault-8.2.0.1b5.tar", max compression
```

## Comparing `dcicsnovault-8.2.0.1b40.tar` & `dcicsnovault-8.2.0.1b5.tar`

### file list

```diff
@@ -1,184 +1,182 @@
--rw-r--r--   0        0        0     1135 2023-06-26 15:35:47.147458 dcicsnovault-8.2.0.1b40/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-06-26 15:35:47.147458 dcicsnovault-8.2.0.1b40/README.rst
--rw-r--r--   0        0        0     5610 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/pyproject.toml
--rw-r--r--   0        0        0     4907 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/aggregated_items.py
--rw-r--r--   0        0        0     9389 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/app.py
--rw-r--r--   0        0        0      358 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/appdefs.py
--rw-r--r--   0        0        0    11879 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/attachment.py
--rw-r--r--   0        0        0    26351 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/authentication.py
--rw-r--r--   0        0        0     4692 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6876 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     5839 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/list_db_tables.py
--rw-r--r--   0        0        0     6212 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     5155 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/prepare_template.py
--rw-r--r--   0        0        0     4350 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/custom_embed.py
--rw-r--r--   0        0        0     7282 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-06-26 15:35:47.155459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0    11485 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/indexing_views.py
--rw-r--r--   0        0        0     6889 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/common.py
--rw-r--r--   0        0        0     1294 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/exceptions.py
--rw-r--r--   0        0        0    26153 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_listener.py
--rw-r--r--   0        0        0      586 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_listener_base.py
--rw-r--r--   0        0        0      692 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_message.py
--rw-r--r--   0        0        0    12257 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_message_handler_decorator.py
--rw-r--r--   0        0        0     3760 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_message_handler_default.py
--rw-r--r--   0        0        0     1107 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_processor_decorator.py
--rw-r--r--   0        0        0      863 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_processors.py
--rw-r--r--   0        0        0     8586 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/ingestion/queue_utils.py
--rw-r--r--   0        0        0      774 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/jsonld_context.py
--rw-r--r--   0        0        0    32979 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/memlimit.py
--rw-r--r--   0        0        0      895 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/nginx-dev.conf
--rw-r--r--   0        0        0     1165 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/predicates.py
--rw-r--r--   0        0        0       98 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/project/access_key.py
--rw-r--r--   0        0        0     1520 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/project/authentication.py
--rw-r--r--   0        0        0      378 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/project/authorization.py
--rw-r--r--   0        0        0      289 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/project/ingestion.py
--rw-r--r--   0        0        0      228 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/project/loadxl.py
--rw-r--r--   0        0        0      107 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/project_app.py
--rw-r--r--   0        0        0      703 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/project_defs.py
--rw-r--r--   0        0        0       95 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22129 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/resource_views.py
--rw-r--r--   0        0        0    26761 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/resources.py
--rw-r--r--   0        0        0     9867 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/root.py
--rw-r--r--   0        0        0      986 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schema_formats.py
--rw-r--r--   0        0        0     3450 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schema_graph.py
--rw-r--r--   0        0        0    18330 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0     5407 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schemas/ingestion_submission.json
--rw-r--r--   0        0        0    18744 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/search/search.py
--rw-r--r--   0        0        0    17915 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/search/search_utils.py
--rw-r--r--   0        0        0     3944 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/server_defaults.py
--rw-r--r--   0        0        0     1020 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/server_defaults_user.py
--rw-r--r--   0        0        0      522 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/settings.py
--rw-r--r--   0        0        0     1769 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/sqlalchemy_tools.py
--rw-r--r--   0        0        0     1498 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-06-26 15:35:47.159459 dcicsnovault-8.2.0.1b40/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2191 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0        0 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/data/inserts/README.rst
--rw-r--r--   0        0        0        0 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/data/master-inserts/README.rst
--rw-r--r--   0        0        0     3086 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3186 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0     8173 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_ingestion_message_handler_decorator.py
--rw-r--r--   0        0        0      384 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_ingestion_processor.py
--rw-r--r--   0        0        0    28258 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     1291 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_util.py
--rw-r--r--   0        0        0    19246 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4620 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/types/__init__.py
--rw-r--r--   0        0        0     5132 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/types/access_key.py
--rw-r--r--   0        0        0     1169 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/types/acl.py
--rw-r--r--   0        0        0     8356 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/types/filter_set.py
--rw-r--r--   0        0        0    11559 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/types/ingestion.py
--rw-r--r--   0        0        0     5638 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-06-26 15:35:47.163459 dcicsnovault-8.2.0.1b40/snovault/upgrader.py
--rw-r--r--   0        0        0    63565 2023-06-26 15:35:47.167459 dcicsnovault-8.2.0.1b40/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-06-26 15:35:47.167459 dcicsnovault-8.2.0.1b40/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-06-26 15:35:47.167459 dcicsnovault-8.2.0.1b40/snovault/validators.py
--rw-r--r--   0        0        0     9183 1970-01-01 00:00:00.000000 dcicsnovault-8.2.0.1b40/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-06-01 19:10:13.202015 dcicsnovault-8.2.0.1b5/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-06-01 19:10:13.202015 dcicsnovault-8.2.0.1b5/README.rst
+-rw-r--r--   0        0        0     5609 2023-06-01 19:10:13.206015 dcicsnovault-8.2.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     4907 2023-06-01 19:10:13.206015 dcicsnovault-8.2.0.1b5/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     9389 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/app.py
+-rw-r--r--   0        0        0      358 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/appdefs.py
+-rw-r--r--   0        0        0    11879 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/attachment.py
+-rw-r--r--   0        0        0    26351 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/authentication.py
+-rw-r--r--   0        0        0     4692 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6876 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     5839 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/list_db_tables.py
+-rw-r--r--   0        0        0     6212 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     5155 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/prepare_template.py
+-rw-r--r--   0        0        0     4350 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7282 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0    11599 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/indexing_views.py
+-rw-r--r--   0        0        0     6889 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/common.py
+-rw-r--r--   0        0        0     1294 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/exceptions.py
+-rw-r--r--   0        0        0    26153 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener.py
+-rw-r--r--   0        0        0      586 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener_base.py
+-rw-r--r--   0        0        0      692 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message.py
+-rw-r--r--   0        0        0    12257 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_decorator.py
+-rw-r--r--   0        0        0     3760 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_default.py
+-rw-r--r--   0        0        0     1107 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processor_decorator.py
+-rw-r--r--   0        0        0      863 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processors.py
+-rw-r--r--   0        0        0     8586 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/queue_utils.py
+-rw-r--r--   0        0        0      774 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    32979 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/memlimit.py
+-rw-r--r--   0        0        0      895 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/nginx-dev.conf
+-rw-r--r--   0        0        0     1165 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/predicates.py
+-rw-r--r--   0        0        0     1520 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/authentication.py
+-rw-r--r--   0        0        0      378 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/authorization.py
+-rw-r--r--   0        0        0      289 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/ingestion.py
+-rw-r--r--   0        0        0      228 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/loadxl.py
+-rw-r--r--   0        0        0      107 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project_app.py
+-rw-r--r--   0        0        0      575 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project_defs.py
+-rw-r--r--   0        0        0       95 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/resource_views.py
+-rw-r--r--   0        0        0    26122 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/resources.py
+-rw-r--r--   0        0        0     9867 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/root.py
+-rw-r--r--   0        0        0      986 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_formats.py
+-rw-r--r--   0        0        0     3450 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_graph.py
+-rw-r--r--   0        0        0    18330 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0     5407 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/ingestion_submission.json
+-rw-r--r--   0        0        0    18744 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/search.py
+-rw-r--r--   0        0        0    17915 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4442 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/settings.py
+-rw-r--r--   0        0        0     1769 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/sqlalchemy_tools.py
+-rw-r--r--   0        0        0     1498 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2191 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/data/inserts/README.rst
+-rw-r--r--   0        0        0        0 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/data/master-inserts/README.rst
+-rw-r--r--   0        0        0     3086 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3186 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0     8173 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_ingestion_message_handler_decorator.py
+-rw-r--r--   0        0        0      384 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_ingestion_processor.py
+-rw-r--r--   0        0        0    28258 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    19246 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4620 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/access_key.py
+-rw-r--r--   0        0        0     8961 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/filter_set.py
+-rw-r--r--   0        0        0    11559 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/ingestion.py
+-rw-r--r--   0        0        0     5583 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/upgrader.py
+-rw-r--r--   0        0        0    63565 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/validators.py
+-rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 dcicsnovault-8.2.0.1b5/PKG-INFO
```

### Comparing `dcicsnovault-8.2.0.1b40/LICENSE.txt` & `dcicsnovault-8.2.0.1b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/README.rst` & `dcicsnovault-8.2.0.1b5/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/pyproject.toml` & `dcicsnovault-8.2.0.1b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.2.0.1b40"  # to become 8.2.0
+version = "8.2.0.1b5"  # to become 8.2.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/__init__.py` & `dcicsnovault-8.2.0.1b5/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/aggregated_items.py` & `dcicsnovault-8.2.0.1b5/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/app.py` & `dcicsnovault-8.2.0.1b5/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/attachment.py` & `dcicsnovault-8.2.0.1b5/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/authentication.py` & `dcicsnovault-8.2.0.1b5/snovault/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/authorization.py` & `dcicsnovault-8.2.0.1b5/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/batchupgrade.py` & `dcicsnovault-8.2.0.1b5/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/cache.py` & `dcicsnovault-8.2.0.1b5/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/calculated.py` & `dcicsnovault-8.2.0.1b5/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/check_rendering.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/es_index_data.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/list_db_tables.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/list_db_tables.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/load_access_keys.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/load_data.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/load_data_by_type.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/prepare_template.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/prepare_template.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/profile.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/purge_item_type.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/config.py` & `dcicsnovault-8.2.0.1b5/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/connection.py` & `dcicsnovault-8.2.0.1b5/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/crud_views.py` & `dcicsnovault-8.2.0.1b5/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/custom_embed.py` & `dcicsnovault-8.2.0.1b5/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/dev_servers.py` & `dcicsnovault-8.2.0.1b5/snovault/dev_servers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/drs.py` & `dcicsnovault-8.2.0.1b5/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/edw_hash.py` & `dcicsnovault-8.2.0.1b5/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/embed.py` & `dcicsnovault-8.2.0.1b5/snovault/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,63 +201,64 @@
     response = request.invoke_subrequest(subreq, use_tweens=False)
     if response.status_code >= 300:  # alas, the response from a pyramid subrequest has no .raise_for_status()
         raise HTTPServerError("Error obtaining object: %s" % object_id)
     object_json = response.json
     return object_json
 
 
-def subrequest_item_creation(request: pyramid.request.Request, item_type: str, json_body: dict = None) -> dict:
-    """
-    Acting as proxy on behalf of request, this creates a new item of the given item_type with attributes per json_body.
-
-    For example,
-
-        subrequest_item_creation(request=request, item_type='NobelPrize',
-                                 json_body={'category': 'peace', 'year': 2016))
-
-    Args:
-        request: the request on behalf of which this subrequest is done
-        item_type: the name of the item item type to be created
-        json_body: a python dictionary representing JSON containing data to use in initializing the newly created item
-
-    Returns:
-        a python dictionary (JSON description) of the item created
-
-    """
-
-    if json_body is None:
-        json_body = {}
-    collection_path = '/' + item_type
-    method = 'POST'
-    # json_utf8 = json.dumps(json_body).encode('utf-8')  # Unused, but here just in case
-    check_true(not request.remote_user, "request.remote_user has %s before we set it." % request.remote_user)
-    request.remote_user = 'EMBED'
-    subrequest = make_subrequest(request=request, path=collection_path, method=method, json_body=json_body)
-    subrequest.remote_user = 'EMBED'
-    subrequest.registry = request.registry
-    # Maybe...
-    # validated = json_body.copy()
-    # subrequest.validated = validated
-    registry: Registry = subrequest.registry  # noQA - PyCharm can't tell subrequest.registry IS a Registry
-    collection: Collection = registry[COLLECTIONS][item_type]
-    check_true(subrequest.json_body, "subrequest.json_body is not properly initialized.")
-    check_true(not subrequest.validated, "subrequest was unexpectedly validated already.")
-    check_true(not subrequest.errors, "subrequest.errors already has errors before trying to validate.")
-    check_true(subrequest.remote_user == request.remote_user,
-               "Mismatch: subrequest.remote_user=%r request.remote_user=%r"
-               % (subrequest.remote_user, request.remote_user))
-    validate_request(schema=collection.type_info.schema, request=subrequest, data=json_body)
-    if not subrequest.validated:
-        return {
-            "@type": ["Exception"],
-            "errors": subrequest.errors
-        }
-    else:
-        json_result: dict = sno_collection_add(context=collection, request=subrequest, render=False)
-        return json_result
+# Does not seemed to be used anywhere (dmichaels/2023-05-30) ...
+#def subrequest_item_creation(request: pyramid.request.Request, item_type: str, json_body: dict = None) -> dict:
+#    """
+#    Acting as proxy on behalf of request, this creates a new item of the given item_type with attributes per json_body.
+#
+#    For example,
+#
+#        subrequest_item_creation(request=request, item_type='NobelPrize',
+#                                 json_body={'category': 'peace', 'year': 2016))
+#
+#    Args:
+#        request: the request on behalf of which this subrequest is done
+#        item_type: the name of the item item type to be created
+#        json_body: a python dictionary representing JSON containing data to use in initializing the newly created item
+#
+#    Returns:
+#        a python dictionary (JSON description) of the item created
+#
+#    """
+#
+#    if json_body is None:
+#        json_body = {}
+#    collection_path = '/' + item_type
+#    method = 'POST'
+#    # json_utf8 = json.dumps(json_body).encode('utf-8')  # Unused, but here just in case
+#    check_true(not request.remote_user, "request.remote_user has %s before we set it." % request.remote_user)
+#    request.remote_user = 'EMBED'
+#    subrequest = make_subrequest(request=request, path=collection_path, method=method, json_body=json_body)
+#    subrequest.remote_user = 'EMBED'
+#    subrequest.registry = request.registry
+#    # Maybe...
+#    # validated = json_body.copy()
+#    # subrequest.validated = validated
+#    registry: Registry = subrequest.registry  # noQA - PyCharm can't tell subrequest.registry IS a Registry
+#    collection: Collection = registry[COLLECTIONS][item_type]
+#    check_true(subrequest.json_body, "subrequest.json_body is not properly initialized.")
+#    check_true(not subrequest.validated, "subrequest was unexpectedly validated already.")
+#    check_true(not subrequest.errors, "subrequest.errors already has errors before trying to validate.")
+#    check_true(subrequest.remote_user == request.remote_user,
+#               "Mismatch: subrequest.remote_user=%r request.remote_user=%r"
+#               % (subrequest.remote_user, request.remote_user))
+#    validate_request(schema=collection.type_info.schema, request=subrequest, data=json_body)
+#    if not subrequest.validated:
+#        return {
+#            "@type": ["Exception"],
+#            "errors": subrequest.errors
+#        }
+#    else:
+#        json_result: dict = sno_collection_add(context=collection, request=subrequest, render=False)
+#        return json_result
 
 
 class NullRenderer:
     '''Sets result value directly as response.
     '''
     def __init__(self, info):
         pass
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/etag.py` & `dcicsnovault-8.2.0.1b5/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/indexing_views.py` & `dcicsnovault-8.2.0.1b5/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/common.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/common.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/exceptions.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_listener.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_listener_base.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener_base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_message.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_message_handler_decorator.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_message_handler_default.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_default.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_processor_decorator.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processor_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/ingestion_processors.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processors.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/ingestion/queue_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/queue_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/interfaces.py` & `dcicsnovault-8.2.0.1b5/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/invalidation.py` & `dcicsnovault-8.2.0.1b5/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/json_renderer.py` & `dcicsnovault-8.2.0.1b5/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/jsongraph.py` & `dcicsnovault-8.2.0.1b5/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/jsonld_context.py` & `dcicsnovault-8.2.0.1b5/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/loadxl.py` & `dcicsnovault-8.2.0.1b5/snovault/loadxl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/memlimit.py` & `dcicsnovault-8.2.0.1b5/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/nginx-dev.conf` & `dcicsnovault-8.2.0.1b5/snovault/nginx-dev.conf`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/parallel.py` & `dcicsnovault-8.2.0.1b5/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/predicates.py` & `dcicsnovault-8.2.0.1b5/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/project/authentication.py` & `dcicsnovault-8.2.0.1b5/snovault/project/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/project_defs.py` & `dcicsnovault-8.2.0.1b5/snovault/project_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from dcicutils.project_utils import C4ProjectRegistry, C4Project
-from .project.access_key import SnovaultProjectAccessKey
 from .project.authentication import SnovaultProjectAuthentication
 from .project.authorization import SnovaultProjectAuthorization
 from .project.ingestion import SnovaultProjectIngestion
 
 
 @C4ProjectRegistry.register("dcicsnovault")
-class SnovaultProject(SnovaultProjectAccessKey,
-                      SnovaultProjectAuthentication,
+class SnovaultProject(SnovaultProjectAuthentication,
                       SnovaultProjectAuthorization,
                       SnovaultProjectIngestion,
-                      
                       C4Project):
     NAMES = {"NAME": "snovault", "PYPI_NAME": "dcicsnovault"}
     ACCESSION_PREFIX = "SNO"
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/redis/redis_connection.py` & `dcicsnovault-8.2.0.1b5/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/renderers.py` & `dcicsnovault-8.2.0.1b5/snovault/renderers.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
     # TransformWorker inits and manages a subprocess
     # it re-uses the subprocess so interestingly data in JS global variables
     # might persist in between renders (from different users, even).
     transform = TransformWorker(
         Response=Response,
         reload_process=reload_process,
         # Other kwargs, including env below, get passed down to subprocess.Popen
-        args=['node', resource_filename('encoded', 'static/build/renderer.js')],
+        args=['node', resource_filename(__name__, 'static/build/renderer.js')],
         env=node_env
     )
 
     def render_page_html_tween(request):
         # Result of downstream tweens. Body not yet transformed into HTML.
         response = handler(request)
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/resource_views.py` & `dcicsnovault-8.2.0.1b5/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/resources.py` & `dcicsnovault-8.2.0.1b5/snovault/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     Authenticated,
     principals_allowed_by_permission
 )
 from pyramid.traversal import (
     resource_path,
     traverse
 )
-from .server_defaults_user import get_userid
-from .types.acl import ONLY_ADMIN_VIEW_ACL
 from .calculated import (
     calculate_properties,
     calculated_property,
 )
 from .interfaces import (
     COLLECTIONS,
     CONNECTION,
@@ -356,14 +354,15 @@
 # schema definition, so we define it here to import & re-use.
 display_title_schema = {
     "title": "Display Title",
     "description": "A calculated title for every object",
     "type": "string",
 }
 
+
 class Item(Resource):
     """
     Base Item resource that corresponds to a Collection or AbstractCollection
     """
     item_type = None
     base_types = ['Item']
     name_key = None
@@ -371,30 +370,19 @@
     aggregated_items = {}
     embedded_list = []
     default_diff = []
     filtered_rev_statuses = ()
     schema = None
     AbstractCollection = AbstractCollection
     Collection = Collection
-    STATUS_ACL = {}  # note that this should ALWAYS be overridden by downstream application
 
     def __init__(self, registry, model):
         self.registry = registry
         self.model = model
 
-    def __acl__(self):
-        """This sets the ACL for the item based on mapping of status to ACL.
-           If there is no status or the status is not included in the STATUS_ACL
-           lookup then the access is set to admin only
-        """
-        # Don't finalize to avoid validation here.
-        properties = self.upgrade_properties().copy()
-        status = properties.get('status')
-        return self.STATUS_ACL.get(status, ONLY_ADMIN_VIEW_ACL)
-
     def __repr__(self):
         return '<%s at %s>' % (type(self).__name__, resource_path(self))
 
     @reify
     def type_info(self):
         return self.registry[TYPES][type(self)]
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/root.py` & `dcicsnovault-8.2.0.1b5/snovault/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schema_formats.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_formats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schema_graph.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schema_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schema_views.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schemas/access_key.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/access_key.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schemas/filter_set.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/filter_set.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schemas/ingestion_submission.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/ingestion_submission.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schemas/mixins.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/schemas/user.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/user.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/search/compound_search.py` & `dcicsnovault-8.2.0.1b5/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/search/lucene_builder.py` & `dcicsnovault-8.2.0.1b5/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/search/search.py` & `dcicsnovault-8.2.0.1b5/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/search/search_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/search/search_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/server_defaults.py` & `dcicsnovault-8.2.0.1b5/snovault/server_defaults.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import uuid
 
 from dcicutils.misc_utils import utc_now_str
 from jsonschema_serialize_fork import NO_DEFAULT
 from pyramid.path import DottedNameResolver
 from pyramid.threadlocal import get_current_request
 from snovault.schema_utils import server_default
-from .interfaces import COLLECTIONS  # , ROOT
+from snovault import COLLECTIONS  # , ROOT
 from string import digits  # , ascii_uppercase
 from .project_app import app_project
-from .server_defaults_user import _userid, get_userid, get_user_resource
 
 
 ACCESSION_FACTORY = __name__ + ':accession_factory'
 ACCESSION_PREFIX = app_project().ACCESSION_PREFIX
 ACCESSION_TEST_PREFIX = 'TST'
 
 
@@ -31,14 +30,22 @@
 
 
 @server_default
 def userid(instance, subschema):  # args required by jsonschema-serialize-fork
     return _userid()
 
 
+def _userid():
+    request = get_current_request()
+    for principal in request.effective_principals:
+        if principal.startswith('userid.'):
+            return principal[7:]
+    return NO_DEFAULT
+
+
 @server_default
 def now(instance, subschema):  # args required by jsonschema-serialize-fork
     return utc_now_str()
 
 
 @server_default
 def uuid4(instance, subschema):
@@ -57,14 +64,27 @@
         new_accession = factory(subschema['accessionType'])
         if new_accession in request.root:
             continue
         return new_accession
     raise AssertionError("Free accession not found in %d attempts" % ATTEMPTS)
 
 
+def get_userid():
+    """ Wrapper for the server_default 'userid' above so it is not called through SERVER_DEFAULTS in our code """
+    return _userid()
+
+
+def get_user_resource():
+    request = get_current_request()
+    userid_found = _userid()
+    if userid_found == NO_DEFAULT:
+        return NO_DEFAULT
+    return request.registry[COLLECTIONS]['user'][userid_found]
+
+
 def get_now():
     """ Wrapper for the server_default 'now' above so it is not called through SERVER_DEFAULTS in our code """
     return utc_now_str()
 
 
 def add_last_modified(properties, **kwargs):
     """
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/settings.py` & `dcicsnovault-8.2.0.1b5/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/sqlalchemy_tools.py` & `dcicsnovault-8.2.0.1b5/snovault/sqlalchemy_tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/standalone_dev.py` & `dcicsnovault-8.2.0.1b5/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/stats.py` & `dcicsnovault-8.2.0.1b5/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/storage.py` & `dcicsnovault-8.2.0.1b5/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/test_schemas/mixins.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/conftest.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/root.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/serverfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_attachment.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_authentication.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_calculated.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_drs.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_edw_hash.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_embedding.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_indexing.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_ingestion_message_handler_decorator.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_ingestion_message_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_key.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_link.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_logging.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_misc.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_schemas.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_stats.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_storage.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_upgrader.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_util.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/test_views.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/testappfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/testing_views.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tests/toolfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/tools.py` & `dcicsnovault-8.2.0.1b5/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/typedsheets.py` & `dcicsnovault-8.2.0.1b5/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/typeinfo.py` & `dcicsnovault-8.2.0.1b5/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/types/access_key.py` & `dcicsnovault-8.2.0.1b5/snovault/types/access_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Access_key types file."""
 
-import datetime
+from pyramid.view import view_config
 from pyramid.security import (
     Allow,
     Deny,
     Authenticated,
     Everyone,
 )
 from pyramid.settings import asbool
-from pyramid.view import view_config
+import datetime
+from .base import (
+    Item,
+    DELETED_ACL,
+    ONLY_ADMIN_VIEW_ACL,
+)
 from .. import (
     collection,
     load_schema,
 )
-from ..authentication import (
-    generate_password,
-    generate_user,
-    CRYPT_CONTEXT,
-)
 from ..crud_views import (
     collection_add,
     item_edit,
 )
-from ..project_app import app_project
 from ..validators import (
     validate_item_content_post,
 )
 from ..util import debug_log
-from .base import (
-    Item,
-    DELETED_ACL,
-    ONLY_ADMIN_VIEW_ACL,
+from ..authentication import (
+    generate_password,
+    generate_user,
+    CRYPT_CONTEXT,
 )
 
 
 @collection(
     name='access-keys',
+    unique_key='access_key:access_key_id',
     properties={
         'title': 'Access keys',
         'description': 'Programmatic access keys',
     },
     acl=[
         (Allow, Authenticated, 'add'),
         (Allow, 'group.admin', 'list'),
@@ -49,27 +49,27 @@
         (Deny, Everyone, 'list'),
     ])
 class AccessKey(Item):
     """AccessKey class."""
     ACCESS_KEY_EXPIRATION_TIME = 90  # days
     item_type = 'access_key'
     schema = load_schema('snovault:schemas/access_key.json')
+    name_key = 'access_key_id'
     embedded_list = []
 
     STATUS_ACL = {
         'current': [(Allow, 'role.owner', ['view', 'edit'])] + ONLY_ADMIN_VIEW_ACL,
         'deleted': DELETED_ACL,
     }
 
     @classmethod
     def create(cls, registry, uuid, properties, sheets=None):
         """ Sets the access key timeout 90 days from creation. """
-        if app_project().access_key_has_expiration_date():
-            properties['expiration_date'] = (datetime.datetime.utcnow() + datetime.timedelta(
-                days=cls.ACCESS_KEY_EXPIRATION_TIME)).isoformat()
+        properties['expiration_date'] = (datetime.datetime.utcnow() + datetime.timedelta(
+            days=cls.ACCESS_KEY_EXPIRATION_TIME)).isoformat()
         return super().create(registry, uuid, properties, sheets)
 
     def __ac_local_roles__(self):
         """grab and return user as owner."""
         owner = 'userid.%s' % self.properties['user']
         return {owner: 'role.owner'}
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/types/base.py` & `dcicsnovault-8.2.0.1b5/snovault/types/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     Everyone,
 )
 from pyramid.view import (
     view_config,
 )
 import re
 import string
-from typing import Any, List, Tuple, Union
 from .. import Item, Collection, AbstractCollection, abstract_collection, calculated_property
 from ..util import debug_log
 from ..validators import (
     validate_item_content_post,
     validate_item_content_put,
     validate_item_content_patch,
     validate_item_content_in_place,
@@ -24,20 +23,45 @@
     no_validate_item_content_patch
 )
 from ..crud_views import (
     collection_add as sno_collection_add,
     item_edit
 )
 from ..interfaces import CONNECTION
+from typing import Any, List, Tuple, Union
 from ..server_defaults import get_userid, add_last_modified
-from .acl import (
-    ONLY_ADMIN_VIEW_ACL,
-    PUBLIC_ACL,
-    DELETED_ACL
-)
+
+
+Acl = List[Tuple[Any, Any, Union[str, List[str]]]]
+
+# Item acls
+# TODO (C4-332): consolidate all acls into one place - i.e. their own file
+ONLY_ADMIN_VIEW_ACL: Acl = [
+    (Allow, 'group.admin', ['view', 'edit']),
+    (Allow, 'group.read-only-admin', ['view']),
+    (Allow, 'remoteuser.INDEXER', ['view']),
+    (Allow, 'remoteuser.EMBED', ['view']),
+    (Deny, Everyone, ['view', 'edit'])
+]
+
+
+PUBLIC_ACL: Acl = [
+    (Allow, Everyone, ['view']),
+] + ONLY_ADMIN_VIEW_ACL
+
+
+DELETED_ACL: Acl = [
+    (Deny, Everyone, 'visible_for_edit')
+] + ONLY_ADMIN_VIEW_ACL
+
+
+# Used for 'draft' status
+ALLOW_OWNER_EDIT: Acl = [
+    (Allow, 'role.owner', ['view', 'edit']),
+] + ONLY_ADMIN_VIEW_ACL
 
 
 def get_item_or_none(request, value, itype=None, frame='object'):
     """
     Return the view of an item with given frame. Can specify different types
     of `value` for item lookup
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/types/filter_set.py` & `dcicsnovault-8.2.0.1b5/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/types/ingestion.py` & `dcicsnovault-8.2.0.1b5/snovault/types/ingestion.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/types/user.py` & `dcicsnovault-8.2.0.1b5/snovault/types/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,20 @@
 
 
 USER_PAGE_VIEW_ATTRIBUTES = ['@id', '@type', 'uuid', 'title', 'display_title']
 
 
 @view_config(context=User, permission='view', request_method='GET', name='page')
 @debug_log
-def user_page_view(context, request, user_page_view_attributes = USER_PAGE_VIEW_ATTRIBUTES):
+def user_page_view(context, request):
     """smth."""
     properties = item_view_page(context, request)
     if not request.has_permission('view_details'):
         filtered = {}
-        for key in user_page_view_attributes:
+        for key in USER_PAGE_VIEW_ATTRIBUTES:
             try:
                 filtered[key] = properties[key]
             except KeyError:
                 pass
         return filtered
     return properties
```

### Comparing `dcicsnovault-8.2.0.1b40/snovault/upgrader.py` & `dcicsnovault-8.2.0.1b5/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/util.py` & `dcicsnovault-8.2.0.1b5/snovault/util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/validation.py` & `dcicsnovault-8.2.0.1b5/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/snovault/validators.py` & `dcicsnovault-8.2.0.1b5/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b40/PKG-INFO` & `dcicsnovault-8.2.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.2.0.1b40
+Version: 8.2.0.1b5
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
```

