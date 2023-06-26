# Comparing `tmp/humlab-penelope-0.7.8.tar.gz` & `tmp/humlab-penelope-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humlab-penelope-0.7.8.tar", max compression
+gzip compressed data, was "humlab-penelope-0.7.9.tar", max compression
```

## Comparing `humlab-penelope-0.7.8.tar` & `humlab-penelope-0.7.9.tar`

### file list

```diff
@@ -1,321 +1,320 @@
--rw-r--r--   0        0        0     3120 2021-06-17 19:02:19.461226 humlab-penelope-0.7.8/README.md
--rw-r--r--   0        0        0        0 2021-05-31 13:11:35.004419 humlab-penelope-0.7.8/penelope/__init__.py
--rw-r--r--   0        0        0      852 2021-07-03 19:31:04.069680 humlab-penelope-0.7.8/penelope/co_occurrence/__init__.py
--rw-r--r--   0        0        0     6106 2022-03-19 22:19:07.342898 humlab-penelope-0.7.8/penelope/co_occurrence/bundle.py
--rw-r--r--   0        0        0     3966 2022-03-19 22:19:07.342898 humlab-penelope-0.7.8/penelope/co_occurrence/convert.py
--rw-r--r--   0        0        0      199 2021-03-15 20:15:14.950000 humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/__init__.py
--rw-r--r--   0        0        0     2832 2021-05-05 09:47:36.605567 humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/co_occurrence_ui.py
--rw-r--r--   0        0        0     4333 2022-03-19 22:19:07.342898 humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/compute_hal_or_glove.py
--rw-r--r--   0        0        0     2822 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/vectorizer_glove.py
--rw-r--r--   0        0        0    10216 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/vectorizer_hal.py
--rw-r--r--   0        0        0     1445 2021-07-05 19:47:05.125302 humlab-penelope-0.7.8/penelope/co_occurrence/interface.py
--rw-r--r--   0        0        0     4046 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/co_occurrence/keyness.py
--rw-r--r--   0        0        0    13039 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/co_occurrence/persistence.py
--rw-r--r--   0        0        0     9407 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/co_occurrence/prepare.py
--rw-r--r--   0        0        0     5924 2022-01-01 10:42:06.496740 humlab-penelope-0.7.8/penelope/co_occurrence/utility.py
--rw-r--r--   0        0        0     5531 2022-03-18 07:12:53.399367 humlab-penelope-0.7.8/penelope/co_occurrence/vectorize.py
--rw-r--r--   0        0        0     6516 2021-09-28 12:56:00.310009 humlab-penelope-0.7.8/penelope/co_occurrence/windows.py
--rw-r--r--   0        0        0        0 2021-03-15 20:15:16.140000 humlab-penelope-0.7.8/penelope/common/__init__.py
--rw-r--r--   0        0        0    10786 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/common/cluster_analysis.py
--rw-r--r--   0        0        0     3570 2021-04-23 12:36:52.077472 humlab-penelope-0.7.8/penelope/common/curve_fit.py
--rw-r--r--   0        0        0     3199 2021-12-16 06:16:48.006294 humlab-penelope-0.7.8/penelope/common/distance_metrics.py
--rw-r--r--   0        0        0    10576 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/common/goodness_of_fit.py
--rw-r--r--   0        0        0      269 2021-06-29 11:52:45.258960 humlab-penelope-0.7.8/penelope/common/keyness/__init__.py
--rw-r--r--   0        0        0     4762 2021-06-30 13:45:43.936217 humlab-penelope-0.7.8/penelope/common/keyness/hal_cwr.py
--rw-r--r--   0        0        0    15269 2021-12-16 06:17:38.226294 humlab-penelope-0.7.8/penelope/common/keyness/metrics.py
--rw-r--r--   0        0        0      833 2022-03-19 22:19:07.352898 humlab-penelope-0.7.8/penelope/common/mdw.py
--rw-r--r--   0        0        0     1193 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/common/pca_analysis.py
--rw-r--r--   0        0        0     2011 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/corpus/__init__.py
--rw-r--r--   0        0        0      706 2021-12-16 09:49:19.674955 humlab-penelope-0.7.8/penelope/corpus/corpus_mixins.py
--rw-r--r--   0        0        0    29102 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/corpus/document_index.py
--rw-r--r--   0        0        0      657 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/corpus/dtm/__init__.py
--rw-r--r--   0        0        0     5516 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/corpus/dtm/convert.py
--rw-r--r--   0        0        0    19466 2022-03-31 05:32:11.801817 humlab-penelope-0.7.8/penelope/corpus/dtm/corpus.py
--rw-r--r--   0        0        0    17258 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/corpus/dtm/group.py
--rw-r--r--   0        0        0     6872 2022-01-06 14:07:28.867693 humlab-penelope-0.7.8/penelope/corpus/dtm/interface.py
--rw-r--r--   0        0        0     1127 2021-10-03 02:14:00.280348 humlab-penelope-0.7.8/penelope/corpus/dtm/optimize.py
--rw-r--r--   0        0        0     8951 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/corpus/dtm/slice.py
--rw-r--r--   0        0        0     7291 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/corpus/dtm/stats.py
--rw-r--r--   0        0        0    12234 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/corpus/dtm/store.py
--rw-r--r--   0        0        0    11820 2022-03-19 22:19:07.362898 humlab-penelope-0.7.8/penelope/corpus/dtm/ttm.py
--rw-r--r--   0        0        0     7194 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/dtm/ttm_legacy.py
--rw-r--r--   0        0        0     9372 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/dtm/vectorizer.py
--rw-r--r--   0        0        0      939 2021-05-30 17:44:38.579000 humlab-penelope-0.7.8/penelope/corpus/interfaces.py
--rw-r--r--   0        0        0      629 2021-12-16 05:30:08.136294 humlab-penelope-0.7.8/penelope/corpus/readers/__init__.py
--rw-r--r--   0        0        0     6306 2022-01-01 10:42:06.496740 humlab-penelope-0.7.8/penelope/corpus/readers/interfaces.py
--rw-r--r--   0        0        0      849 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/readers/pandas_reader.py
--rw-r--r--   0        0        0     1397 2022-01-02 10:25:24.845131 humlab-penelope-0.7.8/penelope/corpus/readers/sparv_csv_tokenizer.py
--rw-r--r--   0        0        0     2793 2022-01-02 10:25:15.785131 humlab-penelope-0.7.8/penelope/corpus/readers/sparv_xml_tokenizer.py
--rw-r--r--   0        0        0     1777 2021-06-09 09:16:27.941029 humlab-penelope-0.7.8/penelope/corpus/readers/streamify_text_source.py
--rw-r--r--   0        0        0     5191 2021-12-16 05:30:08.136294 humlab-penelope-0.7.8/penelope/corpus/readers/text_reader.py
--rw-r--r--   0        0        0     2826 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/corpus/readers/text_tokenizer.py
--rw-r--r--   0        0        0     2575 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/readers/text_transformer.py
--rw-r--r--   0        0        0      344 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/readers/tng/__init__.py
--rw-r--r--   0        0        0     1672 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/readers/tng/factory.py
--rw-r--r--   0        0        0     1910 2021-03-15 20:15:15.770000 humlab-penelope-0.7.8/penelope/corpus/readers/tng/interfaces.py
--rw-r--r--   0        0        0     3872 2021-03-25 11:18:12.894717 humlab-penelope-0.7.8/penelope/corpus/readers/tng/reader.py
--rw-r--r--   0        0        0     6063 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/readers/tng/sources.py
--rw-r--r--   0        0        0     2603 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/readers/tng/transformer.py
--rw-r--r--   0        0        0     2574 2021-06-09 09:16:27.941029 humlab-penelope-0.7.8/penelope/corpus/readers/zip_iterator.py
--rw-r--r--   0        0        0     3297 2021-06-09 09:16:27.941029 humlab-penelope-0.7.8/penelope/corpus/segmented_text_corpus.py
--rw-r--r--   0        0        0      358 2021-03-15 20:15:15.630000 humlab-penelope-0.7.8/penelope/corpus/sparv/NOTES.md
--rw-r--r--   0        0        0        0 2021-03-15 20:15:15.650000 humlab-penelope-0.7.8/penelope/corpus/sparv/__init__.py
--rw-r--r--   0        0        0     1528 2021-03-25 11:18:12.894717 humlab-penelope-0.7.8/penelope/corpus/sparv/parlaclarin_test.xslt
--rw-r--r--   0        0        0     4072 2021-12-16 05:30:08.146294 humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_csv_to_text.py
--rw-r--r--   0        0        0     1587 2021-03-15 20:15:15.640000 humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_extract.v3.xslt
--rw-r--r--   0        0        0     1594 2021-04-16 12:53:17.751957 humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_extract.xslt
--rw-r--r--   0        0        0     1617 2021-09-02 09:51:35.687334 humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_csv.py
--rw-r--r--   0        0        0     1587 2021-03-15 20:15:15.630000 humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_csv.v3.xslt
--rw-r--r--   0        0        0      708 2021-03-15 20:15:15.630000 humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_csv.xslt
--rw-r--r--   0        0        0     2252 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_text.py
--rw-r--r--   0        0        0     4782 2022-01-02 10:25:49.225131 humlab-penelope-0.7.8/penelope/corpus/sparv_corpus.py
--rw-r--r--   0        0        0     1327 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/store_corpus.py
--rw-r--r--   0        0        0     2395 2021-05-30 17:44:39.106000 humlab-penelope-0.7.8/penelope/corpus/text_lines_corpus.py
--rw-r--r--   0        0        0    14176 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/token2id.py
--rw-r--r--   0        0        0     4921 2021-12-26 18:21:25.500488 humlab-penelope-0.7.8/penelope/corpus/tokenized_corpus.py
--rw-r--r--   0        0        0     7400 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/corpus/tokens_transformer.py
--rw-r--r--   0        0        0     6091 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/corpus/transforms.py
--rw-r--r--   0        0        0     2205 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/corpus/utils.py
--rw-r--r--   0        0        0     2980 2022-03-19 22:19:07.372898 humlab-penelope-0.7.8/penelope/ner/stagger_wrapper.py
--rw-r--r--   0        0        0      131 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/__init__.py
--rw-r--r--   0        0        0     4493 2022-03-29 07:29:11.093472 humlab-penelope-0.7.8/penelope/network/bipartite_plot.py
--rw-r--r--   0        0        0        0 2021-03-15 20:15:16.210000 humlab-penelope-0.7.8/penelope/network/graphtool/__init__.py
--rw-r--r--   0        0        0     2395 2021-06-09 09:16:27.951029 humlab-penelope-0.7.8/penelope/network/graphtool/layout.py
--rw-r--r--   0        0        0     1693 2021-06-09 09:16:27.951029 humlab-penelope-0.7.8/penelope/network/graphtool/plot.py
--rw-r--r--   0        0        0     4733 2021-06-09 09:16:27.951029 humlab-penelope-0.7.8/penelope/network/graphtool/utility.py
--rw-r--r--   0        0        0       22 2021-03-15 20:15:16.200000 humlab-penelope-0.7.8/penelope/network/graphviz/__init__.py
--rw-r--r--   0        0        0     1011 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/graphviz/layout.py
--rw-r--r--   0        0        0      406 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/interface.py
--rw-r--r--   0        0        0     1592 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/layout.py
--rw-r--r--   0        0        0     2203 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/layout_source.py
--rw-r--r--   0        0        0     2146 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/metrics.py
--rw-r--r--   0        0        0       34 2021-03-15 20:15:16.280000 humlab-penelope-0.7.8/penelope/network/networkx/__init__.py
--rw-r--r--   0        0        0     1802 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/networkx/layout.py
--rw-r--r--   0        0        0      808 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/networkx/networkx_api.py
--rw-r--r--   0        0        0     1524 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/networkx/plot.py
--rw-r--r--   0        0        0    10015 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/networkx/utility.py
--rw-r--r--   0        0        0     8070 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/plot.py
--rw-r--r--   0        0        0     6122 2022-03-19 22:19:07.392898 humlab-penelope-0.7.8/penelope/network/plot_utility.py
--rw-r--r--   0        0        0        0 2021-03-15 20:15:15.400000 humlab-penelope-0.7.8/penelope/notebook/__init__.py
--rw-r--r--   0        0        0        0 2021-03-15 20:15:15.440000 humlab-penelope-0.7.8/penelope/notebook/cluster_analysis/__init__.py
--rw-r--r--   0        0        0    12497 2022-03-19 22:19:07.402898 humlab-penelope-0.7.8/penelope/notebook/cluster_analysis/cluster_analysis_gui.py
--rw-r--r--   0        0        0     8195 2022-03-19 22:19:07.402898 humlab-penelope-0.7.8/penelope/notebook/cluster_analysis/cluster_plot.py
--rw-r--r--   0        0        0     2900 2022-03-19 22:19:07.402898 humlab-penelope-0.7.8/penelope/notebook/cluster_analysis/plot.py
--rw-r--r--   0        0        0      320 2021-06-09 09:16:27.951029 humlab-penelope-0.7.8/penelope/notebook/co_occurrence/__init__.py
--rw-r--r--   0        0        0     2525 2022-03-19 22:19:07.402898 humlab-penelope-0.7.8/penelope/notebook/co_occurrence/explore_co_occurrence_gui.py
--rw-r--r--   0        0        0     4991 2022-03-19 22:19:07.402898 humlab-penelope-0.7.8/penelope/notebook/co_occurrence/load_co_occurrences_gui.py
--rw-r--r--   0        0        0     3580 2022-03-19 22:19:07.422898 humlab-penelope-0.7.8/penelope/notebook/co_occurrence/main_gui.py
--rw-r--r--   0        0        0    15685 2022-03-19 22:19:07.422898 humlab-penelope-0.7.8/penelope/notebook/co_occurrence/tabular_gui.py
--rw-r--r--   0        0        0     5795 2022-03-19 22:19:07.422898 humlab-penelope-0.7.8/penelope/notebook/co_occurrence/to_co_occurrence_gui.py
--rw-r--r--   0        0        0      121 2021-03-15 20:15:15.160000 humlab-penelope-0.7.8/penelope/notebook/dtm/__init__.py
--rw-r--r--   0        0        0     4616 2022-03-19 22:19:07.422898 humlab-penelope-0.7.8/penelope/notebook/dtm/load_dtm_gui.py
--rw-r--r--   0        0        0     1447 2021-12-29 21:26:21.105642 humlab-penelope-0.7.8/penelope/notebook/dtm/to_dtm_gui.py
--rw-r--r--   0        0        0     2381 2022-03-19 22:19:07.432898 humlab-penelope-0.7.8/penelope/notebook/grid_utility.py
--rw-r--r--   0        0        0    19489 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/gui_base.py
--rw-r--r--   0        0        0       98 2021-03-15 20:15:15.420000 humlab-penelope-0.7.8/penelope/notebook/mdw/__init__.py
--rw-r--r--   0        0        0     1009 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/mdw/main_gui.py
--rw-r--r--   0        0        0     4432 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/mdw/mdw_gui.py
--rw-r--r--   0        0        0     8282 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/notebook/mixins.py
--rw-r--r--   0        0        0      176 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/token_counts/__init__.py
--rw-r--r--   0        0        0    13648 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/token_counts/dtm_gui.py
--rw-r--r--   0        0        0     9996 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/token_counts/pipeline_gui.py
--rw-r--r--   0        0        0     3672 2022-03-29 07:25:59.863472 humlab-penelope-0.7.8/penelope/notebook/token_counts/plot.py
--rw-r--r--   0        0        0     1531 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/__init__.py
--rw-r--r--   0        0        0     2663 2022-03-19 22:19:07.442898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/edit_topic_labels_gui.py
--rw-r--r--   0        0        0     4428 2022-03-23 16:03:00.200622 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/load_topic_model_gui.py
--rw-r--r--   0        0        0     8472 2022-03-19 22:19:07.462898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/mixins.py
--rw-r--r--   0        0        0     2973 2022-03-19 22:19:07.462898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/model_container.py
--rw-r--r--   0        0        0    11376 2022-03-19 22:19:07.462898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/pivot_network_gui.py
--rw-r--r--   0        0        0    10657 2022-03-19 22:19:07.462898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_document_network_gui.py
--rw-r--r--   0        0        0    10319 2022-03-19 22:19:07.462898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_documents_gui.py
--rw-r--r--   0        0        0    16321 2022-03-19 22:19:07.462898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_model_gui.py
--rw-r--r--   0        0        0     3859 2022-03-19 22:19:07.462898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_titles_gui.py
--rw-r--r--   0        0        0    11500 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_topic_network_gui.py
--rw-r--r--   0        0        0     1466 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_topic_network_gui_utility.py
--rw-r--r--   0        0        0     7439 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_gui.py
--rw-r--r--   0        0        0     1296 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_gui_utility.py
--rw-r--r--   0        0        0     7148 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_overview_gui.py
--rw-r--r--   0        0        0     4824 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_overview_gui_utility.py
--rw-r--r--   0        0        0     5089 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_word_distribution_gui.py
--rw-r--r--   0        0        0     3522 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_wordcloud_gui.py
--rw-r--r--   0        0        0    20033 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topics_token_network_gui.py
--rw-r--r--   0        0        0    16749 2022-03-31 00:27:57.529621 humlab-penelope-0.7.8/penelope/notebook/topic_modelling/train_gui/topic_model_gui.py
--rw-r--r--   0        0        0     7203 2022-03-19 22:19:07.472898 humlab-penelope-0.7.8/penelope/notebook/utility.py
--rw-r--r--   0        0        0     5049 2022-03-19 22:19:07.482898 humlab-penelope-0.7.8/penelope/notebook/widgets_utils.py
--rw-r--r--   0        0        0      424 2022-03-19 22:19:07.482898 humlab-penelope-0.7.8/penelope/notebook/word_trends/__init__.py
--rw-r--r--   0        0        0      793 2022-03-19 22:19:07.482898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/__init__.py
--rw-r--r--   0        0        0     3668 2022-03-19 22:19:07.482898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/archive/compile_mixins.py
--rw-r--r--   0        0        0    10578 2022-03-19 22:19:07.492898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/archive/deprecated_plot.py
--rw-r--r--   0        0        0      671 2022-03-19 22:19:07.492898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/archive/display_top_table2.py
--rw-r--r--   0        0        0     2474 2022-03-19 22:19:07.492898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_bar.py
--rw-r--r--   0        0        0     3324 2022-03-19 22:19:07.492898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_line.py
--rw-r--r--   0        0        0     9611 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_network.py
--rw-r--r--   0        0        0     1973 2022-03-19 22:19:07.492898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_stackedbar.py
--rw-r--r--   0        0        0     2759 2022-03-19 22:19:07.492898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_table.py
--rw-r--r--   0        0        0    10408 2022-03-19 22:19:07.492898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_top_table.py
--rw-r--r--   0        0        0      842 2022-03-19 22:19:07.502898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/interface.py
--rw-r--r--   0        0        0     5261 2022-03-19 22:19:07.502898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/plotter.py
--rw-r--r--   0        0        0     2364 2022-03-19 22:19:07.502898 humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/utils.py
--rw-r--r--   0        0        0     1235 2022-03-19 22:19:07.502898 humlab-penelope-0.7.8/penelope/notebook/word_trends/gof_and_trends_gui.py
--rw-r--r--   0        0        0     1671 2022-03-19 22:19:07.502898 humlab-penelope-0.7.8/penelope/notebook/word_trends/gofs_gui.py
--rw-r--r--   0        0        0     7421 2022-03-19 22:19:07.512898 humlab-penelope-0.7.8/penelope/notebook/word_trends/interface.py
--rw-r--r--   0        0        0     3457 2022-03-19 22:19:07.512898 humlab-penelope-0.7.8/penelope/notebook/word_trends/main_gui.py
--rw-r--r--   0        0        0    16567 2022-03-19 22:19:07.512898 humlab-penelope-0.7.8/penelope/notebook/word_trends/trends_gui.py
--rw-r--r--   0        0        0     8524 2022-03-19 22:19:07.512898 humlab-penelope-0.7.8/penelope/notebook/word_trends/trends_with_picks_gui.py
--rw-r--r--   0        0        0     1123 2022-02-10 06:55:17.682926 humlab-penelope-0.7.8/penelope/pipeline/__init__.py
--rw-r--r--   0        0        0      468 2021-09-28 07:35:39.360009 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/__init__.py
--rw-r--r--   0        0        0     8433 2022-03-19 22:19:07.512898 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/checkpoint.py
--rw-r--r--   0        0        0     3508 2022-03-19 22:19:07.522898 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/feather.py
--rw-r--r--   0        0        0     3531 2022-03-19 22:19:07.522898 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/interface.py
--rw-r--r--   0        0        0     2852 2021-07-09 20:15:23.442229 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/legacy.py
--rw-r--r--   0        0        0     5238 2022-03-19 22:19:07.522898 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/load.py
--rw-r--r--   0        0        0     3039 2022-03-19 22:19:07.522898 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/serialize.py
--rw-r--r--   0        0        0     1483 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/pipeline/checkpoint/utility.py
--rw-r--r--   0        0        0      146 2021-06-09 09:16:27.981029 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/__init__.py
--rw-r--r--   0        0        0     5738 2022-03-19 22:19:07.522898 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/builder.py
--rw-r--r--   0        0        0       15 2021-06-09 09:16:27.981029 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/legacy/__init__.py
--rw-r--r--   0        0        0     1198 2021-12-28 21:06:58.133459 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/legacy/pipelines.py
--rw-r--r--   0        0        0     5066 2021-12-16 06:32:55.786294 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/legacy/tasks.py
--rw-r--r--   0        0        0     1126 2021-12-16 11:13:12.674955 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/pipeline_mixin.py
--rw-r--r--   0        0        0     1467 2021-12-28 21:06:58.133459 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/pipelines.py
--rw-r--r--   0        0        0    11543 2022-03-19 22:19:07.522898 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/tasks.py
--rw-r--r--   0        0        0     4443 2022-03-19 22:19:07.522898 humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/tasks_pool.py
--rw-r--r--   0        0        0     8610 2022-03-19 22:19:07.542898 humlab-penelope-0.7.8/penelope/pipeline/config.py
--rw-r--r--   0        0        0    11856 2022-03-19 22:19:07.542898 humlab-penelope-0.7.8/penelope/pipeline/convert.py
--rw-r--r--   0        0        0        0 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/pipeline/dtm/__init__.py
--rw-r--r--   0        0        0      649 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/pipeline/dtm/pipeline_mixin.py
--rw-r--r--   0        0        0     2167 2022-01-01 10:42:06.496740 humlab-penelope-0.7.8/penelope/pipeline/dtm/pipelines.py
--rw-r--r--   0        0        0     1926 2022-01-05 23:10:42.092085 humlab-penelope-0.7.8/penelope/pipeline/dtm/tasks.py
--rw-r--r--   0        0        0     3530 2022-03-19 22:19:07.542898 humlab-penelope-0.7.8/penelope/pipeline/dtm/vectorizer.py
--rw-r--r--   0        0        0    14153 2022-03-19 22:19:07.542898 humlab-penelope-0.7.8/penelope/pipeline/interfaces.py
--rw-r--r--   0        0        0        0 2021-07-08 20:06:07.056481 humlab-penelope-0.7.8/penelope/pipeline/multiprocess/__init__.py
--rw-r--r--   0        0        0     3251 2022-03-19 22:19:07.542898 humlab-penelope-0.7.8/penelope/pipeline/phrases.py
--rw-r--r--   0        0        0     5024 2021-10-04 16:48:51.788710 humlab-penelope-0.7.8/penelope/pipeline/pipeline.py
--rw-r--r--   0        0        0     8676 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/pipeline/pipeline_mixin.py
--rw-r--r--   0        0        0     1470 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/pipeline/pipelines.py
--rw-r--r--   0        0        0      112 2022-02-10 06:53:54.312926 humlab-penelope-0.7.8/penelope/pipeline/spacy/__init__.py
--rw-r--r--   0        0        0     3986 2022-03-19 22:19:07.542898 humlab-penelope-0.7.8/penelope/pipeline/spacy/convert.py
--rw-r--r--   0        0        0     1629 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/pipeline/spacy/pipeline_mixin.py
--rw-r--r--   0        0        0     4562 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/pipeline/spacy/pipelines.py
--rw-r--r--   0        0        0     3618 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/pipeline/spacy/tasks.py
--rw-r--r--   0        0        0      127 2021-09-02 09:55:30.257334 humlab-penelope-0.7.8/penelope/pipeline/sparv/__init__.py
--rw-r--r--   0        0        0     1893 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/pipeline/sparv/convert.py
--rw-r--r--   0        0        0     1520 2022-01-01 10:42:06.496740 humlab-penelope-0.7.8/penelope/pipeline/sparv/pipelines.py
--rw-r--r--   0        0        0     8149 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/pipeline/tagged_frame.py
--rw-r--r--   0        0        0    27737 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/pipeline/tasks.py
--rw-r--r--   0        0        0     5498 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/pipeline/tasks_mixin.py
--rw-r--r--   0        0        0       15 2021-09-27 10:08:55.933176 humlab-penelope-0.7.8/penelope/pipeline/topic_model/__init__.py
--rw-r--r--   0        0        0     3258 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/pipeline/topic_model/pipeline_mixin.py
--rw-r--r--   0        0        0     4317 2022-01-06 11:32:55.227693 humlab-penelope-0.7.8/penelope/pipeline/topic_model/pipelines.py
--rw-r--r--   0        0        0    13413 2022-03-23 16:03:00.210622 humlab-penelope-0.7.8/penelope/pipeline/topic_model/tasks.py
--rw-r--r--   0        0        0      100 2021-03-15 20:15:15.960000 humlab-penelope-0.7.8/penelope/plot/__init__.py
--rw-r--r--   0        0        0      689 2021-03-15 20:15:15.950000 humlab-penelope-0.7.8/penelope/plot/colors.py
--rw-r--r--   0        0        0     1017 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/plot/wordcloud_utility.py
--rw-r--r--   0        0        0       41 2021-03-15 20:15:16.150000 humlab-penelope-0.7.8/penelope/resources/__init__.py
--rw-r--r--   0        0        0     5417 2021-03-15 20:15:16.150000 humlab-penelope-0.7.8/penelope/resources/fox_stopwords.py
--rw-r--r--   0        0        0        0 2021-03-15 20:15:15.070000 humlab-penelope-0.7.8/penelope/scripts/__init__.py
--rw-r--r--   0        0        0     7499 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/scripts/co_occurrence.py
--rwxr-xr-x   0        0        0     1437 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/scripts/co_occurrence.sh
--rw-r--r--   0        0        0        0 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/scripts/dtm/__init__.py
--rw-r--r--   0        0        0     6581 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/scripts/dtm/vectorize.py
--rw-r--r--   0        0        0     6072 2022-03-19 22:19:07.552898 humlab-penelope-0.7.8/penelope/scripts/dtm/vectorize_id.py
--rw-r--r--   0        0        0     2958 2021-12-29 21:26:21.105642 humlab-penelope-0.7.8/penelope/scripts/legacy/coherence.py
--rw-r--r--   0        0        0     1439 2021-12-29 21:26:21.105642 humlab-penelope-0.7.8/penelope/scripts/legacy/install-spacy-models.sh
--rw-r--r--   0        0        0      187 2021-09-22 10:58:18.745079 humlab-penelope-0.7.8/penelope/scripts/legacy/post-install.sh
--rw-r--r--   0        0        0     3410 2022-03-19 22:19:07.562898 humlab-penelope-0.7.8/penelope/scripts/legacy/sparv-xml-extract-text.py
--rw-r--r--   0        0        0      635 2022-03-19 22:19:07.562898 humlab-penelope-0.7.8/penelope/scripts/pos_tag.py
--rw-r--r--   0        0        0        0 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/scripts/tm/__init__.py
--rw-r--r--   0        0        0      976 2022-03-19 22:19:07.562898 humlab-penelope-0.7.8/penelope/scripts/tm/mallet2topicsdata.py
--rw-r--r--   0        0        0     4716 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/scripts/tm/predict.py
--rw-r--r--   0        0        0     8208 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/scripts/tm/train.py
--rw-r--r--   0        0        0     7202 2022-03-23 16:03:00.210622 humlab-penelope-0.7.8/penelope/scripts/tm/train_id.py
--rw-r--r--   0        0        0     4714 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/scripts/tm/train_legacy.py
--rw-r--r--   0        0        0     8971 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/scripts/utils.py
--rw-r--r--   0        0        0      887 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/__init__.py
--rw-r--r--   0        0        0     1053 2021-12-26 18:21:25.500488 humlab-penelope-0.7.8/penelope/topic_modelling/engines/__init__.py
--rw-r--r--   0        0        0     3071 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/__init__.py
--rw-r--r--   0        0        0     2125 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/coherence.py
--rw-r--r--   0        0        0     9162 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/convert.py
--rw-r--r--   0        0        0    13444 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/options.py
--rw-r--r--   0        0        0     3105 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/predict.py
--rw-r--r--   0        0        0     2952 2022-01-23 12:51:56.726124 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/train.py
--rw-r--r--   0        0        0     1959 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/utility.py
--rw-r--r--   0        0        0     2090 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_textacy/__init__.py
--rw-r--r--   0        0        0     1187 2022-03-19 22:19:07.572898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_textacy/predict.py
--rw-r--r--   0        0        0     2138 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_textacy/train.py
--rw-r--r--   0        0        0     4692 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/engines/interface.py
--rw-r--r--   0        0        0     9010 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/interfaces.py
--rw-r--r--   0        0        0     3951 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/predict.py
--rw-r--r--   0        0        0        0 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/rdb/__init__.py
--rw-r--r--   0        0        0     1572 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/rdb/data.py
--rw-r--r--   0        0        0      126 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/saliency/__init__.py
--rw-r--r--   0        0        0     2533 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/saliency/saliency.py
--rw-r--r--   0        0        0     1329 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/__init__.py
--rw-r--r--   0        0        0    11439 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/document.py
--rw-r--r--   0        0        0     8639 2022-03-19 22:19:07.582898 humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/prevelance.py
--rw-r--r--   0        0        0     5715 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/token.py
--rw-r--r--   0        0        0    16433 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/topics_data.py
--rw-r--r--   0        0        0      734 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/topic_modelling/train.py
--rw-r--r--   0        0        0      804 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/topic_modelling/utility.py
--rw-r--r--   0        0        0      884 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/type_alias.py
--rw-r--r--   0        0        0     4395 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/utility/__init__.py
--rw-r--r--   0        0        0     4397 2021-03-15 20:15:15.030000 humlab-penelope-0.7.8/penelope/utility/_color_utility.py
--rw-r--r--   0        0        0     3728 2021-06-21 13:22:46.611091 humlab-penelope-0.7.8/penelope/utility/_decorators.py
--rw-r--r--   0        0        0     6584 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/utility/file_utility.py
--rw-r--r--   0        0        0     3475 2021-06-09 09:16:28.001029 humlab-penelope-0.7.8/penelope/utility/filename_fields.py
--rw-r--r--   0        0        0     5135 2021-10-11 06:46:17.330209 humlab-penelope-0.7.8/penelope/utility/filename_utils.py
--rw-r--r--   0        0        0    17789 2022-03-23 16:03:00.210622 humlab-penelope-0.7.8/penelope/utility/pandas_utils.py
--rw-r--r--   0        0        0     1279 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/utility/paths.py
--rw-r--r--   0        0        0    12216 2022-01-01 10:42:06.506740 humlab-penelope-0.7.8/penelope/utility/pos_tags.py
--rw-r--r--   0        0        0     5897 2021-09-27 10:08:55.943176 humlab-penelope-0.7.8/penelope/utility/streamify_source.py
--rw-r--r--   0        0        0    18421 2022-03-19 22:19:07.592898 humlab-penelope-0.7.8/penelope/utility/utils.py
--rw-r--r--   0        0        0     3942 2021-06-09 09:16:28.011029 humlab-penelope-0.7.8/penelope/utility/zip_utils.py
--rw-r--r--   0        0        0        0 2021-03-15 20:15:16.460000 humlab-penelope-0.7.8/penelope/vendor/__init__.py
--rw-r--r--   0        0        0        0 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/archive/stanza/__init__.py
--rw-r--r--   0        0        0      743 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/archive/stanza/utility.py
--rw-r--r--   0        0        0      206 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/archive/textacy_pipeline/__init__.py
--rw-r--r--   0        0        0     6819 2022-03-31 13:37:03.338700 humlab-penelope-0.7.8/penelope/vendor/archive/textacy_pipeline/pipeline.py
--rw-r--r--   0        0        0      201 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/__init__.py
--rw-r--r--   0        0        0      252 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/__init__.py
--rw-r--r--   0        0        0     7598 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/_corpus.py
--rw-r--r--   0        0        0      894 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/_models.py
--rw-r--r--   0        0        0       74 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/README.md
--rw-r--r--   0        0        0      458 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/__init__.py
--rw-r--r--   0        0        0    21674 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/dtmmodel.py.txt
--rw-r--r--   0        0        0     1369 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/fasttext.py.txt
--rw-r--r--   0        0        0    28452 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/ldavowpalwabbit.py.txt
--rw-r--r--   0        0        0     4737 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/varembed.py.txt
--rw-r--r--   0        0        0    13731 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/wordrank.py.txt
--rw-r--r--   0        0        0    28870 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/ldamallet.py
--rw-r--r--   0        0        0     6292 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/mallet_tm.py
--rw-r--r--   0        0        0    11062 2022-03-19 22:19:07.602898 humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/sttm_tm.py
--rw-r--r--   0        0        0      182 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/mallet_api/__init__.py
--rw-r--r--   0        0        0     6889 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/mallet_api/convert.py
--rw-r--r--   0        0        0     1246 2021-04-28 09:36:47.725900 humlab-penelope-0.7.8/penelope/vendor/nltk/__init__.py
--rw-r--r--   0        0        0     5505 2021-03-15 20:15:16.390000 humlab-penelope-0.7.8/penelope/vendor/nltk/extra_stopwords.py
--rw-r--r--   0        0        0      477 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/spacy_api/__init__.py
--rw-r--r--   0        0        0     6504 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/spacy_api/_spacy.py
--rw-r--r--   0        0        0      635 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/textacy_api/__init__.py
--rw-r--r--   0        0        0      808 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/__init__.py
--rw-r--r--   0        0        0     1172 2022-03-31 13:45:33.018700 humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/__pycache__/fallbacks.cpython-39.pyc
--rw-r--r--   0        0        0     8066 2022-03-31 13:45:33.018700 humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/__pycache__/mdw_modified.cpython-39.pyc
--rw-r--r--   0        0        0     9727 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/extract.py
--rw-r--r--   0        0        0     1220 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/fallbacks.py
--rw-r--r--   0        0        0     9807 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/mdw_modified.py
--rw-r--r--   0        0        0     2404 2022-03-19 22:19:07.612898 humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/utils.py
--rw-r--r--   0        0        0       50 2021-12-29 21:26:21.105642 humlab-penelope-0.7.8/penelope/workflows/__init__.py
--rw-r--r--   0        0        0       45 2021-06-09 09:16:28.011029 humlab-penelope-0.7.8/penelope/workflows/co_occurrence/__init__.py
--rw-r--r--   0        0        0     3240 2022-03-19 22:19:07.622898 humlab-penelope-0.7.8/penelope/workflows/co_occurrence/compute.py
--rw-r--r--   0        0        0    10028 2022-01-01 10:42:06.506740 humlab-penelope-0.7.8/penelope/workflows/compute_opts.py
--rw-r--r--   0        0        0     7009 2022-03-19 22:19:07.622898 humlab-penelope-0.7.8/penelope/workflows/interface.py
--rw-r--r--   0        0        0       15 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/workflows/tm/__init__.py
--rw-r--r--   0        0        0     1436 2022-03-19 22:19:07.622898 humlab-penelope-0.7.8/penelope/workflows/tm/predict.py
--rw-r--r--   0        0        0     2631 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/workflows/tm/train.py
--rw-r--r--   0        0        0     1845 2022-01-06 22:08:24.717693 humlab-penelope-0.7.8/penelope/workflows/tm/train_id.py
--rw-r--r--   0        0        0     2078 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/workflows/tm/train_legacy.py
--rw-r--r--   0        0        0       15 2021-12-16 05:30:08.186294 humlab-penelope-0.7.8/penelope/workflows/vectorize/__init__.py
--rw-r--r--   0        0        0     2098 2022-01-04 14:52:12.265680 humlab-penelope-0.7.8/penelope/workflows/vectorize/dtm.py
--rw-r--r--   0        0        0     1684 2021-12-29 21:26:21.105642 humlab-penelope-0.7.8/penelope/workflows/vectorize/dtm_id.py
--rw-r--r--   0        0        0     4658 2022-03-31 13:45:29.728700 humlab-penelope-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     7038 2022-03-31 13:45:33.308215 humlab-penelope-0.7.8/setup.py
--rw-r--r--   0        0        0     4817 2022-03-31 13:45:33.308659 humlab-penelope-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     3120 2021-06-17 19:02:19.461226 humlab-penelope-0.7.9/README.md
+-rw-r--r--   0        0        0        0 2021-05-31 13:11:35.004419 humlab-penelope-0.7.9/penelope/__init__.py
+-rw-r--r--   0        0        0      852 2021-07-03 19:31:04.069680 humlab-penelope-0.7.9/penelope/co_occurrence/__init__.py
+-rw-r--r--   0        0        0     6106 2022-03-19 22:19:07.342898 humlab-penelope-0.7.9/penelope/co_occurrence/bundle.py
+-rw-r--r--   0        0        0     3966 2022-03-19 22:19:07.342898 humlab-penelope-0.7.9/penelope/co_occurrence/convert.py
+-rw-r--r--   0        0        0      199 2021-03-15 20:15:14.950000 humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/__init__.py
+-rw-r--r--   0        0        0     2832 2021-05-05 09:47:36.605567 humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/co_occurrence_ui.py
+-rw-r--r--   0        0        0     4333 2022-03-19 22:19:07.342898 humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/compute_hal_or_glove.py
+-rw-r--r--   0        0        0     2822 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/vectorizer_glove.py
+-rw-r--r--   0        0        0    10216 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/vectorizer_hal.py
+-rw-r--r--   0        0        0     1445 2021-07-05 19:47:05.125302 humlab-penelope-0.7.9/penelope/co_occurrence/interface.py
+-rw-r--r--   0        0        0     4046 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/co_occurrence/keyness.py
+-rw-r--r--   0        0        0    13039 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/co_occurrence/persistence.py
+-rw-r--r--   0        0        0     9407 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/co_occurrence/prepare.py
+-rw-r--r--   0        0        0     5924 2022-01-01 10:42:06.496740 humlab-penelope-0.7.9/penelope/co_occurrence/utility.py
+-rw-r--r--   0        0        0     5531 2022-03-18 07:12:53.399367 humlab-penelope-0.7.9/penelope/co_occurrence/vectorize.py
+-rw-r--r--   0        0        0     6516 2021-09-28 12:56:00.310009 humlab-penelope-0.7.9/penelope/co_occurrence/windows.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:15:16.140000 humlab-penelope-0.7.9/penelope/common/__init__.py
+-rw-r--r--   0        0        0    10786 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/common/cluster_analysis.py
+-rw-r--r--   0        0        0     3570 2021-04-23 12:36:52.077472 humlab-penelope-0.7.9/penelope/common/curve_fit.py
+-rw-r--r--   0        0        0     3199 2021-12-16 06:16:48.006294 humlab-penelope-0.7.9/penelope/common/distance_metrics.py
+-rw-r--r--   0        0        0    10576 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/common/goodness_of_fit.py
+-rw-r--r--   0        0        0      269 2021-06-29 11:52:45.258960 humlab-penelope-0.7.9/penelope/common/keyness/__init__.py
+-rw-r--r--   0        0        0     4762 2021-06-30 13:45:43.936217 humlab-penelope-0.7.9/penelope/common/keyness/hal_cwr.py
+-rw-r--r--   0        0        0    15269 2021-12-16 06:17:38.226294 humlab-penelope-0.7.9/penelope/common/keyness/metrics.py
+-rw-r--r--   0        0        0      833 2022-03-19 22:19:07.352898 humlab-penelope-0.7.9/penelope/common/mdw.py
+-rw-r--r--   0        0        0     1276 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/common/pca_analysis.py
+-rw-r--r--   0        0        0     2011 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/corpus/__init__.py
+-rw-r--r--   0        0        0      706 2021-12-16 09:49:19.674955 humlab-penelope-0.7.9/penelope/corpus/corpus_mixins.py
+-rw-r--r--   0        0        0    29541 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/corpus/document_index.py
+-rw-r--r--   0        0        0      657 2022-03-19 22:19:07.362898 humlab-penelope-0.7.9/penelope/corpus/dtm/__init__.py
+-rw-r--r--   0        0        0     5516 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/corpus/dtm/convert.py
+-rw-r--r--   0        0        0    19466 2022-03-31 05:32:11.801817 humlab-penelope-0.7.9/penelope/corpus/dtm/corpus.py
+-rw-r--r--   0        0        0    17258 2022-03-19 22:19:07.362898 humlab-penelope-0.7.9/penelope/corpus/dtm/group.py
+-rw-r--r--   0        0        0     6863 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/corpus/dtm/interface.py
+-rw-r--r--   0        0        0     1127 2021-10-03 02:14:00.280348 humlab-penelope-0.7.9/penelope/corpus/dtm/optimize.py
+-rw-r--r--   0        0        0     8951 2022-03-19 22:19:07.362898 humlab-penelope-0.7.9/penelope/corpus/dtm/slice.py
+-rw-r--r--   0        0        0     7291 2022-03-19 22:19:07.362898 humlab-penelope-0.7.9/penelope/corpus/dtm/stats.py
+-rw-r--r--   0        0        0    12234 2022-03-19 22:19:07.362898 humlab-penelope-0.7.9/penelope/corpus/dtm/store.py
+-rw-r--r--   0        0        0    11811 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/corpus/dtm/ttm.py
+-rw-r--r--   0        0        0     7194 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/dtm/ttm_legacy.py
+-rw-r--r--   0        0        0     9372 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/dtm/vectorizer.py
+-rw-r--r--   0        0        0      939 2021-05-30 17:44:38.579000 humlab-penelope-0.7.9/penelope/corpus/interfaces.py
+-rw-r--r--   0        0        0      629 2021-12-16 05:30:08.136294 humlab-penelope-0.7.9/penelope/corpus/readers/__init__.py
+-rw-r--r--   0        0        0     6306 2022-01-01 10:42:06.496740 humlab-penelope-0.7.9/penelope/corpus/readers/interfaces.py
+-rw-r--r--   0        0        0      849 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/readers/pandas_reader.py
+-rw-r--r--   0        0        0     1397 2022-01-02 10:25:24.845131 humlab-penelope-0.7.9/penelope/corpus/readers/sparv_csv_tokenizer.py
+-rw-r--r--   0        0        0     2793 2022-01-02 10:25:15.785131 humlab-penelope-0.7.9/penelope/corpus/readers/sparv_xml_tokenizer.py
+-rw-r--r--   0        0        0     1777 2021-06-09 09:16:27.941029 humlab-penelope-0.7.9/penelope/corpus/readers/streamify_text_source.py
+-rw-r--r--   0        0        0     5191 2021-12-16 05:30:08.136294 humlab-penelope-0.7.9/penelope/corpus/readers/text_reader.py
+-rw-r--r--   0        0        0     2826 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/corpus/readers/text_tokenizer.py
+-rw-r--r--   0        0        0     2575 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/readers/text_transformer.py
+-rw-r--r--   0        0        0      344 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/readers/tng/__init__.py
+-rw-r--r--   0        0        0     1672 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/readers/tng/factory.py
+-rw-r--r--   0        0        0     1910 2021-03-15 20:15:15.770000 humlab-penelope-0.7.9/penelope/corpus/readers/tng/interfaces.py
+-rw-r--r--   0        0        0     3872 2021-03-25 11:18:12.894717 humlab-penelope-0.7.9/penelope/corpus/readers/tng/reader.py
+-rw-r--r--   0        0        0     6063 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/readers/tng/sources.py
+-rw-r--r--   0        0        0     2603 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/readers/tng/transformer.py
+-rw-r--r--   0        0        0     2574 2021-06-09 09:16:27.941029 humlab-penelope-0.7.9/penelope/corpus/readers/zip_iterator.py
+-rw-r--r--   0        0        0     3297 2021-06-09 09:16:27.941029 humlab-penelope-0.7.9/penelope/corpus/segmented_text_corpus.py
+-rw-r--r--   0        0        0      358 2021-03-15 20:15:15.630000 humlab-penelope-0.7.9/penelope/corpus/sparv/NOTES.md
+-rw-r--r--   0        0        0        0 2021-03-15 20:15:15.650000 humlab-penelope-0.7.9/penelope/corpus/sparv/__init__.py
+-rw-r--r--   0        0        0     1528 2021-03-25 11:18:12.894717 humlab-penelope-0.7.9/penelope/corpus/sparv/parlaclarin_test.xslt
+-rw-r--r--   0        0        0     4072 2021-12-16 05:30:08.146294 humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_csv_to_text.py
+-rw-r--r--   0        0        0     1587 2021-03-15 20:15:15.640000 humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_extract.v3.xslt
+-rw-r--r--   0        0        0     1594 2021-04-16 12:53:17.751957 humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_extract.xslt
+-rw-r--r--   0        0        0     1617 2021-09-02 09:51:35.687334 humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_csv.py
+-rw-r--r--   0        0        0     1587 2021-03-15 20:15:15.630000 humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_csv.v3.xslt
+-rw-r--r--   0        0        0      708 2021-03-15 20:15:15.630000 humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_csv.xslt
+-rw-r--r--   0        0        0     2252 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_text.py
+-rw-r--r--   0        0        0     4782 2022-01-02 10:25:49.225131 humlab-penelope-0.7.9/penelope/corpus/sparv_corpus.py
+-rw-r--r--   0        0        0     1327 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/store_corpus.py
+-rw-r--r--   0        0        0     2395 2021-05-30 17:44:39.106000 humlab-penelope-0.7.9/penelope/corpus/text_lines_corpus.py
+-rw-r--r--   0        0        0    14176 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/token2id.py
+-rw-r--r--   0        0        0     4921 2021-12-26 18:21:25.500488 humlab-penelope-0.7.9/penelope/corpus/tokenized_corpus.py
+-rw-r--r--   0        0        0     7400 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/corpus/tokens_transformer.py
+-rw-r--r--   0        0        0     6091 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/corpus/transforms.py
+-rw-r--r--   0        0        0     2205 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/corpus/utils.py
+-rw-r--r--   0        0        0     2980 2022-03-19 22:19:07.372898 humlab-penelope-0.7.9/penelope/ner/stagger_wrapper.py
+-rw-r--r--   0        0        0      131 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/__init__.py
+-rw-r--r--   0        0        0     4551 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/network/bipartite_plot.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:15:16.210000 humlab-penelope-0.7.9/penelope/network/graphtool/__init__.py
+-rw-r--r--   0        0        0     2395 2021-06-09 09:16:27.951029 humlab-penelope-0.7.9/penelope/network/graphtool/layout.py
+-rw-r--r--   0        0        0     1693 2021-06-09 09:16:27.951029 humlab-penelope-0.7.9/penelope/network/graphtool/plot.py
+-rw-r--r--   0        0        0     4733 2021-06-09 09:16:27.951029 humlab-penelope-0.7.9/penelope/network/graphtool/utility.py
+-rw-r--r--   0        0        0       22 2021-03-15 20:15:16.200000 humlab-penelope-0.7.9/penelope/network/graphviz/__init__.py
+-rw-r--r--   0        0        0     1011 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/graphviz/layout.py
+-rw-r--r--   0        0        0      406 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/interface.py
+-rw-r--r--   0        0        0     1592 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/layout.py
+-rw-r--r--   0        0        0     2203 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/layout_source.py
+-rw-r--r--   0        0        0     2146 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/metrics.py
+-rw-r--r--   0        0        0       34 2021-03-15 20:15:16.280000 humlab-penelope-0.7.9/penelope/network/networkx/__init__.py
+-rw-r--r--   0        0        0     1802 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/networkx/layout.py
+-rw-r--r--   0        0        0      808 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/networkx/networkx_api.py
+-rw-r--r--   0        0        0     1524 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/networkx/plot.py
+-rw-r--r--   0        0        0    10015 2022-03-19 22:19:07.392898 humlab-penelope-0.7.9/penelope/network/networkx/utility.py
+-rw-r--r--   0        0        0     8111 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/network/plot.py
+-rw-r--r--   0        0        0     6279 2022-04-08 05:37:06.062657 humlab-penelope-0.7.9/penelope/network/plot_utility.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:15:15.400000 humlab-penelope-0.7.9/penelope/notebook/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:15:15.440000 humlab-penelope-0.7.9/penelope/notebook/cluster_analysis/__init__.py
+-rw-r--r--   0        0        0    12497 2022-03-19 22:19:07.402898 humlab-penelope-0.7.9/penelope/notebook/cluster_analysis/cluster_analysis_gui.py
+-rw-r--r--   0        0        0     8195 2022-04-06 12:31:13.923376 humlab-penelope-0.7.9/penelope/notebook/cluster_analysis/cluster_plot.py
+-rw-r--r--   0        0        0     2900 2022-03-19 22:19:07.402898 humlab-penelope-0.7.9/penelope/notebook/cluster_analysis/plot.py
+-rw-r--r--   0        0        0      320 2021-06-09 09:16:27.951029 humlab-penelope-0.7.9/penelope/notebook/co_occurrence/__init__.py
+-rw-r--r--   0        0        0     2525 2022-03-19 22:19:07.402898 humlab-penelope-0.7.9/penelope/notebook/co_occurrence/explore_co_occurrence_gui.py
+-rw-r--r--   0        0        0     4991 2022-03-19 22:19:07.402898 humlab-penelope-0.7.9/penelope/notebook/co_occurrence/load_co_occurrences_gui.py
+-rw-r--r--   0        0        0     3580 2022-03-19 22:19:07.422898 humlab-penelope-0.7.9/penelope/notebook/co_occurrence/main_gui.py
+-rw-r--r--   0        0        0    15685 2022-03-19 22:19:07.422898 humlab-penelope-0.7.9/penelope/notebook/co_occurrence/tabular_gui.py
+-rw-r--r--   0        0        0     5795 2022-03-19 22:19:07.422898 humlab-penelope-0.7.9/penelope/notebook/co_occurrence/to_co_occurrence_gui.py
+-rw-r--r--   0        0        0      121 2021-03-15 20:15:15.160000 humlab-penelope-0.7.9/penelope/notebook/dtm/__init__.py
+-rw-r--r--   0        0        0     4616 2022-03-19 22:19:07.422898 humlab-penelope-0.7.9/penelope/notebook/dtm/load_dtm_gui.py
+-rw-r--r--   0        0        0     1447 2021-12-29 21:26:21.105642 humlab-penelope-0.7.9/penelope/notebook/dtm/to_dtm_gui.py
+-rw-r--r--   0        0        0     2388 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/grid_utility.py
+-rw-r--r--   0        0        0    19489 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/gui_base.py
+-rw-r--r--   0        0        0       98 2021-03-15 20:15:15.420000 humlab-penelope-0.7.9/penelope/notebook/mdw/__init__.py
+-rw-r--r--   0        0        0     1009 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/mdw/main_gui.py
+-rw-r--r--   0        0        0     4432 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/mdw/mdw_gui.py
+-rw-r--r--   0        0        0    11287 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/mixins.py
+-rw-r--r--   0        0        0      176 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/token_counts/__init__.py
+-rw-r--r--   0        0        0    13648 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/token_counts/dtm_gui.py
+-rw-r--r--   0        0        0     9996 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/token_counts/pipeline_gui.py
+-rw-r--r--   0        0        0     3705 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/token_counts/plot.py
+-rw-r--r--   0        0        0     1531 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/__init__.py
+-rw-r--r--   0        0        0     2663 2022-03-19 22:19:07.442898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/edit_topic_labels_gui.py
+-rw-r--r--   0        0        0     4428 2022-03-23 16:03:00.200622 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/load_topic_model_gui.py
+-rw-r--r--   0        0        0     8461 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/mixins.py
+-rw-r--r--   0        0        0     2973 2022-03-19 22:19:07.462898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/model_container.py
+-rw-r--r--   0        0        0    11376 2022-03-19 22:19:07.462898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/pivot_network_gui.py
+-rw-r--r--   0        0        0    10793 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_document_network_gui.py
+-rw-r--r--   0        0        0    10441 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_documents_gui.py
+-rw-r--r--   0        0        0    16321 2022-03-19 22:19:07.462898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_model_gui.py
+-rw-r--r--   0        0        0     3859 2022-03-19 22:19:07.462898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_titles_gui.py
+-rw-r--r--   0        0        0    11733 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_topic_network_gui.py
+-rw-r--r--   0        0        0     1228 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_topic_network_gui_utility.py
+-rw-r--r--   0        0        0     7687 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_gui.py
+-rw-r--r--   0        0        0     1323 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_gui_utility.py
+-rw-r--r--   0        0        0     7148 2022-03-19 22:19:07.472898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_overview_gui.py
+-rw-r--r--   0        0        0     4851 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_overview_gui_utility.py
+-rw-r--r--   0        0        0     5116 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_word_distribution_gui.py
+-rw-r--r--   0        0        0     3522 2022-03-19 22:19:07.472898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_wordcloud_gui.py
+-rw-r--r--   0        0        0    20033 2022-03-19 22:19:07.472898 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topics_token_network_gui.py
+-rw-r--r--   0        0        0    16749 2022-03-31 00:27:57.529621 humlab-penelope-0.7.9/penelope/notebook/topic_modelling/train_gui/topic_model_gui.py
+-rw-r--r--   0        0        0     7891 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/utility.py
+-rw-r--r--   0        0        0     5049 2022-03-19 22:19:07.482898 humlab-penelope-0.7.9/penelope/notebook/widgets_utils.py
+-rw-r--r--   0        0        0      424 2022-03-19 22:19:07.482898 humlab-penelope-0.7.9/penelope/notebook/word_trends/__init__.py
+-rw-r--r--   0        0        0      793 2022-03-19 22:19:07.482898 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/__init__.py
+-rw-r--r--   0        0        0     3668 2022-03-19 22:19:07.482898 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/archive/compile_mixins.py
+-rw-r--r--   0        0        0    10578 2022-03-19 22:19:07.492898 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/archive/deprecated_plot.py
+-rw-r--r--   0        0        0      671 2022-03-19 22:19:07.492898 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/archive/display_top_table2.py
+-rw-r--r--   0        0        0     2483 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_bar.py
+-rw-r--r--   0        0        0     3333 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_line.py
+-rw-r--r--   0        0        0     9611 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_network.py
+-rw-r--r--   0        0        0     2022 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_stackedbar.py
+-rw-r--r--   0        0        0     2759 2022-03-19 22:19:07.492898 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_table.py
+-rw-r--r--   0        0        0    10408 2022-03-19 22:19:07.492898 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_top_table.py
+-rw-r--r--   0        0        0      842 2022-03-19 22:19:07.502898 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/interface.py
+-rw-r--r--   0        0        0     5313 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/plotter.py
+-rw-r--r--   0        0        0     1644 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/utils.py
+-rw-r--r--   0        0        0     1235 2022-03-19 22:19:07.502898 humlab-penelope-0.7.9/penelope/notebook/word_trends/gof_and_trends_gui.py
+-rw-r--r--   0        0        0     1671 2022-03-19 22:19:07.502898 humlab-penelope-0.7.9/penelope/notebook/word_trends/gofs_gui.py
+-rw-r--r--   0        0        0     7421 2022-03-19 22:19:07.512898 humlab-penelope-0.7.9/penelope/notebook/word_trends/interface.py
+-rw-r--r--   0        0        0     3457 2022-03-19 22:19:07.512898 humlab-penelope-0.7.9/penelope/notebook/word_trends/main_gui.py
+-rw-r--r--   0        0        0    16567 2022-03-19 22:19:07.512898 humlab-penelope-0.7.9/penelope/notebook/word_trends/trends_gui.py
+-rw-r--r--   0        0        0     8524 2022-03-19 22:19:07.512898 humlab-penelope-0.7.9/penelope/notebook/word_trends/trends_with_picks_gui.py
+-rw-r--r--   0        0        0     1123 2022-02-10 06:55:17.682926 humlab-penelope-0.7.9/penelope/pipeline/__init__.py
+-rw-r--r--   0        0        0      468 2021-09-28 07:35:39.360009 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/__init__.py
+-rw-r--r--   0        0        0     8433 2022-03-19 22:19:07.512898 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/checkpoint.py
+-rw-r--r--   0        0        0     3508 2022-03-19 22:19:07.522898 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/feather.py
+-rw-r--r--   0        0        0     3531 2022-03-19 22:19:07.522898 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/interface.py
+-rw-r--r--   0        0        0     2852 2021-07-09 20:15:23.442229 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/legacy.py
+-rw-r--r--   0        0        0     5238 2022-03-19 22:19:07.522898 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/load.py
+-rw-r--r--   0        0        0     3039 2022-03-19 22:19:07.522898 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/serialize.py
+-rw-r--r--   0        0        0     1483 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/pipeline/checkpoint/utility.py
+-rw-r--r--   0        0        0      146 2021-06-09 09:16:27.981029 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/__init__.py
+-rw-r--r--   0        0        0     5738 2022-03-19 22:19:07.522898 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/builder.py
+-rw-r--r--   0        0        0       15 2021-06-09 09:16:27.981029 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/legacy/__init__.py
+-rw-r--r--   0        0        0     1198 2021-12-28 21:06:58.133459 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/legacy/pipelines.py
+-rw-r--r--   0        0        0     5066 2021-12-16 06:32:55.786294 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/legacy/tasks.py
+-rw-r--r--   0        0        0     1126 2021-12-16 11:13:12.674955 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/pipeline_mixin.py
+-rw-r--r--   0        0        0     1467 2021-12-28 21:06:58.133459 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/pipelines.py
+-rw-r--r--   0        0        0    11543 2022-03-19 22:19:07.522898 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/tasks.py
+-rw-r--r--   0        0        0     4443 2022-03-19 22:19:07.522898 humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/tasks_pool.py
+-rw-r--r--   0        0        0     8610 2022-03-19 22:19:07.542898 humlab-penelope-0.7.9/penelope/pipeline/config.py
+-rw-r--r--   0        0        0    11856 2022-03-19 22:19:07.542898 humlab-penelope-0.7.9/penelope/pipeline/convert.py
+-rw-r--r--   0        0        0        0 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/pipeline/dtm/__init__.py
+-rw-r--r--   0        0        0      649 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/pipeline/dtm/pipeline_mixin.py
+-rw-r--r--   0        0        0     2167 2022-01-01 10:42:06.496740 humlab-penelope-0.7.9/penelope/pipeline/dtm/pipelines.py
+-rw-r--r--   0        0        0     1926 2022-01-05 23:10:42.092085 humlab-penelope-0.7.9/penelope/pipeline/dtm/tasks.py
+-rw-r--r--   0        0        0     3530 2022-03-19 22:19:07.542898 humlab-penelope-0.7.9/penelope/pipeline/dtm/vectorizer.py
+-rw-r--r--   0        0        0    14141 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/pipeline/interfaces.py
+-rw-r--r--   0        0        0        0 2021-07-08 20:06:07.056481 humlab-penelope-0.7.9/penelope/pipeline/multiprocess/__init__.py
+-rw-r--r--   0        0        0     3251 2022-03-19 22:19:07.542898 humlab-penelope-0.7.9/penelope/pipeline/phrases.py
+-rw-r--r--   0        0        0     5024 2021-10-04 16:48:51.788710 humlab-penelope-0.7.9/penelope/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8676 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/pipeline/pipeline_mixin.py
+-rw-r--r--   0        0        0     1470 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/pipeline/pipelines.py
+-rw-r--r--   0        0        0      112 2022-02-10 06:53:54.312926 humlab-penelope-0.7.9/penelope/pipeline/spacy/__init__.py
+-rw-r--r--   0        0        0     3986 2022-03-19 22:19:07.542898 humlab-penelope-0.7.9/penelope/pipeline/spacy/convert.py
+-rw-r--r--   0        0        0     1629 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/pipeline/spacy/pipeline_mixin.py
+-rw-r--r--   0        0        0     4562 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/pipeline/spacy/pipelines.py
+-rw-r--r--   0        0        0     3618 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/pipeline/spacy/tasks.py
+-rw-r--r--   0        0        0      127 2021-09-02 09:55:30.257334 humlab-penelope-0.7.9/penelope/pipeline/sparv/__init__.py
+-rw-r--r--   0        0        0     1893 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/pipeline/sparv/convert.py
+-rw-r--r--   0        0        0     1520 2022-01-01 10:42:06.496740 humlab-penelope-0.7.9/penelope/pipeline/sparv/pipelines.py
+-rw-r--r--   0        0        0     8149 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/pipeline/tagged_frame.py
+-rw-r--r--   0        0        0    27737 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/pipeline/tasks.py
+-rw-r--r--   0        0        0     5498 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/pipeline/tasks_mixin.py
+-rw-r--r--   0        0        0       15 2021-09-27 10:08:55.933176 humlab-penelope-0.7.9/penelope/pipeline/topic_model/__init__.py
+-rw-r--r--   0        0        0     3258 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/pipeline/topic_model/pipeline_mixin.py
+-rw-r--r--   0        0        0     4317 2022-01-06 11:32:55.227693 humlab-penelope-0.7.9/penelope/pipeline/topic_model/pipelines.py
+-rw-r--r--   0        0        0    13413 2022-03-23 16:03:00.210622 humlab-penelope-0.7.9/penelope/pipeline/topic_model/tasks.py
+-rw-r--r--   0        0        0      249 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/plot/__init__.py
+-rw-r--r--   0        0        0      689 2021-03-15 20:15:15.950000 humlab-penelope-0.7.9/penelope/plot/colors.py
+-rw-r--r--   0        0        0     4344 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/plot/utility.py
+-rw-r--r--   0        0        0     1017 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/plot/wordcloud_utility.py
+-rw-r--r--   0        0        0       41 2021-03-15 20:15:16.150000 humlab-penelope-0.7.9/penelope/resources/__init__.py
+-rw-r--r--   0        0        0     5417 2021-03-15 20:15:16.150000 humlab-penelope-0.7.9/penelope/resources/fox_stopwords.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:15:15.070000 humlab-penelope-0.7.9/penelope/scripts/__init__.py
+-rw-r--r--   0        0        0     7499 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/scripts/co_occurrence.py
+-rwxr-xr-x   0        0        0     1437 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/scripts/co_occurrence.sh
+-rw-r--r--   0        0        0        0 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/scripts/dtm/__init__.py
+-rw-r--r--   0        0        0     6581 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/scripts/dtm/vectorize.py
+-rw-r--r--   0        0        0     6072 2022-03-19 22:19:07.552898 humlab-penelope-0.7.9/penelope/scripts/dtm/vectorize_id.py
+-rw-r--r--   0        0        0     2958 2021-12-29 21:26:21.105642 humlab-penelope-0.7.9/penelope/scripts/legacy/coherence.py
+-rw-r--r--   0        0        0     1439 2021-12-29 21:26:21.105642 humlab-penelope-0.7.9/penelope/scripts/legacy/install-spacy-models.sh
+-rw-r--r--   0        0        0      187 2021-09-22 10:58:18.745079 humlab-penelope-0.7.9/penelope/scripts/legacy/post-install.sh
+-rw-r--r--   0        0        0     3410 2022-03-19 22:19:07.562898 humlab-penelope-0.7.9/penelope/scripts/legacy/sparv-xml-extract-text.py
+-rw-r--r--   0        0        0      635 2022-03-19 22:19:07.562898 humlab-penelope-0.7.9/penelope/scripts/pos_tag.py
+-rw-r--r--   0        0        0        0 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/scripts/tm/__init__.py
+-rw-r--r--   0        0        0      976 2022-03-19 22:19:07.562898 humlab-penelope-0.7.9/penelope/scripts/tm/mallet2topicsdata.py
+-rw-r--r--   0        0        0     4716 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/scripts/tm/predict.py
+-rw-r--r--   0        0        0     8208 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/scripts/tm/train.py
+-rw-r--r--   0        0        0     7202 2022-03-23 16:03:00.210622 humlab-penelope-0.7.9/penelope/scripts/tm/train_id.py
+-rw-r--r--   0        0        0     4714 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/scripts/tm/train_legacy.py
+-rw-r--r--   0        0        0     8999 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/scripts/utils.py
+-rw-r--r--   0        0        0      887 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/__init__.py
+-rw-r--r--   0        0        0     1053 2021-12-26 18:21:25.500488 humlab-penelope-0.7.9/penelope/topic_modelling/engines/__init__.py
+-rw-r--r--   0        0        0     3071 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/__init__.py
+-rw-r--r--   0        0        0     2125 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/coherence.py
+-rw-r--r--   0        0        0     9162 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/convert.py
+-rw-r--r--   0        0        0    13444 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/options.py
+-rw-r--r--   0        0        0     3105 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/predict.py
+-rw-r--r--   0        0        0     2952 2022-01-23 12:51:56.726124 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/train.py
+-rw-r--r--   0        0        0     1959 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/utility.py
+-rw-r--r--   0        0        0     2090 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_textacy/__init__.py
+-rw-r--r--   0        0        0     1187 2022-03-19 22:19:07.572898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_textacy/predict.py
+-rw-r--r--   0        0        0     2138 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_textacy/train.py
+-rw-r--r--   0        0        0     4692 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/engines/interface.py
+-rw-r--r--   0        0        0     9010 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/interfaces.py
+-rw-r--r--   0        0        0     3951 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/predict.py
+-rw-r--r--   0        0        0        0 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/rdb/__init__.py
+-rw-r--r--   0        0        0     1572 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/rdb/data.py
+-rw-r--r--   0        0        0      126 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/saliency/__init__.py
+-rw-r--r--   0        0        0     2533 2022-03-19 22:19:07.582898 humlab-penelope-0.7.9/penelope/topic_modelling/saliency/saliency.py
+-rw-r--r--   0        0        0     1513 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/__init__.py
+-rw-r--r--   0        0        0    11553 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/document.py
+-rw-r--r--   0        0        0    11040 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/prevelance.py
+-rw-r--r--   0        0        0     5715 2022-03-19 22:19:07.592898 humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/token.py
+-rw-r--r--   0        0        0    16431 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/topics_data.py
+-rw-r--r--   0        0        0      734 2022-03-19 22:19:07.592898 humlab-penelope-0.7.9/penelope/topic_modelling/train.py
+-rw-r--r--   0        0        0      939 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/topic_modelling/utility.py
+-rw-r--r--   0        0        0      884 2022-03-19 22:19:07.592898 humlab-penelope-0.7.9/penelope/type_alias.py
+-rw-r--r--   0        0        0     4395 2022-03-19 22:19:07.592898 humlab-penelope-0.7.9/penelope/utility/__init__.py
+-rw-r--r--   0        0        0     4397 2021-03-15 20:15:15.030000 humlab-penelope-0.7.9/penelope/utility/_color_utility.py
+-rw-r--r--   0        0        0     3728 2021-06-21 13:22:46.611091 humlab-penelope-0.7.9/penelope/utility/_decorators.py
+-rw-r--r--   0        0        0     6584 2022-03-19 22:19:07.592898 humlab-penelope-0.7.9/penelope/utility/file_utility.py
+-rw-r--r--   0        0        0     3475 2021-06-09 09:16:28.001029 humlab-penelope-0.7.9/penelope/utility/filename_fields.py
+-rw-r--r--   0        0        0     5135 2021-10-11 06:46:17.330209 humlab-penelope-0.7.9/penelope/utility/filename_utils.py
+-rw-r--r--   0        0        0    17789 2022-03-23 16:03:00.210622 humlab-penelope-0.7.9/penelope/utility/pandas_utils.py
+-rw-r--r--   0        0        0     1279 2022-03-19 22:19:07.592898 humlab-penelope-0.7.9/penelope/utility/paths.py
+-rw-r--r--   0        0        0    12216 2022-01-01 10:42:06.506740 humlab-penelope-0.7.9/penelope/utility/pos_tags.py
+-rw-r--r--   0        0        0     5897 2021-09-27 10:08:55.943176 humlab-penelope-0.7.9/penelope/utility/streamify_source.py
+-rw-r--r--   0        0        0    18421 2022-03-19 22:19:07.592898 humlab-penelope-0.7.9/penelope/utility/utils.py
+-rw-r--r--   0        0        0     3942 2021-06-09 09:16:28.011029 humlab-penelope-0.7.9/penelope/utility/zip_utils.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:15:16.460000 humlab-penelope-0.7.9/penelope/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/archive/stanza/__init__.py
+-rw-r--r--   0        0        0      743 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/archive/stanza/utility.py
+-rw-r--r--   0        0        0      206 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/archive/textacy_pipeline/__init__.py
+-rw-r--r--   0        0        0     6819 2022-03-31 13:37:03.338700 humlab-penelope-0.7.9/penelope/vendor/archive/textacy_pipeline/pipeline.py
+-rw-r--r--   0        0        0      201 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/__init__.py
+-rw-r--r--   0        0        0      252 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/__init__.py
+-rw-r--r--   0        0        0     7598 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/_corpus.py
+-rw-r--r--   0        0        0      894 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/_models.py
+-rw-r--r--   0        0        0       74 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/README.md
+-rw-r--r--   0        0        0      458 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/__init__.py
+-rw-r--r--   0        0        0    21674 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/dtmmodel.py.txt
+-rw-r--r--   0        0        0     1369 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/fasttext.py.txt
+-rw-r--r--   0        0        0    28452 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/ldavowpalwabbit.py.txt
+-rw-r--r--   0        0        0     4737 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/varembed.py.txt
+-rw-r--r--   0        0        0    13731 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/wordrank.py.txt
+-rw-r--r--   0        0        0    28870 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/ldamallet.py
+-rw-r--r--   0        0        0     6291 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/mallet_tm.py
+-rw-r--r--   0        0        0    11062 2022-03-19 22:19:07.602898 humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/sttm_tm.py
+-rw-r--r--   0        0        0      182 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/mallet_api/__init__.py
+-rw-r--r--   0        0        0     6889 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/mallet_api/convert.py
+-rw-r--r--   0        0        0     1246 2021-04-28 09:36:47.725900 humlab-penelope-0.7.9/penelope/vendor/nltk/__init__.py
+-rw-r--r--   0        0        0     5505 2021-03-15 20:15:16.390000 humlab-penelope-0.7.9/penelope/vendor/nltk/extra_stopwords.py
+-rw-r--r--   0        0        0      469 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/vendor/spacy_api/__init__.py
+-rw-r--r--   0        0        0     6504 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/spacy_api/_spacy.py
+-rw-r--r--   0        0        0      635 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/textacy_api/__init__.py
+-rw-r--r--   0        0        0      808 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/__init__.py
+-rw-r--r--   0        0        0     9727 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/extract.py
+-rw-r--r--   0        0        0     1220 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/fallbacks.py
+-rw-r--r--   0        0        0     9799 2022-04-07 19:14:55.792738 humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/mdw_modified.py
+-rw-r--r--   0        0        0     2404 2022-03-19 22:19:07.612898 humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/utils.py
+-rw-r--r--   0        0        0       50 2021-12-29 21:26:21.105642 humlab-penelope-0.7.9/penelope/workflows/__init__.py
+-rw-r--r--   0        0        0       45 2021-06-09 09:16:28.011029 humlab-penelope-0.7.9/penelope/workflows/co_occurrence/__init__.py
+-rw-r--r--   0        0        0     3240 2022-03-19 22:19:07.622898 humlab-penelope-0.7.9/penelope/workflows/co_occurrence/compute.py
+-rw-r--r--   0        0        0    10028 2022-01-01 10:42:06.506740 humlab-penelope-0.7.9/penelope/workflows/compute_opts.py
+-rw-r--r--   0        0        0     7009 2022-03-19 22:19:07.622898 humlab-penelope-0.7.9/penelope/workflows/interface.py
+-rw-r--r--   0        0        0       15 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/workflows/tm/__init__.py
+-rw-r--r--   0        0        0     1436 2022-03-19 22:19:07.622898 humlab-penelope-0.7.9/penelope/workflows/tm/predict.py
+-rw-r--r--   0        0        0     2631 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/workflows/tm/train.py
+-rw-r--r--   0        0        0     1845 2022-01-06 22:08:24.717693 humlab-penelope-0.7.9/penelope/workflows/tm/train_id.py
+-rw-r--r--   0        0        0     2078 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/workflows/tm/train_legacy.py
+-rw-r--r--   0        0        0       15 2021-12-16 05:30:08.186294 humlab-penelope-0.7.9/penelope/workflows/vectorize/__init__.py
+-rw-r--r--   0        0        0     2098 2022-01-04 14:52:12.265680 humlab-penelope-0.7.9/penelope/workflows/vectorize/dtm.py
+-rw-r--r--   0        0        0     1684 2021-12-29 21:26:21.105642 humlab-penelope-0.7.9/penelope/workflows/vectorize/dtm_id.py
+-rw-r--r--   0        0        0     4658 2022-04-08 05:43:30.992657 humlab-penelope-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     7038 2022-04-08 05:43:34.553638 humlab-penelope-0.7.9/setup.py
+-rw-r--r--   0        0        0     4817 2022-04-08 05:43:34.554038 humlab-penelope-0.7.9/PKG-INFO
```

### Comparing `humlab-penelope-0.7.8/README.md` & `humlab-penelope-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/__init__.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/bundle.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/bundle.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/convert.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/convert.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/co_occurrence_ui.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/co_occurrence_ui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/compute_hal_or_glove.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/compute_hal_or_glove.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/vectorizer_glove.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/vectorizer_glove.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/hal_or_glove/vectorizer_hal.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/hal_or_glove/vectorizer_hal.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/interface.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/interface.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/keyness.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/keyness.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/persistence.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/persistence.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/prepare.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/prepare.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/utility.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/vectorize.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/vectorize.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/co_occurrence/windows.py` & `humlab-penelope-0.7.9/penelope/co_occurrence/windows.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/cluster_analysis.py` & `humlab-penelope-0.7.9/penelope/common/cluster_analysis.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/curve_fit.py` & `humlab-penelope-0.7.9/penelope/common/curve_fit.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/distance_metrics.py` & `humlab-penelope-0.7.9/penelope/common/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/goodness_of_fit.py` & `humlab-penelope-0.7.9/penelope/common/goodness_of_fit.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/keyness/hal_cwr.py` & `humlab-penelope-0.7.9/penelope/common/keyness/hal_cwr.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/keyness/metrics.py` & `humlab-penelope-0.7.9/penelope/common/keyness/metrics.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/mdw.py` & `humlab-penelope-0.7.9/penelope/common/mdw.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/common/pca_analysis.py` & `humlab-penelope-0.7.9/penelope/common/pca_analysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import itertools
+import typing as t
 
 import bokeh
 
 try:
     from sklearn.decomposition import PCA
 except ImportError:
     ...
 
 
