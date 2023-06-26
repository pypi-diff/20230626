# Comparing `tmp/qdls-0.0.6.tar.gz` & `tmp/qdls-0.0.7.tar.gz`

## Comparing `qdls-0.0.6.tar` & `qdls-0.0.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 qdls-0.0.6/build_upload.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/__init__.py
--rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/data.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/loggers.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/losses.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/metrics.py
--rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/object.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/optim.py
--rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/pretrains.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/tensor_ops.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/train.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/draw/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/draw/experiment.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/draw/stats.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/__init__.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/process_utils.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/__init__.py
--rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.interp
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.tokens
--rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.interp
--rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.tokens
--rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherListener.py
--rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherParser.py
--rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/__init__.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/execute.py
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/kqa_eval.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/parse.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/syntax.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/__init__.py
--rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.interp
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.tokens
--rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.interp
--rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
--rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlListener.py
--rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlParser.py
--rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/__init__.py
--rw-r--r--   0        0        0    24277 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/kqa_eval.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/parse.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/syntax.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/register.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/collators/__init__.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/collators/common_collators.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/datamodules/base_dm.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/datamodules/dataset_builder.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/models/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/models/test_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/process_functions/__init__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/process_functions/common.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/process_functions/kqa.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 qdls-0.0.6/test/btest.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 qdls-0.0.6/test/example_config.yaml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.6/test/test_draw.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.6/test/test_reg.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 qdls-0.0.6/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.0.6/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qdls-0.0.6/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qdls-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qdls-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 qdls-0.0.7/build_upload.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/__init__.py
+-rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/data.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/loggers.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/losses.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/metrics.py
+-rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/object.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/optim.py
+-rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/pretrains.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/tensor_ops.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/train.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/draw/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/draw/experiment.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/draw/stats.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/__init__.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/process_utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/__init__.py
+-rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/Cypher.interp
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/Cypher.tokens
+-rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherLexer.interp
+-rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherLexer.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherLexer.tokens
+-rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherListener.py
+-rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherParser.py
+-rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/utils/__init__.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/utils/execute.py
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/utils/kqa_eval.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/utils/parse.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/cypher/utils/syntax.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/__init__.py
+-rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/Sparql.interp
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/Sparql.tokens
+-rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlLexer.interp
+-rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlLexer.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
+-rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlListener.py
+-rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlParser.py
+-rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/utils/__init__.py
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/utils/kqa_eval.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/utils/parse.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/gql/sparql/utils/syntax.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/register.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/collators/__init__.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/collators/common_collators.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/datamodules/base_dm.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/datamodules/dataset_builder.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/models/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/models/test_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/process_functions/__init__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/process_functions/common.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 qdls-0.0.7/src/qdls/reg/process_functions/kqa.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 qdls-0.0.7/test/btest.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 qdls-0.0.7/test/example_config.yaml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.7/test/test_draw.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.7/test/test_reg.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 qdls-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.0.7/LICENSE
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qdls-0.0.7/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qdls-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qdls-0.0.7/PKG-INFO
```

### Comparing `qdls-0.0.6/src/qdls/data.py` & `qdls-0.0.7/src/qdls/data.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/loggers.py` & `qdls-0.0.7/src/qdls/loggers.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/losses.py` & `qdls-0.0.7/src/qdls/losses.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/metrics.py` & `qdls-0.0.7/src/qdls/metrics.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/object.py` & `qdls-0.0.7/src/qdls/object.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/optim.py` & `qdls-0.0.7/src/qdls/optim.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/pretrains.py` & `qdls-0.0.7/src/qdls/pretrains.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/tensor_ops.py` & `qdls-0.0.7/src/qdls/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/test.py` & `qdls-0.0.7/src/qdls/test.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/utils.py` & `qdls-0.0.7/src/qdls/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/draw/experiment.py` & `qdls-0.0.7/src/qdls/draw/experiment.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/draw/stats.py` & `qdls-0.0.7/src/qdls/draw/stats.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/process_utils.py` & `qdls-0.0.7/src/qdls/gql/process_utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/utils.py` & `qdls-0.0.7/src/qdls/gql/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.interp` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/Cypher.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.tokens` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/Cypher.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.interp` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.py` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.tokens` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherListener.py` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherParser.py` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherVisitor.py` & `qdls-0.0.7/src/qdls/gql/cypher/grammar/CypherVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/utils/execute.py` & `qdls-0.0.7/src/qdls/gql/cypher/utils/execute.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/utils/kqa_eval.py` & `qdls-0.0.7/src/qdls/gql/cypher/utils/kqa_eval.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/utils/parse.py` & `qdls-0.0.7/src/qdls/gql/cypher/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/cypher/utils/syntax.py` & `qdls-0.0.7/src/qdls/gql/cypher/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.interp` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/Sparql.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.tokens` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/Sparql.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.interp` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.py` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.tokens` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlListener.py` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlParser.py` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlVisitor.py` & `qdls-0.0.7/src/qdls/gql/sparql/grammar/SparqlVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/utils/kqa_eval.py` & `qdls-0.0.7/src/qdls/gql/sparql/utils/kqa_eval.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,31 @@
-# -*- coding: utf-8 -*-
-# @File    :   kqa_eval.py
-# @Time    :   2023/06/26 16:05:30
-# @Author  :   Qing 
-# @Email   :   aqsz2526@outlook.com
-######################### docstring ########################
-'''
-    Evaluate functions for kqa pro 
-    需要按照以下链接中的说明修改rdflib包的源码 
-    ! https://github.com/shijx12/KQAPro_Baselines/tree/master/Bart_SPARQL 
-'''
-
-import re 
-import json 
-from datetime import date
-from tqdm import tqdm
-from datetime import date
-from queue import Queue
 
 import rdflib
 from rdflib import URIRef, BNode, Literal, XSD
 from rdflib.plugins.stores import sparqlstore
 from itertools import chain
