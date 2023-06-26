# Comparing `tmp/farm_haystack-1.9.1.tar.gz` & `tmp/farm_haystack-1.9.1rc1.tar.gz`

## Comparing `farm_haystack-1.9.1.tar` & `farm_haystack-1.9.1rc1.tar`

### file list

```diff
@@ -1,168 +1,167 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/VERSION.txt
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/environment.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/errors.py
--rw-r--r--   0        0        0    74584 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/schema.py
--rw-r--r--   0        0        0    14213 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/telemetry.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0    44592 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/base.py
--rw-r--r--   0        0        0    34318 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/deepsetcloud.py
--rw-r--r--   0        0        0   101090 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/elasticsearch.py
--rw-r--r--   0        0        0    14477 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/es_converter.py
--rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/faiss.py
--rw-r--r--   0        0        0    29793 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/filter_utils.py
--rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/graphdb.py
--rw-r--r--   0        0        0    42986 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/memory.py
--rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/memory_knowledgegraph.py
--rw-r--r--   0        0        0    35570 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/milvus1.py
--rw-r--r--   0        0        0    32983 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/milvus2.py
--rw-r--r--   0        0        0    40861 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/opensearch.py
--rw-r--r--   0        0        0    74783 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/pinecone.py
--rw-r--r--   0        0        0    33472 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/sql.py
--rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/utils.py
--rw-r--r--   0        0        0    70593 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/document_stores/weaviate.py
--rw-r--r--   0        0        0   106129 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.0.0.schema.json
--rw-r--r--   0        0        0   108418 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.1.0.schema.json
--rw-r--r--   0        0        0   106129 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.2.0.schema.json
--rw-r--r--   0        0        0   113517 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.3.0.schema.json
--rw-r--r--   0        0        0   126009 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.4.0.schema.json
--rw-r--r--   0        0        0   130768 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.5.0.schema.json
--rw-r--r--   0        0        0   140005 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.6.0.schema.json
--rw-r--r--   0        0        0   148292 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.7.0.schema.json
--rw-r--r--   0        0        0   148095 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.7.1.schema.json
--rw-r--r--   0        0        0   170350 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.7.2.schema.json
--rw-r--r--   0        0        0   170350 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.8.0.schema.json
--rw-r--r--   0        0        0   179072 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0.schema.json
--rw-r--r--   0        0        0   179201 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0rc1.schema.json
--rw-r--r--   0        0        0   179078 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0rc2.schema.json
--rw-r--r--   0        0        0   179078 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0rc3.schema.json
--rw-r--r--   0        0        0   179072 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.1.schema.json
--rw-r--r--   0        0        0   179078 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json
--rw-r--r--   0        0        0   179072 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-main.schema.json
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline.schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/__init__.py
--rw-r--r--   0        0        0    32295 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/infer.py
--rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/utils.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/visual.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/__init__.py
--rw-r--r--   0        0        0    37955 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/data_silo.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/dataloader.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/dataset.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/input_features.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/inputs.py
--rw-r--r--   0        0        0   109411 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/processor.py
--rw-r--r--   0        0        0     8030 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/data_handler/samples.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/evaluation/__init__.py
--rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/evaluation/eval.py
--rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/evaluation/metrics.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/evaluation/squad.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/__init__.py
--rw-r--r--   0        0        0    37079 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/adaptive_model.py
--rw-r--r--   0        0        0    25984 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/biadaptive_model.py
--rw-r--r--   0        0        0    45634 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/language_model.py
--rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/optimization.py
--rw-r--r--   0        0        0    54399 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/prediction_head.py
--rw-r--r--   0        0        0    14555 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/predictions.py
--rw-r--r--   0        0        0    14828 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/tokenization.py
--rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/model/triadaptive_model.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/training/__init__.py
--rw-r--r--   0        0        0    48505 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/training/base.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/training/dpr.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/modeling/training/question_answering.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/__init__.py
--rw-r--r--   0        0        0    18642 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/_json_schema.py
--rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/base.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/answer_generator/__init__.py
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/answer_generator/base.py
--rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/answer_generator/openai.py
--rw-r--r--   0        0        0    23448 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/answer_generator/transformers.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/audio/__init__.py
--rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/audio/_text_to_speech.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/audio/answer_to_speech.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/audio/document_to_speech.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/connector/__init__.py
--rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/connector/crawler.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/document_classifier/__init__.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/document_classifier/base.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/document_classifier/transformers.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/evaluator/__init__.py
--rw-r--r--   0        0        0    27052 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/evaluator/evaluator.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/extractor/__init__.py
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/extractor/entity.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_classifier/__init__.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_classifier/file_type.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/__init__.py
--rw-r--r--   0        0        0    15713 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/azure.py
--rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/base.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/docx.py
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/image.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/markdown.py
--rw-r--r--   0        0        0    14471 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/parsr.py
--rw-r--r--   0        0        0    15116 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/pdf.py
--rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/tika.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/file_converter/txt.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/label_generator/__init__.py
--rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/label_generator/pseudo_label_generator.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/other/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/other/docs2answers.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/other/join.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/other/join_answers.py
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/other/join_docs.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/other/route_documents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/preprocessor/__init__.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/preprocessor/base.py
--rw-r--r--   0        0        0    26816 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/preprocessor/preprocessor.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/query_classifier/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/query_classifier/base.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/query_classifier/sklearn.py
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/query_classifier/transformers.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/question_generator/__init__.py
--rw-r--r--   0        0        0    13175 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/question_generator/question_generator.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/ranker/__init__.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/ranker/base.py
--rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/ranker/sentence_transformers.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/reader/__init__.py
--rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/reader/base.py
--rw-r--r--   0        0        0    71807 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/reader/farm.py
--rw-r--r--   0        0        0    37456 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/reader/table.py
--rw-r--r--   0        0        0    17421 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/reader/transformers.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/retriever/__init__.py
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/retriever/_embedding_encoder.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/retriever/_losses.py
--rw-r--r--   0        0        0    17194 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/retriever/base.py
--rw-r--r--   0        0        0   115643 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/retriever/dense.py
--rw-r--r--   0        0        0    31086 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/retriever/sparse.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/retriever/text2sparql.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/summarizer/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/summarizer/base.py
--rw-r--r--   0        0        0    15049 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/summarizer/transformers.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/translator/__init__.py
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/translator/base.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/nodes/translator/transformers.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/pipelines/__init__.py
--rw-r--r--   0        0        0   132007 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/pipelines/base.py
--rw-r--r--   0        0        0    26041 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/pipelines/config.py
--rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/pipelines/ray.py
--rw-r--r--   0        0        0    38310 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/pipelines/standard_pipelines.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/pipelines/utils.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/__init__.py
--rw-r--r--   0        0        0    12515 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/augment_squad.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/cleaning.py
--rw-r--r--   0        0        0    10464 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/context_matching.py
--rw-r--r--   0        0        0    77308 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/deepsetcloud.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/doc_store.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/docker.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/early_stopping.py
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/experiment_tracking.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/export_utils.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/import_utils.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/preprocessing.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/reflection.py
--rw-r--r--   0        0        0    11680 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/squad_data.py
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/squad_to_dpr.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/haystack/utils/torch_utils.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/LICENSE
--rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/README.md
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/pyproject.toml
--rw-r--r--   0        0        0    20977 2020-02-02 00:00:00.000000 farm_haystack-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/VERSION.txt
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/environment.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/errors.py
+-rw-r--r--   0        0        0    74584 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/schema.py
+-rw-r--r--   0        0        0    14213 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/telemetry.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0    44592 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/base.py
+-rw-r--r--   0        0        0    34318 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/deepsetcloud.py
+-rw-r--r--   0        0        0   101090 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/elasticsearch.py
+-rw-r--r--   0        0        0    14477 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/es_converter.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/faiss.py
+-rw-r--r--   0        0        0    29793 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/filter_utils.py
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/graphdb.py
+-rw-r--r--   0        0        0    42986 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/memory.py
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/memory_knowledgegraph.py
+-rw-r--r--   0        0        0    35570 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/milvus1.py
+-rw-r--r--   0        0        0    32983 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/milvus2.py
+-rw-r--r--   0        0        0    40861 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/opensearch.py
+-rw-r--r--   0        0        0    74783 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/pinecone.py
+-rw-r--r--   0        0        0    33472 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/sql.py
+-rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/utils.py
+-rw-r--r--   0        0        0    70593 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/document_stores/weaviate.py
+-rw-r--r--   0        0        0   106129 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.0.0.schema.json
+-rw-r--r--   0        0        0   108418 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.1.0.schema.json
+-rw-r--r--   0        0        0   106129 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.2.0.schema.json
+-rw-r--r--   0        0        0   113517 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.3.0.schema.json
+-rw-r--r--   0        0        0   126009 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.4.0.schema.json
+-rw-r--r--   0        0        0   130768 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.5.0.schema.json
+-rw-r--r--   0        0        0   140005 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.6.0.schema.json
+-rw-r--r--   0        0        0   148292 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.7.0.schema.json
+-rw-r--r--   0        0        0   148095 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.7.1.schema.json
+-rw-r--r--   0        0        0   170350 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.7.2.schema.json
+-rw-r--r--   0        0        0   170350 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.8.0.schema.json
+-rw-r--r--   0        0        0   179072 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0.schema.json
+-rw-r--r--   0        0        0   179201 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0rc1.schema.json
+-rw-r--r--   0        0        0   179078 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0rc2.schema.json
+-rw-r--r--   0        0        0   179078 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0rc3.schema.json
+-rw-r--r--   0        0        0   179078 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json
+-rw-r--r--   0        0        0   179072 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-main.schema.json
+-rw-r--r--   0        0        0     6945 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline.schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/__init__.py
+-rw-r--r--   0        0        0    32295 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/infer.py
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/utils.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/visual.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/__init__.py
+-rw-r--r--   0        0        0    37955 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/data_silo.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/dataloader.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/dataset.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/input_features.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/inputs.py
+-rw-r--r--   0        0        0   109411 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/processor.py
+-rw-r--r--   0        0        0     8030 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/data_handler/samples.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/evaluation/__init__.py
+-rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/evaluation/eval.py
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/evaluation/metrics.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/evaluation/squad.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/__init__.py
+-rw-r--r--   0        0        0    37079 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/adaptive_model.py
+-rw-r--r--   0        0        0    25984 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/biadaptive_model.py
+-rw-r--r--   0        0        0    45634 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/language_model.py
+-rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/optimization.py
+-rw-r--r--   0        0        0    54399 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/prediction_head.py
+-rw-r--r--   0        0        0    14555 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/predictions.py
+-rw-r--r--   0        0        0    14828 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/tokenization.py
+-rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/model/triadaptive_model.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/training/__init__.py
+-rw-r--r--   0        0        0    48505 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/training/base.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/training/dpr.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/modeling/training/question_answering.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/__init__.py
+-rw-r--r--   0        0        0    18642 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/_json_schema.py
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/base.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/answer_generator/__init__.py
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/answer_generator/base.py
+-rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/answer_generator/openai.py
+-rw-r--r--   0        0        0    23448 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/answer_generator/transformers.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/audio/__init__.py
+-rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/audio/_text_to_speech.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/audio/answer_to_speech.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/audio/document_to_speech.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/connector/__init__.py
+-rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/connector/crawler.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/document_classifier/__init__.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/document_classifier/base.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/document_classifier/transformers.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/evaluator/__init__.py
+-rw-r--r--   0        0        0    27052 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/evaluator/evaluator.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/extractor/__init__.py
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/extractor/entity.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_classifier/__init__.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_classifier/file_type.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/__init__.py
+-rw-r--r--   0        0        0    15713 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/azure.py
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/base.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/docx.py
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/image.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/markdown.py
+-rw-r--r--   0        0        0    14471 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/parsr.py
+-rw-r--r--   0        0        0    15116 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/pdf.py
+-rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/tika.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/file_converter/txt.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/label_generator/__init__.py
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/label_generator/pseudo_label_generator.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/other/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/other/docs2answers.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/other/join.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/other/join_answers.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/other/join_docs.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/other/route_documents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/preprocessor/__init__.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/preprocessor/base.py
+-rw-r--r--   0        0        0    26816 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/preprocessor/preprocessor.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/query_classifier/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/query_classifier/base.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/query_classifier/sklearn.py
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/query_classifier/transformers.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/question_generator/__init__.py
+-rw-r--r--   0        0        0    13175 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/question_generator/question_generator.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/ranker/__init__.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/ranker/base.py
+-rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/ranker/sentence_transformers.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/reader/__init__.py
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/reader/base.py
+-rw-r--r--   0        0        0    71807 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/reader/farm.py
+-rw-r--r--   0        0        0    37456 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/reader/table.py
+-rw-r--r--   0        0        0    17421 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/reader/transformers.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/retriever/__init__.py
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/retriever/_embedding_encoder.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/retriever/_losses.py
+-rw-r--r--   0        0        0    17194 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/retriever/base.py
+-rw-r--r--   0        0        0   115643 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/retriever/dense.py
+-rw-r--r--   0        0        0    31086 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/retriever/sparse.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/retriever/text2sparql.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/summarizer/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/summarizer/base.py
+-rw-r--r--   0        0        0    15049 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/summarizer/transformers.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/translator/__init__.py
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/translator/base.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/nodes/translator/transformers.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/pipelines/__init__.py
+-rw-r--r--   0        0        0   132007 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/pipelines/base.py
+-rw-r--r--   0        0        0    26041 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/pipelines/config.py
+-rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/pipelines/ray.py
+-rw-r--r--   0        0        0    38310 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/pipelines/standard_pipelines.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/pipelines/utils.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/__init__.py
+-rw-r--r--   0        0        0    12515 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/augment_squad.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/cleaning.py
+-rw-r--r--   0        0        0    10464 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/context_matching.py
+-rw-r--r--   0        0        0    77308 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/deepsetcloud.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/doc_store.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/docker.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/early_stopping.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/experiment_tracking.py
+-rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/export_utils.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/import_utils.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/preprocessing.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/reflection.py
+-rw-r--r--   0        0        0    11680 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/squad_data.py
+-rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/squad_to_dpr.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/haystack/utils/torch_utils.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/LICENSE
+-rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/README.md
+-rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    20980 2020-02-02 00:00:00.000000 farm_haystack-1.9.1rc1/PKG-INFO
```