-def compute(data, n_components=2):
+def compute(data: t.Any, n_components: int = 2):
     pca = PCA(n_components=n_components)
     X_pca = pca.fit_transform(data)
     return X_pca
 
 
 def plot(X_pca, clusters=None):
 
     if clusters is not None:
-        palette = itertools.cycle(bokeh.palettes.Colorblind8)
-        cmap = {x: next(palette) for x in set(clusters)}
+        palette: t.Iterable[str] = itertools.cycle(bokeh.palettes.Colorblind8)
+        cmap: dict = {x: next(palette) for x in set(clusters)}
         colors = [cmap[x] for x in clusters]
     else:
         colors = 'navy'
 
-    p = bokeh.plotting.figure(plot_width=600, plot_height=600)
+    p = bokeh.plotting.figure(plot_width=600, plot_height=600, sizing_mode='scale_width')
 
     # p.legend(loc="best", shadow=False, scatterpoints=1)
 
     p.title.text = 'PCA decomposition'
 
     p.xaxis.axis_label, p.yaxis.axis_label = 'pca 0', 'pca 1'
```

### Comparing `humlab-penelope-0.7.8/penelope/corpus/__init__.py` & `humlab-penelope-0.7.9/penelope/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/corpus_mixins.py` & `humlab-penelope-0.7.9/penelope/corpus/corpus_mixins.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/document_index.py` & `humlab-penelope-0.7.9/penelope/corpus/document_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -719,25 +719,33 @@
     if column_names is None:
         column_names = document_index.columns.tolist()
 
     if document_index is None:
         return df
 
     if 'document_id' not in df.columns:
