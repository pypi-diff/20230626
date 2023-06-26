# Comparing `tmp/summa_embed-0.17.2.tar.gz` & `tmp/summa_embed-0.17.3.tar.gz`

## Comparing `summa_embed-0.17.2.tar` & `summa_embed-0.17.3.tar`

### file list

```diff
@@ -1,127 +1,125 @@
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 summa_embed-0.17.2/local_dependencies/summa-core/Cargo.toml
--rw-rw-r--   0     1000     1000     1050 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/LICENSE
--rw-rw-r--   0     1000     1000   370551 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/dictionaries/drugs.csv
--rw-rw-r--   0     1000     1000       92 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/collectors/mod.rs
--rw-rw-r--   0     1000     1000     7233 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-rw-r--   0     1000     1000     2107 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-rw-r--   0     1000     1000     5297 2023-06-11 15:20:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-rw-r--   0     1000     1000     1021 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/driver.rs
--rw-rw-r--   0     1000     1000    13794 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-rw-r--   0     1000     1000    24321 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_holder.rs
--rw-rw-r--   0     1000     1000    13903 2023-06-14 08:03:09.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_registry.rs
--rw-rw-r--   0     1000     1000    14323 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-rw-r--   0     1000     1000     1694 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-rw-r--   0     1000     1000      144 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-rw-r--   0     1000     1000     2045 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-rw-r--   0     1000     1000     5057 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/mod.rs
--rw-rw-r--   0     1000     1000     4711 2023-06-01 07:26:24.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-rw-r--   0     1000     1000       54 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-rw-r--   0     1000     1000      239 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-rw-r--   0     1000     1000      615 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
--rw-rw-r--   0     1000     1000     1376 2023-06-11 17:57:08.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/english_nn.rs
--rw-rw-r--   0     1000     1000      847 2023-06-11 17:57:08.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
--rw-rw-r--   0     1000     1000     2131 2023-06-11 14:16:30.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
--rw-rw-r--   0     1000     1000    15903 2023-06-11 14:05:01.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-rw-r--   0     1000     1000     1695 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-rw-r--   0     1000     1000    64254 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-rw-r--   0     1000     1000     6095 2023-06-13 12:10:55.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-rw-r--   0     1000     1000     1039 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/utils.rs
--rw-rw-r--   0     1000     1000     2216 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-rw-r--   0     1000     1000     1901 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-rw-r--   0     1000     1000    11274 2023-06-01 07:26:30.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_document.rs
--rw-rw-r--   0     1000     1000     7462 2023-06-11 14:08:38.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-rw-r--   0     1000     1000     2162 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-rw-r--   0     1000     1000     4680 2023-06-13 08:40:32.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/core.rs
--rw-rw-r--   0     1000     1000     3512 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-rw-r--   0     1000     1000      383 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/mod.rs
--rw-rw-r--   0     1000     1000     3335 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-rw-r--   0     1000     1000     8009 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-rw-r--   0     1000     1000     8014 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-rw-r--   0     1000     1000     7015 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-rw-r--   0     1000     1000     5258 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-rw-r--   0     1000     1000    17667 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-rw-r--   0     1000     1000     2255 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/mod.rs
--rw-rw-r--   0     1000     1000     6756 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-rw-r--   0     1000     1000     5192 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/errors.rs
--rw-rw-r--   0     1000     1000     2421 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-rw-r--   0     1000     1000      742 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/lib.rs
--rw-rw-r--   0     1000     1000     1471 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-rw-r--   0     1000     1000      960 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/label.rs
--rw-rw-r--   0     1000     1000       92 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/mod.rs
--rw-rw-r--   0     1000     1000      583 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/page_rank.rs
--rw-rw-r--   0     1000     1000     5474 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-rw-r--   0     1000     1000     2294 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-rw-r--   0     1000     1000     1068 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-rw-r--   0     1000     1000      323 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-rw-r--   0     1000     1000      662 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-rw-r--   0     1000     1000      582 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-rw-r--   0     1000     1000      411 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-rw-r--   0     1000     1000     2048 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-rw-r--   0     1000     1000     1538 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-rw-r--   0     1000     1000      826 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-rw-r--   0     1000     1000      218 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/mod.rs
--rw-rw-r--   0     1000     1000      480 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-rw-r--   0     1000     1000     7908 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-rw-r--   0     1000     1000      415 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/utils/mod.rs
--rw-rw-r--   0     1000     1000      309 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/utils/random.rs
--rw-rw-r--   0     1000     1000     3165 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/utils/sync.rs
--rw-rw-r--   0     1000     1000      450 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.2/local_dependencies/summa-server/Cargo.toml
--rw-rw-r--   0     1000     1000       43 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/.cargo/config.toml
--rw-rw-r--   0     1000     1000     1050 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/LICENSE
--rw-rw-r--   0     1000     1000     2832 2023-05-29 14:03:22.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/consumer.rs
--rw-rw-r--   0     1000     1000    13111 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/index.rs
--rw-rw-r--   0     1000     1000      105 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/mod.rs
--rw-rw-r--   0     1000     1000     2909 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/reflection.rs
--rw-rw-r--   0     1000     1000     1278 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/search.rs
--rw-rw-r--   0     1000     1000      783 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/bin/main.rs
--rw-rw-r--   0     1000     1000     5186 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumer_manager.rs
--rw-rw-r--   0     1000     1000      813 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
--rw-rw-r--   0     1000     1000     1082 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/dummy.rs
--rw-rw-r--   0     1000     1000    12123 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
--rw-rw-r--   0     1000     1000       84 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
--rw-rw-r--   0     1000     1000      532 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
--rw-rw-r--   0     1000     1000      155 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/mod.rs
--rw-rw-r--   0     1000     1000     3811 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/index_meter.rs
--rw-rw-r--   0     1000     1000      258 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/mod.rs
--rw-rw-r--   0     1000     1000      943 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/api.rs
--rw-rw-r--   0     1000     1000      919 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/consumer.rs
--rw-rw-r--   0     1000     1000      434 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/metrics.rs
--rw-rw-r--   0     1000     1000      116 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/mod.rs
--rw-rw-r--   0     1000     1000     3994 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/server.rs
--rw-rw-r--   0     1000     1000      991 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/store.rs
--rw-rw-r--   0     1000     1000     3459 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/errors.rs
--rw-rw-r--   0     1000     1000     1427 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/lib.rs
--rw-rw-r--   0     1000     1000     3681 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/logging.rs
--rw-rw-r--   0     1000     1000    15747 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/server.rs
--rw-rw-r--   0     1000     1000     7716 2023-06-01 07:26:30.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/api.rs
--rw-rw-r--   0     1000     1000    40405 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/index.rs
--rw-rw-r--   0     1000     1000     5174 2023-05-29 14:03:22.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/metrics.rs
--rw-rw-r--   0     1000     1000      287 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/mod.rs
--rw-rw-r--   0     1000     1000     2108 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/utils/mod.rs
--rw-rw-r--   0     1000     1000      923 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/utils/thread_handler.rs
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.2/local_dependencies/summa-proto/Cargo.toml
--rw-rw-r--   0     1000     1000     1050 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/LICENSE
--rw-rw-r--   0     1000     1000     2381 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-proto/build.rs
--rwxrwxr-x   0     1000     1000      244 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/gen-docs.sh
--rw-rw-r--   0     1000     1000     2561 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/markdown.tmpl
--rw-rw-r--   0     1000     1000        0 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/__init__.py
--rw-rw-r--   0     1000     1000     1556 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-rw-r--   0     1000     1000      393 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-rw-r--   0     1000     1000    10274 2023-06-13 08:40:32.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/index_service.proto
--rw-rw-r--   0     1000     1000     7871 2023-06-13 08:40:32.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/query.proto
--rw-rw-r--   0     1000     1000      499 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-rw-r--   0     1000     1000      867 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/search_service.proto
--rw-rw-r--   0     1000     1000      407 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/unixfs.proto
--rw-rw-r--   0     1000     1000       96 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/utils.proto
--rw-rw-r--   0     1000     1000     2523 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/lib.rs
--rw-rw-r--   0     1000     1000     2683 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-rw-r--   0     1000     1000      212 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-rw-r--   0     1000     1000      394 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-rw-r--   0     1000     1000      613 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.2/Cargo.toml
--rw-rw-r--   0     1000     1000      685 2023-05-29 09:11:14.000000 summa_embed-0.17.2/.gitignore
--rw-rw-r--   0     1000     1000      400 2023-06-16 10:18:53.000000 summa_embed-0.17.2/pyproject.toml
--rw-rw-r--   0     1000     1000     2220 2023-06-16 10:18:53.000000 summa_embed-0.17.2/src/lib.rs
--rw-rw-r--   0     1000     1000   116194 2023-06-16 10:19:02.000000 summa_embed-0.17.2/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.2/PKG-INFO
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.3/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20   370551 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-r--r--   0      501       20       92 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7233 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5492 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20    13820 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    31266 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13903 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    20309 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5962 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     6539 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      250 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20     1193 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-r--r--   0      501       20      693 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-r--r--   0      501       20     2092 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-r--r--   0      501       20    13740 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1899 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    67734 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     5812 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     2498 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-r--r--   0      501       20     2216 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11998 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7462 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     4680 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8015 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      559 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.3/local_dependencies/summa-server/Cargo.toml
+-rw-r--r--   0      501       20       43 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/.cargo/config.toml
+-rw-r--r--   0      501       20     1050 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/LICENSE
+-rw-r--r--   0      501       20     2832 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/consumer.rs
+-rw-r--r--   0      501       20    13268 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/index.rs
+-rw-r--r--   0      501       20      105 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/mod.rs
+-rw-r--r--   0      501       20     2909 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/reflection.rs
+-rw-r--r--   0      501       20     1278 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/search.rs
+-rw-r--r--   0      501       20      783 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/bin/main.rs
+-rw-r--r--   0      501       20     5305 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumer_manager.rs
+-rw-r--r--   0      501       20      813 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
+-rw-r--r--   0      501       20     1082 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/dummy.rs
+-rw-r--r--   0      501       20    11633 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
+-rw-r--r--   0      501       20      270 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
+-rw-r--r--   0      501       20      532 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
+-rw-r--r--   0      501       20      155 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/mod.rs
+-rw-r--r--   0      501       20     3811 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/index_meter.rs
+-rw-r--r--   0      501       20      258 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/mod.rs
+-rw-r--r--   0      501       20      943 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/api.rs
+-rw-r--r--   0      501       20      919 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/consumer.rs
+-rw-r--r--   0      501       20      434 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/metrics.rs
+-rw-r--r--   0      501       20      116 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/mod.rs
+-rw-r--r--   0      501       20     3994 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/server.rs
+-rw-r--r--   0      501       20      991 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/store.rs
+-rw-r--r--   0      501       20     3459 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/errors.rs
+-rw-r--r--   0      501       20     1427 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/lib.rs
+-rw-r--r--   0      501       20     3681 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/logging.rs
+-rw-r--r--   0      501       20    15704 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/server.rs
+-rw-r--r--   0      501       20     8110 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/api.rs
+-rw-r--r--   0      501       20    40378 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/index.rs
+-rw-r--r--   0      501       20     5174 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/metrics.rs
+-rw-r--r--   0      501       20      287 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/mod.rs
+-rw-r--r--   0      501       20     2108 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/utils/mod.rs
+-rw-r--r--   0      501       20      923 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/utils/thread_handler.rs
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.3/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2381 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10641 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7871 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.3/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-06-26 09:16:47.000000 summa_embed-0.17.3/.gitignore
+-rw-r--r--   0      501       20      400 2023-06-26 09:16:47.000000 summa_embed-0.17.3/pyproject.toml
+-rw-r--r--   0      501       20     2199 2023-06-26 09:16:47.000000 summa_embed-0.17.3/src/lib.rs
+-rw-r--r--   0      501       20   104388 2023-06-26 09:16:57.000000 summa_embed-0.17.3/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.3/PKG-INFO
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.3/local_dependencies/summa-core/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [package]
 name = "summa-core"
-version = "0.17.2"
+version = "0.17.3"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
 path = "src/lib.rs"
 doc = true
 
 [features]
 fs = ["tantivy/mmap", "tokio/fs"]
 hyper-external-request = ["hyper", "hyper-tls"]
 metrics = ["opentelemetry"]
-nn = ["rust-bert"]
 tokio-rt = ["tokio/rt"]
 
 [dependencies]
 anyhow = "1.0"
 async-trait = "0.1"
 base64 = "0.21"
 bytes = "1.3"
+chrono = "0.4"
 config = "0.13"
 derive_builder = "0.12"
 downcast-rs = "1.2"
 fasteval2 = { version = "2.1.1", features = ["unsafe-vars"] }
 futures = "0.3"
 hyper = { version = "0.14", default_features = false, features = ["client", "http1", "http2", "tcp"] , optional = true }
 hyper-tls = { version = "0.5.0", features = ["vendored"] , optional = true }
@@ -39,15 +39,14 @@
 pest = "2.5"
 pest_derive = "2.5"
 pluralize-rs = "0.1"
 prost = "0.11"
 rand = { version = "0.8", features = ["small_rng"] }
 rayon = "1.6.1"
 regex = "1.8"
-rust-bert = { version = "0.21", optional = true }
 rustc-hash = "1.1.0"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_bytes = "0.11"
 serde_cbor = "0.11"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
 strfmt = "0.2"
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.3/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/dictionaries/drugs.csv` & `summa_embed-0.17.3/local_dependencies/summa-core/dictionaries/drugs.csv`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use tantivy::tokenizer::{LowerCaser, RawTokenizer, RemoveLongFilter, SimpleTokenizer, StopWordFilter, TextAnalyzer};
+use tantivy::tokenizer::{LowerCaser, RawTokenizer, RemoveLongFilter, SimpleTokenizer, StopWordFilter, TextAnalyzer, WhitespaceTokenizer};
 
 use super::summa_tokenizer::SummaTokenizer;
 
 /// List of stop words mixed for multiple languages