-
 import os, sys 
-from qdls.data import load_json, save_json
+try:
+    from q_snippets.data import load_json, save_json
+except:
+    from qdls.data import load_json, save_json
+from qdls.gql.sparql.utils.syntax import syntax_check
 from qdls.utils import print_string
-from multiprocessing import Pool 
+from multiprocessing import Pool
 
+# FILE_DIR = os.path.dirname(os.path.abspath(__file__))
+# PROJ_DIR = FILE_DIR[:FILE_DIR.index('src')]
+# PROJ_DIR = "/home/qing/workspace/archive/ACL23"
+# sys.path.append(PROJ_DIR)
 
 
-
-def comp(a, b, op):
-    """
-    Args:
-        - a (ValueClass): attribute value of a certain entity
-        - b (ValueClass): comparison target
-        - op: =/>/</!=
-    Example:
-        a is someone's birthday, 1960-02-01, b is 1960, op is '=', then return True
-    """
-    if b.isTime():
-        # Note: for time, 'a=b' actually means a in b, 'a!=b' means a not in b
-        if op == '=':
-            return b.contains(a)
-        elif op == '!=':
-            return not b.contains(a)
-    if op == '=':
-        return a == b
-    elif op == '<':
-        return a < b
-    elif op == '>':
-        return a > b
-    elif op == '!=':
-        return a != b
+import json 
+import re 
+from datetime import date
+from tqdm import tqdm
 
 class ValueClass():
     def __init__(self, type, value, unit=None):
         """
         When type is
             - string, value is a str
             - quantity, value is a number and unit is required
@@ -148,15 +117,14 @@
         elif self.type == 'date':
             return self.value.isoformat()
 
 
 class DataForSPARQL(object):
     def __init__(self, kb_path):
         kb = json.load(open(kb_path))
-        print_string(f"{kb_path} is loaded!")
         self.concepts = kb['concepts']
         self.entities = kb['entities']
 
         # replace adjacent space and tab in name, which may cause errors when building sparql query
         for con_id, con_info in self.concepts.items():
             con_info['name'] = ' '.join(con_info['name'].split())
         for ent_id, ent_info in self.entities.items():
@@ -268,25 +236,17 @@
 
     def get_relation_facts(self, ent_id):
         facts = self.entities[ent_id]['relations']
         facts = [(f['predicate'], f['object'], f['direction'], f['qualifiers']) for f in facts]
         return facts
 
 
-# print_string('loading data...', color='red')
-# try:
-#     kb = DataForSPARQL("/home/qing/datasets/kqa_pro/kb.json")
-#     virtuoso_address = "http://127.0.0.1:28890/sparql"
-#     virtuoso_graph_uri = ''
-# except Exception as e:
-#     print_string('failed to load data', color='red')
-#     print_string(" import this file and set `module_name.db, module_name.virtuoso_address, module_name.virtuoso_graph_uri` ")
 
-# print_string(f"virtuoso_address: {virtuoso_address}", color='red')
-# print_string(f"virtuoso_graph_uri: {virtuoso_graph_uri}", color='red')
+# kb = DataForSPARQL(os.path.join(PROJ_DIR, 'data/dataset/kb.json'))
+# kb = DataForSPARQL("/Users/qing/Downloads/kb.json")
 
 def legal(s):
     # convert predicate and attribute keys to legal format
     return s.replace(' ', '_')
 
 class SparqlEngine():
     gs1 = None
@@ -382,24 +342,24 @@
         node = BNode()
         self.graph.add((node, self.nodes[SparqlEngine.PRED_FACT_H], h))
         self.graph.add((node, self.nodes[SparqlEngine.PRED_FACT_R], r))
         self.graph.add((node, self.nodes[SparqlEngine.PRED_FACT_T], t))
         return node
 
 
+
 def query_virtuoso(q, virtuoso_address, virtuoso_graph_uri):
     endpoint = virtuoso_address
     store=sparqlstore.SPARQLUpdateStore(endpoint)
     gs = rdflib.ConjunctiveGraph(store)
     gs.open((endpoint, endpoint))
     gs1 = gs.get_context(rdflib.URIRef(virtuoso_graph_uri))
     res = gs1.query(q)
     return res
 
-
 def get_sparql_answer(sparql, data, config):
     """
     data: DataForSPARQL object, we need the key_type
     """
     try:
         # infer the parse_type based on sparql
         if sparql.startswith('SELECT DISTINCT ?e') or sparql.startswith('SELECT ?e'):
@@ -418,28 +378,29 @@
                     key = tokens[i-2]
                     break
             key = key[1:-1].replace('_', ' ')
             t = data.key_type[key]
             parse_type = 'attr_{}'.format(t)
 
         parsed_answer = None
-        res = query_virtuoso(sparql, config.address, config.uri)
-        
+
+        res = query_virtuoso(sparql, virtuoso_address=config.virtuoso_address, virtuoso_graph_uri=config.virtuoso_graph_uri)
+
         if res.vars:
             res = [[binding[v] for v in res.vars] for binding in res.bindings]
             if len(res) != 1:
                 return None
         else:
             res = res.askAnswer
             assert parse_type == 'bool'
         
         if parse_type == 'name':
             node = res[0][0]
             sp = 'SELECT DISTINCT ?v WHERE {{ <{}> <{}> ?v .  }}'.format(node, SparqlEngine.PRED_NAME)
-            res = query_virtuoso(sp)
+            res = query_virtuoso(sp, virtuoso_address=config.virtuoso_address, virtuoso_graph_uri=config.virtuoso_graph_uri)
             res = [[binding[v] for v in res.vars] for binding in res.bindings]
             name = res[0][0].value
             parsed_answer = name
         elif parse_type == 'count':
             count = res[0][0].value
             parsed_answer = str(count)
         elif parse_type.startswith('attr_'):
@@ -454,38 +415,40 @@
                 sp = 'SELECT DISTINCT ?v,?u,(str(?v) as ?sv) WHERE {{ <{}> <{}> ?v ; <{}> ?u .  }}'.format(node, SparqlEngine.PRED_VALUE, SparqlEngine.PRED_UNIT)
             elif v_type == 'year':
                 sp = 'SELECT DISTINCT ?v WHERE {{ <{}> <{}> ?v .  }}'.format(node, SparqlEngine.PRED_YEAR)
             elif v_type == 'date':
                 sp = 'SELECT DISTINCT ?v WHERE {{ <{}> <{}> ?v .  }}'.format(node, SparqlEngine.PRED_DATE)
             else:
                 raise Exception('unsupported parse type')
-            res = query_virtuoso(sp)
+            res = query_virtuoso(sp, virtuoso_address=config.virtuoso_address, virtuoso_graph_uri=config.virtuoso_graph_uri)
             res = [[binding[v] for v in res.vars] for binding in res.bindings]
             # if there is no specific date, then convert the type to year
             if len(res)==0 and v_type == 'date':
                 v_type = 'year'
                 sp = 'SELECT DISTINCT ?v WHERE {{ <{}> <{}> ?v .  }}'.format(node, SparqlEngine.PRED_YEAR)
-                res = query_virtuoso(sp)
+                res = query_virtuoso(sp, virtuoso_address=config.virtuoso_address, virtuoso_graph_uri=config.virtuoso_graph_uri)
                 res = [[binding[v] for v in res.vars] for binding in res.bindings]
             if v_type == 'quantity':
                 value = float(res[0][2].value)
                 unit = res[0][1].value
             else:
                 value = res[0][0].value
             value = ValueClass(v_type, value, unit)
             parsed_answer = str(value)
         elif parse_type == 'bool':
             parsed_answer = 'yes' if res else 'no'
         elif parse_type == 'pred':
             parsed_answer = str(res[0][0])
             parsed_answer = parsed_answer.replace('_', ' ')
-        return parsed_answer
+        # return parsed_answer
     except Exception as e:
-        # print(e)
-        return None
+        print(e)
+        parsed_answer = None 
+    # print(parsed_answer)
+    return parsed_answer
 
 def whether_equal(answer, pred):
     """
     check whether the two arguments are equal as attribute value
     answer type should be str 
     """
     def truncate_float(x):
@@ -528,16 +491,18 @@
     answer = truncate_float(answer)
     pred = truncate_float(pred)
     if equal_as_date(answer, pred):
         return True
     else:
         return answer == pred
 
+
 def post_process(text):
     """