+        logger.warning("overload: `document_id` not found in target.")
         return df
 
     if isinstance(column_names, str):
         column_names = [column_names]
 
-    column_names = ['document_id'] + [c for c in column_names if c not in df.columns and c in document_index.columns]
+    missing_columns: list[str] = [c for c in column_names if c not in df.columns and c not in document_index.columns]
+    if len(missing_columns) > 0:
+        logger.warning(f"overload: none of {', '.join(missing_columns)} found in document index.")
 
-    if len(column_names) == 1:
+    overload_columns: list[str] = [c for c in column_names if c not in df.columns and c in document_index.columns]
+    if len(overload_columns) == 0:
         return df
 
-    overload_data: pd.DataFrame = document_index[column_names].set_index('document_id')
+    overload_data: pd.DataFrame = (
+        document_index.set_index('document_id')[overload_columns]
+        if 'document_id' in document_index.columns
+        else document_index[overload_columns]
+    )
 
     df = df.merge(overload_data, how='inner', left_on='document_id', right_index=True)
 
     return df
 
 
 def count_documents_in_index_by_pivot(document_index: DocumentIndex, attribute: str) -> List[int]:
```

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/__init__.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/convert.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/convert.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/corpus.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/corpus.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/group.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/group.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/interface.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,16 +235,14 @@
         document_index: DocumentIndex,
         overridden_term_frequency: Dict[str, int] = None,
     ) -> "IVectorizedCorpus":
         ...
 
 
 class IVectorizedCorpusProtocol(Protocol):
-    ...
-
     @staticmethod
     def create(
         bag_term_matrix: scipy.sparse.csr_matrix,
         token2id: Dict[str, int],
         document_index: DocumentIndex,
         overridden_term_frequency: Dict[str, int] = None,
         **kwargs,
```

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/optimize.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/optimize.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/slice.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/slice.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/stats.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/stats.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/store.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/store.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/ttm.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/ttm.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 
     from .corpus import VectorizedCorpus
 
 # pylint: disable=no-member
 
 
 class ICoOccurrenceVectorizedCorpusProtocol(IVectorizedCorpusProtocol):