-const STOP_WORDS: [&str; 318] = [
+pub const STOP_WORDS: [&str; 318] = [
     "a",
     "an",
     "and",
     "are",
     "as",
     "at",
     "be",
@@ -321,30 +321,32 @@
     "ya",
     "o",
     "este",
     "sí",
 ];
 
 /// Instantiate default tokenizers
-pub fn default_tokenizers() -> [(String, TextAnalyzer); 4] {
+pub fn default_tokenizers() -> [(String, TextAnalyzer); 5] {
     let summa_tokenizer = TextAnalyzer::builder(SummaTokenizer)
         .filter(RemoveLongFilter::limit(100))
         .filter(LowerCaser)
         .filter(StopWordFilter::remove(STOP_WORDS.map(String::from).to_vec()))
         .build();
     let summa_without_stop_words_tokenizer = TextAnalyzer::builder(SummaTokenizer)
         .filter(RemoveLongFilter::limit(100))
         .filter(LowerCaser)
         .build();
     let default_tokenizer = TextAnalyzer::builder(SimpleTokenizer::default())
         .filter(RemoveLongFilter::limit(100))
         .filter(LowerCaser)
         .filter(StopWordFilter::remove(STOP_WORDS.map(String::from).to_vec()))
         .build();
+    let whitespace_tokenizer = TextAnalyzer::builder(WhitespaceTokenizer::default()).filter(LowerCaser).build();
     let raw_tokenizer = TextAnalyzer::builder(RawTokenizer::default()).filter(LowerCaser).build();
     [
         ("summa".to_owned(), summa_tokenizer),
         ("summa_without_stop_words".to_owned(), summa_without_stop_words_tokenizer),
         ("default".to_owned(), default_tokenizer),
         ("raw".to_owned(), raw_tokenizer),
+        ("whitespace".to_owned(), whitespace_tokenizer),
     ]
 }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     collector_proto: proto::Collector,
     query: &dyn Query,
     multi_collector: &mut MultiCollector,
 ) -> SummaResult<Box<dyn FruitExtractor>> {
     match collector_proto.collector {
         Some(proto::collector::Collector::TopDocs(top_docs_collector_proto)) => {
             let query_fields = validators::parse_fields(searcher.schema(), &top_docs_collector_proto.fields)?;
-            let query_fields = (!query_fields.is_empty()).then(|| HashSet::from_iter(query_fields.into_iter()));
+            let query_fields = (!query_fields.is_empty()).then(|| HashSet::from_iter(query_fields.into_iter().map(|x| x.0)));
             Ok(match top_docs_collector_proto.scorer {
                 None | Some(proto::Scorer { scorer: None }) => Box::new(
                     TopDocsBuilder::default()
                         .handle(multi_collector.add_collector(tantivy::collector::TopDocs::with_limit(
                             (top_docs_collector_proto.offset + top_docs_collector_proto.limit + 1) as usize,
                         )))
                         .index_alias(index_alias.to_string())
@@ -174,15 +174,15 @@
                             .build()?,
                     ) as Box<dyn FruitExtractor>
                 }
             })
         }
         Some(proto::collector::Collector::ReservoirSampling(reservoir_sampling_collector_proto)) => {
             let query_fields = validators::parse_fields(searcher.schema(), &reservoir_sampling_collector_proto.fields)?;
-            let query_fields = (!query_fields.is_empty()).then(|| HashSet::from_iter(query_fields.into_iter()));
+            let query_fields = (!query_fields.is_empty()).then(|| HashSet::from_iter(query_fields.into_iter().map(|x| x.0)));
             let reservoir_sampling_collector = collectors::ReservoirSampling::with_limit(reservoir_sampling_collector_proto.limit as usize);
             Ok(Box::new(
                 ReservoirSamplingBuilder::default()
                     .handle(multi_collector.add_collector(reservoir_sampling_collector))
                     .index_alias(index_alias.to_string())
                     .searcher(searcher)
                     .multi_fields(index_holder.multi_fields().clone())
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files 25% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 use tracing::{error, info, warn};
 use tracing::{instrument, trace};
 
 use super::SummaSegmentAttributes;
 use super::{build_fruit_extractor, default_tokenizers, FruitExtractor, ProtoQueryParser};
 use crate::components::fruit_extractors::IntermediateExtractionResult;
 use crate::components::segment_attributes::SegmentAttributesMergerImpl;
-use crate::components::{Driver, IndexWriterHolder, SummaDocument};
+use crate::components::{IndexWriterHolder, SummaDocument};
 use crate::configs::ConfigProxy;
 use crate::directories::{CachingDirectory, ExternalRequest, ExternalRequestGenerator, FileStats, HotDirectory, NetworkDirectory, StaticDirectoryCache};
-use crate::errors::SummaResult;
+use crate::errors::{SummaResult, ValidationError};
 use crate::proto_traits::Wrapper;
 use crate::Error;
 
 pub struct IndexHolder {
     index_engine_config: Arc<dyn ConfigProxy<proto::IndexEngineConfig>>,
     index_name: String,
     index: Index,
@@ -46,15 +46,14 @@
     cached_multi_fields: HashSet<Field>,
     index_reader: IndexReader,
     index_writer_holder: Option<Arc<RwLock<IndexWriterHolder>>>,
     query_parser: ProtoQueryParser,
     /// Counters
     #[cfg(feature = "metrics")]
     search_times_meter: Histogram<f64>,
-    driver: Driver,
 }
 
 impl Hash for IndexHolder {
     fn hash<H: Hasher>(&self, state: &mut H) {
         self.index_name.hash(state)
     }
 }
@@ -91,15 +90,15 @@
             .finish()
     }
 }
 
 /// Sets up standard Summa tokenizers
 ///
 /// The set of tokenizers includes standard Tantivy tokenizers as well as `SummaTokenizer` that supports CJK
-fn register_default_tokenizers(index: &Index) {
+pub fn register_default_tokenizers(index: &Index) {
     for (tokenizer_name, tokenizer) in &default_tokenizers() {
         index.tokenizers().register(tokenizer_name, tokenizer.clone())
     }
 }
 
 /// Cleanup after index deletion
 ///
@@ -157,15 +156,14 @@
     pub fn create_holder(
         core_config: &crate::configs::core::Config,
         mut index: Index,
         index_name: &str,
         index_engine_config: Arc<dyn ConfigProxy<proto::IndexEngineConfig>>,
         merge_policy: Option<proto::MergePolicy>,
         query_parser_config: proto::QueryParserConfig,
-        driver: Driver,
     ) -> SummaResult<IndexHolder> {
         register_default_tokenizers(&index);
 
         index.settings_mut().docstore_compress_threads = core_config.doc_store_compress_threads;
         index.set_segment_attributes_merger(Arc::new(SegmentAttributesMergerImpl::<SummaSegmentAttributes>::new()));
 
         let metas = index.load_metas()?;
@@ -216,15 +214,14 @@
             index_writer_holder,
             #[cfg(feature = "metrics")]
             search_times_meter: global::meter("summa")
                 .f64_histogram("search_times")
                 .with_unit(Unit::new("seconds"))
                 .with_description("Search times")
                 .init(),
-            driver,
         })
     }
 
     /// Creates index and sets it up via `setup`
     #[instrument(skip_all)]
     pub fn create_memory_index(index_builder: IndexBuilder) -> SummaResult<Index> {
         let index = index_builder.create_in_ram()?;
@@ -344,24 +341,29 @@
 
     /// Load term dictionaries into memory
     pub async fn partial_warmup<T: AsRef<str>>(&self, load_dictionaries: bool, fields: &[T]) -> SummaResult<()> {
         let searcher = self.index_reader().searcher();
         let mut warm_up_futures = Vec::new();
         let default_fields = fields
             .iter()
-            .map(|field_name| self.cached_schema.get_field(field_name.as_ref()))
-            .collect::<Result<Vec<_>, _>>()?;
+            .map(|field_name| {
+                self.cached_schema
+                    .find_field(field_name.as_ref())
+                    .map(|x| x.0)
+                    .ok_or_else(|| ValidationError::MissingField(field_name.as_ref().to_string()))
+            })
+            .collect::<Result<HashSet<_>, _>>()?;
         for field in default_fields {
             for segment_reader in searcher.segment_readers() {
                 let inverted_index = segment_reader.inverted_index_async(field).await?.clone();
                 if load_dictionaries {
                     warm_up_futures.push(async move {
                         let dict = inverted_index.terms();
                         info!(action = "warming_up_dictionary", index_name = ?self.index_name());
-                        dict.warm_up_dictionary().await
+                        dict.warm_up_dictionary_async().await
                     });
                 }
             }
         }
         info!(action = "warming_up");
         try_join_all(warm_up_futures).await?;
         Ok(())
@@ -479,18 +481,18 @@
     /// `IndexUpdater` bounds unbounded `SummaDocument` inside
     pub async fn index_document(&self, document: SummaDocument<'_>) -> SummaResult<()> {
         let document = document.bound_with(&self.index.schema()).try_into()?;
         self.index_writer_holder()?.read().await.index_document(document, self.conflict_strategy())
     }
 
     /// Index multiple documents at a time
-    pub async fn index_bulk(&self, documents: &Vec<Vec<u8>>) -> SummaResult<(u64, u64)> {
+    pub async fn index_bulk(&self, documents: &Vec<Vec<u8>>, conflict_strategy: Option<proto::ConflictStrategy>) -> SummaResult<(u64, u64)> {
         let (mut success_docs, mut failed_docs) = (0u64, 0u64);
         let index_writer_holder = self.index_writer_holder()?.read().await;
-        let conflict_strategy = self.conflict_strategy();
+        let conflict_strategy = conflict_strategy.unwrap_or_else(|| self.conflict_strategy());
         for document in documents {
             match SummaDocument::UnboundJsonBytes(document)
                 .bound_with(&self.index.schema())
                 .try_into()
                 .and_then(|document| index_writer_holder.index_document(document, conflict_strategy))
             {
                 Ok(_) => success_docs += 1,
@@ -547,35 +549,38 @@
 }
 
 #[cfg(test)]
 pub mod tests {
     use std::error::Error;
     use std::sync::Arc;
 
+    use serde_json::json;
     use summa_proto::proto;
     use summa_proto::proto::ConflictStrategy;
-    use tantivy::collector::Count;
-    use tantivy::query::TermQuery;
+    use tantivy::collector::{Count, TopDocs};
+    use tantivy::query::{AllQuery, TermQuery};
     use tantivy::schema::IndexRecordOption;
     use tantivy::{doc, Document, IndexBuilder, Term};
 
+    use crate::components::index_holder::register_default_tokenizers;
     use crate::components::test_utils::{create_test_schema, generate_documents};
     use crate::components::IndexWriterHolder;
     use crate::configs::core::WriterThreads;
 
     #[test]
     fn test_deletes() -> Result<(), Box<dyn Error>> {
         let schema = create_test_schema();
         let index = IndexBuilder::new()
             .schema(schema.clone())
             .index_attributes(proto::IndexAttributes {
                 unique_fields: vec!["id".to_string()],
                 ..Default::default()
             })
             .create_in_ram()?;
+        register_default_tokenizers(&index);
         let mut index_writer_holder = IndexWriterHolder::create(
             &index,
             WriterThreads::N(12),
             1024 * 1024 * 1024,
             Arc::new(tantivy::merge_policy::LogMergePolicy::default()),
         )?;
         let mut last_document = None;
@@ -603,8 +608,175 @@
         let counter = searcher.search(
             &TermQuery::new(Term::from_field_i64(schema.get_field("id").unwrap(), id), IndexRecordOption::WithFreqs),
             &Count,
         )?;
         assert_eq!(counter, 1);
         Ok(())
     }
+
+    #[test]
+    fn test_mapped_fields() -> Result<(), Box<dyn Error>> {
+        let schema = create_test_schema();
+        let metadata_field = schema.get_field("metadata").expect("no field");
+        let tags_field = schema.get_field("tags").expect("no field");
+        let title_field = schema.get_field("title").expect("no field");
+        let extra_field = schema.get_field("extra").expect("no field");
+        let index = IndexBuilder::new()
+            .schema(schema.clone())
+            .index_attributes(proto::IndexAttributes {
+                mapped_fields: vec![
+                    proto::MappedField {
+                        source_field: "metadata.isbn".to_string(),
+                        target_field: "extra".to_string(),
+                    },
+                    proto::MappedField {
+                        source_field: "tags".to_string(),
+                        target_field: "extra".to_string(),
+                    },
+                    proto::MappedField {
+                        source_field: "title".to_string(),
+                        target_field: "extra".to_string(),
+                    },
+                ],
+                ..Default::default()
+            })
+            .create_in_ram()?;
+        register_default_tokenizers(&index);
+        let mut index_writer_holder = IndexWriterHolder::create(
+            &index,
+            WriterThreads::N(12),
+            1024 * 1024 * 1024,
+            Arc::new(tantivy::merge_policy::LogMergePolicy::default()),
+        )?;
+        index_writer_holder.index_document(
+            doc!(
+                title_field => "Hitchhiker's guide",
+                metadata_field => json!({"isbn": ["100", "200", "300", "500", "600"], "another_title": "Super Title"}),
+                tags_field => "reality",
+            ),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.index_document(
+            doc!(
+                title_field => "Envy of the Stars",
+                metadata_field => json!({"isbn": "500"}),
+                tags_field => "scifi",
+                tags_field => "novel",
+            ),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.commit()?;
+        let reader = index.reader()?;
+        reader.reload()?;
+        let searcher = reader.searcher();
+        let docs = searcher
+            .search(
+                &TermQuery::new(Term::from_field_text(extra_field, "500"), IndexRecordOption::Basic),
+                &TopDocs::with_limit(10),
+            )?
+            .into_iter()
+            .map(|x| {
+                searcher
+                    .doc(x.1)
+                    .unwrap()
+                    .get_first(title_field)
+                    .unwrap()
+                    .as_text()
+                    .map(|x| x.to_string())
+                    .unwrap()
+            })
+            .collect::<Vec<_>>();
+        assert_eq!(format!("{:?}", docs), "[\"Envy of the Stars\", \"Hitchhiker's guide\"]");
+        let docs = searcher
+            .search(
+                &TermQuery::new(Term::from_field_text(extra_field, "scifi"), IndexRecordOption::Basic),
+                &TopDocs::with_limit(10),
+            )?
+            .into_iter()
+            .map(|x| {
+                searcher
+                    .doc(x.1)
+                    .unwrap()
+                    .get_first(title_field)
+                    .unwrap()
+                    .as_text()
+                    .map(|x| x.to_string())
+                    .unwrap()
+            })
+            .collect::<Vec<_>>();
+        assert_eq!(format!("{:?}", docs), "[\"Envy of the Stars\"]");
+        Ok(())
+    }
+
+    #[test]
+    fn test_unique_json_fields() -> Result<(), Box<dyn Error>> {
+        let schema = create_test_schema();
+        let index = IndexBuilder::new()
+            .schema(schema.clone())
+            .index_attributes(proto::IndexAttributes {
+                unique_fields: vec!["metadata.id".to_string()],
+                ..Default::default()
+            })
+            .create_in_ram()?;
+        register_default_tokenizers(&index);
+        let mut index_writer_holder = IndexWriterHolder::create(
+            &index,
+            WriterThreads::N(12),
+            1024 * 1024 * 1024,
+            Arc::new(tantivy::merge_policy::LogMergePolicy::default()),
+        )?;
+
+        index_writer_holder.index_document(
+            doc!(schema.get_field("metadata").expect("no field") => json!({"id": 1})),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.index_document(
+            doc!(schema.get_field("metadata").expect("no field") => json!({"id": 2})),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.index_document(
+            doc!(schema.get_field("metadata").expect("no field") => json!({"id": 3})),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.commit()?;
+        let reader = index.reader()?;
+        reader.reload()?;
+        let searcher = reader.searcher();
+        let counter = searcher.search(&AllQuery, &Count)?;
+        assert_eq!(counter, 3);
+        index_writer_holder.index_document(
+            doc!(schema.get_field("metadata").expect("no field") => json!({"id": "g"})),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.commit()?;
+        let reader = index.reader()?;
+        reader.reload()?;
+        let searcher = reader.searcher();
+        let counter = searcher.search(&AllQuery, &Count)?;
+        assert_eq!(counter, 4);
+        index_writer_holder.index_document(
+            doc!(schema.get_field("metadata").expect("no field") => json!({"id": "g"})),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.commit()?;
+        let reader = index.reader()?;
+        reader.reload()?;
+        let searcher = reader.searcher();
+        let counter = searcher.search(&AllQuery, &Count)?;
+        assert_eq!(counter, 4);
+        index_writer_holder.index_document(
+            doc!(schema.get_field("metadata").expect("no field") => json!({"id": 2})),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.index_document(
+            doc!(schema.get_field("metadata").expect("no field") => json!({"id": 4})),
+            ConflictStrategy::Merge,
+        )?;
+        index_writer_holder.commit()?;
+        let reader = index.reader()?;
+        reader.reload()?;
+        let searcher = reader.searcher();
+        let counter = searcher.search(&AllQuery, &Count)?;
+        assert_eq!(counter, 5);
+        Ok(())
+    }
 }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 mod custom_serializer;
 mod default_tokenizers;
-mod driver;
 mod fruit_extractors;
 mod index_holder;
 mod index_registry;
 mod index_writer_holder;
 pub mod merge_policies;
 pub mod queries;
 mod query_parser;
 mod segment_attributes;
 mod snippet_generator;
 mod summa_document;
 mod summa_tokenizer;
 
 pub use custom_serializer::NamedFieldDocument;
-pub use default_tokenizers::default_tokenizers;
-pub use driver::Driver;
+pub use default_tokenizers::{default_tokenizers, STOP_WORDS};
 pub use fruit_extractors::{build_fruit_extractor, FruitExtractor, IntermediateExtractionResult};
 pub use index_holder::{cleanup_index, IndexHolder};
 pub use index_registry::IndexRegistry;
 pub use index_writer_holder::IndexWriterHolder;
 pub use query_parser::{MorphologyManager, ProtoQueryParser, QueryParser, QueryParserError};
 pub use segment_attributes::SummaSegmentAttributes;
 pub use summa_document::{DocumentParsingError, SummaDocument};
@@ -28,16 +26,17 @@
 pub mod test_utils {
     use std::default::Default;
     use std::sync::atomic::{AtomicI64, Ordering};
 
     use itertools::Itertools;
     use rand::rngs::SmallRng;
     use rand::{Rng, SeedableRng};
+    use serde_json::json;
     use tantivy::doc;
-    use tantivy::schema::{IndexRecordOption, Schema, TextFieldIndexing, TextOptions, FAST, INDEXED, STORED};
+    use tantivy::schema::{IndexRecordOption, JsonObjectOptions, Schema, TextFieldIndexing, TextOptions, FAST, INDEXED, STORED};
 
     use crate::components::SummaDocument;
 
     pub fn create_test_schema() -> Schema {
         let mut schema_builder = Schema::builder();
 
         schema_builder.add_i64_field("id", FAST | INDEXED | STORED);
@@ -60,14 +59,33 @@
         );
         schema_builder.add_text_field(
             "tags",
             TextOptions::default()
                 .set_stored()
                 .set_indexing_options(TextFieldIndexing::default().set_tokenizer("summa").set_index_option(IndexRecordOption::Basic)),
         );
+        schema_builder.add_json_field(
+            "metadata",
+            JsonObjectOptions::default()
+                .set_stored()
+                .set_indexing_options(
+                    TextFieldIndexing::default()
+                        .set_tokenizer("summa_without_stop_words")
+                        .set_index_option(IndexRecordOption::Basic),
+                )
+                .set_expand_dots_enabled(),
+        );
+        schema_builder.add_text_field(
+            "extra",
+            TextOptions::default().set_stored().set_indexing_options(
+                TextFieldIndexing::default()
+                    .set_tokenizer("summa")
+                    .set_index_option(IndexRecordOption::WithFreqsAndPositions),
+            ),
+        );
         schema_builder.build()
     }
 
     #[inline]
     fn generate_term(rng: &mut SmallRng, prefix: &str, power: usize) -> String {
         if power > 0 {
             format!("{}{}", prefix, rng.gen_range(0..power))
@@ -91,21 +109,23 @@
         body_power: usize,
         tag_prefix: &'a str,
         tag_power: usize,
     ) -> SummaDocument<'a> {
         static DOC_ID: AtomicI64 = AtomicI64::new(1);
 
         let issued_at = 1674041452i64 - rng.gen_range(100..1000);
+        let doc_id = doc_id.unwrap_or_else(|| DOC_ID.fetch_add(1, Ordering::SeqCst));
 
         SummaDocument::TantivyDocument(doc!(
-            schema.get_field("id").expect("no expected field") => doc_id.unwrap_or_else(|| DOC_ID.fetch_add(1, Ordering::SeqCst)),
+            schema.get_field("id").expect("no expected field") => doc_id,
             schema.get_field("title").expect("no expected field") => generate_sentence(rng, title_prefix, title_power, 3),
             schema.get_field("body").expect("no expected field") => generate_sentence(rng, body_prefix, body_power, 50),
             schema.get_field("tags").expect("no expected field") => generate_sentence(rng, tag_prefix, tag_power, 5),
-            schema.get_field("issued_at").expect("no expected field") => issued_at
+            schema.get_field("issued_at").expect("no expected field") => issued_at,
+            schema.get_field("metadata").expect("no expected field") => json!({"id": doc_id}),
         ))
     }
 
     pub fn generate_unique_document<'a>(schema: &'a Schema, title: &'a str) -> SummaDocument<'a> {
         generate_document(None, &mut SmallRng::seed_from_u64(42), schema, title, 0, "body", 1000, "tag", 100)
     }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+use std::ops::RangeInclusive;
+
+use tantivy::json_utils::JsonTermWriter;
 use tantivy::query::{BitSetDocSet, ConstScorer, EnableScoring, Explanation, Query, Scorer, Weight};
 use tantivy::schema::{Field, IndexRecordOption};
-use tantivy::{DocId, Result, Score, SegmentReader, TantivyError};
+use tantivy::{DocId, Result, Score, SegmentReader, TantivyError, Term};
 use tantivy_common::BitSet;
 
 /// An Exists Query matches all of the documents
 /// containing a specific indexed field.
 ///
 /// ```rust
 /// use tantivy::collector::Count;
@@ -33,58 +36,92 @@
 ///     ))?;
 ///     index_writer.commit()?;
 /// }
 ///
 /// let reader = index.reader()?;
 /// let searcher = reader.searcher();
 ///
-/// let query = ExistsQuery::new(author);
+/// let query = ExistsQuery::new(author, "");
 /// let count = searcher.search(&query, &Count)?;
 /// assert_eq!(count, 2);
 /// Ok(())
 /// # }
 /// # assert!(test().is_ok());
 /// ```
+
+pub const JSON_SEGMENT_UPPER_TERMINATOR: u8 = 2u8;
+pub const JSON_SEGMENT_UPPER_TERMINATOR_STR: &str = unsafe { std::str::from_utf8_unchecked(&[JSON_SEGMENT_UPPER_TERMINATOR]) };
+
 #[derive(Clone, Debug)]
 pub struct ExistsQuery {
     field: Field,
+    full_path: String,
 }
 
 impl ExistsQuery {
     /// Creates a new ExistsQuery with a given field
-    pub fn new(field: Field) -> Self {
-        ExistsQuery { field }
+    pub fn new(field: Field, full_path: &str) -> Self {
+        ExistsQuery {
+            field,
+            full_path: full_path.to_string(),
+        }
     }
 }
 
 #[async_trait]
 impl Query for ExistsQuery {
     fn weight(&self, _: EnableScoring<'_>) -> Result<Box<dyn Weight>> {
-        Ok(Box::new(ExistsWeight { field: self.field }))
+        Ok(Box::new(ExistsWeight {
+            field: self.field,
+            full_path: self.full_path.clone(),
+        }))
     }
 
-    async fn weight_async(&self, _: EnableScoring<'_>) -> Result<Box<dyn Weight>> {
-        Ok(Box::new(ExistsWeight { field: self.field }))
+    async fn weight_async(&self, enable_scoring: EnableScoring<'_>) -> Result<Box<dyn Weight>> {
+        self.weight(enable_scoring)
     }
 }
 
 /// Weight associated with the `ExistsQuery` query.
 pub struct ExistsWeight {
     field: Field,
+    full_path: String,
+}
+
+impl ExistsWeight {
+    fn get_json_term(&self, json_path: &str) -> Term {
+        let mut term = Term::with_capacity(128);
+        let json_term_writer = JsonTermWriter::from_field_and_json_path(self.field, json_path, true, &mut term);
+        json_term_writer.term().clone()
+    }
+    fn generate_json_term_range(&self) -> RangeInclusive<Term> {
+        let start_term_str = format!("{}\0", self.full_path);
+        let end_term_str = format!("{}{}", self.full_path, JSON_SEGMENT_UPPER_TERMINATOR_STR);
+        self.get_json_term(&start_term_str)..=self.get_json_term(&end_term_str)
+    }
 }
 
 #[async_trait]
 impl Weight for ExistsWeight {
     fn scorer(&self, reader: &SegmentReader, boost: Score) -> Result<Box<dyn Scorer>> {
         let max_doc = reader.max_doc();
         let mut doc_bitset = BitSet::with_max_value(max_doc);
 
         let inverted_index = reader.inverted_index(self.field)?;
-        let mut term_stream = inverted_index.terms().stream()?;
-
+        let terms = inverted_index.terms();
+        let mut term_stream = if self.full_path.is_empty() {
+            terms.stream()?
+        } else {
+            let json_term_range = self.generate_json_term_range();
+            terms
+                .range()
+                .ge(json_term_range.start().serialized_value_bytes())
+                .le(json_term_range.end().serialized_value_bytes())
+                .into_stream()?
+        };
         while term_stream.advance() {
             let term_info = term_stream.value();
 
             let mut block_segment_postings = inverted_index.read_block_postings_from_terminfo(term_info, IndexRecordOption::Basic)?;
 
             loop {
                 let docs = block_segment_postings.docs();
@@ -104,16 +141,26 @@
     }
 
     async fn scorer_async(&self, reader: &SegmentReader, boost: Score) -> Result<Box<dyn Scorer>> {
         let max_doc = reader.max_doc();
         let mut doc_bitset = BitSet::with_max_value(max_doc);
 
         let inverted_index = reader.inverted_index_async(self.field).await?;
-        let mut term_stream = inverted_index.terms().range().into_stream_async().await?;
-
+        let terms = inverted_index.terms();
+        let mut term_stream = if self.full_path.is_empty() {
+            terms.range().into_stream_async().await?
+        } else {
+            let json_term_range = self.generate_json_term_range();
+            terms
+                .range()
+                .ge(json_term_range.start().serialized_value_bytes())
+                .le(json_term_range.end().serialized_value_bytes())
+                .into_stream_async()
+                .await?
+        };
         while term_stream.advance() {
             let term_info = term_stream.value();
 
             let mut block_segment_postings = inverted_index
                 .read_block_postings_from_terminfo_async(term_info, IndexRecordOption::Basic)
                 .await?;
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 use summa_proto::proto;
 use tantivy::query::{DisjunctionMaxQuery, Query, TermQuery};
 use tantivy::schema::{Field, FieldType, IndexRecordOption};
 
 mod english;
-#[cfg(feature = "nn")]
-mod english_nn;
 mod manager;
 
 pub use manager::MorphologyManager;
 
 use crate::components::query_parser::utils::cast_field_to_term;
 
 pub trait Morphology: MorphologyClone + Send + Sync {
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 use std::ops::Bound;
 use std::ops::Bound::Unbounded;
 use std::str::FromStr;
 
-use base64::Engine;
 #[cfg(feature = "metrics")]
 use opentelemetry::metrics::Counter;
 #[cfg(feature = "metrics")]
 use opentelemetry::Context;
 #[cfg(feature = "metrics")]
 use opentelemetry::{global, KeyValue};
 use summa_proto::proto;
-use tantivy::json_utils::{convert_to_fast_value_and_get_term, JsonTermWriter};
 use tantivy::query::{
     AllQuery, BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, MoreLikeThisQuery, Occur, PhraseQuery, Query, RangeQuery, RegexQuery, TermQuery,
 };
 use tantivy::schema::{Field, FieldEntry, FieldType, IndexRecordOption, Schema};
-use tantivy::{DateTime, Index, Score, Term};
+use tantivy::{Index, Score, Term};
 use tracing::info;
 
 use crate::components::queries::ExistsQuery;
 use crate::components::query_parser::morphology::MorphologyManager;
+use crate::components::query_parser::utils::cast_field_to_typed_term;
 use crate::components::query_parser::{QueryParser, QueryParserError};
 use crate::configs::core::QueryParserConfig;
 use crate::errors::{Error, SummaResult, ValidationError};
 #[cfg(feature = "metrics")]
 use crate::metrics::ToLabel;
 
 /// Responsible for casting `crate::proto::Query` message to `tantivy::query::Query`
@@ -53,56 +52,19 @@
             Some(proto::query_parser_config::DefaultMode::DisjuctionMaxMode(proto::MatchQueryDisjuctionMaxMode { tie_breaker })) => {
                 QueryParserDefaultMode::DisjuctionMax { tie_breaker }
             }
         }
     }
 }
 
-fn cast_value_to_term(field: Field, full_path: &str, field_type: &FieldType, value: &str) -> SummaResult<Term> {
-    Ok(match field_type {
-        FieldType::Str(_) => Term::from_field_text(field, value),
-        FieldType::JsonObject(json_options) => {
-            let mut term = Term::with_capacity(128);
-            let mut json_term_writer = JsonTermWriter::from_field_and_json_path(field, full_path, json_options.is_expand_dots_enabled(), &mut term);
-            convert_to_fast_value_and_get_term(&mut json_term_writer, value).unwrap_or_else(|| {
-                json_term_writer.set_str(value.trim_matches(|c| c == '\'' || c == '\"'));
-                json_term_writer.term().clone()
-            })
-        }
-        FieldType::I64(_) => Term::from_field_i64(
-            field,
-            i64::from_str(value).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as i64")))?,
-        ),
-        FieldType::U64(_) => Term::from_field_u64(
-            field,
-            u64::from_str(value).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as u64")))?,
-        ),
-        FieldType::F64(_) => Term::from_field_f64(
-            field,
-            f64::from_str(value).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as f64")))?,
-        ),
-        FieldType::Bytes(_) => Term::from_field_bytes(
-            field,
-            &base64::engine::general_purpose::STANDARD
-                .decode(value)
-                .map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as bytes")))?,
-        ),
-        FieldType::Date(_) => Term::from_field_date(
-            field,
-            DateTime::from_timestamp_secs(i64::from_str(value).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as date")))?),
-        ),
-        _ => return Err(Error::InvalidSyntax("invalid range type".to_owned())),
-    })
-}
-
-fn cast_value_to_bound_term(field: Field, full_path: &str, field_type: &FieldType, value: &str, including: bool) -> SummaResult<Bound<Term>> {
+fn cast_value_to_bound_term(field: &Field, full_path: &str, field_type: &FieldType, value: &str, including: bool) -> SummaResult<Bound<Term>> {
     Ok(match value {
         "*" => Unbounded,
         value => {
-            let casted_value = cast_value_to_term(field, full_path, field_type, value)?;
+            let casted_value = cast_field_to_typed_term(field, full_path, field_type, value)?;
             if including {
                 Bound::Included(casted_value)
             } else {
                 Bound::Excluded(casted_value)
             }
         }
     })
@@ -203,16 +165,16 @@
                     Err(QueryParserError::FieldDoesNotExist(field)) => Err(ValidationError::MissingField(field).into()),
                     Err(e) => Err(Error::InvalidQuerySyntax(Box::new(e), match_query_proto.value.to_owned())),
                 }?
             }
             proto::query::Query::Range(range_query_proto) => {
                 let (field, full_path, field_entry) = self.field_and_field_entry(&range_query_proto.field)?;
                 let value = range_query_proto.value.as_ref().ok_or(ValidationError::MissingRange)?;
-                let left = cast_value_to_bound_term(field, full_path, field_entry.field_type(), &value.left, value.including_left)?;
-                let right = cast_value_to_bound_term(field, full_path, field_entry.field_type(), &value.right, value.including_right)?;
+                let left = cast_value_to_bound_term(&field, full_path, field_entry.field_type(), &value.left, value.including_left)?;
+                let right = cast_value_to_bound_term(&field, full_path, field_entry.field_type(), &value.right, value.including_right)?;
                 Box::new(RangeQuery::new_term_bounds(
                     range_query_proto.field.clone(),
                     field_entry.field_type().value_type(),
                     &left,
                     &right,
                 ))
             }
@@ -227,15 +189,18 @@
             proto::query::Query::Phrase(phrase_query_proto) => {
                 let (field, full_path, field_entry) = self.field_and_field_entry(&phrase_query_proto.field)?;
                 let mut tokenizer = self.index.tokenizer_for_field(field)?;
 
                 let mut token_stream = tokenizer.token_stream(&phrase_query_proto.value);
                 let mut terms: Vec<(usize, Term)> = vec![];
                 while let Some(token) = token_stream.next() {
-                    terms.push((token.position, cast_value_to_term(field, full_path, field_entry.field_type(), &token.text)?))
+                    terms.push((
+                        token.position,
+                        cast_field_to_typed_term(&field, full_path, field_entry.field_type(), &token.text)?,
+                    ))
                 }
                 if terms.is_empty() {
                     Box::new(EmptyQuery)
                 } else if terms.len() == 1 {
                     Box::new(TermQuery::new(
                         terms[0].1.clone(),
                         field_entry.field_type().index_record_option().unwrap_or(IndexRecordOption::Basic),
@@ -243,15 +208,15 @@
                 } else {
                     Box::new(PhraseQuery::new_with_offset_and_slop(terms, phrase_query_proto.slop))
                 }
             }
             proto::query::Query::Term(term_query_proto) => {
                 let (field, full_path, field_entry) = self.field_and_field_entry(&term_query_proto.field)?;
                 Box::new(TermQuery::new(
-                    cast_value_to_term(field, full_path, field_entry.field_type(), &term_query_proto.value)?,
+                    cast_field_to_typed_term(&field, full_path, field_entry.field_type(), &term_query_proto.value)?,
                     field_entry.field_type().index_record_option().unwrap_or(IndexRecordOption::Basic),
                 ))
             }
             proto::query::Query::MoreLikeThis(more_like_this_query_proto) => {
                 let document = self
                     .cached_schema
                     .parse_document(&more_like_this_query_proto.document)
@@ -289,22 +254,15 @@
             }
             proto::query::Query::Exists(exists_query_proto) => {
                 let (field, full_path, field_entry) = self.field_and_field_entry(&exists_query_proto.field)?;
                 if !field_entry.field_type().is_indexed() {
                     let fni = QueryParserError::FieldNotIndexed(field_entry.name().to_string());
                     return Err(Error::InvalidQuerySyntax(Box::new(fni), exists_query_proto.field.to_string()));
                 }
-                if full_path.is_empty() {
-                    Box::new(ExistsQuery::new(field))
-                } else {
-                    Box::new(TermQuery::new(
-                        cast_value_to_term(field, full_path, field_entry.field_type(), "")?,
-                        field_entry.field_type().index_record_option().unwrap_or(IndexRecordOption::Basic),
-                    ))
-                }
+                Box::new(ExistsQuery::new(field, full_path))
             }
         })
     }
 
     pub fn parse_query(&self, query: proto::query::Query) -> SummaResult<Box<dyn Query>> {
         #[cfg(feature = "metrics")]
         self.query_counter.add(
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 pre_term = _{ phrase | regex | range | word }
 
 positive_term = ${ "+" ~ pre_term }
 negative_term = ${ "-" ~ pre_term }
 default_term = ${ pre_term }
 
+pre_grouping = _{ "(" ~ WHITE_SPACE? ~ term ~ (WHITE_SPACE+ ~ term)* ~ WHITE_SPACE? ~ ")" }
+
+positive_grouping = ${ "+" ~ pre_grouping }
+negative_grouping = ${ "-" ~ pre_grouping }
+default_grouping = ${ pre_grouping }
+
 term = { positive_term | negative_term | default_term }
-grouping = { "(" ~ WHITE_SPACE? ~ term ~ (WHITE_SPACE+ ~ term)* ~ WHITE_SPACE? ~ ")" }
+grouping = { positive_grouping | negative_grouping | default_grouping }
 search_group = ${ field_name ~ ":" ~ (grouping | term) }
 
 statement = ${ (isbn | wrapped_doi | search_group | term) ~ ("^" ~ boost)? }
 statements = _{ statement_sep* ~ statement? ~ (statement_sep+ ~ statement)* ~ statement_sep* }
 main = _{SOI ~ statements}
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 use std::collections::Bound;
 use std::ops::Bound::{Included, Unbounded};
 use std::ops::Deref;
 use std::str::FromStr;
 
+use base64::engine::general_purpose::STANDARD as BASE64;
+use base64::Engine;
 use pest::iterators::{Pair, Pairs};
 use pest::Parser;
 use pest_derive::Parser;
 use summa_proto::proto;
 use tantivy::query::{BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, PhraseQuery, Query, QueryClone, RangeQuery, RegexQuery, TermQuery};
-use tantivy::schema::{FacetParseError, Field, FieldEntry, FieldType, IndexRecordOption, Schema, TextFieldIndexing, Type};
+use tantivy::schema::{Facet, FacetParseError, Field, FieldEntry, FieldType, IndexRecordOption, Schema, TextFieldIndexing, Type};
 use tantivy::tokenizer::{TextAnalyzer, TokenizerManager};
 use tantivy::{Index, Term};
 use tantivy_query_grammar::Occur;
 
 use crate::components::query_parser::morphology::MorphologyManager;
 use crate::components::query_parser::proto_query_parser::QueryParserDefaultMode;
 use crate::components::query_parser::term_field_mappers::TermFieldMappersManager;
@@ -136,26 +138,26 @@
 
 fn reduce_should_clause(query: Box<dyn Query>) -> Box<dyn Query> {
     if let Some(boolean_query) = query.deref().as_any().downcast_ref::<BooleanQuery>() {
         let mut subqueries = vec![];
         for (occur, nested_query) in boolean_query.clauses() {
             let nested_query = reduce_should_clause(nested_query.box_clone());
             match occur {
-                Occur::Must | Occur::MustNot => subqueries.push((*occur, reduce_should_clause(nested_query.box_clone()))),
+                Occur::Must | Occur::MustNot => subqueries.push((*occur, nested_query)),
                 Occur::Should => {
-                    if let Some(nested_nested_query) = nested_query.deref().as_any().downcast_ref::<BooleanQuery>() {
-                        subqueries.extend(nested_nested_query.clauses().iter().map(|(o, q)| (*o, q.box_clone())))
+                    if let Some(nested_boolean_query) = nested_query.deref().as_any().downcast_ref::<BooleanQuery>() {
+                        subqueries.extend(nested_boolean_query.clauses().iter().map(|(o, q)| (*o, reduce_should_clause(q.box_clone()))))
                     } else {
-                        subqueries.push((*occur, reduce_should_clause(nested_query.box_clone())))
+                        subqueries.push((*occur, nested_query))
                     }
                 }
             }
         }
         if subqueries.len() == 1 && subqueries[0].0 == Occur::Should {
-            return subqueries[0].1.box_clone();
+            return subqueries.into_iter().next().expect("impossible").1;
         }
         return Box::new(BooleanQuery::new(subqueries)) as Box<dyn Query>;
     }
     query
 }
 
 fn reduce_empty_queries(query: Box<dyn Query>) -> Box<dyn Query> {
@@ -234,15 +236,15 @@
         let default_field_queries = self
             .query_parser_config
             .0
             .default_fields
             .iter()
             .map(|field| {
                 let (field, full_path) = self.schema.find_field(field).expect("inconsistent state");
-                self.parse_pre_term(&field, full_path, term.clone(), boost)
+                self.parse_pre_term(&field, full_path, term.clone(), boost, true)
             })
             .collect::<Result<Vec<_>, _>>()?;
 
         Ok(match occur {
             Occur::Should => {
                 let default_field_queries = default_field_queries.into_iter().flatten();
                 match QueryParserDefaultMode::from(self.query_parser_config.0.default_mode.clone()) {
@@ -289,27 +291,34 @@
             field_entry.name().to_string(),
             field_entry.field_type().value_type(),
             &left,
             &right,
         ))
     }
 
-    fn parse_words(&self, field: Field, option: &TextFieldIndexing, words: &str) -> Result<Vec<(usize, Term)>, QueryParserError> {
+    pub fn parse_words(&self, field: Field, full_path: &str, option: &TextFieldIndexing, words: &str) -> Result<Vec<(usize, Term)>, QueryParserError> {
         let field_entry = self.schema.get_field_entry(field);
         let mut text_analyzer = self.get_text_analyzer(field_entry, option)?;
         let mut token_stream = text_analyzer.token_stream(words);
         let mut terms = Vec::new();
         token_stream.process(&mut |token| {
-            let term = Term::from_field_text(field, &token.text);
+            let term = cast_field_to_term(&field, full_path, field_entry.field_type(), &token.text, true);
             terms.push((token.position, term));
         });
         Ok(terms)
     }
 
-    fn parse_pre_term(&self, field: &Field, full_path: &str, pre_term: Pair<Rule>, boost: Option<f32>) -> Result<Vec<Box<dyn Query>>, QueryParserError> {
+    fn parse_pre_term(
+        &self,
+        field: &Field,
+        full_path: &str,
+        pre_term: Pair<Rule>,
+        boost: Option<f32>,
+        ignore_phrase_for_non_position_field: bool,
+    ) -> Result<Vec<Box<dyn Query>>, QueryParserError> {
         let field_entry = self.schema.get_field_entry(*field);
         let field_type = field_entry.field_type();
 
         if field_type.value_type() == Type::Json && full_path.is_empty() {
             return Err(QueryParserError::JsonFieldWithoutPath(field_entry.name().to_string()));
         }
 
@@ -328,14 +337,23 @@
         let boost = multiply_boosts(self.query_parser_config.0.field_boosts.get(field_entry.name()).copied(), boost);
 
         if matches!(pre_term.as_rule(), Rule::range) {
             return Ok(vec![boost_query(Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>, boost)]);
         }
 
         return match *field_type {
+            FieldType::Bytes(_) => match pre_term.as_rule() {
+                Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
+                Rule::phrase | Rule::word => {
+                    let val = &BASE64.decode(pre_term.as_str())?;
+                    let query = Box::new(TermQuery::new(Term::from_field_bytes(*field, val), IndexRecordOption::Basic)) as Box<dyn Query>;
+                    Ok(vec![boost_query(query, boost)])
+                }
+                _ => unreachable!(),
+            },
             FieldType::U64(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
                     let val: u64 = u64::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_u64(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
@@ -346,14 +364,22 @@
                 Rule::phrase | Rule::word => {
                     let val: i64 = i64::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_i64(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
+            FieldType::Facet(_) => match pre_term.as_rule() {
+                Rule::phrase | Rule::word => {
+                    let val = Facet::from_text(pre_term.as_str())?;
+                    let query = Box::new(TermQuery::new(Term::from_facet(*field, &val), IndexRecordOption::Basic)) as Box<dyn Query>;
+                    Ok(vec![boost_query(query, boost)])
+                }
+                _ => unreachable!(),
+            },
             FieldType::F64(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
                     if !field_type.is_indexed() {
                         return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
                     }
                     let val: f64 = f64::from_str(pre_term.as_str())?;
@@ -390,15 +416,21 @@
                                 .query_parser_config
                                 .0
                                 .morphology_configs
                                 .get(field_entry.name())
                                 .cloned()
                                 .unwrap_or_default();
                             let query = if let Some(morphology) = self.morphology_manager.get(self.query_parser_config.0.query_language()) {
-                                morphology.derive_query(morphology_config, field, full_path, field_type, &token.text)
+                                // ToDo: Change heuristic
+                                if pre_term.as_str().len() < 24 {
+                                    morphology.derive_query(morphology_config, field, full_path, field_type, &token.text)
+                                } else {
+                                    let term = cast_field_to_term(field, full_path, field_type, &token.text, false);
+                                    Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>
+                                }
                             } else {
                                 let term = cast_field_to_term(field, full_path, field_type, &token.text, false);
                                 Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>
                             };
                             queries.push(boost_query(query, boost))
                         });
                         Ok(queries)
@@ -406,53 +438,39 @@
                     Rule::phrase => {
                         let mut phrase_pairs = pre_term.into_inner();
                         let words = match phrase_pairs.next() {
                             None => return Ok(vec![]),
                             Some(words) => words,
                         };
 
-                        match field_type {
-                            FieldType::JsonObject(_) => {
-                                let mut text_analyzer = self.get_text_analyzer(field_entry, indexing)?;
-                                let mut token_stream = text_analyzer.token_stream(words.as_str());
-                                let mut queries = Vec::new();
-
-                                token_stream.process(&mut |token| {
-                                    let term = cast_field_to_term(field, full_path, field_type, &token.text, true);
+                        let slop = phrase_pairs
+                            .next()
+                            .map(|v| match v.as_str() {
+                                "" => 0,
+                                _ => u32::from_str(v.as_str()).expect("cannot parse"),
+                            })
+                            .unwrap_or(0);
+                        let terms = self.parse_words(*field, full_path, indexing, words.as_str())?;
+                        if terms.len() <= 1 {
+                            return Ok(terms
+                                .into_iter()
+                                .map(|(_, term)| {
                                     let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
-                                    queries.push(boost_query(query, boost));
-                                });
-
-                                Ok(queries)
-                            }
-                            _ => {
-                                let slop = phrase_pairs
-                                    .next()
-                                    .map(|v| match v.as_str() {
-                                        "" => 0,
-                                        _ => u32::from_str(v.as_str()).expect("cannot parse"),
-                                    })
-                                    .unwrap_or(0);
-                                let terms = self.parse_words(*field, indexing, words.as_str())?;
-                                if terms.len() <= 1 {
-                                    return Ok(terms
-                                        .into_iter()
-                                        .map(|(_, term)| {
-                                            let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
-                                            boost_query(query, boost)
-                                        })
-                                        .collect());
-                                }
-                                if !indexing.index_option().has_positions() {
-                                    return Err(QueryParserError::FieldDoesNotHavePositionsIndexed(field_entry.name().to_string()));
-                                }
-                                let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, slop)) as Box<dyn Query>;
-                                return Ok(vec![boost_query(query, boost)]);
-                            }
+                                    boost_query(query, boost)
+                                })
+                                .collect());
                         }
+                        return if indexing.index_option().has_positions() {
+                            let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, slop)) as Box<dyn Query>;
+                            Ok(vec![boost_query(query, boost)])
+                        } else if ignore_phrase_for_non_position_field {
+                            Ok(vec![])
+                        } else {
+                            Err(QueryParserError::FieldDoesNotHavePositionsIndexed(field_entry.name().to_string()))
+                        };
                     }
                     Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                     Rule::regex => {
                         let query = Box::new(
                             RegexQuery::from_pattern(pre_term.clone().into_inner().next().expect("grammar failure").as_str(), *field)
                                 .map_err(|_| QueryParserError::Syntax(pre_term.as_str().to_string()))?,
                         ) as Box<dyn Query>;
@@ -463,27 +481,27 @@
             }
             _ => unreachable!(),
         };
     }
 
     fn parse_occur(&self, occur: &Pair<Rule>) -> Occur {
         match occur.as_rule() {
-            Rule::positive_term => Occur::Must,
-            Rule::negative_term => Occur::MustNot,
-            Rule::default_term => Occur::Should,
+            Rule::positive_term | Rule::positive_grouping => Occur::Must,
+            Rule::negative_term | Rule::negative_grouping => Occur::MustNot,
+            Rule::default_term | Rule::default_grouping => Occur::Should,
             _ => unreachable!(),
         }
     }
 
     fn parse_term(&self, term: Pair<Rule>, field: &Field, full_path: &str, boost: Option<f32>) -> Result<Box<dyn Query>, QueryParserError> {
-        let term = term.into_inner().next().expect("grammar_failure");
+        let term = term.into_inner().next().expect("grammar failure");
         let occur = self.parse_occur(&term);
         let pre_term = term.into_inner().next().expect("grammar failure");
         Ok(Box::new(BooleanQuery::new(
-            self.parse_pre_term(field, full_path, pre_term, boost)?
+            self.parse_pre_term(field, full_path, pre_term, boost, false)?
                 .into_iter()
                 .map(|q| (occur, q))
                 .collect(),
         )))
     }
 
     fn compute_boundary_term(&self, field: Field, phrase: &str) -> Result<Term, QueryParserError> {
@@ -508,14 +526,18 @@
                 let val: f64 = f64::from_str(phrase)?;
                 Ok(Term::from_field_f64(field, val))
             }
             FieldType::Bool(_) => {
                 let val: bool = bool::from_str(phrase)?;
                 Ok(Term::from_field_bool(field, val))
             }
+            FieldType::Bytes(_) => {
+                let val = &BASE64.decode(phrase)?;
+                Ok(Term::from_field_bytes(field, val))
+            }
             FieldType::Str(ref str_options) => {
                 let option = str_options.get_indexing_options().ok_or_else(|| {
                     // This should have been seen earlier really.
                     QueryParserError::FieldNotIndexed(field_entry.name().to_string())
                 })?;
                 let mut terms: Vec<Term> = Vec::new();
                 let mut text_analyzer = self
@@ -577,34 +599,41 @@
         let statement_result = match isbn_doi_or_search_group_or_term.as_rule() {
             Rule::search_group => {
                 let mut search_group = isbn_doi_or_search_group_or_term.into_inner();
                 let field_name = search_group.next().expect("grammar failure");
                 let grouping_or_term = search_group.next().expect("grammar failure");
                 match grouping_or_term.as_rule() {
                     Rule::grouping => {
+                        let grouping = grouping_or_term.into_inner().next().expect("grammar failure");
+                        let occur = self.parse_occur(&grouping);
                         let mut intermediate_results = vec![];
                         match self.schema.find_field(self.resolve_field_name(field_name.as_str())) {
                             Some((field, full_path)) => {
-                                for term in grouping_or_term.into_inner() {
+                                for term in grouping.into_inner() {
                                     intermediate_results.push(self.parse_term(term, &field, full_path, statement_boost)?);
                                 }
                             }
                             None => match proto::MissingFieldPolicy::from_i32(self.query_parser_config.0.missing_field_policy) {
                                 Some(proto::MissingFieldPolicy::AsUsualTerms) => {
                                     intermediate_results.push(self.default_field_queries(field_name, statement_boost)?);
-                                    for term in grouping_or_term.into_inner() {
+                                    for term in grouping.into_inner() {
                                         intermediate_results.push(self.default_field_queries(term, statement_boost)?)
                                     }
                                 }
                                 Some(proto::MissingFieldPolicy::Remove) => return Ok(Box::new(EmptyQuery {})),
                                 Some(proto::MissingFieldPolicy::Fail) => return Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
                                 _ => unreachable!(),
                             },
                         }
-                        Ok(Box::new(BooleanQuery::new(intermediate_results.into_iter().map(|q| (Occur::Should, q)).collect())) as Box<dyn Query>)
+                        let group_query = Box::new(BooleanQuery::new(intermediate_results.into_iter().map(|q| (Occur::Should, q)).collect())) as Box<dyn Query>;
+                        match occur {
+                            Occur::Should => Ok(group_query),
+                            Occur::Must => Ok(Box::new(BooleanQuery::new(vec![(Occur::Must, group_query)])) as Box<dyn Query>),
+                            Occur::MustNot => Ok(Box::new(BooleanQuery::new(vec![(Occur::MustNot, group_query)])) as Box<dyn Query>),
+                        }
                     }
                     Rule::term => match self.schema.find_field(self.resolve_field_name(field_name.as_str())) {
                         Some((field, full_path)) => self.parse_term(grouping_or_term, &field, full_path, statement_boost),
                         None => match proto::MissingFieldPolicy::from_i32(self.query_parser_config.0.missing_field_policy) {
                             Some(proto::MissingFieldPolicy::AsUsualTerms) => Ok(Box::new(BooleanQuery::new(vec![
                                 (Occur::Should, self.default_field_queries(field_name, statement_boost)?),
                                 (Occur::Should, self.default_field_queries(grouping_or_term, statement_boost)?),
@@ -671,22 +700,22 @@
                     };
                     let entities = morphology.detect_ners(&top_level_phrase);
                     subqueries.extend(
                         fields
                             .map(|field| {
                                 let mut subsubqueries = vec![];
                                 for entity in &entities {
-                                    let field = self.schema.get_field(field).expect("no field");
+                                    let (field, full_path) = self.schema.find_field(self.resolve_field_name(field)).expect("no field");
                                     let field_entry = self.schema.get_field_entry(field);
                                     let field_boost = self.query_parser_config.0.field_boosts.get(field_entry.name()).copied();
                                     if let FieldType::Str(ref str_option) = field_entry.field_type() {
                                         let Some(option) = str_option.get_indexing_options() else {
                                         continue
                                     };
-                                        let terms = match self.parse_words(field, option, entity) {
+                                        let terms = match self.parse_words(field, full_path, option, entity) {
                                             Ok(terms) => terms,
                                             Err(err) => return Err(err),
                                         };
                                         if terms.len() > 1 && option.index_option().has_positions() {
                                             let query = Box::new(PhraseQuery::new_with_offset(terms)) as Box<dyn Query>;
                                             subsubqueries.push(boost_query(query, multiply_boosts(ner_matches_promoter.boost, field_boost)))
                                         }
@@ -706,31 +735,45 @@
                     self.query_parser_config.0.default_fields.iter()
                 } else {
                     exact_matches_promoter.fields.iter()
                 };
                 subqueries.extend(
                     fields
                         .filter_map(|field| {
-                            let field = self.schema.get_field(field).expect("no field");
+                            let (field, full_path) = self.schema.find_field(self.resolve_field_name(field)).expect("no field");
                             let field_entry = self.schema.get_field_entry(field);
                             let field_boost = self.query_parser_config.0.field_boosts.get(field_entry.name()).copied();
-                            if let FieldType::Str(ref str_option) = field_entry.field_type() {
-                                let Some(option) = str_option.get_indexing_options() else {
-                                    return None
-                                };
-                                let terms = match self.parse_words(field, option, &top_level_phrase) {
-                                    Ok(terms) => terms,
-                                    Err(err) => return Some(Err(err)),
-                                };
-                                (terms.len() > 1 && option.index_option().has_positions()).then(|| {
-                                    let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, exact_matches_promoter.slop)) as Box<dyn Query>;
-                                    Ok(boost_query(query, multiply_boosts(exact_matches_promoter.boost, field_boost)))
-                                })
-                            } else {
-                                None
+                            match field_entry.field_type() {
+                                FieldType::Str(ref str_option) => {
+                                    let Some(option) = str_option.get_indexing_options() else {
+                                        return None
+                                    };
+                                    let terms = match self.parse_words(field, full_path, option, &top_level_phrase) {
+                                        Ok(terms) => terms,
+                                        Err(err) => return Some(Err(err)),
+                                    };
+                                    (terms.len() > 1 && option.index_option().has_positions()).then(|| {
+                                        let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, exact_matches_promoter.slop)) as Box<dyn Query>;
+                                        Ok(boost_query(query, multiply_boosts(exact_matches_promoter.boost, field_boost)))
+                                    })
+                                }
+                                FieldType::JsonObject(ref json_option) => {
+                                    let Some(option) = json_option.get_text_indexing_options() else {
+                                        return None
+                                    };
+                                    let terms = match self.parse_words(field, full_path, option, &top_level_phrase) {
+                                        Ok(terms) => terms,
+                                        Err(err) => return Some(Err(err)),
+                                    };
+                                    (terms.len() > 1 && option.index_option().has_positions()).then(|| {
+                                        let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, exact_matches_promoter.slop)) as Box<dyn Query>;
+                                        Ok(boost_query(query, multiply_boosts(exact_matches_promoter.boost, field_boost)))
+                                    })
+                                }
+                                _ => None,
                             }
                         })
                         .collect::<Result<Vec<_>, _>>()?
                         .into_iter()
                         .map(|q| (Occur::Should, q)),
                 )
             }
@@ -1018,14 +1061,31 @@
             format!("{:?}", query_parser.parse_query("metadata.a:1")),
             "Ok(TermQuery(Term(field=5, type=Json, path=a, type=I64, 1)))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("metadata.a:\"1\"")),
             "Ok(TermQuery(Term(field=5, type=Json, path=a, type=Str, \"1\")))"
         );
+        assert_eq!(
+            format!("{:?}", query_parser.parse_query("metadata.a:\"1 2 3\"")),
+            "Ok(PhraseQuery { field: Field(5), phrase_terms: [(0, Term(field=5, type=Json, path=a, type=Str, \"1\")), (1, Term(field=5, type=Json, path=a, type=Str, \"2\")), (2, Term(field=5, type=Json, path=a, type=Str, \"3\"))], slop: 0 })"
+        );
+    }
+
+    #[test]
+    pub fn test_grouping() {
+        let query_parser = create_query_parser();
+        assert_eq!(
+            format!("{:?}", query_parser.parse_query("body:+(a b)")),
+            "Ok(BooleanQuery { subqueries: [(Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(field=1, type=Str, \"a\"))), (Should, TermQuery(Term(field=1, type=Str, \"b\")))] })] })"
+        );
+        assert_eq!(
+            format!("{:?}", query_parser.parse_query("body:-(a b)")),
+            "Ok(BooleanQuery { subqueries: [(MustNot, BooleanQuery { subqueries: [(Should, TermQuery(Term(field=1, type=Str, \"a\"))), (Should, TermQuery(Term(field=1, type=Str, \"b\")))] })] })"
+        );
     }
 
     #[test]
     pub fn test_plus_minus() {
         let query_parser = create_query_parser();
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:+search -engine")),
@@ -1119,16 +1179,18 @@
             "title".to_string(),
             proto::MorphologyConfig {
                 derive_tenses_coefficient: Some(0.3),
             },
         );
         query_parser.query_parser_config.0.morphology_configs = morphology_configs;
         query_parser.query_parser_config.0.query_language = Some("en".to_string());
-        let query = query_parser.parse_query("search engine");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"search\")), TermQuery(Term(field=0, type=Str, \"searches\"))], tie_breaker: 0.3 }), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.3 })] })");
+        let query = query_parser.parse_query("red1 search engine going");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"red1\"))), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"search\")), TermQuery(Term(field=0, type=Str, \"searches\"))], tie_breaker: 0.3 }), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.3 }), (Should, TermQuery(Term(field=0, type=Str, \"going\")))] })");
+        let query = query_parser.parse_query("iso 34-1:2022");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"iso\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"1\")))] })");
     }
 
     #[test]
     pub fn test_ner() {
         let mut query_parser = create_query_parser();
         let mut morphology_configs = HashMap::new();
         morphology_configs.insert(
@@ -1141,10 +1203,9 @@
         query_parser.query_parser_config.0.ner_matches_promoter = Some(proto::NerMatchesPromoter {
             boost: Some(1.3),
             fields: vec!["title".to_string()],
         });
         query_parser.query_parser_config.0.query_language = Some("en".to_string());
         let query = query_parser.parse_query("london is the capital of Great Britain");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"london\"))), (Should, TermQuery(Term(field=0, type=Str, \"is\"))), (Should, TermQuery(Term(field=0, type=Str, \"the\"))), (Should, TermQuery(Term(field=0, type=Str, \"capital\"))), (Should, TermQuery(Term(field=0, type=Str, \"of\"))), (Should, TermQuery(Term(field=0, type=Str, \"great\"))), (Should, TermQuery(Term(field=0, type=Str, \"britain\")))] })");
-        // assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"london\"))), (Should, TermQuery(Term(field=0, type=Str, \"is\"))), (Should, TermQuery(Term(field=0, type=Str, \"the\"))), (Should, TermQuery(Term(field=0, type=Str, \"capital\"))), (Should, TermQuery(Term(field=0, type=Str, \"of\"))), (Should, TermQuery(Term(field=0, type=Str, \"great\"))), (Should, TermQuery(Term(field=0, type=Str, \"britain\"))), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"great\")), (1, Term(field=0, type=Str, \"britain\"))], slop: 0 }, boost=1.3))] })");
     }
 }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,26 @@
 use regex::Regex;
 use tantivy::query::{BooleanQuery, Occur, Query};
 use tantivy::schema::{Field, FieldType, Schema};
 use tantivy::tokenizer::TokenizerManager;
 use tantivy::Term;
 
 use crate::components::query_parser::utils::cast_field_to_term;
-use crate::components::QueryParserError;
 
 pub trait TermFieldMapper {
-    fn map(&self, value: &str, fields: &Vec<String>) -> Option<Box<dyn Query>>;
+    fn map(&self, value: &str, fields: &[String]) -> Option<Box<dyn Query>>;
 }
 
 fn tokenize_value(schema: &Schema, field: &Field, full_path: &str, value: &str, tokenizer_manager: &TokenizerManager) -> Vec<Term> {
     let field_entry = schema.get_field_entry(*field);
     let mut terms = vec![];
     match field_entry.field_type() {
         FieldType::Str(ref str_options) => {
-            let option = str_options.get_indexing_options().unwrap();
-            let mut text_analyzer = tokenizer_manager
-                .get(option.tokenizer())
-                .ok_or_else(|| QueryParserError::UnknownTokenizer {
-                    field: field_entry.name().to_string(),
-                    tokenizer: option.tokenizer().to_string(),
-                })
-                .unwrap();
+            let option = str_options.get_indexing_options().expect("no options");
+            let mut text_analyzer = tokenizer_manager.get(option.tokenizer()).expect("unknown tokenizer");
             let mut token_stream = text_analyzer.token_stream(value);
             token_stream.process(&mut |token| {
                 let term = cast_field_to_term(field, full_path, schema.get_field_entry(*field).field_type(), &token.text, true);
                 terms.push(term);
             });
         }
         _ => terms.push(cast_field_to_term(
@@ -51,22 +44,21 @@
 impl DoiMapper {
     pub fn new(schema: Schema, tokenizer_manager: TokenizerManager) -> Self {
         DoiMapper { schema, tokenizer_manager }
     }
 }
 
 impl TermFieldMapper for DoiMapper {
-    fn map(&self, value: &str, fields: &Vec<String>) -> Option<Box<dyn Query>> {
+    fn map(&self, value: &str, fields: &[String]) -> Option<Box<dyn Query>> {
         let terms = fields
             .iter()
-            .map(|field_name| {
+            .flat_map(|field_name| {
                 let (field, full_path) = self.schema.find_field(field_name).expect("inconsistent state");
                 tokenize_value(&self.schema, &field, full_path, value, &self.tokenizer_manager)
             })
-            .flatten()
             .collect();
         Some(Box::new(BooleanQuery::new_multiterms_query(terms)) as Box<dyn Query>)
     }
 }
 
 pub struct DoiIsbnMapper {
     schema: Schema,
@@ -76,15 +68,15 @@
 impl DoiIsbnMapper {
     pub fn new(schema: Schema, tokenizer_manager: TokenizerManager) -> Self {
         DoiIsbnMapper { schema, tokenizer_manager }
     }
 }
 
 impl TermFieldMapper for DoiIsbnMapper {
-    fn map(&self, value: &str, fields: &Vec<String>) -> Option<Box<dyn Query>> {
+    fn map(&self, value: &str, fields: &[String]) -> Option<Box<dyn Query>> {
         thread_local! {
             static MATCHER: Regex = Regex::new(r"(10.[0-9]+)/((?:cbo)?(?:(?:978[0-9]{10})|(?:978[0-9]{13})|(?:978[-0-9]+)))(.*)").expect("cannot compile regex");
         }
         MATCHER.with(|matcher| {
             let lowercased_doi = value.to_lowercase();
             for cap in matcher.captures_iter(&lowercased_doi) {
                 let (_, isbn, _) = (&cap[1], &cap[2], &cap[3]);
@@ -115,15 +107,15 @@
 impl IsbnMapper {
     pub fn new(schema: Schema, tokenizer_manager: TokenizerManager) -> Self {
         IsbnMapper { schema, tokenizer_manager }
     }
 }
 
 impl TermFieldMapper for IsbnMapper {
-    fn map(&self, value: &str, fields: &Vec<String>) -> Option<Box<dyn Query>> {
+    fn map(&self, value: &str, fields: &[String]) -> Option<Box<dyn Query>> {
         let subqueries: Vec<_> = fields
             .iter()
             .map(|field_name| {
                 let (field, full_path) = self.schema.find_field(field_name).expect("inconsistent state");
                 let terms = tokenize_value(&self.schema, &field, full_path, &value.replace('-', ""), &self.tokenizer_manager);
                 (Occur::Should, Box::new(BooleanQuery::new_multiterms_query(terms)) as Box<dyn Query>)
             })
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,29 @@
                 json_object.insert("quantized_page_rank".to_string(), json!(quantize_page_rank(v)));
             }
         }
     }
     if schema.get_field("updated_at").is_ok() {
         json_object.insert("updated_at".to_string(), json!(current_time()));
     }
+    if schema.get_field("custom_score").is_ok() && !json_object.contains_key("custom_score") {
+        match json_object.get("type") {
+            Some(serde_json::value::Value::String(s)) => {
+                if s == "book-chapter" {
+                    json_object.insert("custom_score".to_string(), json!(0.85))
+                } else {
+                    json_object.insert("custom_score".to_string(), json!(1.0))
+                }
+            }
+            _ => json_object.insert("custom_score".to_string(), json!(1.0)),
+        };
+    }
+    if schema.get_field("links").is_ok() && schema.get_field("ctr").is_ok() && !json_object.contains_key("ctr") {
+        json_object.insert("ctr".to_string(), json!(0.1));
+    }
 }
 
 impl<'a> SummaDocument<'a> {
     pub fn bound_with(self, schema: &'a Schema) -> SummaDocument {
         match self {
             SummaDocument::UnboundJsonBytes(json_bytes) => SummaDocument::BoundJsonBytes((schema, json_bytes)),
             SummaDocument::BoundJsonBytes((_, json_bytes)) => SummaDocument::BoundJsonBytes((schema, json_bytes)),
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 }
 
 impl CachingDirectory {
     /// Creates a new CachingDirectory.
     ///
     /// Warming: The resulting CacheDirectory will cache all information without ever
     /// removing any item from the cache.
-    pub fn bounded(underlying: Arc<dyn Directory>, capacity_in_bytes: usize, file_stats: FileStats) -> CachingDirectory {
+    pub fn bounded(underlying: Arc<dyn Directory>, _capacity_in_bytes: usize, file_stats: FileStats) -> CachingDirectory {
         CachingDirectory {
             underlying,
             cache: Arc::new(ByteRangeCache::with_infinite_capacity()),
             file_stats,
         }
     }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.3/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/Cargo.toml` & `summa_embed-0.17.3/local_dependencies/summa-server/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "summa-server"
-version = "0.17.2"
+version = "0.17.3"
 license-file = "LICENSE"
 description = "Fast full-text search server"
 homepage = "https://github.com/izihawa/summa"
 repository = "https://github.com/izihawa/summa"
 keywords = ["async", "search", "server", "grpc"]
 
 [lib]
@@ -51,15 +51,15 @@
 rand = { version = "0.8", features = ["small_rng"] }
 rdkafka = { version = "0.29", optional = true }
 rlimit = "0.9"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_derive = "1.0"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
-summa-core = { version = "0.17.2", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.3", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { features = ["grpc"] , path = "../summa-proto" }
 take_mut = "0.2"
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tantivy-fst = "0.4.0"
 time = { version = "0.3", features = ["serde-well-known", "wasm-bindgen"] }
 thiserror = "1.0"
 tokio = { version = "1.25", default_features = false , features = ["full", "time"] }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/LICENSE` & `summa_embed-0.17.3/local_dependencies/summa-server/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/apis/consumer.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/apis/index.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/index.rs`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         let _ = span.enter();
         let index_holder = self.index_service.get_index_holder(&proto_request.index_name).await?;
         let searcher = index_holder.index_reader().searcher();
         let schema = index_holder.schema().clone();
         let multi_fields = index_holder.multi_fields().clone();
 
         let query_fields = validators::parse_fields(searcher.schema(), &proto_request.fields).map_err(crate::errors::Error::from)?;
-        let query_fields = (!query_fields.is_empty()).then(|| HashSet::from_iter(query_fields.into_iter()));
+        let query_fields = (!query_fields.is_empty()).then(|| HashSet::from_iter(query_fields.into_iter().map(|x| x.0)));
 
         let documents_receiver = index_holder
             .documents(&searcher, move |document| {
                 let document = NamedFieldDocument::from_document(&schema, &query_fields, &multi_fields, &document).to_json_string();
                 Some(Ok(DocumentsResponse { document }))
             })
             .map_err(crate::errors::Error::from)?;
@@ -191,15 +191,18 @@
         let mut last_status_report = Instant::now();
         while let Some(chunk) = in_stream.next().await {
             match chunk {
                 Ok(chunk) => {
                     info!(action = "received_chunk", index_name = chunk.index_name, documents = ?chunk.documents.len());
                     let now = Instant::now();
                     let index_holder = self.index_service.get_index_holder(&chunk.index_name).await?;
-                    let (success_bulk_docs, failed_bulk_docs) = index_holder.index_bulk(&chunk.documents).await.map_err(crate::errors::Error::from)?;
+                    let (success_bulk_docs, failed_bulk_docs) = index_holder
+                        .index_bulk(&chunk.documents, chunk.conflict_strategy.and_then(proto::ConflictStrategy::from_i32))
+                        .await
+                        .map_err(crate::errors::Error::from)?;
                     elapsed_secs += now.elapsed().as_secs_f64();
                     success_docs += success_bulk_docs;
                     failed_docs += failed_bulk_docs;
                     if last_status_report.elapsed().as_secs_f64() > 60f64 {
                         info!(action = "indexed", success_docs = success_docs, failed_docs = failed_docs);
                         last_status_report = Instant::now();
                     }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/apis/reflection.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/reflection.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/apis/search.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/search.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/bin/main.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/bin/main.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumer_manager.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumer_manager.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,20 @@
 
 #[derive(Debug)]
 pub struct PreparedConsumption {
     committed_consumer_thread: Box<dyn ConsumerThread>,
 }
 
 impl PreparedConsumption {
-    pub fn from_config(consumer_name: &str, consumer_config: &crate::configs::consumer::Config) -> SummaServerResult<PreparedConsumption> {
-        #[cfg(not(feature = "kafka"))]
+    #[cfg(not(feature = "kafka"))]
+    pub fn from_config(_consumer_name: &str, _consumer_config: &crate::configs::consumer::Config) -> SummaServerResult<PreparedConsumption> {
         unimplemented!();
-        #[cfg(feature = "kafka")]
+    }
+    #[cfg(feature = "kafka")]
+    pub fn from_config(consumer_name: &str, consumer_config: &crate::configs::consumer::Config) -> SummaServerResult<PreparedConsumption> {
         Ok(PreparedConsumption {
             committed_consumer_thread: Box::new(crate::components::consumers::kafka::KafkaConsumerThread::new(consumer_name, consumer_config)?)
                 as Box<dyn ConsumerThread>,
         })
     }
 
     pub fn on_create(&self) -> impl Future<Output = SummaServerResult<()>> + '_ {
@@ -76,16 +78,15 @@
         }
         let index_writer_holder = index_holder.index_writer_holder()?.clone().read_owned().await;
         let schema = index_holder.schema().clone();
         let conflict_strategy = index_holder.conflict_strategy();
         prepared_consumption
             .committed_consumer_thread
             .start(index_writer_holder, conflict_strategy, schema)
-            .await
-            .unwrap();
+            .await?;
         self.consumptions.insert(index_holder.clone(), prepared_consumption.committed_consumer_thread);
         Ok(())
     }
 
     /// Stops all consuming threads
     #[instrument(skip(self))]
     pub async fn stop(&mut self) -> SummaServerResult<()> {
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/dummy.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/dummy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -79,30 +79,28 @@
             .set("max.poll.interval.ms", config.max_poll_interval_ms.to_string())
             .set("auto.offset.reset", "earliest")
             .set("allow.auto.create.topics", "true");
 
         let mut kafka_producer_config = ClientConfig::new();
         kafka_producer_config.set("bootstrap.servers", config.bootstrap_servers.join(","));
 
-        let stream_consumer: KafkaStreamConsumer = kafka_consumer_config.create().map_err(|e| Error::Consumer(e.to_string()))?;
-        stream_consumer
-            .subscribe(&config.topics.iter().map(String::as_str).collect::<Vec<_>>())
-            .map_err(|e| Error::Consumer(e.to_string()))?;
+        let stream_consumer: KafkaStreamConsumer = kafka_consumer_config.create()?;
+        stream_consumer.subscribe(&config.topics.iter().map(String::as_str).collect::<Vec<_>>())?;
 
         Ok(KafkaConsumerThread {
             consumer_name: consumer_name.to_owned(),
             config: config.clone(),
             kafka_producer_config,
             consuming_state: Arc::new(Mutex::new(Some(ConsumingState::Disabled(stream_consumer)))),
         })
     }
 
     #[instrument(skip(self))]
     async fn create_topics(&self) -> SummaServerResult<()> {
-        let admin_client = AdminClient::from_config(&self.kafka_producer_config).map_err(|e| Error::Consumer(e.to_string()))?;
+        let admin_client = AdminClient::from_config(&self.kafka_producer_config)?;
         let admin_options = AdminOptions::new().operation_timeout(Some(Timeout::Never));
         let new_topics: Vec<_> = self
             .config
             .topics
             .iter()
             .map(|topic_name| NewTopic::new(topic_name.as_str(), 1, TopicReplication::Fixed(1)))
             .collect();
@@ -113,40 +111,33 @@
             .map(|topic_name| {
                 AlterConfig::new(ResourceSpecifier::Topic(topic_name.as_str()))
                     .set("retention.ms", "14400000")
                     .set("retention.bytes", "1073741824")
                     .set("max.message.bytes", "134217728")
             })
             .collect();
-        let response = admin_client
-            .create_topics(&new_topics, &admin_options)
-            .await
-            .map_err(|e| Error::Consumer(e.to_string()))?;
+        let response = admin_client.create_topics(&new_topics, &admin_options).await?;
         info!(action = "create_topics", topics = ?new_topics, response = ?response);
-        let response = admin_client
-            .alter_configs(&alter_topics, &admin_options)
-            .await
-            .map_err(|e| Error::Consumer(e.to_string()))?;
+        let response = admin_client.alter_configs(&alter_topics, &admin_options).await?;
         info!(action = "alter_configs", topics = ?new_topics, response = ?response);
         Ok(())
     }
 
     #[instrument(skip(self))]
     async fn delete_topics(&self) -> SummaServerResult<()> {
-        let admin_client = AdminClient::from_config(&self.kafka_producer_config).map_err(|e| Error::Consumer(e.to_string()))?;
+        let admin_client = AdminClient::from_config(&self.kafka_producer_config)?;
         let topics: Vec<_> = self.config.topics.iter().map(String::as_str).collect();
         let response = admin_client
             .delete_topics(
                 &topics,
                 &AdminOptions::new()
                     .operation_timeout(Some(Timeout::Never))
                     .request_timeout(Some(Timeout::After(Duration::from_secs(600)))),
             )
-            .await
-            .map_err(|e| Error::Consumer(e.to_string()))?;
+            .await?;
         info!(action = "delete_topics", topics = ?topics, response = ?response);
         Ok(())
     }
 }
 
 #[async_trait]
 impl ConsumerThread for KafkaConsumerThread {
@@ -241,16 +232,15 @@
                             Ok(())
                         }
                         Err(KafkaError::ConsumerCommit(RDKafkaErrorCode::NoOffset)) => {
                             warn!(error = "no_offset");
                             Ok(())
                         }
                         Err(e) => Err(e),
-                    }
-                    .map_err(|e| Error::Consumer(e.to_string()))?;
+                    }?;
                     Ok::<StreamConsumer, Error>(stream_consumer)
                 })
                 .await?;
                 Some(ConsumingState::Disabled(stream_consumer?))
             }
             old => old,
         };
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/status.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/status.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/components/index_meter.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/components/index_meter.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/configs/api.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/configs/consumer.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/configs/server.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/configs/store.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/store.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/errors.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/lib.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/logging.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/logging.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/server.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/server.rs`

 * *Files 2% similar despite different names*

```diff
@@ -98,21 +98,20 @@
         #[cfg(unix)]
         match increase_fd_limit() {
             Ok(soft) => tracing::debug!("NOFILE limit: soft = {}", soft),
             Err(err) => tracing::error!("Error increasing NOFILE limit: {}", err),
         }
 
         let mut futures: Vec<Box<dyn Future<Output = SummaServerResult<()>> + Send>> = vec![];
-        let server_config = self.server_config_holder.read().await.get().clone();
 
         let index_service = Index::new(&self.server_config_holder)?;
         futures.push(Box::new(index_service.prepare_serving_future(terminator.clone()).await?));
 
         #[cfg(feature = "metrics")]
-        if let Some(metrics_config) = &server_config.metrics {
+        if let Some(metrics_config) = &self.server_config_holder.read().await.get().metrics.clone() {
             let metrics_service = Metrics::new(metrics_config)?;
             futures.push(Box::new(metrics_service.prepare_serving_future(&index_service, terminator.clone()).await?));
         }
 
         let api_service = Api::new(&self.server_config_holder, &index_service)?;
         futures.push(Box::new(api_service.prepare_serving_future(terminator.clone()).await?));
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/services/api.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/services/api.rs`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,22 @@
                     .on_request(Api::on_request)
                     .on_response(Api::on_response)
                     .on_failure(Api::on_failure),
             )
             .into_inner();
 
         let consumer_service = ConsumerApiServer::new(consumer_api);
-        let index_service = IndexApiServer::new(index_api);
+        let mut index_service = IndexApiServer::new(index_api)
+            .accept_compressed(CompressionEncoding::Gzip)
+            .send_compressed(CompressionEncoding::Gzip);
+        if let Some(max_from_size_bytes) = api_config.max_frame_size_bytes {
+            index_service = index_service
+                .max_decoding_message_size(max_from_size_bytes as usize)
+                .max_encoding_message_size(max_from_size_bytes as usize);
+        }
         let reflection_service = ReflectionApiServer::new(reflection_api);
         let mut search_service = SearchApiServer::new(search_api)
             .accept_compressed(CompressionEncoding::Gzip)
             .send_compressed(CompressionEncoding::Gzip);
         if let Some(max_from_size_bytes) = api_config.max_frame_size_bytes {
             search_service = search_service
                 .max_decoding_message_size(max_from_size_bytes as usize)
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/services/index.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/services/index.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use std::future::Future;
 use std::sync::atomic::{AtomicBool, Ordering};
 use std::sync::Arc;
 use std::time::{Duration, SystemTime, UNIX_EPOCH};
 
 use async_broadcast::Receiver;
 use futures_util::future::join_all;
-use summa_core::components::{cleanup_index, Driver, IndexHolder, IndexRegistry};
+use summa_core::components::{cleanup_index, IndexHolder, IndexRegistry};
 use summa_core::configs::ConfigProxy;
 use summa_core::configs::PartialProxy;
 use summa_core::directories::DefaultExternalRequestGenerator;
 use summa_core::errors::SummaResult;
 use summa_core::hyper_external_request::HyperExternalRequest;
 use summa_core::proto_traits::Wrapper;
 use summa_core::utils::sync::{Handler, OwningHandler};
@@ -132,15 +132,14 @@
                 IndexHolder::create_holder(
                     &core_config,
                     index,
                     &index_name_clone,
                     index_engine_config_holder,
                     merge_policy,
                     query_parser_config,
-                    Driver::current_tokio(),
                 )
             })
             .await??;
             index_holder.partial_warmup(false, &default_fields).await?;
             index_holders.insert(index_name, OwningHandler::new(index_holder));
         }
         info!(action = "setting_index_holders", indices = ?index_holders.keys().collect::<Vec<_>>());
@@ -200,23 +199,15 @@
         let merge_policy = index_engine_config.merge_policy.clone();
         let query_parser_config = index_engine_config.query_parser_config.as_ref().cloned().unwrap_or_default();
         let index_name = index_name.to_string();
         Ok(self
             .index_registry
             .add(
                 tokio::task::spawn_blocking(move || {
-                    IndexHolder::create_holder(
-                        &core_config,
-                        index,
-                        &index_name,
-                        index_engine_config_holder,
-                        merge_policy,
-                        query_parser_config,
-                        Driver::current_tokio(),
-                    )
+                    IndexHolder::create_holder(&core_config, index, &index_name, index_engine_config_holder, merge_policy, query_parser_config)
                 })
                 .await??,
             )
             .await?)
     }
 
     /// Create consumer and insert it into the consumer registry. Add it to the `IndexHolder` afterwards.
@@ -262,31 +253,37 @@
         let index_holder = self.insert_index(&attach_index_request.index_name, index, &index_engine_config).await?;
         index_holder
             .partial_warmup(false, &query_parser_config.map(|q| q.default_fields).unwrap_or_default())
             .await?;
         Ok(index_holder)
     }
 
-    /// Create consumer and insert it into the consumer registry. Add it to the `IndexHolder` afterwards.
     #[instrument(skip_all, fields(source_index_name = ?copy_documents_request.source_index_name, target_index_name = ?copy_documents_request.target_index_name))]
     pub async fn copy_documents(&self, copy_documents_request: proto::CopyDocumentsRequest) -> SummaServerResult<u32> {
         let target_index_holder = self.get_index_holder(&copy_documents_request.target_index_name).await?;
-        let target_index_writer = target_index_holder.index_writer_holder()?.clone().read_owned().await;
-        let conflict_strategy = target_index_holder.conflict_strategy();
+        let mut target_index_writer = target_index_holder.index_writer_holder()?.clone().read_owned().await;
+        let conflict_strategy = copy_documents_request
+            .conflict_strategy
+            .and_then(proto::ConflictStrategy::from_i32)
+            .unwrap_or(target_index_holder.conflict_strategy());
         let source_index_holder = self.get_index_holder(&copy_documents_request.source_index_name).await?;
         let searcher = source_index_holder.index_reader().searcher();
         let mut source_documents_receiver = source_index_holder.documents(&searcher, Some)?;
         let mut documents = 0u32;
         while let Some(document) = source_documents_receiver.recv().await {
             target_index_writer
                 .index_document(document, conflict_strategy)
                 .map_err(crate::errors::Error::from)?;
             documents += 1;
-            if documents % 100_000 == 0 {
-                info!(action = "copied", documents = documents)
+            target_index_writer = if documents % 100_000 == 0 {
+                info!(action = "copied", documents = documents);
+                drop(target_index_writer);
+                target_index_holder.index_writer_holder()?.clone().read_owned().await
+            } else {
+                target_index_writer
             }
         }
         Ok(documents)
     }
 
     /// Create consumer and insert it into the consumer registry. Add it to the `IndexHolder` afterwards.
     #[instrument(skip_all, fields(index_name = ?create_index_request.index_name))]
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/services/metrics.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/services/metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/utils/mod.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-server/src/utils/thread_handler.rs` & `summa_embed-0.17.3/local_dependencies/summa-server/src/utils/thread_handler.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.3/local_dependencies/summa-proto/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-proto"
-version = "0.28.0"
+version = "0.28.2"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa search server proto files"
 
 [lib]
 name = "summa_proto"
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.3/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.3/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.3/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.3/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.3/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 
 // Copy documents from one index to another. Their schemes must be compatible
 message CopyDocumentsRequest {
   // Where documents should be taken from
   string source_index_name = 1;
   // Where documents should be copied to
   string target_index_name = 2;
+  // How to deal with conflicts on unique fields. Recommended to set to DoNothing for large updates and maintain uniqueness in your application
+  optional ConflictStrategy conflict_strategy = 3;
 }
 
 // Copy documents response
 message CopyDocumentsResponse {
   double elapsed_secs = 1;
   uint32 copied_documents = 2;
 }
@@ -139,24 +141,30 @@
 enum ConflictStrategy {
   DO_NOTHING = 0;
   OVERWRITE_ALWAYS = 1;
   OVERWRITE = 2;
   MERGE = 3;
 }
 
+message MappedField {
+  string source_field = 1;
+  string target_field = 2;
+}
+
 message IndexAttributes {
   // Timestamp when index has been created
   uint64 created_at = 1;
   // Unique fields of the index. Summa maintains unique constraint on them and uses for deduplicating data
   repeated string unique_fields = 2;
   // Multi fields is ones that may have multiple values and processed as lists. All other fields will be forcefully converted to singular value
   repeated string multi_fields = 4;
   // Text index description
   optional string description = 6;
   ConflictStrategy conflict_strategy = 8;
+  repeated MappedField mapped_fields = 9;
 }
 
 // Request for index creation
 message CreateIndexRequest {
   // Index name
   string index_name = 1;
   // Index engine
@@ -219,14 +227,15 @@
 message GetIndicesResponse {
   repeated string index_names = 1;
 }
 
 message IndexDocumentStreamRequest {
   string index_name = 1;
   repeated bytes documents = 2;
+  optional ConflictStrategy conflict_strategy = 3;
 }
 
 message IndexDocumentStreamResponse {
   double elapsed_secs = 1;
   uint64 success_docs = 2;
   uint64 failed_docs = 3;
 }
```

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.3/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.3/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.3/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/Cargo.toml` & `summa_embed-0.17.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-embed-py"
-version = "0.17.2"
+version = "0.17.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
@@ -13,12 +13,12 @@
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.8"
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.17.2", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
-summa-server = { version = "0.17.2", path = "local_dependencies/summa-server", default_features = false }
+summa-core = { version = "0.17.3", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-server = { version = "0.17.3", path = "local_dependencies/summa-server", default_features = false }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.17.2/.gitignore` & `summa_embed-0.17.3/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.2/src/lib.rs` & `summa_embed-0.17.3/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             if thread_handler.is_some() {
                 return Ok(());
             }
             let server_config_holder = ConfigHolder::from_config(server_config);
             let server = Server::from_server_config(server_config_holder);
             let (sender, receiver) = async_broadcast::broadcast(1);
             let fut = server.serve(receiver).await.unwrap();
-            let join_handle = tokio::spawn(async move { fut.await });
+            let join_handle = tokio::spawn(fut);
             *thread_handler = Some(ThreadHandler::new(join_handle, sender));
             Ok(())
         })
     }
 
     fn stop<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
         let thread_handler = self.thread_handler.clone().lock_owned();
```

### Comparing `summa_embed-0.17.2/Cargo.lock` & `summa_embed-0.17.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,14 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "aes"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "433cfd6710c9986c576a25ca913c39d66a6474107b406f34f91d4a8923395241"
-dependencies = [
- "cfg-if",
- "cipher",
- "cpufeatures",
-]
-
-[[package]]
 name = "ahash"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
  "getrandom",
  "once_cell",
@@ -47,14 +36,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "anstream"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
@@ -63,23 +67,23 @@
  "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
+checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
 version = "1.0.0"
@@ -115,17 +119,17 @@
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8868f09ff8cea88b079da74ae569d9b8c62a23c68c746240b704ee6f7525c89c"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-broadcast"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c48ccdbf6ca6b121e0f586cbc0e73ae440e56c67c30fa0873b4e110d9c26d2b"
 dependencies = [
@@ -148,26 +152,26 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -176,15 +180,15 @@
 name = "axum"
 version = "0.6.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8175979259124331c1d7bf6586ee7e0da434155e4b2d48ec2c8386281d8df39"
 dependencies = [
  "async-trait",
  "axum-core",
- "bitflags",
+ "bitflags 1.3.2",
  "bytes",
  "futures-util",
  "http",
  "http-body",
  "hyper",
  "itoa",
  "matchit",
@@ -232,20 +236,14 @@
 [[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
-name = "base64ct"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
-
-[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
@@ -253,14 +251,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6dbe3c979c178231552ecba20214a8272df4e09f232a87aef4320cf06539aded"
+
+[[package]]
 name = "bitpacking"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8c7d2ac73c167c06af4a5f37e6e59d84148d57ccbe4480b76f0273eefea82d7"
 dependencies = [
  "crunchy",
 ]
@@ -281,39 +285,39 @@
 name = "blake2b_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c2f0dc9a68c6317d884f97cc36cf5a3d20ba14ce404227df55e1af708ab04bc"
 dependencies = [
  "arrayref",
  "arrayvec",
- "constant_time_eq 0.2.6",
+ "constant_time_eq",
 ]
 
 [[package]]
 name = "blake2s_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6637f448b9e61dfadbdcbae9a885fadee1f3eaffb1f8d3c1965d3ade8bdfd44f"
 dependencies = [
  "arrayref",
  "arrayvec",
- "constant_time_eq 0.2.6",
+ "constant_time_eq",
 ]
 
 [[package]]
 name = "blake3"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "729b71f35bd3fa1a4c86b85d32c8b9069ea7fe14f7a53cfabb65f62d4265b888"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if",
- "constant_time_eq 0.2.6",
+ "constant_time_eq",
 ]
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
@@ -336,57 +340,14 @@
 [[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
-name = "bzip2"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
-dependencies = [
- "bzip2-sys",
- "libc",
-]
-
-[[package]]
-name = "bzip2-sys"
-version = "0.1.11+1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "736a955f3fa7875102d57c82b8cac37ec45224a07fd32d58f9f7a186b6cd4cdc"
-dependencies = [
- "cc",
- "libc",
- "pkg-config",
-]
-
-[[package]]
-name = "cached-path"
-version = "0.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "097968e38f1319207f057d0f4d76452e4f4f847a5de61c5215379f297fa034f3"
-dependencies = [
- "flate2",
- "fs2",
- "glob",
- "indicatif",
- "log",
- "rand 0.8.5",
- "reqwest",
- "serde",
- "serde_json",
- "sha2",
- "tar",
- "tempfile",
- "thiserror",
- "zip",
-]
-
-[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 dependencies = [
  "jobserver",
 ]
@@ -400,14 +361,29 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chrono"
+version = "0.4.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
+dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
+ "js-sys",
+ "num-traits",
+ "time 0.1.45",
+ "wasm-bindgen",
+ "winapi",
+]
+
+[[package]]
 name = "cid"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9b68e3193982cd54187d71afdb2a271ad4cf8af157858e9cb911b91321de143"
 dependencies = [
  "core2",
  "multibase",
@@ -426,41 +402,31 @@
  "multibase",
  "multihash 0.18.1",
  "serde",
  "unsigned-varint",
 ]
 
 [[package]]
-name = "cipher"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
-dependencies = [
- "crypto-common",
- "inout",
-]
-
-[[package]]
 name = "clap"
-version = "4.3.4"
+version = "4.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80672091db20273a15cf9fdd4e47ed43b5091ec9841bf4c6145c9dfbbcae09ed"
+checksum = "d9394150f5b4273a1763355bd1c2ec54cc5a2593f790587bcd6b2c947cfa9211"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.4"
+version = "4.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1458a1df40e1e2afebb7ab60ce55c1fa8f431146205aa5f4887e0b111c27636"
+checksum = "9a78fbdd3cc2914ddf37ba444114bc7765bbdcb55ec9cbe6fa054f0137400717"
 dependencies = [
  "anstream",
  "anstyle",
- "bitflags",
+ "bitflags 1.3.2",
  "clap_lex",
  "once_cell",
  "strsim",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -499,43 +465,25 @@
  "serde",
  "serde_json",
  "toml",
  "yaml-rust",
 ]
 
 [[package]]
-name = "console"
-version = "0.15.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
-dependencies = [
- "encode_unicode",
- "lazy_static",
- "libc",
- "windows-sys 0.45.0",
-]
-
-[[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "constant_time_eq"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
-
-[[package]]
-name = "constant_time_eq"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21a53c0a4d288377e7415b53dcfc3c04da5cdc2cc95c8d5ac178b58f0b861ad6"
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
@@ -559,17 +507,17 @@
 checksum = "b49ba7ef1ad6107f8824dbe97de947cbaac53c44e7f9756a1fba0d37c1eec505"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -635,35 +583,14 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "csv"
-version = "1.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "626ae34994d3d8d668f4269922248239db4ae42d538b14c398b74a52208e8086"
-dependencies = [
- "csv-core",
- "itoa",
- "ryu",
- "serde",
-]
-
-[[package]]
-name = "csv-core"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
 dependencies = [
  "darling_core",
  "darling_macro",
@@ -768,35 +695,14 @@
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
- "subtle",
-]
-
-[[package]]
-name = "dirs"
-version = "4.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
-dependencies = [
- "dirs-sys",
-]
-
-[[package]]
-name = "dirs-sys"
-version = "0.3.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
-dependencies = [
- "libc",
- "redox_users",
- "winapi",
 ]
 
 [[package]]
 name = "dlv-list"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0688c2a7f92e427f44895cd63841bff7b29f8d7a1648b9e7e07a4a365b2e1257"
@@ -810,29 +716,14 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
-name = "encode_unicode"
-version = "0.3.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
-
-[[package]]
-name = "encoding_rs"
-version = "0.8.32"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
@@ -856,15 +747,15 @@
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "examples"
 version = "0.0.0"
 dependencies = [
  "serde_json",
- "summa-proto 0.28.0",
+ "summa-proto 0.28.2",
  "tokio",
  "tonic 0.9.2",
 ]
 
 [[package]]
 name = "fail"
 version = "0.5.1"
@@ -949,23 +840,14 @@
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
-name = "form_urlencoded"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
-dependencies = [
- "percent-encoding",
-]
-
-[[package]]
 name = "format-bytes"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48942366ef93975da38e175ac9e10068c6fc08ca9e85930d4f098f4d5b14c2fd"
 dependencies = [
  "format-bytes-macros",
 ]
@@ -1065,15 +947,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1109,17 +991,17 @@
 checksum = "c31b6d751ae2c7f11320402d34e41349dd1016f8d5d45e48c4312bc8625af50c"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "generator"
-version = "0.7.4"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3e123d9ae7c02966b4d892e550bdc32164f05853cd40ab570650ad600596a8a"
+checksum = "5cc16584ff22b460a382b7feec54b23d2908d858152e5739a120b949293bd74e"
 dependencies = [
  "cc",
  "libc",
  "log",
  "rustversion",
  "windows",
 ]
@@ -1139,25 +1021,19 @@
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
- "wasi",
+ "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "glob"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
-
-[[package]]
 name = "h2"
 version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
 dependencies = [
  "bytes",
  "fnv",
@@ -1175,23 +1051,14 @@
 [[package]]
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
-name = "half"
-version = "2.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
-dependencies = [
- "crunchy",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
  "ahash 0.7.6",
 ]
@@ -1208,15 +1075,15 @@
 [[package]]
 name = "headers"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3e372db8e5c0d213e0cd0b9be18be2aca3d44cf2fe30a9d46a65581cd454584"
 dependencies = [
  "base64 0.13.1",
- "bitflags",
+ "bitflags 1.3.2",
  "bytes",
  "headers-core",
  "http",
  "httpdate",
  "mime",
  "sha1",
 ]
@@ -1248,23 +1115,14 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
-name = "hmac"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
-dependencies = [
- "digest",
-]
-
-[[package]]
 name = "htmlescape"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9025058dae765dee5070ec375f591e2ba14638c63feff74f13805a72e523163"
 
 [[package]]
 name = "http"
@@ -1352,67 +1210,59 @@
  "hyper",
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
-name = "ident_case"
-version = "1.0.1"
+name = "iana-time-zone"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows",
+]
 
 [[package]]
-name = "idna"
-version = "0.4.0"
+name = "iana-time-zone-haiku"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "unicode-bidi",
- "unicode-normalization",
+ "cc",
 ]
 
 [[package]]
+name = "ident_case"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
-name = "indicatif"
-version = "0.16.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d207dc617c7a380ab07ff572a6e52fa202a2a8f355860ac9c38e23f8196be1b"
-dependencies = [
- "console",
- "lazy_static",
- "number_prefix",
- "regex",
-]
-
-[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
-name = "inout"
-version = "0.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
  "js-sys",
@@ -1459,20 +1309,14 @@
  "cid 0.10.1",
  "ipfs-hamt-directory",
  "multihash 0.18.1",
  "pyo3",
 ]
 
 [[package]]
-name = "ipnet"
-version = "2.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
-
-[[package]]
 name = "is-terminal"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
@@ -1554,17 +1398,17 @@
 name = "levenshtein_automata"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2cdeb66e45e9f36bfad5bbdb4d2384e70936afbee843c6f6543f0c551ebb25"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libipld"
 version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a20e38e0ad9a2fd600476691fa0780421931a198279985e398a3a0851903e1b2"
 dependencies = [
@@ -1737,24 +1581,14 @@
 [[package]]
 name = "matchit"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b87248edafb776e59e6ee64a79086f65890d3510f2c656c000bf2a7e8a0aea40"
 
 [[package]]
-name = "matrixmultiply"
-version = "0.3.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
-dependencies = [
- "autocfg",
- "rawpointer",
-]
-
-[[package]]
 name = "measure_time"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56220900f1a0923789ecd6bf25fbae8af3b2f1ff3e9e297fc9b6b8674dd4d852"
 dependencies = [
  "instant",
  "log",
@@ -1837,15 +1671,15 @@
 [[package]]
 name = "mio"
 version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "wasi",
+ "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multibase"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1931,27 +1765,14 @@
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
-name = "ndarray"
-version = "0.15.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
-dependencies = [
- "matrixmultiply",
- "num-complex",
- "num-integer",
- "num-traits",
- "rawpointer",
-]
-
-[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -1964,33 +1785,14 @@
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
-name = "num-complex"
-version = "0.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -2023,20 +1825,14 @@
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "number_prefix"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
-
-[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oneshot"
@@ -2045,19 +1841,19 @@
 checksum = "fc22d22931513428ea6cc089e942d38600e3d00976eef8c86de6b8a3aadec6eb"
 dependencies = [
  "loom",
 ]
 
 [[package]]
 name = "openssl"
-version = "0.10.54"
+version = "0.10.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
+checksum = "345df152bc43501c5eb9e4654ff05f794effb78d4efe3d53abc158baddc0703d"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -2066,15 +1862,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -2086,17 +1882,17 @@
 checksum = "efc62c9f12b22b8f5208c23a7200a442b2e5999f8bdf80233852122b5a4f6f37"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.88"
+version = "0.9.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2ce0f250f34a308dcfdbb351f511359857d4ed2134ba715a4eadd46e1ffd617"
+checksum = "374533b0e45f3a7ced10fcaeccca020e66656bc03dac384f852e4e5a7a8104a6"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
@@ -2157,23 +1953,14 @@
  "rand 0.8.5",
  "thiserror",
  "tokio",
  "tokio-stream",
 ]
 
 [[package]]
-name = "ordered-float"
-version = "3.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fc2dbde8f8a79f2102cc474ceb0ad68e3b80b85289ea62389b60e66777e4213"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
 name = "ordered-multimap"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccd746e37177e1711c20dd619a1620f34f5c8b569c53590a72dedd5344d8924a"
 dependencies = [
  "dlv-list",
  "hashbrown 0.12.3",
@@ -2184,15 +1971,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -2234,26 +2021,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.3.5",
  "smallvec",
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "password-hash"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7676374caaee8a325c9e7a2ae557f216c5563a171d6997b0ef8a65af35147700"
-dependencies = [
- "base64ct",
- "rand_core 0.6.4",
- "subtle",
+ "windows-targets",
 ]
 
 [[package]]
 name = "path-absolutize"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43eb3595c63a214e1b37b44f44b0a84900ef7ae0b4c5efce59e123d246d7a0de"
@@ -2273,69 +2049,57 @@
 [[package]]
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
-name = "pbkdf2"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
-dependencies = [
- "digest",
- "hmac",
- "password-hash",
- "sha2",
-]
-
-[[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pest"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
+checksum = "f73935e4d55e2abf7f130186537b19e7a4abc886a0252380b59248af473a3fc9"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b79d4c71c865a25a4322296122e3924d30bc8ee0834c8bfc8b95f7f054afbfb"
+checksum = "aef623c9bbfa0eedf5a0efba11a5ee83209c326653ca31ff019bec3a95bfff2b"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c435bf1076437b851ebc8edc3a18442796b30f1728ffea6262d59bbe28b077e"
+checksum = "b3e8cba4ec22bada7fc55ffe51e2deb6a0e0db2d0b7ab0b103acc80d2510c190"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
+checksum = "a01f71cb40bd8bb94232df14b946909e14660e33fc05db3e50ae2a82d7ea0ca0"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
@@ -2361,15 +2125,15 @@
 name = "pin-project-internal"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -2445,17 +2209,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prometheus"
 version = "0.13.3"
@@ -2767,20 +2531,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
-name = "rawpointer"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
-
-[[package]]
 name = "rayon"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
@@ -2839,35 +2597,24 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
-]
-
-[[package]]
-name = "redox_users"
-version = "0.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
-dependencies = [
- "getrandom",
- "redox_syscall 0.2.16",
- "thiserror",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
@@ -2904,51 +2651,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
-name = "reqwest"
-version = "0.11.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
-dependencies = [
- "base64 0.21.2",
- "bytes",
- "encoding_rs",
- "futures-core",
- "futures-util",
- "h2",
- "http",
- "http-body",
- "hyper",
- "hyper-tls",
- "ipnet",
- "js-sys",
- "log",
- "mime",
- "native-tls",
- "once_cell",
- "percent-encoding",
- "pin-project-lite",
- "serde",
- "serde_json",
- "serde_urlencoded",
- "tokio",
- "tokio-native-tls",
- "tower-service",
- "url",
- "wasm-bindgen",
- "wasm-bindgen-futures",
- "web-sys",
- "winreg",
-]
-
-[[package]]
 name = "rlimit"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8a29d87a652dc4d43c586328706bb5cdff211f3f39a530f240b53f7221dab8e"
 dependencies = [
  "libc",
 ]
@@ -2956,36 +2666,16 @@
 [[package]]
 name = "ron"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88073939a61e5b7680558e6be56b419e208420c2adb92be54921fa6b72283f1a"
 dependencies = [
  "base64 0.13.1",
- "bitflags",
- "serde",
-]
-
-[[package]]
-name = "rust-bert"
-version = "0.21.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8792cccdf842159ef04a35f247df68ccc42192e9a67e389e6cd0f1a83970a6a0"
-dependencies = [
- "cached-path",
- "dirs",
- "half 2.2.1",
- "lazy_static",
- "ordered-float",
- "regex",
- "rust_tokenizers",
+ "bitflags 1.3.2",
  "serde",
- "serde_json",
- "tch",
- "thiserror",
- "uuid",
 ]
 
 [[package]]
 name = "rust-ini"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6d5f2436026b4f6e79dc829837d467cc7e9a55ee40e750d716713540715a2df"
@@ -3014,46 +2704,26 @@
  "filetime",
  "libipld",
  "quick-protobuf",
  "sha2",
 ]
 
 [[package]]
-name = "rust_tokenizers"
-version = "8.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f367f6b13bc686e822237b97caeb4b2e366dd1936ec204f11d266ede402c31b"
-dependencies = [
- "csv",
- "hashbrown 0.13.2",
- "itertools",
- "lazy_static",
- "protobuf",
- "rayon",
- "regex",
- "serde",
- "serde_json",
- "thiserror",
- "unicode-normalization",
- "unicode-normalization-alignments",
-]
-
-[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
 version = "0.37.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
 ]
 
@@ -3066,24 +2736,14 @@
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
-name = "safetensors"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1d818a2cb3f564a1844be835011acf5c7ec8ad1986a47f73abc7b5fea91cc3a"
-dependencies = [
- "serde",
- "serde_json",
-]
-
-[[package]]
 name = "schannel"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
  "windows-sys 0.42.0",
 ]
@@ -3102,15 +2762,15 @@
 
 [[package]]
 name = "security-framework"
 version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
@@ -3154,53 +2814,41 @@
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2bef2ebfde456fb76bbcf9f59315333decc4fda0b2b44b420243c11e0f5ec1f5"
 dependencies = [
- "half 1.8.2",
+ "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "serde_urlencoded"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
-dependencies = [
- "form_urlencoded",
- "itoa",
- "ryu",
- "serde",
-]
-
-[[package]]
 name = "serde_yaml"
 version = "0.8.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578a7433b776b56a35785ed5ce9a7e777ac0598aac5a6dd1b4b18a307c7fc71b"
 dependencies = [
  "indexmap",
  "ryu",
@@ -3217,17 +2865,17 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -3333,27 +2981,22 @@
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
-name = "subtle"
-version = "2.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
-
-[[package]]
 name = "summa-core"
-version = "0.17.2"
+version = "0.17.3"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
+ "chrono",
  "config",
  "derive_builder",
  "downcast-rs",
  "fasteval2",
  "futures",
  "hyper",
  "hyper-tls",
@@ -3367,47 +3010,46 @@
  "pest",
  "pest_derive",
  "pluralize-rs",
  "prost",
  "rand 0.8.5",
  "rayon",
  "regex",
- "rust-bert",
  "rustc-hash",
  "serde",
  "serde_bytes",
  "serde_cbor",
  "serde_json",
  "serde_yaml",
  "strfmt",
- "summa-proto 0.28.0",
+ "summa-proto 0.28.2",
  "take_mut",
  "tantivy",
  "tantivy-common",
  "tantivy-query-grammar",
  "thiserror",
- "time",
+ "time 0.3.22",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.17.2"
+version = "0.17.3"
 dependencies = [
  "async-broadcast",
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "pythonize",
  "serde_json",
  "summa-core",
- "summa-proto 0.28.0",
+ "summa-proto 0.28.2",
  "summa-server",
  "tantivy",
  "tokio",
 ]
 
 [[package]]
 name = "summa-proto"
@@ -3423,30 +3065,30 @@
  "tonic 0.8.3",
  "tonic-build 0.8.4",
  "tonic-reflection 0.6.0",
 ]
 
 [[package]]
 name = "summa-proto"
-version = "0.28.0"
+version = "0.28.2"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
  "tokio",
  "tonic 0.9.2",
  "tonic-build 0.9.2",
  "tonic-reflection 0.9.2",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.17.2"
+version = "0.17.3"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3466,22 +3108,22 @@
  "rdkafka",
  "rlimit",
  "serde",
  "serde_derive",
  "serde_json",
  "serde_yaml",
  "summa-core",
- "summa-proto 0.28.0",
+ "summa-proto 0.28.2",
  "take_mut",
  "tantivy",
  "tantivy-fst",
  "tempdir",
  "thiserror",
  "tikv-jemallocator",
- "time",
+ "time 0.3.22",
  "tokio",
  "tokio-stream",
  "tokio-util",
  "tonic 0.9.2",
  "tonic-build 0.9.2",
  "tonic-reflection 0.9.2",
  "tonic-web",
@@ -3491,29 +3133,29 @@
  "tracing-appender",
  "tracing-futures",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "summa-wasm"
-version = "0.123.8"
+version = "0.124.0"
 dependencies = [
  "async-trait",
  "console_error_panic_hook",
  "futures",
  "getrandom",
  "instant",
  "js-sys",
  "parking_lot 0.12.1",
  "prost",
  "serde",
  "serde-wasm-bindgen",
  "strfmt",
  "summa-core",
- "summa-proto 0.28.0",
+ "summa-proto 0.28.2",
  "tantivy",
  "thiserror",
  "tokio",
  "tracing",
  "tracing-wasm",
  "wasm-bindgen",
  "wasm-bindgen-futures",
@@ -3529,17 +3171,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3565,15 +3207,15 @@
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.20.2"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
@@ -3612,54 +3254,54 @@
  "tantivy-common",
  "tantivy-query-grammar",
  "tantivy-sstable",
  "tantivy-stacker",
  "tantivy-tokenizer-api",
  "tempfile",
  "thiserror",
- "time",
+ "time 0.3.22",
  "tokio",
  "uuid",
  "winapi",
- "zstd 0.12.3+zstd.1.5.2",
+ "zstd",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.4.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
- "time",
+ "time 0.3.22",
 ]
 
 [[package]]
 name = "tantivy-fst"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc3c506b1a8443a3a65352df6382a1fb6a7afe1a02e871cee0d25e2c3d5f3944"
@@ -3668,87 +3310,59 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.20.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
- "zstd 0.12.3+zstd.1.5.2",
+ "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
-name = "tar"
-version = "0.4.38"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b55807c0344e1e6c04d7c965f5289c39a8d94ae23ed5c0b57aabac549f871c6"
-dependencies = [
- "filetime",
- "libc",
- "xattr",
-]
-
-[[package]]
 name = "target-lexicon"
-version = "0.12.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
-
-[[package]]
-name = "tch"
-version = "0.13.0"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cbd9ce6fb581a1b918db880b649d1364b50f7f6717eda8497bcdc929cddd4b9"
-dependencies = [
- "half 2.2.1",
- "lazy_static",
- "libc",
- "ndarray",
- "rand 0.8.5",
- "safetensors",
- "thiserror",
- "torch-sys",
- "zip",
-]
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "tempdir"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15f2b5fb00ccdf689e0149d1b1b3c03fead81c2b37735d812fa8bddbbf41b6d8"
 dependencies = [
@@ -3783,15 +3397,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -3818,14 +3432,25 @@
 dependencies = [
  "libc",
  "tikv-jemalloc-sys",
 ]
 
 [[package]]
 name = "time"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
+dependencies = [
+ "libc",
+ "wasi 0.10.0+wasi-snapshot-preview1",
+ "winapi",
+]
+
+[[package]]
+name = "time"
 version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "js-sys",
  "serde",
@@ -3845,29 +3470,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
-name = "tinyvec"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
-dependencies = [
- "tinyvec_macros",
-]
-
-[[package]]
-name = "tinyvec_macros"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
-
-[[package]]
 name = "tokio"
 version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
@@ -3896,15 +3506,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -4080,26 +3690,14 @@
  "tower-http",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
-name = "torch-sys"
-version = "0.13.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42b2b81a479510717464df1d07c02cb4aebb26539a39b5db6637dda114a476cb"
-dependencies = [
- "anyhow",
- "cc",
- "libc",
- "zip",
-]
-
-[[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
  "futures-core",
  "futures-util",
@@ -4113,19 +3711,19 @@
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "tower-http"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d1d42a9b3f3ec46ba828e8d376aec14592ea199f70a06a548587ecd1c4ab658"
+checksum = "a8bd22a874a2d0b70452d5597b12c537331d49060824a95f49f108994f94aa4c"
 dependencies = [
- "bitflags",
+ "bitflags 2.3.2",
  "bytes",
  "futures-core",
  "futures-util",
  "http",
  "http-body",
  "http-range-header",
  "pin-project-lite",
@@ -4162,27 +3760,27 @@
 [[package]]
 name = "tracing-appender"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09d48f71a791638519505cefafe162606f706c25592e4bde4d97600c0195312e"
 dependencies = [
  "crossbeam-channel",
- "time",
+ "time 0.3.22",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.24"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -4269,44 +3867,20 @@
 [[package]]
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
-name = "unicode-bidi"
-version = "0.3.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
-
-[[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
-name = "unicode-normalization"
-version = "0.1.22"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
-dependencies = [
- "tinyvec",
-]
-
-[[package]]
-name = "unicode-normalization-alignments"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43f613e4fa046e69818dd287fdc4bc78175ff20331479dab6e1b0f98d57062de"
-dependencies = [
- "smallvec",
-]
-
-[[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
 name = "unicode-xid"
@@ -4323,25 +3897,14 @@
 [[package]]
 name = "unsigned-varint"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d86a8dc7f45e4c1b0d30e43038c38f274e77af056aa5f74b93c2cf9eb3c1c836"
 
 [[package]]
-name = "url"
-version = "2.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
-dependencies = [
- "form_urlencoded",
- "idna",
- "percent-encoding",
-]
-
-[[package]]
 name = "urlencoding"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
 
 [[package]]
 name = "utf8-ranges"
@@ -4401,14 +3964,20 @@
 checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
+version = "0.10.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
+
+[[package]]
+name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
 version = "0.2.87"
@@ -4426,15 +3995,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4460,15 +4029,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -4520,15 +4089,15 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
@@ -4540,43 +4109,19 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
@@ -4671,95 +4216,38 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
-name = "winreg"
-version = "0.10.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
-name = "xattr"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d1526bbe5aaeb5eb06885f4d987bcdfa5e23187055de9b83fe00156a821fabc"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
-name = "zip"
-version = "0.6.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
-dependencies = [
- "aes",
- "byteorder",
- "bzip2",
- "constant_time_eq 0.1.5",
- "crc32fast",
- "crossbeam-utils",
- "flate2",
- "hmac",
- "pbkdf2",
- "sha1",
- "time",
- "zstd 0.11.2+zstd.1.5.2",
-]
-
-[[package]]
-name = "zstd"
-version = "0.11.2+zstd.1.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
-dependencies = [
- "zstd-safe 5.0.2+zstd.1.5.2",
-]
-
-[[package]]
 name = "zstd"
 version = "0.12.3+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
- "zstd-safe 6.0.5+zstd.1.5.4",
-]
-
-[[package]]
-name = "zstd-safe"
-version = "5.0.2+zstd.1.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
-dependencies = [
- "libc",
- "zstd-sys",
+ "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
 version = "6.0.5+zstd.1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
```