### Comparing `farm_haystack-1.9.1/haystack/__init__.py` & `farm_haystack-1.9.1rc1/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/environment.py` & `farm_haystack-1.9.1rc1/haystack/environment.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/errors.py` & `farm_haystack-1.9.1rc1/haystack/errors.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/schema.py` & `farm_haystack-1.9.1rc1/haystack/schema.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/telemetry.py` & `farm_haystack-1.9.1rc1/haystack/telemetry.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/__init__.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/base.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/deepsetcloud.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/deepsetcloud.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/elasticsearch.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/es_converter.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/es_converter.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/faiss.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/filter_utils.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/filter_utils.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/graphdb.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/graphdb.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/memory.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/memory.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/memory_knowledgegraph.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/memory_knowledgegraph.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/milvus1.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/milvus1.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/milvus2.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/milvus2.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/opensearch.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/pinecone.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/sql.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/sql.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/utils.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/utils.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/document_stores/weaviate.py` & `farm_haystack-1.9.1rc1/haystack/document_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.0.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.0.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.1.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.1.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.2.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.2.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.3.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.3.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.4.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.4.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.5.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.5.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.6.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.6.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.7.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.7.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.7.1.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.7.1.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.7.2.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.7.2.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.8.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.8.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0rc1.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0rc1.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0rc2.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0rc2.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.0rc3.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.0rc3.schema.json`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.1.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.94921875%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json'",*

 * * "'properties'": "{'version': {'const': '1.9.1rc1'}}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-1.9.1.schema.json",