-    ...
-
     @property
     def window_counts(self) -> Optional[TokenWindowCountMatrix]:
         ...
 
     @window_counts.setter
     def window_counts(self, value: TokenWindowCountMatrix) -> None:
         ...
```

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/ttm_legacy.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/ttm_legacy.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/dtm/vectorizer.py` & `humlab-penelope-0.7.9/penelope/corpus/dtm/vectorizer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/interfaces.py` & `humlab-penelope-0.7.9/penelope/corpus/interfaces.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/__init__.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/interfaces.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/interfaces.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/pandas_reader.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/pandas_reader.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/sparv_csv_tokenizer.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/sparv_csv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/sparv_xml_tokenizer.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/sparv_xml_tokenizer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/streamify_text_source.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/streamify_text_source.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/text_reader.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/text_reader.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/text_tokenizer.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/text_tokenizer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/text_transformer.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/text_transformer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/tng/factory.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/tng/factory.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/tng/interfaces.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/tng/interfaces.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/tng/reader.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/tng/reader.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/tng/sources.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/tng/sources.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/tng/transformer.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/tng/transformer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/readers/zip_iterator.py` & `humlab-penelope-0.7.9/penelope/corpus/readers/zip_iterator.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/segmented_text_corpus.py` & `humlab-penelope-0.7.9/penelope/corpus/segmented_text_corpus.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/parlaclarin_test.xslt` & `humlab-penelope-0.7.9/penelope/corpus/sparv/parlaclarin_test.xslt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_csv_to_text.py` & `humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_csv_to_text.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_extract.v3.xslt` & `humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_extract.v3.xslt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_extract.xslt` & `humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_extract.xslt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_csv.py` & `humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_csv.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_csv.v3.xslt` & `humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_csv.v3.xslt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_csv.xslt` & `humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_csv.xslt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv/sparv_xml_to_text.py` & `humlab-penelope-0.7.9/penelope/corpus/sparv/sparv_xml_to_text.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/sparv_corpus.py` & `humlab-penelope-0.7.9/penelope/corpus/sparv_corpus.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/store_corpus.py` & `humlab-penelope-0.7.9/penelope/corpus/store_corpus.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/text_lines_corpus.py` & `humlab-penelope-0.7.9/penelope/corpus/text_lines_corpus.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/token2id.py` & `humlab-penelope-0.7.9/penelope/corpus/token2id.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/tokenized_corpus.py` & `humlab-penelope-0.7.9/penelope/corpus/tokenized_corpus.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/tokens_transformer.py` & `humlab-penelope-0.7.9/penelope/corpus/tokens_transformer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/transforms.py` & `humlab-penelope-0.7.9/penelope/corpus/transforms.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/corpus/utils.py` & `humlab-penelope-0.7.9/penelope/corpus/utils.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/ner/stagger_wrapper.py` & `humlab-penelope-0.7.9/penelope/ner/stagger_wrapper.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/bipartite_plot.py` & `humlab-penelope-0.7.9/penelope/network/bipartite_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, List, Sequence
+from typing import Any, Sequence
 
 import bokeh.models as bm
 import bokeh.plotting as bp
 import pandas as pd
 
 from penelope.notebook import widgets_utils as wu
 
@@ -87,20 +87,25 @@
     target_source: bm.ColumnDataSource = layout_source.create_nodes_subset_data_source(
         network, layout_data, target_nodes, color_map=color_map
     )
     lines_source: bm.ColumnDataSource = layout_source.create_edges_layout_data_source(
         network, layout_data, scale=6.0, normalize=False
     )
 
-    edges_alphas: List[float] = metrics.compute_alpha_vector(lines_source.data['weights'])
+    edges_alphas: [float] = metrics.compute_alpha_vector(lines_source.data['weights'])
 
     lines_source.add(edges_alphas, 'alphas')
 
     p: bp.Figure = bp.figure(
-        plot_width=plot_width, plot_height=plot_height, x_axis_type=None, y_axis_type=None, tools=tools
+        plot_width=plot_width,
+        plot_height=plot_height,
+        sizing_mode='scale_width',
+        x_axis_type=None,
+        y_axis_type=None,
+        tools=tools,
     )
 
     _ = p.multi_line(
         xs='xs', ys='ys', line_width='weights', level='underlay', alpha='alphas', color='black', source=lines_source
     )
     _ = p.circle(x='x', y='y', size=40, source=source_source, color='lightgreen', line_width=1, alpha=1.0)
```