+    针对BART生成结果的预处理
     字符串提取出来，其余部分是chunks， 需要增加?和.前的空格， 最后再组装起来即可
     !!!!!!!!!  只需要处理生成的， trainset里的就不用处理了
     """
     pattern = re.compile(r'".*?"')    # 匹配字符串？
     nes = []
     for item in pattern.finditer(text):
         nes.append((item.group(), item.span()))
@@ -552,52 +517,61 @@
         chunks[i] = chunks[i].replace('?', ' ?').replace('.', ' .')           # 增加空格
     bingo = ''
     for i in range(len(chunks) - 1):
         bingo += chunks[i] + nes[i][0]
     bingo += chunks[-1]
     return bingo
 
-def exec_sparql(sparql, answer, config):
-    sparql = post_process(sparql)
-    pred_answer = get_sparql_answer(sparql, config.kb, config)
+def pseudo_post_process(text):
+    return text 
+
+def exec_sparql(sparql, answer, config, kb, process_fn=pseudo_post_process):
+    sparql = process_fn(sparql)
+    # print("==>", sparql)
+    pred_answer = get_sparql_answer(sparql, kb, config)
     is_match = whether_equal(answer, pred_answer)
+    # print(sparql)
+    # print(is_match, pred_answer, answer)
     return is_match, pred_answer
 
 
-def sparql_exec_acc(path, key='pred', nproc=1, resave=False, config=None):
+def sparql_exec_acc(path, key='pred', nproc=1, resave=False, config=None, kb=None, process_fn=pseudo_post_process):
     """ path: 可以是字符串（读取文件）也可以是读取后的对象list 
         key: 每一个sample字典中, 预测的sparql语句的key
         nproc: 并行处理的进程数
         resave: bool or string  是否重新保存结果, 保存在原目录, 文件名前加上exec_