+    "$id": "https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "definitions": {
         "AnswerToSpeechComponent": {
             "additionalProperties": false,
             "properties": {
                 "name": {
@@ -6398,15 +6398,15 @@
                 },
                 "type": "object"
             },
             "title": "Pipelines",
             "type": "array"
         },
         "version": {
-            "const": "1.9.1",
+            "const": "1.9.1rc1",
             "description": "Version of the Haystack Pipeline file.",
             "title": "Version",
             "type": "string"
         }
     },
     "required": [
         "version",
```

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline-main.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.94921875%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-main.schema.json'",*

 * * "'properties'": "{'version': {'const': 'ignore'}}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json",
+    "$id": "https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-main.schema.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "definitions": {
         "AnswerToSpeechComponent": {
             "additionalProperties": false,
             "properties": {
                 "name": {
@@ -6398,15 +6398,15 @@
                 },
                 "type": "object"
             },
             "title": "Pipelines",
             "type": "array"
         },
         "version": {
-            "const": "1.9.1rc1",
+            "const": "ignore",
             "description": "Version of the Haystack Pipeline file.",
             "title": "Version",
             "type": "string"
         }
     },
     "required": [
         "version",
```

### Comparing `farm_haystack-1.9.1/haystack/json-schemas/haystack-pipeline.schema.json` & `farm_haystack-1.9.1rc1/haystack/json-schemas/haystack-pipeline.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996031746031746%*

 * *Differences: {"'oneOf'": '{delete: [20]}'}*

```diff
@@ -278,26 +278,12 @@
                         }
                     }
                 },
                 {
                     "$ref": "https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-1.9.1rc1.schema.json"
                 }
             ]
-        },
-        {
-            "allOf": [
-                {
-                    "properties": {
-                        "version": {
-                            "const": "1.9.1"
-                        }
-                    }
-                },
-                {
-                    "$ref": "https://raw.githubusercontent.com/deepset-ai/haystack/main/haystack/json-schemas/haystack-pipeline-1.9.1.schema.json"
-                }
-            ]
         }
     ],
     "title": "Haystack Pipeline",
     "type": "object"
 }
```

### Comparing `farm_haystack-1.9.1/haystack/modeling/infer.py` & `farm_haystack-1.9.1rc1/haystack/modeling/infer.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/utils.py` & `farm_haystack-1.9.1rc1/haystack/modeling/utils.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/visual.py` & `farm_haystack-1.9.1rc1/haystack/modeling/visual.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/data_handler/data_silo.py` & `farm_haystack-1.9.1rc1/haystack/modeling/data_handler/data_silo.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/data_handler/dataloader.py` & `farm_haystack-1.9.1rc1/haystack/modeling/data_handler/dataloader.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/data_handler/dataset.py` & `farm_haystack-1.9.1rc1/haystack/modeling/data_handler/dataset.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/data_handler/input_features.py` & `farm_haystack-1.9.1rc1/haystack/modeling/data_handler/input_features.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/data_handler/inputs.py` & `farm_haystack-1.9.1rc1/haystack/modeling/data_handler/inputs.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/data_handler/processor.py` & `farm_haystack-1.9.1rc1/haystack/modeling/data_handler/processor.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/data_handler/samples.py` & `farm_haystack-1.9.1rc1/haystack/modeling/data_handler/samples.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/evaluation/eval.py` & `farm_haystack-1.9.1rc1/haystack/modeling/evaluation/eval.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/evaluation/metrics.py` & `farm_haystack-1.9.1rc1/haystack/modeling/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/evaluation/squad.py` & `farm_haystack-1.9.1rc1/haystack/modeling/evaluation/squad.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/adaptive_model.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/adaptive_model.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/biadaptive_model.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/biadaptive_model.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/language_model.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/language_model.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/optimization.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/optimization.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/prediction_head.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/prediction_head.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/predictions.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/predictions.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/tokenization.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/tokenization.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/model/triadaptive_model.py` & `farm_haystack-1.9.1rc1/haystack/modeling/model/triadaptive_model.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/modeling/training/base.py` & `farm_haystack-1.9.1rc1/haystack/modeling/training/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/__init__.py` & `farm_haystack-1.9.1rc1/haystack/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/_json_schema.py` & `farm_haystack-1.9.1rc1/haystack/nodes/_json_schema.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/answer_generator/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/answer_generator/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/answer_generator/openai.py` & `farm_haystack-1.9.1rc1/haystack/nodes/answer_generator/openai.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/answer_generator/transformers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/answer_generator/transformers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/audio/_text_to_speech.py` & `farm_haystack-1.9.1rc1/haystack/nodes/audio/_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/audio/answer_to_speech.py` & `farm_haystack-1.9.1rc1/haystack/nodes/audio/answer_to_speech.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/audio/document_to_speech.py` & `farm_haystack-1.9.1rc1/haystack/nodes/audio/document_to_speech.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/connector/crawler.py` & `farm_haystack-1.9.1rc1/haystack/nodes/connector/crawler.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/document_classifier/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/document_classifier/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/document_classifier/transformers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/document_classifier/transformers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/evaluator/evaluator.py` & `farm_haystack-1.9.1rc1/haystack/nodes/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/extractor/entity.py` & `farm_haystack-1.9.1rc1/haystack/nodes/extractor/entity.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_classifier/file_type.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_classifier/file_type.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/__init__.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/azure.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/azure.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/docx.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/docx.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/image.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/image.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/markdown.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/markdown.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/parsr.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/parsr.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/pdf.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/pdf.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/tika.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/tika.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/file_converter/txt.py` & `farm_haystack-1.9.1rc1/haystack/nodes/file_converter/txt.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/label_generator/pseudo_label_generator.py` & `farm_haystack-1.9.1rc1/haystack/nodes/label_generator/pseudo_label_generator.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/other/docs2answers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/other/docs2answers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/other/join.py` & `farm_haystack-1.9.1rc1/haystack/nodes/other/join.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/other/join_answers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/other/join_answers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/other/join_docs.py` & `farm_haystack-1.9.1rc1/haystack/nodes/other/join_docs.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/other/route_documents.py` & `farm_haystack-1.9.1rc1/haystack/nodes/other/route_documents.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/preprocessor/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/preprocessor/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/preprocessor/preprocessor.py` & `farm_haystack-1.9.1rc1/haystack/nodes/preprocessor/preprocessor.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/query_classifier/sklearn.py` & `farm_haystack-1.9.1rc1/haystack/nodes/query_classifier/sklearn.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/query_classifier/transformers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/query_classifier/transformers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/question_generator/question_generator.py` & `farm_haystack-1.9.1rc1/haystack/nodes/question_generator/question_generator.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/ranker/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/ranker/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/ranker/sentence_transformers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/ranker/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/reader/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/reader/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/reader/farm.py` & `farm_haystack-1.9.1rc1/haystack/nodes/reader/farm.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/reader/table.py` & `farm_haystack-1.9.1rc1/haystack/nodes/reader/table.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/reader/transformers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/reader/transformers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/retriever/_embedding_encoder.py` & `farm_haystack-1.9.1rc1/haystack/nodes/retriever/_embedding_encoder.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/retriever/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/retriever/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/retriever/dense.py` & `farm_haystack-1.9.1rc1/haystack/nodes/retriever/dense.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/retriever/sparse.py` & `farm_haystack-1.9.1rc1/haystack/nodes/retriever/sparse.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/retriever/text2sparql.py` & `farm_haystack-1.9.1rc1/haystack/nodes/retriever/text2sparql.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/summarizer/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/summarizer/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/summarizer/transformers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/summarizer/transformers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/translator/base.py` & `farm_haystack-1.9.1rc1/haystack/nodes/translator/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/nodes/translator/transformers.py` & `farm_haystack-1.9.1rc1/haystack/nodes/translator/transformers.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/pipelines/base.py` & `farm_haystack-1.9.1rc1/haystack/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/pipelines/config.py` & `farm_haystack-1.9.1rc1/haystack/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/pipelines/ray.py` & `farm_haystack-1.9.1rc1/haystack/pipelines/ray.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/pipelines/standard_pipelines.py` & `farm_haystack-1.9.1rc1/haystack/pipelines/standard_pipelines.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/pipelines/utils.py` & `farm_haystack-1.9.1rc1/haystack/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/__init__.py` & `farm_haystack-1.9.1rc1/haystack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/augment_squad.py` & `farm_haystack-1.9.1rc1/haystack/utils/augment_squad.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/cleaning.py` & `farm_haystack-1.9.1rc1/haystack/utils/cleaning.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/context_matching.py` & `farm_haystack-1.9.1rc1/haystack/utils/context_matching.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/deepsetcloud.py` & `farm_haystack-1.9.1rc1/haystack/utils/deepsetcloud.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/doc_store.py` & `farm_haystack-1.9.1rc1/haystack/utils/doc_store.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/docker.py` & `farm_haystack-1.9.1rc1/haystack/utils/docker.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/early_stopping.py` & `farm_haystack-1.9.1rc1/haystack/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/experiment_tracking.py` & `farm_haystack-1.9.1rc1/haystack/utils/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/export_utils.py` & `farm_haystack-1.9.1rc1/haystack/utils/export_utils.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/import_utils.py` & `farm_haystack-1.9.1rc1/haystack/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/preprocessing.py` & `farm_haystack-1.9.1rc1/haystack/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/reflection.py` & `farm_haystack-1.9.1rc1/haystack/utils/reflection.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/squad_data.py` & `farm_haystack-1.9.1rc1/haystack/utils/squad_data.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/haystack/utils/squad_to_dpr.py` & `farm_haystack-1.9.1rc1/haystack/utils/squad_to_dpr.py`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/.gitignore` & `farm_haystack-1.9.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/LICENSE` & `farm_haystack-1.9.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/README.md` & `farm_haystack-1.9.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/pyproject.toml` & `farm_haystack-1.9.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `farm_haystack-1.9.1/PKG-INFO` & `farm_haystack-1.9.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farm-haystack
-Version: 1.9.1
+Version: 1.9.1rc1
 Summary: Neural Question Answering & Semantic Search at Scale. Use modern transformer based models like BERT to find answers in large document collections
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
```