### Comparing `humlab-penelope-0.7.8/penelope/network/graphtool/layout.py` & `humlab-penelope-0.7.9/penelope/network/graphtool/layout.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/graphtool/plot.py` & `humlab-penelope-0.7.9/penelope/network/graphtool/plot.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/graphtool/utility.py` & `humlab-penelope-0.7.9/penelope/network/graphtool/utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/graphviz/layout.py` & `humlab-penelope-0.7.9/penelope/network/graphviz/layout.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/layout.py` & `humlab-penelope-0.7.9/penelope/network/layout.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/layout_source.py` & `humlab-penelope-0.7.9/penelope/network/layout_source.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/metrics.py` & `humlab-penelope-0.7.9/penelope/network/metrics.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/networkx/layout.py` & `humlab-penelope-0.7.9/penelope/network/networkx/layout.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/networkx/networkx_api.py` & `humlab-penelope-0.7.9/penelope/network/networkx/networkx_api.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/networkx/plot.py` & `humlab-penelope-0.7.9/penelope/network/networkx/plot.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/networkx/utility.py` & `humlab-penelope-0.7.9/penelope/network/networkx/utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/network/plot.py` & `humlab-penelope-0.7.9/penelope/network/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,17 @@
 
     edges_source: ColumnDataSource = ColumnDataSource(edges)
     nodes_source: ColumnDataSource = ColumnDataSource(nodes)
 
     node_opts = pu.extend(DFLT_NODE_OPTS, node_opts or {})
     line_opts = pu.extend(DFLT_EDGE_OPTS, line_opts or {})
 
-    p = figure(plot_width=figsize[0], plot_height=figsize[1], tools=tools or TOOLS, **figkwargs)
+    p = figure(
+        plot_width=figsize[0], plot_height=figsize[1], sizing_mode='scale_width', tools=tools or TOOLS, **figkwargs
+    )
 
     p.xgrid.grid_line_color = None
     p.ygrid.grid_line_color = None
 
     _ = p.multi_line(
         xs='xs', ys='ys', line_width='weights', source=edges_source, **line_opts
     )  # pylint: disable=too-many-function-args
```

### Comparing `humlab-penelope-0.7.8/penelope/network/plot_utility.py` & `humlab-penelope-0.7.9/penelope/network/plot_utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from typing import Any, Callable, Dict, Sequence, Tuple, Union
+import typing as t
 
 import bokeh.models as bm
 import bokeh.palettes
 import pandas as pd
 from bokeh.plotting import figure
 
 from penelope.notebook import widgets_utils as wu
 
 from . import layout_source, metrics
 from .networkx import utility as nu
 from .networkx.networkx_api import nx
 
-# pylint: disable=too-many-arguments, unnecessary-lambda
+# pylint: disable=too-many-arguments,unnecessary-lambda,unsubscriptable-object,unsupported-assignment-operation
 
 
 if 'extend' not in globals():
     extend = lambda a, b: a.update(b) or a
 
 layout_algorithms = {
     'Fruchterman-Reingold': lambda x, **args: nx.spring_layout(x, **args),
     'Eigenvectors of Laplacian': lambda x, **args: nx.spectral_layout(x, **args),
     'Circular': lambda x, **args: nx.circular_layout(x, **args),
     'Shell': lambda x, **args: nx.shell_layout(x, **args),
     'Kamada-Kawai': lambda x, **args: nx.kamada_kawai_layout(x, **args),
 }
 
 
-def _layout_args(layout_algorithm: str, network: nx.Graph, scale: float, weight_name: str = 'weight') -> Dict[str, Any]:
+def _layout_args(
+    layout_algorithm: str, network: nx.Graph, scale: float, weight_name: str = 'weight'
+) -> dict[str, t.Any]:
 
     args = None
 
     if layout_algorithm == 'Shell':
         if nx.is_bipartite(network):
             nodes, other_nodes = nu.get_bipartite_node_set(network, bipartite=0)
             args = dict(nlist=[nodes, other_nodes])
@@ -44,15 +46,15 @@
 
     if layout_algorithm == "Circular":
         args = dict(dim=2, center=None, scale=1.0)
 
     return args
 
 
-def _get_layout_algorithm(layout_algorithm: str) -> Callable:
+def _get_layout_algorithm(layout_algorithm: str) -> t.Callable:
     if layout_algorithm not in layout_algorithms:
         raise Exception("Unknown algorithm {}".format(layout_algorithm))
     return layout_algorithms.get(layout_algorithm, None)
 
 
 def _project_series_to_range(series: pd.Series, low: float, high: float) -> pd.Series:
     norm_series = series / series.max()
@@ -60,35 +62,35 @@
 
 
 def project_to_range(value: float, low: float, high: float) -> float:
     """Project a single value to a range (low, high)"""
     return low + (high - low) * value
 
 
-def project_values_to_range(values: Sequence[float], low: float, high: float) -> Sequence[float]:
+def project_values_to_range(values: t.Sequence[float], low: float, high: float) -> t.Sequence[float]:
     w_max = max(values)
     return [low + (high - low) * (x / w_max) for x in values]
 
 
 def _plot_network(
     network: nx.Graph,
     layout_algorithm: str = None,
     scale: float = 1.0,
     threshold: float = 0.0,
     node_description: pd.Series = None,
-    node_proportions: Union[int, str] = None,
+    node_proportions: t.Union[int, str] = None,
     weight_name: str = 'weight',
     weight_scale: float = 5.0,
     normalize_weights: bool = True,
     node_opts=None,
     line_opts=None,
     element_id: str = 'nx_id3',
-    figsize: Tuple[int, int] = (900, 900),
-    node_range: Tuple[int, int] = (20, 60),
-    edge_range: Tuple[int, int] = (1.0, 5.0),
+    figsize: tuple[int, int] = (900, 900),
+    node_range: tuple[int, int] = (20, 60),
+    edge_range: tuple[int, int] = (1.0, 5.0),
 ):
     if threshold > 0:
 
         values = nx.get_edge_attributes(network, weight_name).values()
         max_weight = max(1.0, max(values))
 
         print('Max weigth: {}'.format(max_weight))
@@ -107,34 +109,36 @@
         layout,
         weight=weight_name,
         scale=weight_scale,
         normalize=normalize_weights,
         project_range=edge_range,
     )
 
-    nodes_source = layout_source.create_nodes_data_source(sub_network, layout)
+    nodes_source: bm.ColumnDataSource = layout_source.create_nodes_data_source(sub_network, layout)
     nodes_community = metrics.compute_partition(sub_network)
-    community_colors = metrics.partition_colors(nodes_community, bokeh.palettes.Category20[20])
+    community_colors: list[str] = metrics.partition_colors(nodes_community, bokeh.palettes.Category20[20])
 
     nodes_source.add(nodes_community, 'community')
     nodes_source.add(community_colors, 'community_color')
 
     nodes_size = 5
     if node_proportions is not None:
         if isinstance(node_proportions, int):
             nodes_size = node_proportions
         else:
             nodes_size = 'size'
-            nodes_weight = project_values_to_range([node_proportions[n] for n in sub_network.nodes], *node_range)
+            nodes_weight = project_values_to_range([node_proportions[int(n)] for n in sub_network.nodes], *node_range)
             nodes_source.add(nodes_weight, nodes_size)
 
     node_opts = extend(dict(color='green', alpha=1.0), node_opts or {})
     line_opts = extend(dict(color='black', alpha=0.4), line_opts or {})
 
-    p = figure(plot_width=figsize[0], plot_height=figsize[1], x_axis_type=None, y_axis_type=None)
+    p = figure(
+        plot_width=figsize[0], plot_height=figsize[1], sizing_mode='scale_width', x_axis_type=None, y_axis_type=None
+    )
 
     _ = p.multi_line('xs', 'ys', line_width='weights', level='underlay', source=lines_source, **line_opts)
     r_nodes = p.circle('x', 'y', size=nodes_size, source=nodes_source, **node_opts)
 
     p.add_tools(
         bokeh.models.HoverTool(
             renderers=[r_nodes],
@@ -145,29 +149,30 @@
         )
     )
 
     text_opts = dict(x='x', y='y', text='name', level='overlay', x_offset=0, y_offset=0, text_font_size='12pt')
 
     r_nodes.glyph.fill_color = 'lightgreen'  # 'community_color'
 
+    # nodes_source.add([str(x) for x in nodes_source.data['name']], 'name')
     nodes_source.data['name'] = [str(x) for x in nodes_source.data['name']]  # pylint: disable=unsubscriptable-object
+
     p.add_layout(
         bm.LabelSet(source=nodes_source, text_align='center', text_baseline='middle', text_color='black', **text_opts)
     )
 
     return p
 
 
-def layout_args(layout_algorithm: str, network: nx.Graph, scale: float) -> Dict[str, Any]:
+def layout_args(layout_algorithm: str, network: nx.Graph, scale: float) -> dict[str, t.Any]:
     return _layout_args(layout_algorithm, network, scale)
 
 
-def get_layout_algorithm(layout_algorithm: str) -> Callable:
+def get_layout_algorithm(layout_algorithm: str) -> t.Callable:
     return _get_layout_algorithm(layout_algorithm)
 
 
 def project_series_to_range(series: pd.Series, low: float, high: float) -> pd.Series:
     return _project_series_to_range(series, low, high)
 
 
 plot_network = _plot_network
-plot_network = _plot_network
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/cluster_analysis/cluster_analysis_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/cluster_analysis/cluster_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/cluster_analysis/cluster_plot.py` & `humlab-penelope-0.7.9/penelope/notebook/cluster_analysis/cluster_plot.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/cluster_analysis/plot.py` & `humlab-penelope-0.7.9/penelope/notebook/cluster_analysis/plot.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/co_occurrence/explore_co_occurrence_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/co_occurrence/explore_co_occurrence_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/co_occurrence/load_co_occurrences_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/co_occurrence/load_co_occurrences_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/co_occurrence/main_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/co_occurrence/main_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/co_occurrence/tabular_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/co_occurrence/tabular_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/co_occurrence/to_co_occurrence_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/co_occurrence/to_co_occurrence_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/dtm/load_dtm_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/dtm/load_dtm_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/dtm/to_dtm_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/dtm/to_dtm_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/grid_utility.py` & `humlab-penelope-0.7.9/penelope/notebook/grid_utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     )
     grid.transform([{"type": "sort", "columnIndex": 0, "desc": False}])
     grid.auto_fit_params = {"area": "all", "padding": 40, "numCols": 1}
     grid.auto_fit_columns = True
     return grid
 
 