+        config: 配置文件, 主要是virtuoso的 address 和 graph uri
+        kb: 知识库
+        process_fn: 对sparql进行处理的函数
     """
     data = load_json(path) if type(path) is str else path 
     Results = []
     if nproc > 1:
         with Pool(nproc) as pool:
             R = {}
             for sample in data:
                 assert key in sample, f"key `{key}` not in provided data, sample.keys()={sample.keys()}"
                 sparql = sample[key]
                 answer = sample['answer']
-                future = pool.apply_async(exec_sparql, (sparql, answer, config))
+                future = pool.apply_async(exec_sparql, (sparql, answer, config, kb, process_fn))
                 R[future] = sample
             
             for future in tqdm(R):
                 try:
                     res = future.get(timeout=3)
                 except:
                     res = False, 'timeout'  
                 Results.append(res)
     else:
         print_string("sequential processing")
         for sample in tqdm(data):
             assert key in sample, f"key `{key}` not in provided data, sample.keys()={sample.keys()}"
             sparql = sample[key]
             answer = sample['answer']
-            Results.append(exec_sparql(sparql, answer, config))
+            Results.append(exec_sparql(sparql, answer, config, kb, process_fn))
 
     cnt = len(data)
     correct, wrong = 0, 0
     for is_match, pred in Results:
         if is_match:
             correct += 1
         else:
@@ -621,18 +595,8 @@
         save_json(data, new_path)
 
     return acc, Results
 
 
 
 if __name__ == '__main__':
-    pass 
-    """
-    from qdls.gql.sparql.utils import kqa_eval
-    kqa_eval.kb = DataForSPARQL("/home/qing/datasets/kqa_pro/kb.json")
-    kqa_eval.virtuoso_address = "http://127.0.0.1:28890/sparql"
-    kqa_eval.virtuoso_graph_uri = 'xxx'
-
-    """ 
-
-
-
+    pass
```

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/utils/parse.py` & `qdls-0.0.7/src/qdls/gql/sparql/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/gql/sparql/utils/syntax.py` & `qdls-0.0.7/src/qdls/gql/sparql/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/reg/register.py` & `qdls-0.0.7/src/qdls/reg/register.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/reg/collators/common_collators.py` & `qdls-0.0.7/src/qdls/reg/collators/common_collators.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/reg/datamodules/base_dm.py` & `qdls-0.0.7/src/qdls/reg/datamodules/base_dm.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/reg/datamodules/dataset_builder.py` & `qdls-0.0.7/src/qdls/reg/datamodules/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/src/qdls/reg/process_functions/kqa.py` & `qdls-0.0.7/src/qdls/reg/process_functions/kqa.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/test/test_draw.py` & `qdls-0.0.7/test/test_draw.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/test/test_reg.py` & `qdls-0.0.7/test/test_reg.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/.gitignore` & `qdls-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/LICENSE` & `qdls-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qdls-0.0.6/pyproject.toml` & `qdls-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "qdls"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Qing25", email="aqsz2526@outlook.com" },
 ]
 description = "Q-Deep Learning Snippets, my working code snippets"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qdls-0.0.6/PKG-INFO` & `qdls-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdls
-Version: 0.0.6
+Version: 0.0.7
 Summary: Q-Deep Learning Snippets, my working code snippets
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Qing25 <aqsz2526@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