-def table_widget(data: pd.DataFrame, **kwargs) -> None:
+def table_widget(data: pd.DataFrame, **kwargs) -> dg.DataGrid:
 
     """If handler is passed, then create wrapper handler that passes row as argument"""
     handler: Callable[[pd.Series], None] = kwargs.pop('handler', None)
 
     _defaults: dict = dict(
         selection_mode="row",
         auto_fit_columns=True,
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/gui_base.py` & `humlab-penelope-0.7.9/penelope/notebook/gui_base.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/mdw/main_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/mdw/main_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/mdw/mdw_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/mdw/mdw_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/mixins.py` & `humlab-penelope-0.7.9/penelope/notebook/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 import contextlib
+import typing as t
 from collections import defaultdict
-from typing import Any, Callable, List, Mapping, Set, Tuple, Union
 
 import ipywidgets as w
 import pandas as pd
 from IPython.display import display as ipydisplay
 
 from penelope import utility as pu
 
 from . import utility as nu
 from .widgets_utils import register_observer
 
-PivotKeySpec = Mapping[str, Union[str, Mapping[str, int]]]
-PivotKeySpecArg = Union[List[PivotKeySpec], Mapping[str, List[PivotKeySpec]]]
+PivotKeySpec = dict[str, t.Union[str, dict[str, int]]]
+PivotKeySpecArg = t.Union[list[PivotKeySpec], dict[str, list[PivotKeySpec]]]
+
+# pylint: disable=no-member
 
 
 class DownloadMixIn:
     def __init__(self) -> None:
         super().__init__()
         self._download: w.Button = w.Button(description='Download', layout=dict(width='auto'))
         self._download_output: w.Output = w.Output()
@@ -37,15 +39,15 @@
 class PivotKeysMixIn:
     """Defines controls and event logics for pivot keys and filters for pivot key values."""
 
     def __init__(self, pivot_key_specs: PivotKeySpecArg = None, **kwargs):
 
         super().__init__(**kwargs)
 
-        self._display_event_handler: Callable[[Any], None] = None
+        self._display_event_handler: t.Callable[[t.Any], None] = None
 
         self.pivot_keys: pu.PivotKeys = (
             pivot_key_specs if isinstance(pivot_key_specs, pu.PivotKeys) else pu.PivotKeys(pivot_key_specs)
         )
 
         """Single-select"""
         single_key_options: dict = {v['text_name']: v['id_name'] for v in self.pivot_keys.pivot_keys.values()}
@@ -69,20 +71,20 @@
         self._unstack_tabular: w.ToggleButton = w.ToggleButton(
             description="Unstack", icon='check', value=False, layout=dict(width='140px')
         )
         self.autoselect_key_values: bool = False
         self.prevent_event: bool = False
 
     @property
-    def filter_key_values(self) -> List[str]:
+    def filter_key_values(self) -> list[str]:
         """Avaliable filter key values"""
         return self._filter_keys.options
 
     @property
-    def filter_key_selected_values(self) -> List[str]:
+    def filter_key_selected_values(self) -> list[str]:
         """Avaliable filter key values"""
         return self._filter_keys.value
 
     def setup(self, **kwargs) -> "PivotKeysMixIn":
         if hasattr(super(), 'setup'):
             getattr(super(), 'setup')(**kwargs)
         register_observer(self._multi_pivot_keys_picker, handler=self.pivot_key_handler, value=True)
@@ -113,28 +115,28 @@
 
     @property
     def picked_pivot_value_mapping(self) -> dict[int, str]:
         """Returns ID to VALUE-NAME mapping of picked pivot key (single picked dropdown)"""
         return self.pivot_keys.key_value_id2name(self.picked_pivot_name)
 
     @property
-    def pivot_keys_text_names(self) -> List[str]:
+    def pivot_keys_text_names(self) -> list[str]:
         """Return column names for selected the pivot keys"""
         return [x for x in self._multi_pivot_keys_picker.value if x != 'None']
 
     @property
-    def pivot_keys_id_names(self) -> List[str]:
+    def pivot_keys_id_names(self) -> list[str]:
         """Return ID column names for selected pivot key"""
         return [self.pivot_keys.key_name2key_id.get(x) for x in self.pivot_keys_text_names]
 
     @property
     def filter_opts(self) -> pu.PropertyValueMaskingOpts:
         """Returns user's filter selections as a name-to-values mapping."""
         key_values = defaultdict(list)
-        value_tuples: Tuple[str, str] = [x.split(': ') for x in self._filter_keys.value]
+        value_tuples: tuple[str, str] = [x.split(': ') for x in self._filter_keys.value]
         for k, v in value_tuples:
             key_values[k].append(v)
         filter_opts = self.pivot_keys.create_filter_key_values_dict(key_values, decode=True)
         if hasattr(super(), 'filter_opts'):
             filter_opts.update(super().filter_opts)
         return filter_opts
 
@@ -152,23 +154,23 @@
         try:
 
             if self.prevent_event:
                 return
 
             self.prevent_event = True
 
-            old_keys: Set[str] = set(change['old']) - set(('None',))
-            new_keys: Set[str] = set(change['new']) - set(('None',))
+            old_keys: set[str] = set(change['old']) - set(('None',))
+            new_keys: set[str] = set(change['new']) - set(('None',))
 
-            add_options: Set[str] = set(self.pivot_keys.key_values_str(new_keys - old_keys, sep=': '))
-            del_options: Set[str] = set(self.pivot_keys.key_values_str(old_keys - new_keys, sep=': '))
+            add_options: set[str] = set(self.pivot_keys.key_values_str(new_keys - old_keys, sep=': '))
+            del_options: set[str] = set(self.pivot_keys.key_values_str(old_keys - new_keys, sep=': '))
 
-            ctrl_options: Set[str] = (set(self._filter_keys.options) - del_options) | add_options
-            current_values: Set[str] = set(self._filter_keys.value)
-            ctrl_values: Set[str] = (current_values - del_options) | (
+            ctrl_options: set[str] = (set(self._filter_keys.options) - del_options) | add_options
+            current_values: set[str] = set(self._filter_keys.value)
+            ctrl_values: set[str] = (current_values - del_options) | (
                 add_options if self.autoselect_key_values else set()
             )
 
             values_changed: bool = ctrl_values != current_values
 
             if values_changed:
                 self._filter_keys.value = []
@@ -177,34 +179,38 @@
 
             if values_changed:
                 self._filter_keys.value = sorted(list(ctrl_values))
 
         finally:
             self.prevent_event = False
 
-    def observe(self, value: bool, *, handler: Callable[[Any], None], **kwargs) -> None:
+    def display_trigger_ctrls(self) -> list[w.Widget]:
+        return (
+            [self._unstack_tabular, self._filter_keys]
+            if self.pivot_keys.has_pivot_keys
+            else [self._multi_pivot_keys_picker]
+        )
+
+    def observe(self, value: bool, *, handler: t.Callable[[t.Any], None], **kwargs) -> None:
 
         if handler is None:
             return
 
         self._display_event_handler = handler
 
-        display_trigger_ctrls: List[Any] = (
-            [self._unstack_tabular, self._filter_keys, self._unstack_tabular]
-            if self.pivot_keys.has_pivot_keys
-            else [self._multi_pivot_keys_picker]
-        )
-
-        for ctrl in display_trigger_ctrls:
+        for ctrl in self.display_trigger_ctrls():
             register_observer(ctrl, handler=handler, value=value)
 
         if hasattr(super(), "observe"):
             getattr(super(), "observe")(value=value, handler=handler, **kwargs)
 
     def default_pivot_keys_layout(self, vertical: bool = False, **kwargs) -> w.Widget:
+        if not self.pivot_keys.has_pivot_keys:
+            return w.VBox()
+
         width: str = kwargs.get('width', '100px')
         self._filter_keys.rows = kwargs.get('rows', 12)
         self._filter_keys.layout = kwargs.get('layout', dict(width='120px'))
         self._multi_pivot_keys_picker.layout = kwargs.get('layout', dict(width=width))
         if vertical:
             return w.VBox(
                 [
@@ -216,7 +222,83 @@
             )
         return w.HBox(
             [
                 w.VBox([w.HTML("<b>Filter by</b>"), self._multi_pivot_keys_picker]),
                 w.VBox([w.HTML("<b>Value</b>"), self._filter_keys]),
             ]
         )
+
+
+class MultiLinePivotKeysMixIn(PivotKeysMixIn):
+    def __init__(self, pivot_key_specs: t.Any = None, **kwargs):
+        super().__init__(pivot_key_specs, **kwargs)
+        self._line_name: w.Text = w.Text(description="", layout=dict(width='80px'))
+        self._add_line: w.Button = w.Button(description="➕")
+        self._del_line: w.Button = w.Button(description="➖")
+        self._lines: w.Dropdown = w.Dropdown()
+
+    def default_pivot_keys_layout(self, vertical: bool = False, **kwargs) -> w.Widget:
+        width: str = kwargs.get('width', '120px')
+        self._filter_keys.rows = kwargs.get('rows', 12)
+        self._filter_keys.layout = kwargs.get('layout', dict(width=width))
+        # self._single_pivot_key_picker.layout = kwargs.get('layout', dict(width=width))
+        return w.VBox(
+            [
+                w.HBox([self._lines, self._del_line]),
+                self._filter_keys,
+                w.HBox([w.HTML("Add line:"), self._line_name, self._add_line]),
+            ]
+        )
+
+    def display_trigger_ctrls(self) -> list[w.Widget]:
+        return []
+
+    def setup(self, **kwargs) -> "PivotKeysMixIn":
+        if hasattr(super(), 'setup'):
+            getattr(super(), 'setup')(**kwargs)
+        self._add_line.on_click(self._add_line_callback)
+        self._del_line.on_click(self._del_line_callback)
+        self._lines.observe(self.line_selected, type='change')
+        return self
+
+    def _add_line_callback(self, *_):
+        self.add_line(name=self.line_name, values=self.filter_key_selected_values)
+        self._line_name.value = ""
+        self._filter_keys.value = []
+
+    def add_line(self, name: str, values: list[str]):
+        if not name:
+            self.alert("😡 you must give the line a name")
+            return
+        if not values:
+            self.alert("😡 please select value(s) that define the line")
+            return
+        self._lines.options = list(self._lines.options or []) + [(name, values)]
+        self.alert(f"✅ {name} added!")
+
+    def _del_line_callback(self, *_):
+        if not self._lines.options:
+            self.alert("😡 no lines to delete")
+            return
+        if not self._lines.value:
+            self.alert("😡 please select line to delete")
+        options = list(self._lines.options)
+        name = options[self._lines.index][0]
+        del options[self._lines.index]
+        self._lines.value = None
+        self._lines.options = options
+        self.alert(f"✅ {name} deleted")
+        if options:
+            self._lines.index = 0
+
+    def line_selected(self, *_):
+        if self._lines.value:
+            self._line_name.value = self._lines.options[self._lines.index][0]
+            self._filter_keys.value = self._lines.options[self._lines.index][1]
+
+    @property
+    def line_name(self) -> str:
+        return self._line_name.value
+
+    @property
+    def lines(self) -> list:
+        return self._lines.options or []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/token_counts/dtm_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/token_counts/dtm_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/token_counts/pipeline_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/token_counts/pipeline_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/token_counts/plot.py` & `humlab-penelope-0.7.9/penelope/notebook/token_counts/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import bokeh.models
 import bokeh.plotting
 import numpy as np
 import pandas as pd
 import scipy
 from bokeh.plotting import Figure, figure
 
-from penelope.notebook.word_trends.displayers.utils import generate_temporal_ticks
+from penelope.notebook.utility import generate_temporal_ticks
 from penelope.utility import take
 
 DEFAULT_FIGOPTS: dict = dict(plot_width=1000, plot_height=600)
 DEFAULT_PALETTE = bokeh.palettes.Category10[10]
 
 
 def generate_colors(n: int, palette: Sequence[str]) -> Iterable[str]:
@@ -39,15 +39,15 @@
     figopts = {**DEFAULT_FIGOPTS, **(figopts or {})}
 
     columns: List[str] = df.columns.tolist()
 
     data_source: dict = dict(category=[str(x) for x in df.index], **{column: df[column] for column in columns})
     colors: Iterable[str] = generate_colors(len(columns), DEFAULT_PALETTE)
 
-    p: Figure = figure(x_range=data_source['category'], **figopts)
+    p: Figure = figure(x_range=data_source['category'], **figopts, sizing_mode='scale_width')
 
     p.left[0].formatter.use_scientific = False  # pylint: disable=unsubscriptable-object
 
     p.vbar_stack(columns, x='category', color=colors, width=0.9, source=data_source, legend_label=columns)
 
     p.y_range.start = 0
     p.x_range.range_padding = 0.1
@@ -86,15 +86,15 @@
 
     if smooth:
         df = pchip_interpolate_frame(df).set_index('category') if smooth else df
         x_ticks = generate_temporal_ticks(df.index.tolist())
 
     data_source: dict = to_multiline_data_source(data=df, smoother=None)
 
-    p: Figure = figure(**(figopts or {}))
+    p: Figure = figure(**(figopts or {}), sizing_mode='scale_width')
 
     p.left[0].formatter.use_scientific = False  # pylint: disable=unsubscriptable-object
     p.y_range.start = 0
     p.yaxis.axis_label = 'Frequency'
     p.toolbar.autohide = True
 
     if x_ticks is not None:
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/__init__.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/edit_topic_labels_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/edit_topic_labels_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/load_topic_model_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/load_topic_model_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/mixins.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 
     @property
     def inferred_n_topics(self) -> int:
         return self.inferred_topics.num_topics
 
     @property
     def topic_labels(self) -> dict[int, str]:
-        if 'label' in self.inferred_topics.topic_token_overview.columns:
-            return self.inferred_topics.topic_token_overview['label'].to_dict()
-        return None
+        return self.inferred_topics.topic_labels
+
+    def topic_label(self, topic_id: int) -> str:
+        return self.topic_labels.get(topic_id, f"#{topic_id}")
 
     def topic_id_options(self) -> list[tuple[str, int]]:
         fx: Callable[[int], str] = self.inferred_topics.topic_labels.get
         options = [(fx(i, f'Topic #{i}'), i) for i in range(0, self.inferred_n_topics)]
         return options
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/model_container.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/model_container.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/pivot_network_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/pivot_network_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_document_network_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_document_network_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,17 @@
             ["document_name"]
         ]
         network_data = network_data.pipe(pu.set_index, columns='document_id').merge(
             di, left_index=True, right_index=True
         )
         network_data["title"] = network_data["document_name"]
 
+        if self.topic_labels is not None:
+            network_data['topic_id'] = network_data['topic_id'].apply(self.topic_labels.get)
+
         if len(network_data) == 0:
             raise pu.EmptyDataError()
 
         return network_data
 
     def update_handler(self, *_):
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_documents_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_documents_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,15 @@
     def update(self) -> pd.DataFrame:
         data: pd.DataFrame = (
             self.inferred_topics.calculator.reset()
             .filter_by_data_keys(topic_id=self.topic_id)
             .threshold(self.threshold)
             .filter_by_document_keys(**self.filter_opts.opts)
             .filter_by_n_top(self.max_count)
+            .overload("document_name,n_raw_tokens,n_tokens")
             .value
         )
         return data
 
     def update_handler(self, *_):
         self._text.value = self.inferred_topics.get_topic_title2(self.topic_id)
         super().update_handler()
@@ -250,14 +251,15 @@
     def update(self) -> pd.DataFrame:
         data: pd.DataFrame = (
             self.inferred_topics.calculator.reset()
             .filter_by_text(search_text=self.text, n_top=self.n_top_token)
             .threshold(self.threshold)
             .filter_by_document_keys(**self.filter_opts.opts)
             .filter_by_n_top(self.max_count)
+            .overload("document_name,n_raw_tokens,n_tokens")
             .value
         )
         return data
 
     def update_handler(self, *_):
 
         if len(self.text) < 3:
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_model_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_model_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_titles_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_titles_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_topic_network_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_topic_network_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     def compute(self) -> pd.DataFrame:
         return (
             self.inferred_topics.calculator.reset()
             .filter_by_keys(**self.filter_opts.opts)
             .threshold(threshold=self.threshold)
             .filter_by_topics(topic_ids=self.topic_ids, negate=self.exclude_mode)
-            .to_topic_topic_network(self.n_docs, topic_labels=None)
+            .to_topic_topic_network(self.n_docs, topic_labels=self.topic_labels)
         ).value
 
     def update(self) -> pd.DataFrame:
 
         network_data: pd.DataFrame = self.compute()
 
         if len(network_data) == 0:
@@ -190,58 +190,63 @@
         return network_data
 
     def update_handler(self, *_):
 
         self.alert("⌛ Computing...")
         try:
             self.network_data = self.update()
-            self.alert("✅")
+            self.alert(f"✅ {len(self.network_data)} records found.")
         except pu.EmptyDataError:
             self.network_data = None
         except Exception as ex:
             self.warn(f"😡 {ex}")
 
         self.display_handler()
 
     def display_handler(self, *_):
 
-        self._output.clear_output()
+        try:
+
+            self._output.clear_output()
+
+            with self._output:
 
-        with self._output:
+                if self.network_data is None:
 
-            if self.network_data is None:
+                    self.alert("😡 No data, please change filters..")
 
-                self.alert("😡 No data, please change filters..")
+                elif self.output_format in ('xlsx', 'csv', 'clipboard', 'table', 'gephi'):
 
-            elif self.output_format in ('xlsx', 'csv', 'clipboard', 'table', 'gephi'):
+                    data: pd.DataFrame = self.network_data
 
-                data: pd.DataFrame = self.network_data
+                    if self.output_format == "gephi":
+                        data = data[['topic_id', "title", 'weight']]
+                        data.columns = ['Source', 'Target', 'Weight']
 
-                if self.output_format == "gephi":
-                    data = data[['topic_id', "title", 'weight']]
-                    data.columns = ['Source', 'Target', 'Weight']
+                    if self.output_format != "table":
+                        pu.ts_store(data=data, extension=self.output_format, basename='heatmap_weights')
 
-                if self.output_format != "table":
-                    pu.ts_store(data=data, extension=self.output_format, basename='heatmap_weights')
+                    g: gu.TableWidget = gu.table_widget(data)
+                    display(g)
 
-                g: gu.TableWidget = gu.table_widget(data)
-                display(g)
+                else:
 
-            else:
+                    display_topic_topic_network(
+                        data=self.network_data,
+                        layout=self._network_layout.value,
+                        titles=self.titles,
+                        scale=self._scale.value,
+                        element_id=self.text_id,
+                        node_range=self._node_range.value,
+                        edge_range=self._edge_range.value,
+                        topic_proportions=self.topic_proportions,
+                    )
 
-                display_topic_topic_network(
-                    data=self.network_data,
-                    layout=self._network_layout.value,
-                    titles=self.titles,
-                    scale=self._scale.value,
-                    element_id=self.text_id,
-                    node_range=self._node_range.value,
-                    edge_range=self._edge_range.value,
-                    topic_proportions=self.topic_proportions,
-                )
+        except Exception as ex:
+            self.warn(f"😡 {ex}")
 
     @property
     def threshold(self) -> float:
         """Threshodl for topic's weight in document"""
         return self._threshold.value
 
     @property
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_topic_network_gui_utility.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_topic_network_gui_utility.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,38 +16,32 @@
     scale: float = 1.0,
     element_id: str = '',
     titles=None,
     topic_proportions=None,
     node_range: Tuple[int, int] = (20, 60),
     edge_range: Tuple[int, int] = (1, 10),
 ):
-    try:
+    if len(data) == 0:
+        logger.info('No data. Please change selections.')
+        return
 
-        if len(data) == 0:
-            logger.info('No data. Please change selections.')
-            return
-
-        network = network_utility.create_network(
-            data,
-            source_field='source',
-            target_field='target',
-            weight='n_docs',
-        )
-        p = plot_utility.plot_network(
-            network=network,
-            layout_algorithm=layout,
-            scale=scale,
-            threshold=0.0,
-            node_description=titles,
-            node_proportions=topic_proportions,
-            weight_scale=1.0,
-            normalize_weights=False,
-            element_id=element_id,
-            figsize=(1200, 800),
-            node_range=node_range,
-            edge_range=edge_range,
-        )
-        bokeh.plotting.show(p)
-
-    except Exception as ex:  # pylint: disable=bare-except
-        print("No data: please adjust filters")
-        logger.info(ex)
+    network = network_utility.create_network(
+        data,
+        source_field='source',
+        target_field='target',
+        weight='n_docs',
+    )
+    p = plot_utility.plot_network(
+        network=network,
+        layout_algorithm=layout,
+        scale=scale,
+        threshold=0.0,
+        node_description=titles,
+        node_proportions=topic_proportions,
+        weight_scale=1.0,
+        normalize_weights=False,
+        element_id=element_id,
+        figsize=(1200, 800),
+        node_range=node_range,
+        edge_range=edge_range,
+    )
+    bokeh.plotting.show(p)
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,36 +28,40 @@
             'handle_color': 'lightblue',
         }
         timespan: tuple[int, int] = self.inferred_topics.timespan
         yearspan: tuple[int, int] = self.inferred_topics.startspan(10)
 
         self._text: w.HTML = w.HTML()
 
-        weighings = [(x['description'], x['key']) for x in tm.YEARLY_AVERAGE_COMPUTE_METHODS]
+        weighings = [(x['short_description'], x['key']) for x in tm.YEARLY_AVERAGE_COMPUTE_METHODS]
 
         self._aggregate: w.Dropdown = w.Dropdown(options=weighings, value='true_average_weight')
 
         self._year_range_label: w.HTML = w.HTML("Years")
         self._year_range: w.IntRangeSlider = w.IntRangeSlider(
             min=timespan[0], max=timespan[1], value=yearspan, **slider_opts
         )
         self._threshold_label: w.HTML = w.HTML("<b>Threshold</b>")
         self._threshold: w.FloatSlider = w.FloatSlider(min=0.01, max=1.0, value=0.05, step=0.01, **slider_opts)
 
         self._output_format: w.Dropdown = w.Dropdown(
             options=['Chart', 'Table', 'xlsx', 'csv', 'clipboard', 'pandas'], value='Chart'
         )
         self._output: w.Output = w.Output()
-        self._compute_handler: Callable[[Any], None] = self.update_handler
+        self._compute_handler: Callable[[Any], None] = self._compute_handler_callback
         self._content_placeholder: w.Box = None
         self._extra_placeholder: w.VBox = w.HBox()
         self._aggregate.layout.width = '140px'
         self._auto_compute.layout.width = "80px"
         self._output_format.layout.width = '140px'
 
+    def _compute_handler_callback(self, *args, **kwargs) -> None:
+        """level of indirection to allow override of update_handler"""
+        self.update_handler(*args, **kwargs)
+
     def setup(self, **kwargs) -> "TopicTrendsGUI":
         super().setup(**kwargs)
 
         self.topic_id = (0, self.inferred_n_topics - 1, self.inferred_topics.topic_labels)
         self.observe_slider_update_label(self._year_range, self._year_range_label, "Years")
         self.observe_slider_update_label(self._threshold, self._threshold_label, "Threshold")
         self.observe(value=True, handler=self.update_handler)
@@ -120,15 +124,15 @@
             .threshold(self.threshold)
             .filter_by_keys(**self.filter_opts.opts)
             .yearly_topic_weights(self.get_result_threshold(), n_top_relevance=n_top_relevance)
             .value
         )
         return yearly_weights
 
-    def update_handler(self, *_):
+    def update_handler(self, *args, **kwargs):  # pylint: disable=unused-argument
 
         self.alert("⌛ Computing...")
         try:
             self.yearly_topic_weights = self.update()
             self.alert("✅")
         except pu.EmptyDataError:
             self.yearly_topic_weights = None
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_gui_utility.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_gui_utility.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         toolbar_location="right",
         x_range=list(map(str, range(year_range[0], year_range[1] + 1))),
         y_range=(0.0, ys.max()),
     )
 
     figopts: dict = {**default_figopts, **figopts}
 
-    p: bp.Figure = bp.figure(**figopts)
+    p: bp.Figure = bp.figure(**figopts, sizing_mode='scale_width')
 
     _ = p.vbar(x=xs, top=ys, width=0.5, fill_color="#b3de69")
 
     p.xaxis.major_label_orientation = math.pi / 4
     p.xgrid.grid_line_color = None
     p.left[0].formatter.use_scientific = False  # pylint: disable=unsubscriptable-object
     p.xaxis[0].axis_label = (x_label or category_column.title().replace('_', ' ')).title()
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_overview_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_overview_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_trends_overview_gui_utility.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_trends_overview_gui_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     if x_range is not None:
         figopts['x_range'] = x_range
 
     if y_range is not None:
         figopts['y_range'] = y_range
         figopts['plot_height'] = max(len(y_range) * line_height, 600)
 
-    p = bokeh.plotting.figure(**figopts)
+    p = bokeh.plotting.figure(**figopts, sizing_mode='scale_width')
 
     cr = p.rect(
         x=xs,
         y=ys,
         source=source,
         alpha=1.0,
         hover_color='red',
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_word_distribution_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_word_distribution_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 
 def plot_topic_word_distribution(tokens: pd.DataFrame, **args):
 
     source = bokeh.models.ColumnDataSource(tokens)
 
-    p = bokeh.plotting.figure(toolbar_location="right", **args)
+    p = bokeh.plotting.figure(toolbar_location="right", sizing_mode='scale_width', **args)
     p.left[0].formatter.use_scientific = False  # pylint: disable=unsubscriptable-object
 
     _ = p.circle(x='xs', y='ys', source=source)
 
     label_style = dict(level='overlay', text_font_size='8pt', angle=np.pi / 6.0)
 
     text_aligns = ['left', 'right']
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topic_wordcloud_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topic_wordcloud_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/topics_token_network_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/topics_token_network_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/topic_modelling/train_gui/topic_model_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/topic_modelling/train_gui/topic_model_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/utility.py` & `humlab-penelope-0.7.9/penelope/notebook/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,14 +177,32 @@
     if palette in all_palettes:
         palette_id: int = palette_id if palette_id is not None else max(all_palettes[palette].keys())
         return list(islice(cycle(all_palettes[palette][palette_id]), n))
 
     raise ValueError(f"unknown palette {palette}")
 
 
+def generate_temporal_ticks(categories: list[int], n_tick: int = 5) -> list[int]:
+    """Gets ticks every n_tick years if category is year
+    Returns all categories if all values are either, lustrum and decade"""
+
+    if all(int(x) % 5 in (0, 5) for x in categories):
+        return categories
+
+    return list(range(low_bound(categories, n_tick), high_bound(categories, n_tick) + 1, n_tick))
+
+
+def high_bound(categories: list[int], n_tick: int) -> tuple[int, int]:
+    return (lambda x: x if x % n_tick == 0 else x + (n_tick - x % n_tick))(int(max(categories)))
+
+
+def low_bound(categories: list[int], n_tick: int) -> int:
+    return (lambda x: x - (x % n_tick))(int(min(categories)))
+
+
 class FileChooserExt(ipyfilechooser.FileChooser):
 
     label_max_length = 50
 
     _LBL_TEMPLATE = types.SimpleNamespace(
         format=lambda p, c: super()._LBL_TEMPLATE.format(
             shorten_path_with_ellipsis(p, FileChooserExt.label_max_length),
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/widgets_utils.py` & `humlab-penelope-0.7.9/penelope/notebook/widgets_utils.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/__init__.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/archive/compile_mixins.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/archive/compile_mixins.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/archive/deprecated_plot.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/archive/deprecated_plot.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/archive/display_top_table2.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/archive/display_top_table2.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_bar.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from typing import Iterable, List, Sequence
 
 import bokeh.models as bm
 import bokeh.plotting as bp
 import pandas as pd
 from bokeh.io import show
 
-from ...utility import generate_colors
+from ...utility import generate_colors, generate_temporal_ticks
 from .interface import ITrendDisplayer
-from .utils import generate_temporal_ticks
 
 
 class BarDisplayer(ITrendDisplayer):
     def __init__(self, name: str = "Bar", **opts):
         super().__init__(name=name, **opts)
         self.year_tick: int = 5
 
@@ -48,15 +47,15 @@
             **{temporal_key: [str(x) for x in unstacked_data.index]},
         }
 
         value_fields: List[str] = [w for w in plot_data.keys() if w not in (temporal_key, 'year')]
         colors: Iterable[str] = iter(generate_colors(len(value_fields)))
         source = bm.ColumnDataSource(data=plot_data)
 
-        p: bp.Figure = bp.figure(plot_height=self.height, plot_width=self.width, title="TF")
+        p: bp.Figure = bp.figure(plot_height=self.height, plot_width=self.width, sizing_mode='scale_width', title="TF")
 
         offset: float = -0.25
         v: List[bm.GlyphRenderer] = []
         for value_field in value_fields:
             w: bm.GlyphRenderer = p.vbar(x=temporal_key, top=value_field, width=1.0, source=source, color=next(colors))
             offset += 0.25
             v.append(w)
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_line.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 import bokeh.models as bm
 import bokeh.plotting as bp
 import ipywidgets
 import pandas as pd
 from bokeh.io import push_notebook
 
-from penelope.notebook.utility import generate_colors
+from penelope.notebook.utility import generate_colors, generate_temporal_ticks
 
 from .interface import ITrendDisplayer
-from .utils import generate_temporal_ticks
 
 
 class LineDisplayer(ITrendDisplayer):
     def __init__(self, name: str = "Line", **opts):
         super().__init__(name=name, **opts)
 
         self.chart: bp.Figure = None
@@ -26,15 +25,15 @@
 
         self.output = ipywidgets.Output()
         self.data_source = bm.ColumnDataSource(dict(xs=[[0]], ys=[[0]], labels=[""], colors=['red']))
         self.chart = self.figure(data_source=self.data_source)
 
     def figure(self, *, data_source: bm.ColumnDataSource, x_ticks: Sequence[int] = None):
 
-        p = bp.figure(plot_width=self.width, plot_height=self.height)
+        p = bp.figure(plot_width=self.width, plot_height=self.height, sizing_mode='scale_width')
 
         p.y_range.start = 0
         p.yaxis.axis_label = 'Frequency'
         p.toolbar.autohide = True
 
         if x_ticks is not None:
             p.xaxis.ticker = x_ticks
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_network.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_network.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_stackedbar.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_stackedbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 
         source = bm.ColumnDataSource(data=plot_data)
 
         temporal_values: List[str] = [str(x) for x in plot_data[temporal_key]]
         tokens: List[str] = [t for t in plot_data.keys() if t != temporal_key]
         colors: List[str] = generate_colors(len(tokens))
 
-        p: bp.Figure = bp.figure(x_range=temporal_values, height=self.height, width=self.width, title="TF")
+        p: bp.Figure = bp.figure(
+            x_range=temporal_values, height=self.height, width=self.width, sizing_mode='scale_width', title="TF"
+        )
 
         p.vbar_stack(tokens, x=temporal_key, width=0.9, color=colors, source=source, legend_label=tokens)
 
         p.y_range.start = 0
         p.x_range.range_padding = 0.02
         p.xaxis.major_label_orientation = math.pi / 4
         # p.xaxis.ticker = generate_temporal_ticks(plot_data[temporal_key])
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_table.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_table.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/display_top_table.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/display_top_table.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/interface.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/interface.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/displayers/plotter.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/displayers/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     Returns
     -------
     Figure
     """
     if plot is None:
 
         p: Figure = bokeh.plotting.figure(
-            plot_width=kwargs.get('plot_width', 400), plot_height=kwargs.get('plot_height', 200)
+            plot_width=kwargs.get('plot_width', 400),
+            plot_height=kwargs.get('plot_height', 200),
+            sizing_mode='scale_width',
         )
         p.y_range.start = 0
         # p.y_range.end = 0.5
         # p.title.text = title.upper()
         p.yaxis.axis_label = 'Frequency'
         p.toolbar.autohide = True
         if ticker_labels is not None:
```

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/gof_and_trends_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/gof_and_trends_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/gofs_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/gofs_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/interface.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/interface.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/main_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/main_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/trends_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/trends_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/notebook/word_trends/trends_with_picks_gui.py` & `humlab-penelope-0.7.9/penelope/notebook/word_trends/trends_with_picks_gui.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/__init__.py` & `humlab-penelope-0.7.9/penelope/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/checkpoint/checkpoint.py` & `humlab-penelope-0.7.9/penelope/pipeline/checkpoint/checkpoint.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/checkpoint/feather.py` & `humlab-penelope-0.7.9/penelope/pipeline/checkpoint/feather.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/checkpoint/interface.py` & `humlab-penelope-0.7.9/penelope/pipeline/checkpoint/interface.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/checkpoint/legacy.py` & `humlab-penelope-0.7.9/penelope/pipeline/checkpoint/legacy.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/checkpoint/load.py` & `humlab-penelope-0.7.9/penelope/pipeline/checkpoint/load.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/checkpoint/serialize.py` & `humlab-penelope-0.7.9/penelope/pipeline/checkpoint/serialize.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/checkpoint/utility.py` & `humlab-penelope-0.7.9/penelope/pipeline/checkpoint/utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/builder.py` & `humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/builder.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/legacy/pipelines.py` & `humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/legacy/pipelines.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/legacy/tasks.py` & `humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/legacy/tasks.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/pipeline_mixin.py` & `humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/pipelines.py` & `humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/pipelines.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/tasks.py` & `humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/tasks.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/co_occurrence/tasks_pool.py` & `humlab-penelope-0.7.9/penelope/pipeline/co_occurrence/tasks_pool.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/config.py` & `humlab-penelope-0.7.9/penelope/pipeline/config.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/convert.py` & `humlab-penelope-0.7.9/penelope/pipeline/convert.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/dtm/pipeline_mixin.py` & `humlab-penelope-0.7.9/penelope/pipeline/dtm/pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/dtm/pipelines.py` & `humlab-penelope-0.7.9/penelope/pipeline/dtm/pipelines.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/dtm/tasks.py` & `humlab-penelope-0.7.9/penelope/pipeline/dtm/tasks.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/dtm/vectorizer.py` & `humlab-penelope-0.7.9/penelope/pipeline/dtm/vectorizer.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/interfaces.py` & `humlab-penelope-0.7.9/penelope/pipeline/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
             columns['text_column'],
             columns['pos_column'],
             columns['lemma_column'],
         )
 
     def extend(self, _: DocumentPayload):
         """Add properties of `other` to self. Used when combining two pipelines"""
-        ...
 
     def extend_document_index(self, other_index: DocumentIndex) -> "PipelinePayload":
         if self.effective_document_index is None:
             self.effective_document_index = other_index
         else:
             self.effective_document_index = (
                 DocumentIndexHelper(self.effective_document_index).extend(other_index).document_index
```

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/phrases.py` & `humlab-penelope-0.7.9/penelope/pipeline/phrases.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/pipeline.py` & `humlab-penelope-0.7.9/penelope/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/pipeline_mixin.py` & `humlab-penelope-0.7.9/penelope/pipeline/pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/pipelines.py` & `humlab-penelope-0.7.9/penelope/pipeline/pipelines.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/spacy/convert.py` & `humlab-penelope-0.7.9/penelope/pipeline/spacy/convert.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/spacy/pipeline_mixin.py` & `humlab-penelope-0.7.9/penelope/pipeline/spacy/pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/spacy/pipelines.py` & `humlab-penelope-0.7.9/penelope/pipeline/spacy/pipelines.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/spacy/tasks.py` & `humlab-penelope-0.7.9/penelope/pipeline/spacy/tasks.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/sparv/convert.py` & `humlab-penelope-0.7.9/penelope/pipeline/sparv/convert.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/sparv/pipelines.py` & `humlab-penelope-0.7.9/penelope/pipeline/sparv/pipelines.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/tagged_frame.py` & `humlab-penelope-0.7.9/penelope/pipeline/tagged_frame.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/tasks.py` & `humlab-penelope-0.7.9/penelope/pipeline/tasks.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/tasks_mixin.py` & `humlab-penelope-0.7.9/penelope/pipeline/tasks_mixin.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/topic_model/pipeline_mixin.py` & `humlab-penelope-0.7.9/penelope/pipeline/topic_model/pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/topic_model/pipelines.py` & `humlab-penelope-0.7.9/penelope/pipeline/topic_model/pipelines.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/pipeline/topic_model/tasks.py` & `humlab-penelope-0.7.9/penelope/pipeline/topic_model/tasks.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/plot/colors.py` & `humlab-penelope-0.7.9/penelope/plot/colors.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/plot/wordcloud_utility.py` & `humlab-penelope-0.7.9/penelope/plot/wordcloud_utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/resources/fox_stopwords.py` & `humlab-penelope-0.7.9/penelope/resources/fox_stopwords.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/co_occurrence.py` & `humlab-penelope-0.7.9/penelope/scripts/co_occurrence.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/co_occurrence.sh` & `humlab-penelope-0.7.9/penelope/scripts/co_occurrence.sh`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/dtm/vectorize.py` & `humlab-penelope-0.7.9/penelope/scripts/dtm/vectorize.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/dtm/vectorize_id.py` & `humlab-penelope-0.7.9/penelope/scripts/dtm/vectorize_id.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/legacy/coherence.py` & `humlab-penelope-0.7.9/penelope/scripts/legacy/coherence.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/legacy/install-spacy-models.sh` & `humlab-penelope-0.7.9/penelope/scripts/legacy/install-spacy-models.sh`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/legacy/sparv-xml-extract-text.py` & `humlab-penelope-0.7.9/penelope/scripts/legacy/sparv-xml-extract-text.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/pos_tag.py` & `humlab-penelope-0.7.9/penelope/scripts/pos_tag.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/tm/mallet2topicsdata.py` & `humlab-penelope-0.7.9/penelope/scripts/tm/mallet2topicsdata.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/tm/predict.py` & `humlab-penelope-0.7.9/penelope/scripts/tm/predict.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/tm/train.py` & `humlab-penelope-0.7.9/penelope/scripts/tm/train.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/tm/train_id.py` & `humlab-penelope-0.7.9/penelope/scripts/tm/train_id.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/tm/train_legacy.py` & `humlab-penelope-0.7.9/penelope/scripts/tm/train_legacy.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/scripts/utils.py` & `humlab-penelope-0.7.9/penelope/scripts/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from penelope import pipeline, utility
 
 try:
     import click
 except ImportError:
     click = object()
 
+# pylint: disable=no-member
 
 CLI_LOG_PATH = './logs'
 
 CLI_OPTIONS = {
     '--alpha': dict(help='Prior belief of topic probability. symmetric/asymmetric/auto', default='asymmetric'),
     '--append-pos': dict(help='Append PoS to tokems', default=False, is_flag=True),
     '--compute-chunk-size': dict(help='Compute process chunk size', default=10, type=click.INT),
```

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/__init__.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/__init__.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/__init__.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/coherence.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/coherence.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/convert.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/convert.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/options.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/options.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/predict.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/predict.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/train.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/train.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_gensim/utility.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_gensim/utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_textacy/__init__.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_textacy/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_textacy/predict.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_textacy/predict.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/engine_textacy/train.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/engine_textacy/train.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/engines/interface.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/engines/interface.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/interfaces.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/interfaces.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/predict.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/predict.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/rdb/data.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/rdb/data.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/saliency/saliency.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/saliency/saliency.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/__init__.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,26 @@
     TopicPrevalenceOverTimeCalculator,
     compute_yearly_topic_weights,
 )
 from .token import TopicTokensMixIn, get_topic_title, get_topic_title2, get_topic_titles, top_topic_token_weights
 from .topics_data import InferredTopicsData, PickleUtility
 
 YEARLY_AVERAGE_COMPUTE_METHODS = [
-    {'key': 'max_weight', 'description': 'Max value', 'tooltip': 'Use maximum value over documents'},
+    {
+        'key': 'max_weight',
+        'description': 'Max value',
+        'short_description': 'Max value',
+        'tooltip': 'Use maximum value over documents',
+    },
     {
         'key': 'average_weight',
         'description': 'Average of document-topic weights filtered by threshold',
+        'short_description': 'Average above threshold',
         'tooltip': 'Use average of document where topic is returned by engine (Gensim skips weights less than 1%), above 0 or above given threshold',
     },
     {
         'key': 'true_average_weight',
         'description': 'Average of all documents, even those where weight is 0',
+        'short_description': 'Average of all weights',
         'tooltip': 'Use average of all document weights even those where topic weight is 0',
     },
 ]
```

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/document.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,20 +213,26 @@
         return self
 
     def topic_proportions(self) -> pd.DataFrame:
         """Compute topics' proportion in entire corpus."""
         data: pd.DataFrame = compute_topic_proportions(self.data, self.document_index)
         return data
 
-    def yearly_topic_weights(self, result_threshold: float, n_top_relevance: int) -> "DocumentTopicsCalculator":
+    def yearly_topic_weights(
+        self,
+        result_threshold: float,
+        n_top_relevance: int,
+        topic_ids: None | int | list[int] = None,
+    ) -> "DocumentTopicsCalculator":
         self.data = prevelance.compute_yearly_topic_weights(
             self.data,
             document_index=self.document_index,
             threshold=result_threshold or 0,
             n_top_relevance=n_top_relevance,
+            topic_ids=topic_ids,
         )
         return self
 
     def to_topic_topic_network(
         self,
         n_docs: int,
         pivot_keys: list[str] | str = None,
```

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/prevelance.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/prevelance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import abc
 import itertools
-from typing import TYPE_CHECKING, List, NamedTuple, Tuple
+from typing import TYPE_CHECKING, Literal, NamedTuple, get_args
 
 import numpy as np
 import pandas as pd
 
 from penelope import utility as pu
 
 if TYPE_CHECKING:
@@ -143,33 +143,45 @@
         document_topic_weights[document_topic_weights.weight >= threshold]
         .groupby(['year', 'topic_id'])
         .agg(**{target_name: ('weight', np.mean)})
     )
     return yearly_weights
 
 
-def _compute_yearly_topic_weights(dtw: pd.DataFrame) -> pd.DataFrame:
+def _compute_yearly_topic_weights_statistics(
+    dtw: pd.DataFrame,
+    topic_ids: None | int | list[int] = None,
+) -> pd.DataFrame:
     """Setup all topic-year combinations, aggregate max, sum, average & count."""
 
-    if len(dtw) is None:
+    if len(dtw) == 0:
         raise pu.EmptyDataError()
 
-    year_range = dtw.year.min(), dtw.year.max() + 1
-    topic_range = 0, dtw.topic_id.max() + 1
-    year_topics: List[Tuple[int, int]] = list(itertools.product(range(*year_range), range(*topic_range)))
-    return (
+    year_range = range(dtw.year.min(), dtw.year.max() + 1)
+    topic_ids = (
+        range(0, dtw.topic_id.max() + 1)
+        if topic_ids is None
+        else [topic_ids]
+        if isinstance(topic_ids, int)
+        else topic_ids
+    )
+
+    year_topics: list[tuple[int, int]] = list(itertools.product(year_range, topic_ids))
+    ytw: pd.DataFrame = (
         pd.DataFrame(year_topics, columns=['year', 'topic_id'])
         .set_index(['year', 'topic_id'])
         .join(
             dtw.groupby(['year', 'topic_id'])['weight'].agg([np.max, np.sum, np.mean, len]),
             how='left',
         )
         .fillna(0)
-        .pipe(pu.rename_columns, columns=['max_weight', 'sum_weight', 'average_weight', 'n_topic_documents'])
+        .pipe(pu.rename_columns, columns=['max_weight', 'sum_weight', 'avg_weight', 'n_topic_documents'])
     )
+    ytw['average_weight'] = ytw['avg_weight']
+    return ytw
 
 
 def _add_average_yearly_topic_weight_above_threshold(
     yearly_weights: pd.DataFrame,
     dtw: pd.DataFrame,
     threshold: float = None,
     target_name: str = 'average_weight',
@@ -179,15 +191,15 @@
         data: pd.DataFrame = _compute_average_yearly_topic_weights_above_threshold(dtw, threshold, target_name)
         yearly_weights = yearly_weights.drop(columns=target_name).join(data, how='left').fillna(0)
     return yearly_weights
 
 
 def _add_yearly_corpus_document_count(yearly_weights: pd.DataFrame, document_index: pd.DataFrame) -> pd.DataFrame:
     """Add a column with _total_ number of documents in corpus for given year."""
-    yearly_weights = yearly_weights.join(
+    yearly_weights: pd.DataFrame = yearly_weights.join(
         document_index.groupby('year').size().rename('n_documents'), how='left'
     ).fillna(0)
     return yearly_weights
 
 
 def _add_average_yearly_topic_weight_by_all_documents(yearly_weights: pd.DataFrame) -> pd.DataFrame:
     """Compute "true" average weights (weight divided by total number of documents)"""
@@ -211,27 +223,85 @@
 
     yearly_weights = yearly_weights.join(top_n_counts, how='left').fillna(0)
     yearly_weights['top_n_weight'] = yearly_weights.apply(lambda x: x['top_n_documents'] / x['n_documents'], axis=1)
     return yearly_weights
 
 
 def compute_yearly_topic_weights(
-    dtw: pd.DataFrame, *, document_index: pd.DataFrame, threshold: float = None, n_top_relevance: int = None
+    dtw: pd.DataFrame,
+    *,
+    document_index: pd.DataFrame,
+    threshold: float = None,
+    n_top_relevance: int = None,
+    topic_ids: None | int | list[int] = None,
 ) -> pd.DataFrame:
     """Compute yearly document topic weights
          average_weight: average weight of all documents that has a weight in (i.e. assigned by engine) or a weight above a given threshold
     true_average_weight: average weight of all documents based on all documents (even documents where topic weight is 0)
 
     MALLET: Computes a weight for all topics in all documents
     GENSIM: Excludes topics having a weight less than 0
     """
 
     yearly_weights: pd.DataFrame = (
-        _compute_yearly_topic_weights(dtw)
+        _compute_yearly_topic_weights_statistics(dtw, topic_ids)
         .pipe(_add_yearly_corpus_document_count, document_index)
         .pipe(_add_average_yearly_topic_weight_by_all_documents)
         .pipe(_add_average_yearly_topic_weight_above_threshold, dtw, threshold, 'average_weight')
         .pipe(_add_top_n_topic_prevelance_weight, dtw, n_top_relevance)
         .reset_index()
     )
+    # yearly_weights: pd.DataFrame = _compute_yearly_topic_weights_statistics(dtw, topic_ids)
+    # yearly_weights = _add_yearly_corpus_document_count(yearly_weights, document_index)
+    # yearly_weights = _add_average_yearly_topic_weight_by_all_documents(yearly_weights)
+    # yearly_weights = _add_average_yearly_topic_weight_above_threshold(yearly_weights, dtw, threshold, 'average_weight')
+    # yearly_weights = _add_top_n_topic_prevelance_weight(yearly_weights, dtw, n_top_relevance)
+    # yearly_weights = yearly_weights.reset_index()
 
     return yearly_weights
+
+
+AggregateKeys = Literal['top_n_weight', 'average_weight', 'true_average_weight']
+AggregateKeyValues = get_args(AggregateKeys)
+
+# @not_used
+def compute_specified_yearly_topic_weights(
+    dtw: pd.DataFrame,
+    *,
+    document_index: pd.DataFrame,
+    aggregate_keys: str | AggregateKeys | list[AggregateKeys] = AggregateKeyValues,
+    threshold: float = None,
+    n_top_relevance: int = None,
+    drop_stats: bool = True,
+) -> pd.DataFrame:
+    """Compute specified yearly document topic weight only"""
+    fxs: dict = {
+        'true_average_weight': (_add_average_yearly_topic_weight_by_all_documents, tuple()),
+        'average_weight': (_add_average_yearly_topic_weight_above_threshold, (dtw, threshold, 'average_weight')),
+        'top_n_weight': (
+            _add_top_n_topic_prevelance_weight,
+            (
+                dtw,
+                n_top_relevance,
+            ),
+        ),
+    }
+    aggregate_keys: list[str] = (
+        aggregate_keys
+        if isinstance(aggregate_keys, (list, tuple))
+        else aggregate_keys.split(',')
+        if isinstance(aggregate_keys, str)
+        else AggregateKeyValues
+    )
+
+    ytw: pd.DataFrame = _compute_yearly_topic_weights_statistics(dtw).pipe(
+        _add_yearly_corpus_document_count, document_index
+    )
+
+    if drop_stats:
+        ytw.drop(columns=['max_weight', 'sum_weight', 'avg_weight'], inplace=True)
+
+    for key in aggregate_keys:
+        fx, args = fxs[key]
+        ytw = fx(ytw, *args)
+
+    return ytw.reset_index()
```

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/token.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/token.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/topics_data/topics_data.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/topics_data/topics_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     def load_token2id(folder: str) -> pc.Token2Id:
         dictionary: pd.DataFrame = smart_load(
             jj(folder, 'dictionary.zip'), feather_pipe=pu.set_index, columns='token_id'
         )
         token2id: pc.Token2Id = pc.Token2Id(data={t: i for (t, i) in zip(dictionary.token, dictionary.index)})
         return token2id
 
-    @property
+    @cached_property
     def topic_labels(self) -> dict:
         if 'label' not in self.topic_token_overview.columns:
             return {}
         return self.topic_token_overview['label'].to_dict()
 
 
 def fix_renamed_columns(di: pd.DataFrame) -> pd.DataFrame:
@@ -350,16 +350,14 @@
     if 'n_terms' in di.columns:
         di = di.drop(columns='n_terms')
     return di
 
 
 # FXIME: Reprecate pickled stora
 class PickleUtility:
-    ...
-
     @staticmethod
     def load(folder: str) -> InferredTopicsData:
 
         if not isfile(jj(folder, "inferred_topics.pickle")):
             return None
 
         with open(jj(folder, "inferred_topics.pickle"), 'rb') as f:
```

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/train.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/train.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/topic_modelling/utility.py` & `humlab-penelope-0.7.9/penelope/topic_modelling/utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,12 +11,16 @@
     models = [
         {'folder': x, 'name': os.path.split(x)[1], 'options': pu.read_json(os.path.join(x, "model_options.json"))}
         for x in folders
     ]
     return models
 
 
+def find_model(path: str, model_name: str) -> dict:
+    return next((x for x in find_models(path) if x["name"] == model_name), None)
+
+
 def find_inferred_topics_folders(folder: str) -> List[str]:
     """Return inferred data in sub-folders to `folder`"""
     filenames = glob.glob(os.path.join(folder, "**/*document_topic_weights.zip"), recursive=True)
     folders = [os.path.split(filename)[0] for filename in filenames]
     return folders
```

### Comparing `humlab-penelope-0.7.8/penelope/type_alias.py` & `humlab-penelope-0.7.9/penelope/type_alias.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/__init__.py` & `humlab-penelope-0.7.9/penelope/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/_color_utility.py` & `humlab-penelope-0.7.9/penelope/utility/_color_utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/_decorators.py` & `humlab-penelope-0.7.9/penelope/utility/_decorators.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/file_utility.py` & `humlab-penelope-0.7.9/penelope/utility/file_utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/filename_fields.py` & `humlab-penelope-0.7.9/penelope/utility/filename_fields.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/filename_utils.py` & `humlab-penelope-0.7.9/penelope/utility/filename_utils.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/pandas_utils.py` & `humlab-penelope-0.7.9/penelope/utility/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/paths.py` & `humlab-penelope-0.7.9/penelope/utility/paths.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/pos_tags.py` & `humlab-penelope-0.7.9/penelope/utility/pos_tags.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/streamify_source.py` & `humlab-penelope-0.7.9/penelope/utility/streamify_source.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/utils.py` & `humlab-penelope-0.7.9/penelope/utility/utils.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/utility/zip_utils.py` & `humlab-penelope-0.7.9/penelope/utility/zip_utils.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/archive/stanza/utility.py` & `humlab-penelope-0.7.9/penelope/vendor/archive/stanza/utility.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/archive/textacy_pipeline/pipeline.py` & `humlab-penelope-0.7.9/penelope/vendor/archive/textacy_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/_corpus.py` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/_corpus.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/_models.py` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/_models.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/dtmmodel.py.txt` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/dtmmodel.py.txt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/fasttext.py.txt` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/fasttext.py.txt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/ldavowpalwabbit.py.txt` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/ldavowpalwabbit.py.txt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/varembed.py.txt` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/varembed.py.txt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/archive/wordrank.py.txt` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/archive/wordrank.py.txt`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/ldamallet.py` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/ldamallet.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/mallet_tm.py` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/mallet_tm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-import xml.etree.cElementTree as ET
+import xml.etree.ElementTree as ET
 from typing import Iterable, Mapping, Tuple
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 
 from penelope.utility import inspect_filter_args
```

### Comparing `humlab-penelope-0.7.8/penelope/vendor/gensim_api/_gensim/wrappers/sttm_tm.py` & `humlab-penelope-0.7.9/penelope/vendor/gensim_api/_gensim/wrappers/sttm_tm.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/mallet_api/convert.py` & `humlab-penelope-0.7.9/penelope/vendor/mallet_api/convert.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/nltk/__init__.py` & `humlab-penelope-0.7.9/penelope/vendor/nltk/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/nltk/extra_stopwords.py` & `humlab-penelope-0.7.9/penelope/vendor/nltk/extra_stopwords.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/spacy_api/_spacy.py` & `humlab-penelope-0.7.9/penelope/vendor/spacy_api/_spacy.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/textacy_api/__init__.py` & `humlab-penelope-0.7.9/penelope/vendor/textacy_api/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/__init__.py` & `humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/__init__.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/extract.py` & `humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/extract.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/fallbacks.py` & `humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/fallbacks.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/mdw_modified.py` & `humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/mdw_modified.py`

 * *Files identical despite different names*

```diff
@@ -25,15 +25,14 @@
 import pandas as pd
 import scipy.sparse as sp
 from memoization import cached
 
 try:
     from textacy.representations import get_doc_freqs
 except ImportError:
-    ...
 
     def get_doc_freqs(doc_term_matrix: sp.csr_matrix) -> np.ndarray:
         """Copyright 2016 Chartbeat, Inc.
 
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `humlab-penelope-0.7.8/penelope/vendor/textacy_api/_textacy/utils.py` & `humlab-penelope-0.7.9/penelope/vendor/textacy_api/_textacy/utils.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/co_occurrence/compute.py` & `humlab-penelope-0.7.9/penelope/workflows/co_occurrence/compute.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/compute_opts.py` & `humlab-penelope-0.7.9/penelope/workflows/compute_opts.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/interface.py` & `humlab-penelope-0.7.9/penelope/workflows/interface.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/tm/predict.py` & `humlab-penelope-0.7.9/penelope/workflows/tm/predict.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/tm/train.py` & `humlab-penelope-0.7.9/penelope/workflows/tm/train.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/tm/train_id.py` & `humlab-penelope-0.7.9/penelope/workflows/tm/train_id.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/tm/train_legacy.py` & `humlab-penelope-0.7.9/penelope/workflows/tm/train_legacy.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/vectorize/dtm.py` & `humlab-penelope-0.7.9/penelope/workflows/vectorize/dtm.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/penelope/workflows/vectorize/dtm_id.py` & `humlab-penelope-0.7.9/penelope/workflows/vectorize/dtm_id.py`

 * *Files identical despite different names*

### Comparing `humlab-penelope-0.7.8/pyproject.toml` & `humlab-penelope-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "humlab-penelope"
-version = "0.7.8"
+version = "0.7.9"
 description = "Utilities that simplify enelpeing in Jupyter Lab"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [{ include = "penelope" }]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
     'Topic :: Software Development',
```

### Comparing `humlab-penelope-0.7.8/setup.py` & `humlab-penelope-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                      'tm-predict = penelope.scripts.tm.predict:click_main',
                      'tm-train = penelope.scripts.tm.train:click_main',
                      'tm-train-id = penelope.scripts.tm.train_id:click_main',
                      'vectorize = penelope.scripts.dtm.vectorize:main']}
 
 setup_kwargs = {
     'name': 'humlab-penelope',
-    'version': '0.7.8',
+    'version': '0.7.9',
     'description': 'Utilities that simplify enelpeing in Jupyter Lab',
     'long_description': '# Humlab Penelope\n\nNLP package used in the following research projects:\n\n    - Welfare State Analytics (westac.se)\n    - International Ideas at UNESCO: Digital Approaches to Global Conceptual History (inidun.github.io)\n\n======\n\n[![current release version](https://img.shields.io/github/release/humlab/penelope.svg?style=flat-square)](https://github.com/humlab/penelope/releases)\n[![pypi version](https://img.shields.io/pypi/v/humlab-penelope.svg?style=flat-square)](https://pypi.python.org/pypi/humlab-penelope)\n[![build-status](https://github.com/humlab/penelope/workflows/ci/badge.svg)](https://github.com/humlab/penelope/workflows/ci/badge.svg)\n<!-- [![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg)](https://doi.org/10.5281/zenodo.595120) -->\n\n|MIT license|\n\nInstallation\n------------\n\n```\npip install humlab-penelope\n```\n\nDependencies\n\nUsage\n\nDevelopment\n\nTesting\n\nVersioning\n\nReferences\n\n<!-- .. |Coverage-Status| image:: https://coveralls.io/repos/tqdm/tqdm/badge.svg?branch=master\n   :target: https://coveralls.io/github/tqdm/tqdm\n.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge\n   :target: https://bestpractices.coreinfrastructure.org/projects/3264\n.. |GitHub-Status| image:: https://img.shields.io/github/tag/tqdm/tqdm.svg?maxAge=86400&logo=github&logoColor=white\n   :target: https://github.com/tqdm/tqdm/releases\n.. |GitHub-Stars| image:: https://img.shields.io/github/stars/tqdm/tqdm.svg?logo=github&logoColor=white\n   :target: https://github.com/tqdm/tqdm/stargazers\n.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/tqdm/tqdm.svg?logo=git&logoColor=white\n   :target: https://github.com/tqdm/tqdm/graphs/commit-activity\n.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/tqdm/tqdm.svg?logo=github&logoColor=white\n   :target: https://github.com/tqdm/tqdm/issues?q=\n.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/tqdm/tqdm.svg?logo=github&logoColor=white\n   :target: https://github.com/tqdm/tqdm/pulls\n.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/tqdm/tqdm.svg?logo=github&logoColor=white\n   :target: https://github.com/tqdm/tqdm/graphs/contributors\n.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/tqdm/tqdm/master.svg?logo=github&logoColor=white&label=pushed\n   :target: https://github.com/tqdm/tqdm/pulse\n.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/tqdm.svg?label=pypi%20downloads&logo=PyPI&logoColor=white\n   :target: https://pypi.org/project/tqdm\n.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/tqdm.svg?logo=python&logoColor=white\n   :target: https://pypi.org/project/tqdm\n.. |LICENCE| image:: https://img.shields.io/pypi/l/tqdm.svg\n   :target: https://raw.githubusercontent.com/tqdm/tqdm/master/LICENCE\n.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg\n   :target: https://doi.org/10.5281/zenodo.595120\n.. |binder-demo| image:: https://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/tqdm/tqdm/master?filepath=DEMO.ipynb\n -->\n',
     'author': 'Roger Mähler',
     'author_email': 'roger.mahler@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/humlab/penelope',
```

### Comparing `humlab-penelope-0.7.8/PKG-INFO` & `humlab-penelope-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humlab-penelope
-Version: 0.7.8
+Version: 0.7.9
 Summary: Utilities that simplify enelpeing in Jupyter Lab
 Home-page: https://github.com/humlab/penelope
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.9.0,<3.10.0
 Classifier: License :: OSI Approved :: Apache Software License
```

